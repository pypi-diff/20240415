# Comparing `tmp/eradiate-0.26.2rc1.tar.gz` & `tmp/eradiate-0.26.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eradiate-0.26.2rc1.tar", last modified: Fri Mar 15 15:56:47 2024, max compression
+gzip compressed data, was "eradiate-0.26.3rc1.tar", last modified: Mon Apr 15 15:55:33 2024, max compression
```

## Comparing `eradiate-0.26.2rc1.tar` & `eradiate-0.26.3rc1.tar`

### file list

```diff
@@ -1,639 +1,639 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.219153 eradiate-0.26.2rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.127152 eradiate-0.26.2rc1/.devcontainer/
--rwxr-xr-x   0 runner    (1001) docker     (127)      135 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.devcontainer/create-command.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.127152 eradiate-0.26.2rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.131152 eradiate-0.26.2rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.131152 eradiate-0.26.2rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-03-15 15:56:47.219153 eradiate-0.26.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.131152 eradiate-0.26.2rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.131152 eradiate-0.26.2rc1/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_ext/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_ext/pluginparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.131152 eradiate-0.26.2rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (127)    17013 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    32795 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-black.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25531 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-darkgrey.png
--rw-r--r--   0 runner    (1001) docker     (127)    34059 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-darkgrey.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18587 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    34061 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.119151 eradiate-0.26.2rc1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.135152 eradiate-0.26.2rc1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.135152 eradiate-0.26.2rc1/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/_templates/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/convert_figures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.143152 eradiate-0.26.2rc1/docs/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    20540 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/atmosphere_attributes.png
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/atmosphere_attributes.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28149 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-east_left.png
--rw-r--r--   0 runner    (1001) docker     (127)    32937 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-east_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28852 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-east_right.png
--rw-r--r--   0 runner    (1001) docker     (127)    35278 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-east_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-north_left.png
--rw-r--r--   0 runner    (1001) docker     (127)    32862 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-north_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28115 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-north_right.png
--rw-r--r--   0 runner    (1001) docker     (127)    32455 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-north_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28153 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-south_left.png
--rw-r--r--   0 runner    (1001) docker     (127)    32939 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-south_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28118 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-south_right.png
--rw-r--r--   0 runner    (1001) docker     (127)    32455 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-south_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28178 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-west_left.png
--rw-r--r--   0 runner    (1001) docker     (127)    32935 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-west_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-west_right.png
--rw-r--r--   0 runner    (1001) docker     (127)    32437 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/azimuth-west_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/cartesian-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (127)    15939 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/cartesian-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25301 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/cuboid_leaf_cloud_params.png
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/cuboid_leaf_cloud_params.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.143152 eradiate-0.26.2rc1/docs/fig/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/diagrams/class_diagram_biosphere.drawio
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
--rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/diagrams/package.drawio
--rw-r--r--   0 runner    (1001) docker     (127)    40438 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/eradiate-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/icon_eradiate.png
--rw-r--r--   0 runner    (1001) docker     (127)    38873 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/package.png
--rw-r--r--   0 runner    (1001) docker     (127)    57417 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/package.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32384 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/radiancemeter_hsphere.png
--rw-r--r--   0 runner    (1001) docker     (127)    43351 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/radiancemeter_hsphere.svg
--rw-r--r--   0 runner    (1001) docker     (127)    36773 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/radiancemeter_plane.png
--rw-r--r--   0 runner    (1001) docker     (127)    31853 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/radiancemeter_plane.svg
--rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/requirement_layers.png
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/requirement_layers.svg
--rw-r--r--   0 runner    (1001) docker     (127)    21451 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/solid_2017.png
--rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spectral_discretization_ckd_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (127)    16459 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (127)    27127 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png
--rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spherical-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (127)    19861 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/spherical-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/fig/thuillier_2003.png
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/generate_md_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/generate_rst_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/generate_rst_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/index_latex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    17968 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.143152 eradiate-0.26.2rc1/docs/rst/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22779 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/dependencies.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.143152 eradiate-0.26.2rc1/docs/rst/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/developer_guide/design_atmosphere.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/developer_guide/dev_install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/developer_guide/factory_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/developer_guide/lazy_loading.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/developer_guide/scene_generator.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/developer_guide/update.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/maintainer_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.151152 eradiate-0.26.2rc1/docs/rst/reference_api/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/attrs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/constants.rst
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/converters.rst
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/eradiate_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/experiments.rst
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/factory.rst
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/frame.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/kernel.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/mode.rst
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/notebook.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/plot.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/quad.rst
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/radprops.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/rng.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/scenes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/spectral.rst
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/srf_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/test_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/units.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/util.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/validators.rst
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/warp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_api/xarray.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.151152 eradiate-0.26.2rc1/docs/rst/reference_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/reference_plugins/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.151152 eradiate-0.26.2rc1/docs/rst/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.151152 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/absorption.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.151152 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
--rw-r--r--   0 runner    (1001) docker     (127)    26889 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png
--rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/fig/line.png
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/homogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/molecular.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/particle_layer.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/basic_concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/conventions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.155152 eradiate-0.26.2rc1/docs/rst/user_guide/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/absorption.rst
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/atmosphere_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/atmosphere_thermoprops.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.155152 eradiate-0.26.2rc1/docs/rst/user_guide/data/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    30117 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
--rw-r--r--   0 runner    (1001) docker     (127)    59107 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/fig/pt_points.png
--rw-r--r--   0 runner    (1001) docker     (127)    28580 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/particle_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/solar_irradiance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/data/srf.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/onedim_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/package_structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/scene_loader.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/spectral_discretization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/rst/user_guide/unit_guide_user.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.155152 eradiate-0.26.2rc1/docs/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/src/reference_cli.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.155152 eradiate-0.26.2rc1/docs/src/release_notes/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/src/release_notes/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/src/release_notes/v0.23.x_and_older.md
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/src/release_notes/v0.24.x.md
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/src/release_notes/v0.25.x.md
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/docs/src/release_notes/v0.26.x.md
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.155152 eradiate-0.26.2rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/check_conda_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.163152 eradiate-0.26.2rc1/requirements/conda/
--rw-r--r--   0 runner    (1001) docker     (127)    22740 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-dependencies-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-dependencies-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-dependencies-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-dependencies.yml
--rw-r--r--   0 runner    (1001) docker     (127)    44654 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-dev-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    37451 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-dev-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    40096 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-dev-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)    30111 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-docs-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    21006 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-docs-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-docs-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22740 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-main-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-main-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-main-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)    44654 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-optional-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    37451 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-optional-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    40096 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-optional-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-optional.yml
--rw-r--r--   0 runner    (1001) docker     (127)    26200 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-recommended-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    24478 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-recommended-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    25980 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-recommended-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-recommended.yml
--rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-tests-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-tests-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)    16990 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-tests-win-64.lock
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/conda/environment-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/copy_envvars.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/environment.in
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/layered.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/make_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/make_pip_in_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/make_pip_txt_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.163152 eradiate-0.26.2rc1/requirements/pip/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/dependencies.in
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/dependencies.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-15 15:56:43.000000 eradiate-0.26.2rc1/requirements/pip/dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/dev.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/docs.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/main.in
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/main.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/optional.in
--rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/optional.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/recommended.in
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/recommended.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-15 15:56:43.000000 eradiate-0.26.2rc1/requirements/pip/recommended.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/tests.in
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/requirements/pip/tests.lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/setpath.bat
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/setpath.ps1
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/setpath.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 15:56:47.219153 eradiate-0.26.2rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.119151 eradiate-0.26.2rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.167152 eradiate-0.26.2rc1/src/eradiate/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9405 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11586 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/cfconventions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.171152 eradiate-0.26.2rc1/src/eradiate/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/cli/srf.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.171152 eradiate-0.26.2rc1/src/eradiate/data/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/_safe_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)   211288 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/downloads_all.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16905 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/data/downloads_minimal.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.171152 eradiate-0.26.2rc1/src/eradiate/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/experiments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/experiments/_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/experiments/_canopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14479 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/experiments/_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/experiments/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/experiments/_dem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/experiments/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/frame.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.175152 eradiate-0.26.2rc1/src/eradiate/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/_bitmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/_bsdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/kernel/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.175152 eradiate-0.26.2rc1/src/eradiate/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/notebook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/notebook/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.175152 eradiate-0.26.2rc1/src/eradiate/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/pipelines/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/pipelines/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24859 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/pipelines/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/quad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.175152 eradiate-0.26.2rc1/src/eradiate/radprops/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/radprops/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/radprops/_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/radprops/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/radprops/absorption.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/radprops/rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/rng.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.179152 eradiate-0.26.2rc1/src/eradiate/scenes/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.179152 eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29357 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_molecular.py
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.179152 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_canopies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_canopy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)    39011 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_rami_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)    17140 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.183152 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_black.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_hapke.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_opacity_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_rpv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_rtls.py
--rw-r--r--   0 runner    (1001) docker     (127)    17684 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.183152 eradiate-0.26.2rc1/src/eradiate/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/illumination/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_astro_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.183152 eradiate-0.26.2rc1/src/eradiate/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/integrators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/integrators/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/integrators/_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.187152 eradiate-0.26.2rc1/src/eradiate/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)    22448 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/_perspective.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/measure/_radiancemeter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.187152 eradiate-0.26.2rc1/src/eradiate/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/phase/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/phase/_blend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/phase/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/phase/_hg.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/phase/_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/phase/_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/phase/_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.187152 eradiate-0.26.2rc1/src/eradiate/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/shapes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.191152 eradiate-0.26.2rc1/src/eradiate/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/spectra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_multi_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.191152 eradiate-0.26.2rc1/src/eradiate/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/surface/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/surface/_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/surface/_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/surface/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/scenes/surface/_dem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.191152 eradiate-0.26.2rc1/src/eradiate/spectral/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/spectral/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17480 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/spectral/ckd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/spectral/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/spectral/mono.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/spectral/spectral_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    26484 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.191152 eradiate-0.26.2rc1/src/eradiate/test_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/test_tools/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/test_tools/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/test_tools/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/test_tools/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/units.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.191152 eradiate-0.26.2rc1/src/eradiate/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11933 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13952 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/util/numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/util/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.195152 eradiate-0.26.2rc1/src/eradiate/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/xarray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/xarray/_accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/xarray/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/src/eradiate/xarray/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.215153 eradiate-0.26.2rc1/src/eradiate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-03-15 15:56:47.000000 eradiate-0.26.2rc1/src/eradiate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22586 2024-03-15 15:56:47.000000 eradiate-0.26.2rc1/src/eradiate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:56:47.000000 eradiate-0.26.2rc1/src/eradiate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 15:56:47.000000 eradiate-0.26.2rc1/src/eradiate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-15 15:56:47.000000 eradiate-0.26.2rc1/src/eradiate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-15 15:56:47.000000 eradiate-0.26.2rc1/src/eradiate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.195152 eradiate-0.26.2rc1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.195152 eradiate-0.26.2rc1/tests/01_eradiate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.195152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.199152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_safe_online.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.199152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.199152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.199152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/pipelines/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/pipelines/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/pipelines/test_logic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.199152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/test_absorption.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/test_us76_approx.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/test_zgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.203153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.203153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.203153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.203153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_hapke.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rtls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.207152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.207152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.207152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.207152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_blend.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_hg.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.207152 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.211153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_multi_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.211153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    29486 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/test_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.211153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/spectral/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/spectral/test_ckd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/spectral/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/spectral/test_mono.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_quad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.211153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_tools/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_warp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.211153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/util/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/util/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.211153 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/xarray/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/01_unit/xarray/test_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.215153 eradiate-0.26.2rc1/tests/01_eradiate/02_system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_albedo.py
--rw-r--r--   0 runner    (1001) docker     (127)    25384 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_atmosphere_rpv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_ckd_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_irradiance_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_kernel_render_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_maximum_scene_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_mdistant_insitu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_onedim_phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_onedim_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_spectral_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.215153 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.215153 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/atmospheres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/atmospheres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.215153 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/rami4atm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/rami4atm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:47.215153 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/romc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/romc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/romc/test_het01.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/romc/test_het04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/03_regression/romc/test_het06.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/01_eradiate/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-15 15:56:38.000000 eradiate-0.26.2rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.050712 eradiate-0.26.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.958712 eradiate-0.26.3rc1/.devcontainer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      135 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.devcontainer/create-command.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.958712 eradiate-0.26.3rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.962712 eradiate-0.26.3rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.962712 eradiate-0.26.3rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-04-15 15:55:33.050712 eradiate-0.26.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.962712 eradiate-0.26.3rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.962712 eradiate-0.26.3rc1/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_ext/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_ext/pluginparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.962712 eradiate-0.26.3rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)    17013 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32795 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25531 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-darkgrey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34059 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-darkgrey.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18587 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34061 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.950712 eradiate-0.26.3rc1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.966712 eradiate-0.26.3rc1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.966712 eradiate-0.26.3rc1/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/_templates/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/convert_figures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.974712 eradiate-0.26.3rc1/docs/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    20540 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/atmosphere_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/atmosphere_attributes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28149 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-east_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32937 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-east_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28852 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-east_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35278 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-east_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-north_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32862 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-north_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28115 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-north_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32455 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-north_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28153 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-south_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32939 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-south_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28118 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-south_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32455 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-south_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28178 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-west_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32935 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-west_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-west_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32437 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/azimuth-west_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/cartesian-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15939 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/cartesian-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25301 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/cuboid_leaf_cloud_params.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/cuboid_leaf_cloud_params.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.974712 eradiate-0.26.3rc1/docs/fig/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/diagrams/class_diagram_biosphere.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/diagrams/package.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)    40438 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/eradiate-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/icon_eradiate.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38873 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/package.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57417 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/package.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32384 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/radiancemeter_hsphere.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43351 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/radiancemeter_hsphere.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    36773 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/radiancemeter_plane.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31853 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/radiancemeter_plane.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/requirement_layers.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/requirement_layers.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    21451 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/solid_2017.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spectral_discretization_ckd_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16459 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27127 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spherical-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19861 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/spherical-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/fig/thuillier_2003.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/generate_md_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/generate_rst_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/generate_rst_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/index_latex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    17968 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.974712 eradiate-0.26.3rc1/docs/rst/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22779 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/dependencies.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.974712 eradiate-0.26.3rc1/docs/rst/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/developer_guide/design_atmosphere.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/developer_guide/dev_install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/developer_guide/factory_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/developer_guide/lazy_loading.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/developer_guide/scene_generator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/developer_guide/update.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/maintainer_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.978712 eradiate-0.26.3rc1/docs/rst/reference_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/attrs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/converters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/eradiate_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/experiments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/factory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/frame.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/kernel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/mode.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/notebook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/quad.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/rng.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/spectral.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/srf_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/test_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/units.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/warp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_api/xarray.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.978712 eradiate-0.26.3rc1/docs/rst/reference_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/reference_plugins/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.982712 eradiate-0.26.3rc1/docs/rst/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.982712 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/absorption.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.982712 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26889 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/fig/line.png
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/homogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/molecular.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/particle_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/basic_concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/conventions.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.986712 eradiate-0.26.3rc1/docs/rst/user_guide/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/absorption.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/atmosphere_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/atmosphere_thermoprops.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.986712 eradiate-0.26.3rc1/docs/rst/user_guide/data/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    30117 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59107 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/fig/pt_points.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28580 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/particle_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/solar_irradiance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/data/srf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/onedim_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/package_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/scene_loader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/spectral_discretization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/rst/user_guide/unit_guide_user.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.986712 eradiate-0.26.3rc1/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/src/reference_cli.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.986712 eradiate-0.26.3rc1/docs/src/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/src/release_notes/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/src/release_notes/v0.23.x_and_older.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/src/release_notes/v0.24.x.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/src/release_notes/v0.25.x.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/docs/src/release_notes/v0.26.x.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.986712 eradiate-0.26.3rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/check_conda_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.994712 eradiate-0.26.3rc1/requirements/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)    22740 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-dependencies-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-dependencies-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-dependencies-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    44654 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-dev-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    37451 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-dev-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    40096 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-dev-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    30111 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-docs-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    21006 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-docs-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-docs-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22740 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-main-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-main-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-main-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    44654 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-optional-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    37451 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-optional-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    40096 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-optional-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-optional.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    26200 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-recommended-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    24478 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-recommended-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    25980 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-recommended-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-recommended.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-tests-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-tests-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)    16990 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-tests-win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/conda/environment-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/copy_envvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/environment.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/layered.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/make_conda_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/make_pip_in_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/make_pip_txt_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.994712 eradiate-0.26.3rc1/requirements/pip/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/dependencies.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-15 15:55:27.000000 eradiate-0.26.3rc1/requirements/pip/dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/dev.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/docs.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/main.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/main.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/optional.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/optional.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/recommended.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/recommended.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-15 15:55:27.000000 eradiate-0.26.3rc1/requirements/pip/recommended.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/tests.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/requirements/pip/tests.lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/setpath.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/setpath.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/setpath.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:55:33.050712 eradiate-0.26.3rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.950712 eradiate-0.26.3rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:32.998712 eradiate-0.26.3rc1/src/eradiate/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9405 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11586 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/cfconventions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.002712 eradiate-0.26.3rc1/src/eradiate/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/cli/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/cli/srf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.002712 eradiate-0.26.3rc1/src/eradiate/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/_safe_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211295 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/downloads_all.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16905 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/data/downloads_minimal.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.002712 eradiate-0.26.3rc1/src/eradiate/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/experiments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/experiments/_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/experiments/_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14479 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/experiments/_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/experiments/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/experiments/_dem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/experiments/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/frame.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.006712 eradiate-0.26.3rc1/src/eradiate/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/_bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/_bsdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/kernel/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.006712 eradiate-0.26.3rc1/src/eradiate/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/notebook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/notebook/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.006712 eradiate-0.26.3rc1/src/eradiate/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/pipelines/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/pipelines/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24859 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/pipelines/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/quad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.006712 eradiate-0.26.3rc1/src/eradiate/radprops/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/radprops/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/radprops/_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/radprops/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/radprops/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/radprops/rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/rng.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.010712 eradiate-0.26.3rc1/src/eradiate/scenes/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.010712 eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29357 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_molecular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.010712 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_canopies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_canopy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39011 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_rami_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17140 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.014712 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_black.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_hapke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_opacity_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_rtls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17684 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.014712 eradiate-0.26.3rc1/src/eradiate/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/illumination/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_astro_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.014712 eradiate-0.26.3rc1/src/eradiate/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/integrators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/integrators/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/integrators/_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.018712 eradiate-0.26.3rc1/src/eradiate/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22448 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/measure/_radiancemeter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.018712 eradiate-0.26.3rc1/src/eradiate/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/phase/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/phase/_blend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/phase/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/phase/_hg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/phase/_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/phase/_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/phase/_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.018712 eradiate-0.26.3rc1/src/eradiate/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/shapes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.022712 eradiate-0.26.3rc1/src/eradiate/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/spectra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_multi_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.022712 eradiate-0.26.3rc1/src/eradiate/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/surface/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/surface/_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/surface/_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/surface/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/scenes/surface/_dem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.022712 eradiate-0.26.3rc1/src/eradiate/spectral/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/spectral/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17480 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/spectral/ckd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/spectral/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/spectral/mono.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/spectral/spectral_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26484 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.022712 eradiate-0.26.3rc1/src/eradiate/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/test_tools/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/test_tools/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/test_tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/test_tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/units.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.022712 eradiate-0.26.3rc1/src/eradiate/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11933 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13952 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/util/numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/util/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.026712 eradiate-0.26.3rc1/src/eradiate/xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/xarray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/xarray/_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/xarray/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/src/eradiate/xarray/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.046712 eradiate-0.26.3rc1/src/eradiate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-04-15 15:55:32.000000 eradiate-0.26.3rc1/src/eradiate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22586 2024-04-15 15:55:32.000000 eradiate-0.26.3rc1/src/eradiate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:55:32.000000 eradiate-0.26.3rc1/src/eradiate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 15:55:32.000000 eradiate-0.26.3rc1/src/eradiate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-15 15:55:32.000000 eradiate-0.26.3rc1/src/eradiate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 15:55:32.000000 eradiate-0.26.3rc1/src/eradiate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.026712 eradiate-0.26.3rc1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.026712 eradiate-0.26.3rc1/tests/01_eradiate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.026712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.030712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_safe_online.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.030712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.030712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.030712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/pipelines/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/pipelines/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/pipelines/test_logic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.030712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/test_absorption.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/test_us76_approx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/test_zgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.034712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.034712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.034712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.034712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_hapke.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rtls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.038712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.038712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.038712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.038712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/phase/test_blend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/phase/test_hg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.038712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.042712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_multi_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.042712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/surface/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/surface/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29486 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.042712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/spectral/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/spectral/test_ckd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/spectral/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/spectral/test_mono.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_quad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.042712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_tools/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_warp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.042712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/util/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/util/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.042712 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/xarray/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/01_unit/xarray/test_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.046712 eradiate-0.26.3rc1/tests/01_eradiate/02_system/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_albedo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25384 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_atmosphere_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_ckd_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_irradiance_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_kernel_render_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_maximum_scene_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_mdistant_insitu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_onedim_phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_onedim_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_spectral_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.046712 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.046712 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/atmospheres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/atmospheres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.046712 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/rami4atm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/rami4atm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:33.046712 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/romc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/romc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/romc/test_het01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/romc/test_het04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/03_regression/romc/test_het06.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/01_eradiate/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-15 15:55:20.000000 eradiate-0.26.3rc1/tests/conftest.py
```

### Comparing `eradiate-0.26.2rc1/.clang-format` & `eradiate-0.26.3rc1/.clang-format`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/.devcontainer/devcontainer.json` & `eradiate-0.26.3rc1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `eradiate-0.26.3rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `eradiate-0.26.3rc1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/.github/pull_request_template.md` & `eradiate-0.26.3rc1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/.github/workflows/cd.yml` & `eradiate-0.26.3rc1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/.github/workflows/ci.yml` & `eradiate-0.26.3rc1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/.pre-commit-config.yaml` & `eradiate-0.26.3rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/.readthedocs.yml` & `eradiate-0.26.3rc1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/CITATION.cff` & `eradiate-0.26.3rc1/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 identifiers:
   - type: doi
     value: 10.5281/zenodo.7224314
     description: Latest version on Zenodo
 repository-code: 'https://github.com/eradiate/eradiate'
 url: 'https://www.eradiate.eu'
 license: LGPL-3.0
-version: 0.26.2
-date-released: '2024-03-15'
+version: 0.26.3
+date-released: '2024-04-15'
```

### Comparing `eradiate-0.26.2rc1/CONTRIBUTING.md` & `eradiate-0.26.3rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/LICENSE` & `eradiate-0.26.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/Makefile` & `eradiate-0.26.3rc1/Makefile`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/PKG-INFO` & `eradiate-0.26.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.26.2rc1
+Version: 0.26.3rc1
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: eradiate-mitsuba==0.2.0
+Requires-Dist: eradiate-mitsuba==0.2.1
 Requires-Dist: aenum
 Requires-Dist: attrs>=22.2
 Requires-Dist: click
 Requires-Dist: dessinemoi>=23.1.0
 Requires-Dist: environ-config
 Requires-Dist: importlib_resources
 Requires-Dist: joseki>=2.6.0
@@ -30,15 +30,15 @@
 Requires-Dist: ruamel.yaml
 Requires-Dist: scipy
 Requires-Dist: sf-hamilton>=1.40
 Requires-Dist: shellingham!=1.5.1
 Requires-Dist: tqdm
 Requires-Dist: typer>=0.9.0
 Requires-Dist: xarray!=0.20.*,>=0.19
-Requires-Dist: eradiate-mitsuba==0.2.0
+Requires-Dist: eradiate-mitsuba==0.2.1
 Provides-Extra: recommended
 Requires-Dist: aabbtree; extra == "recommended"
 Requires-Dist: astropy; extra == "recommended"
 Requires-Dist: ipython; extra == "recommended"
 Requires-Dist: ipywidgets; extra == "recommended"
 Requires-Dist: jupyterlab; extra == "recommended"
 Requires-Dist: python-dateutil; extra == "recommended"
```

### Comparing `eradiate-0.26.2rc1/README.md` & `eradiate-0.26.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/Makefile` & `eradiate-0.26.3rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_ext/exec.py` & `eradiate-0.26.3rc1/docs/_ext/exec.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_ext/pluginparameters.py` & `eradiate-0.26.3rc1/docs/_ext/pluginparameters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-black.png` & `eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-black.svg` & `eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-black.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-darkgrey.png` & `eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-darkgrey.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-darkgrey.svg` & `eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-darkgrey.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-white.png` & `eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-white.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_static/eradiate-logo-typo-white.svg` & `eradiate-0.26.3rc1/docs/_static/eradiate-logo-typo-white.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_templates/autosummary/module.rst` & `eradiate-0.26.3rc1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/_templates/sections/footer-content.html` & `eradiate-0.26.3rc1/docs/_templates/sections/footer-content.html`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/conf.py` & `eradiate-0.26.3rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/atmosphere_attributes.png` & `eradiate-0.26.3rc1/docs/fig/atmosphere_attributes.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/atmosphere_attributes.svg` & `eradiate-0.26.3rc1/docs/fig/atmosphere_attributes.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-east_left.png` & `eradiate-0.26.3rc1/docs/fig/azimuth-east_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-east_left.svg` & `eradiate-0.26.3rc1/docs/fig/azimuth-east_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-east_right.png` & `eradiate-0.26.3rc1/docs/fig/azimuth-east_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-east_right.svg` & `eradiate-0.26.3rc1/docs/fig/azimuth-east_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-north_left.png` & `eradiate-0.26.3rc1/docs/fig/azimuth-north_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-north_left.svg` & `eradiate-0.26.3rc1/docs/fig/azimuth-north_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-north_right.png` & `eradiate-0.26.3rc1/docs/fig/azimuth-north_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-north_right.svg` & `eradiate-0.26.3rc1/docs/fig/azimuth-north_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-south_left.png` & `eradiate-0.26.3rc1/docs/fig/azimuth-south_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-south_left.svg` & `eradiate-0.26.3rc1/docs/fig/azimuth-south_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-south_right.png` & `eradiate-0.26.3rc1/docs/fig/azimuth-south_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-south_right.svg` & `eradiate-0.26.3rc1/docs/fig/azimuth-south_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-west_left.png` & `eradiate-0.26.3rc1/docs/fig/azimuth-west_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-west_left.svg` & `eradiate-0.26.3rc1/docs/fig/azimuth-west_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-west_right.png` & `eradiate-0.26.3rc1/docs/fig/azimuth-west_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/azimuth-west_right.svg` & `eradiate-0.26.3rc1/docs/fig/azimuth-west_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/cartesian-coordinate-system.png` & `eradiate-0.26.3rc1/docs/fig/cartesian-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/cartesian-coordinate-system.svg` & `eradiate-0.26.3rc1/docs/fig/cartesian-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/cuboid_leaf_cloud_params.png` & `eradiate-0.26.3rc1/docs/fig/cuboid_leaf_cloud_params.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/cuboid_leaf_cloud_params.svg` & `eradiate-0.26.3rc1/docs/fig/cuboid_leaf_cloud_params.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/diagrams/class_diagram_biosphere.drawio` & `eradiate-0.26.3rc1/docs/fig/diagrams/class_diagram_biosphere.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio` & `eradiate-0.26.3rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/diagrams/package.drawio` & `eradiate-0.26.3rc1/docs/fig/diagrams/package.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/eradiate-logo-typo-black.png` & `eradiate-0.26.3rc1/docs/fig/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/eradiate-logo.svg` & `eradiate-0.26.3rc1/docs/fig/eradiate-logo.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/icon_eradiate.png` & `eradiate-0.26.3rc1/docs/fig/icon_eradiate.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/package.png` & `eradiate-0.26.3rc1/docs/fig/package.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/package.svg` & `eradiate-0.26.3rc1/docs/fig/package.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/radiancemeter_hsphere.png` & `eradiate-0.26.3rc1/docs/fig/radiancemeter_hsphere.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/radiancemeter_hsphere.svg` & `eradiate-0.26.3rc1/docs/fig/radiancemeter_hsphere.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/radiancemeter_plane.png` & `eradiate-0.26.3rc1/docs/fig/radiancemeter_plane.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/radiancemeter_plane.svg` & `eradiate-0.26.3rc1/docs/fig/radiancemeter_plane.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/requirement_layers.png` & `eradiate-0.26.3rc1/docs/fig/requirement_layers.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/requirement_layers.svg` & `eradiate-0.26.3rc1/docs/fig/requirement_layers.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/solid_2017.png` & `eradiate-0.26.3rc1/docs/fig/solid_2017.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spectral_discretization_ckd_atm_interval.png` & `eradiate-0.26.3rc1/docs/fig/spectral_discretization_ckd_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png` & `eradiate-0.26.3rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png` & `eradiate-0.26.3rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png` & `eradiate-0.26.3rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_atm_interval.png` & `eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_atm_isolated.png` & `eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png` & `eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png` & `eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png` & `eradiate-0.26.3rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spherical-coordinate-system.png` & `eradiate-0.26.3rc1/docs/fig/spherical-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/spherical-coordinate-system.svg` & `eradiate-0.26.3rc1/docs/fig/spherical-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/fig/thuillier_2003.png` & `eradiate-0.26.3rc1/docs/fig/thuillier_2003.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/generate_md_cli.py` & `eradiate-0.26.3rc1/docs/generate_md_cli.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/generate_rst_api.py` & `eradiate-0.26.3rc1/docs/generate_rst_api.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/generate_rst_plugins.py` & `eradiate-0.26.3rc1/docs/generate_rst_plugins.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/index.rst` & `eradiate-0.26.3rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/make.bat` & `eradiate-0.26.3rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/references.bib` & `eradiate-0.26.3rc1/docs/references.bib`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/contributing.rst` & `eradiate-0.26.3rc1/docs/rst/contributing.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/dependencies.rst` & `eradiate-0.26.3rc1/docs/rst/dependencies.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/developer_guide/design_atmosphere.rst` & `eradiate-0.26.3rc1/docs/rst/developer_guide/design_atmosphere.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/developer_guide/dev_install.rst` & `eradiate-0.26.3rc1/docs/rst/developer_guide/dev_install.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/developer_guide/factory_guide.rst` & `eradiate-0.26.3rc1/docs/rst/developer_guide/factory_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/developer_guide/lazy_loading.rst` & `eradiate-0.26.3rc1/docs/rst/developer_guide/lazy_loading.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst` & `eradiate-0.26.3rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/developer_guide/scene_generator.rst` & `eradiate-0.26.3rc1/docs/rst/developer_guide/scene_generator.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/developer_guide/update.rst` & `eradiate-0.26.3rc1/docs/rst/developer_guide/update.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/maintainer_guide.rst` & `eradiate-0.26.3rc1/docs/rst/maintainer_guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -328,20 +328,26 @@
 branch of the PR.
 
 .. _sec-maintainer_guide-release:
 
 Preparing a  release
 --------------------
 
-1. Update the change log.
-2. Update the version and release date fields in `CITATION.cff`.
-3. Tag the target commit for release.
+1. Make sure all tests pass.
+2. Update the change log.
+3. Update the version and release date fields in `CITATION.cff`.
+4. Create a draft release on GitHub and update it.
+5. Using release candidates, make sure that built Pyhon wheels will work as
+   expected.
+6. Finalize release notes and create the release tag. **Make sure that the \
+   release commit is referenced only by one tag.**
+7. Build and upload Python wheels.
 
-Tagging a commit for release
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Tagging a commit for release manually
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Eradiate picks up its version number using the `setuptools-scm <https://github.com/pypa/setuptools_scm>`_
 package. Under the hood, it uses Git tags and the ``git describe`` command,
 which only picks up annotated tags. To make sure that the tags will be
 correctly picked up,
 `make sure that they are annotated <https://stackoverflow.com/questions/4154485/git-describe-ignores-a-tag>`_
 using
```

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/data.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/data.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/eradiate_core.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/eradiate_core.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/experiments.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/experiments.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/factory.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/factory.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/index.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/kernel.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/kernel.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/pipelines.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/pipelines.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/scenes.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/scenes.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/spectral.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/spectral.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/srf_tools.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/srf_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/test_tools.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/test_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/reference_api/xarray.rst` & `eradiate-0.26.3rc1/docs/rst/reference_api/xarray.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/absorption.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png` & `eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png` & `eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/fig/line.png` & `eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/fig/line.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/intro.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/molecular.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/molecular.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/basic_concepts.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/basic_concepts.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/conventions.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/conventions.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/absorption.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/atmosphere_radprops.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/atmosphere_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/atmosphere_thermoprops.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/atmosphere_thermoprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/fig/pt_points.png` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/fig/pt_points.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/intro.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/particle_radprops.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/particle_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/solar_irradiance.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/solar_irradiance.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/data/srf.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/data/srf.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/index.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/install.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/install.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/onedim_experiment.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/onedim_experiment.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/package_structure.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/package_structure.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/scene_loader.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/scene_loader.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/spectral_discretization.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/spectral_discretization.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/rst/user_guide/unit_guide_user.rst` & `eradiate-0.26.3rc1/docs/rst/user_guide/unit_guide_user.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/src/reference_cli.md` & `eradiate-0.26.3rc1/docs/src/reference_cli.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ```console
 $ eradiate [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
-* `--log-level [CRITICAL|ERROR|WARNING|INFO|DEBUG|NOTSET]`: Set log level.  [default: LogLevel.WARNING]
+* `--log-level [CRITICAL|ERROR|WARNING|INFO|DEBUG|NOTSET]`: Set log level.  [default: WARNING]
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `data`: Manage data.
```

### Comparing `eradiate-0.26.2rc1/docs/src/release_notes/index.md` & `eradiate-0.26.3rc1/docs/src/release_notes/index.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/src/release_notes/v0.23.x_and_older.md` & `eradiate-0.26.3rc1/docs/src/release_notes/v0.23.x_and_older.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/src/release_notes/v0.24.x.md` & `eradiate-0.26.3rc1/docs/src/release_notes/v0.24.x.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/src/release_notes/v0.25.x.md` & `eradiate-0.26.3rc1/docs/src/release_notes/v0.25.x.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/docs/src/release_notes/v0.26.x.md` & `eradiate-0.26.3rc1/docs/src/release_notes/v0.26.x.md`

 * *Files 11% similar despite different names*

```diff
@@ -97,7 +97,22 @@
 
 ### Fixed
 
 * When opening a molecular absorption coefficient database, bins are sorted by
   ascending lower bound values ({ghpr}`395`).
 * Fix a bug in post-processing pipelines where radiosity node would not appear
   for in situ sensors ({ghpr}`395`).
+
+## v0.26.3 (15th April 2024)
+
+This is a fix release.
+
+### Changed
+
+* Required custom Mitsuba build bumped to v0.2.1 (based on Mitsuba v3.4.1). This
+  update contains fixes for the Hapke BSDF plugin.
+
+### Fixed
+
+* Fix incorrect path to the `komodo` dataset ({ghpr}`398`).
+* Online data stores now make additional attempts if a download fails
+  ({ghpr}`398`).
```

### Comparing `eradiate-0.26.2rc1/pyproject.toml` & `eradiate-0.26.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/_utils.py` & `eradiate-0.26.3rc1/requirements/_utils.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-dependencies-linux-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-dependencies-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-dependencies-osx-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-dependencies-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-dependencies-win-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-dependencies-win-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-dev-linux-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-dev-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-dev-osx-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-dev-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-dev-win-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-dev-win-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-dev.yml` & `eradiate-0.26.3rc1/requirements/conda/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-docs-linux-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-docs-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-docs-osx-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-docs-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-docs-win-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-docs-win-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-docs.yml` & `eradiate-0.26.3rc1/requirements/conda/environment-docs.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-main-linux-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-main-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-main-osx-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-main-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-main-win-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-main-win-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-optional-linux-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-optional-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-optional-osx-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-optional-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-optional-win-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-optional-win-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-optional.yml` & `eradiate-0.26.3rc1/requirements/conda/environment-optional.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-recommended-linux-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-recommended-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-recommended-osx-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-recommended-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-recommended-win-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-recommended-win-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-tests-linux-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-tests-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-tests-osx-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-tests-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/conda/environment-tests-win-64.lock` & `eradiate-0.26.3rc1/requirements/conda/environment-tests-win-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/copy_envvars.py` & `eradiate-0.26.3rc1/requirements/copy_envvars.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/layered.yml` & `eradiate-0.26.3rc1/requirements/layered.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file establishes dependencies between layered requirement specs
 dependencies:
   includes:
     - main
   constraints:
     - optional
   packages:
-    - "eradiate-mitsuba==0.2.0"
+    - "eradiate-mitsuba==0.2.1"
 
 main:
   packages:
     - "aenum"
     - "attrs>=22.2"
     - "click"
     - "dessinemoi>=23.1.0"
@@ -79,8 +79,8 @@
     - "setuptools>=61"  # Required by dependency management scripts
     - "networkx>=3.1"  # Required by dependency management scripts
 
 optional:
   includes:
     - dev
   packages:
-    - "eradiate-mitsuba==0.2.0"
+    - "eradiate-mitsuba==0.2.1"
```

### Comparing `eradiate-0.26.2rc1/requirements/make_conda_env.py` & `eradiate-0.26.3rc1/requirements/make_conda_env.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/make_pip_in_files.py` & `eradiate-0.26.3rc1/requirements/make_pip_in_files.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/make_pip_txt_files.py` & `eradiate-0.26.3rc1/requirements/make_pip_txt_files.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/pip/dependencies.lock.txt` & `eradiate-0.26.3rc1/requirements/pip/dependencies.lock.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/pip/dev.lock.txt` & `eradiate-0.26.3rc1/requirements/pip/dev.lock.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/pip/docs.lock.txt` & `eradiate-0.26.3rc1/requirements/pip/docs.lock.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/pip/main.lock.txt` & `eradiate-0.26.3rc1/requirements/pip/main.lock.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/pip/optional.lock.txt` & `eradiate-0.26.3rc1/requirements/pip/optional.lock.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/pip/recommended.lock.txt` & `eradiate-0.26.3rc1/requirements/pip/recommended.lock.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/requirements/pip/tests.lock.txt` & `eradiate-0.26.3rc1/requirements/pip/tests.lock.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/setpath.sh` & `eradiate-0.26.3rc1/setpath.sh`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/__init__.pyi` & `eradiate-0.26.3rc1/src/eradiate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/_config.py` & `eradiate-0.26.3rc1/src/eradiate/_config.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/_factory.py` & `eradiate-0.26.3rc1/src/eradiate/_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/_mode.py` & `eradiate-0.26.3rc1/src/eradiate/_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/attrs.py` & `eradiate-0.26.3rc1/src/eradiate/attrs.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/cfconventions.py` & `eradiate-0.26.3rc1/src/eradiate/cfconventions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/cli/__init__.py` & `eradiate-0.26.3rc1/src/eradiate/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/cli/data.py` & `eradiate-0.26.3rc1/src/eradiate/cli/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                     / "src"
                     / "eradiate"
                     / "data"
                     / "downloads_minimal.yml"
                 )
         console.print(f"Reading file list from '{from_file}'")
         yaml = YAML()
-        file_list = yaml.load(from_file)
+        file_list = yaml.load(Path(from_file))
 
     for filename in file_list:
         try:
             console.print(f"[blue]Fetching '{filename}'[/]")
             path = eradiate.data.data_store.fetch(filename)
         except DataError:
             console.print("[red]✗[/] not found")
@@ -166,15 +166,15 @@
             console.print(f"[green]✓[/] found \[{path}]")
 
 
 @app.command()
 def purge_cache(
     keep: Annotated[
         bool, typer.Option("--keep", "-k", help="Keep registered files.")
-    ] = False
+    ] = False,
 ):
     """
     Purge the cache of online data stores.
     """
     for data_store_id, data_store in eradiate.data.data_store.stores.items():
         console.print(
             f"[bold cyan]{data_store_id}[/] [{data_store.__class__.__name__}]"
```

### Comparing `eradiate-0.26.2rc1/src/eradiate/cli/show.py` & `eradiate-0.26.3rc1/src/eradiate/cli/show.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/cli/srf.py` & `eradiate-0.26.3rc1/src/eradiate/cli/srf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/contexts.py` & `eradiate-0.26.3rc1/src/eradiate/contexts.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/converters.py` & `eradiate-0.26.3rc1/src/eradiate/converters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/__init__.pyi` & `eradiate-0.26.3rc1/src/eradiate/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/_access.py` & `eradiate-0.26.3rc1/src/eradiate/data/_access.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/_blind_directory.py` & `eradiate-0.26.3rc1/src/eradiate/data/_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/_blind_online.py` & `eradiate-0.26.3rc1/src/eradiate/data/_blind_online.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from __future__ import annotations
 
+import logging
 import os
 import shutil
+import time
 import typing as t
 from pathlib import Path
 
 import attrs
 import pooch
 from requests import RequestException
 
 from ._core import DataStore, expand_rules
 from ..attrs import documented, parse_docs
 from ..exceptions import DataError
 from ..typing import PathLike
 from ..util.misc import LoggingContext
 
+logger = logging.getLogger(__name__)
+
 
 @parse_docs
 @attrs.define
 class BlindOnlineDataStore(DataStore):
     """
     Serve data downloaded from a remote source without integrity check.
     """
@@ -32,14 +36,21 @@
     path: Path = documented(
         attrs.field(converter=lambda x: Path(x).absolute()),
         type="Path",
         init_type="path-like",
         doc="Path to the local cache location.",
     )
 
+    attempts: int = documented(
+        attrs.field(default=3, converter=int),
+        type="int",
+        doc="Number of download attempts to make before giving up because of "
+        "connection errors.",
+    )
+
     @property
     def base_url(self) -> str:
         # Inherit docstring
         return self._base_url
 
     @property
     def registry(self) -> dict:
@@ -84,49 +95,70 @@
         If a compressed resource exists, it will be served automatically.
         For instance, if ``"foo.nc"`` is requested and ``"foo.nc.gz"`` is
         registered, the latter will be downloaded, decompressed and served as
         ``"foo.nc"``.
         """
 
         fname = Path(filename).as_posix()
+        url = self.base_url + fname
+        max_wait = 10
+        result = None
 
         with LoggingContext(
             pooch.get_logger(), level="WARNING"
         ):  # Silence pooch messages temporarily
-            url = self.base_url + fname
-            # Try first to get a compressed file
-            try:
-                return Path(
-                    pooch.retrieve(
-                        url + ".gz",
-                        known_hash=None,
-                        fname=fname + ".gz",
-                        path=self.path,
-                        processor=pooch.processors.Decompress(
-                            name=os.path.basename(fname)
-                        ),
+            for i in range(self.attempts):
+                # Try first to get a compressed file
+                try:
+                    result = Path(
+                        pooch.retrieve(
+                            url + ".gz",
+                            known_hash=None,
+                            fname=fname + ".gz",
+                            path=self.path,
+                            processor=pooch.processors.Decompress(
+                                name=os.path.basename(fname)
+                            ),
+                        )
                     )
-                )
-            except RequestException:
-                pass
+                    break
+                except RequestException:
+                    pass
 
                 # If no gzip-compressed file is available, try the actual file
                 try:
-                    return Path(
+                    result = Path(
                         pooch.retrieve(
                             url,
                             known_hash=None,
                             fname=fname,
                             path=self.path,
                         ),
                     )
-                except RequestException as e:
-                    raise DataError(
-                        f"file '{fname}' could not be retrieved from {self.base_url}"
-                    ) from e
+                    break
+                except RequestException:
+                    pass
+
+                # If we get here, it means download failed
+                retries_left = self.attempts - (i + 1)
+                logger.info(
+                    "Failed to download '%s'. "
+                    "Will attempt the download again %d more time%s.",
+                    fname,
+                    retries_left,
+                    "s" if retries_left > 1 else "",
+                )
+                time.sleep(min(i + 1, max_wait))
+
+        if result is None:
+            raise DataError(
+                f"file '{fname}' could not be retrieved from {self.base_url}"
+            )
+        else:
+            return result
 
     def purge(self, keep: None | str | list[str] = None) -> None:
         """
         Purge local storage location. The default behaviour is very aggressive
         and will wipe out the entire directory contents.
 
         Parameters
```

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/_core.py` & `eradiate-0.26.3rc1/src/eradiate/data/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/_multi.py` & `eradiate-0.26.3rc1/src/eradiate/data/_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/_safe_directory.py` & `eradiate-0.26.3rc1/src/eradiate/data/_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/_safe_online.py` & `eradiate-0.26.3rc1/src/eradiate/data/_safe_online.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
     path : path-like
         Path to the local cache location.
 
     registry_fname : path-like, optional
         Path to the registry file, relative to `path`.
 
+    attempts : int, default: 3
+        Number of download attempts to make before giving up because of
+        connection errors or a hash mismatch.
+
     Fields
     ------
     manager : pooch.Pooch
         The Pooch instance used to manage downloaded content.
 
     registry_fname : Path
         Path to the registry file, relative to `path`.
@@ -46,25 +50,30 @@
     This class basically wraps a :class:`pooch.Pooch` instance.
     """
 
     manager: pooch.Pooch = attrs.field()
     registry_fname: Path = attrs.field(converter=Path)
 
     def __init__(
-        self, base_url: str, path: PathLike, registry_fname: PathLike = "registry.txt"
+        self,
+        base_url: str,
+        path: PathLike,
+        registry_fname: PathLike = "registry.txt",
+        attempts: int = 3,
     ):
         # Initialize attributes
         if not base_url.endswith("/"):
             base_url += "/"
         path = Path(path).absolute()
 
         manager = pooch.create(
             base_url=base_url,
             path=path,
             registry=None,  # We'll load it later
+            retry_if_failed=attempts - 1,
         )
         self.__attrs_init__(manager=manager, registry_fname=registry_fname)
 
         # Initialize register load the registry
         registry = registry_from_file(self.registry_fetch())
         manager.registry = registry
 
@@ -92,14 +101,18 @@
         return Path(self.manager.path)
 
     @property
     def registry(self) -> dict[str, str]:
         # Inherit docstring
         return self.manager.registry
 
+    @property
+    def retry_if_failed(self):
+        return self.manager.retry_if_failed
+
     def registry_files(
         self, filter: t.Callable[[t.Any], bool] | None = None
     ) -> list[str]:
         """
         Get a list of registered files.
 
         Parameters
```

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/_store.py` & `eradiate-0.26.3rc1/src/eradiate/data/_store.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/_util.py` & `eradiate-0.26.3rc1/src/eradiate/data/_util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/downloads_all.yml` & `eradiate-0.26.3rc1/src/eradiate/data/downloads_all.yml`

 * *Files 0% similar despite different names*

```diff
@@ -366,16 +366,16 @@
 - spectra/srf/terra-modis-8-raw.nc
 - spectra/srf/terra-modis-9-raw.nc
 - tutorials/spectra/srf/aqua-modis-1.nc
 - tutorials/spectra/srf/aqua-modis-14.nc
 # Absorption coefficient datasets (monochromatic)
 - spectra/absorption/mono/gecko/gecko.nc
 - spectra/absorption/mono/gecko/metadata.json
+- spectra/absorption/mono/komodo/komodo.nc
 - spectra/absorption/mono/komodo/metadata.json
-- spectra/absorption/mono/komodo.nc
 # Absorption coefficient datasets (CKD): monotropa
 - spectra/absorption/ckd/monotropa/metadata.json
 - spectra/absorption/ckd/monotropa/index.csv
 - spectra/absorption/ckd/monotropa/monotropa-3200_3300.nc
 - spectra/absorption/ckd/monotropa/monotropa-3300_3400.nc
 - spectra/absorption/ckd/monotropa/monotropa-3400_3500.nc
 - spectra/absorption/ckd/monotropa/monotropa-3500_3600.nc
```

### Comparing `eradiate-0.26.2rc1/src/eradiate/data/downloads_minimal.yml` & `eradiate-0.26.3rc1/src/eradiate/data/downloads_minimal.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/exceptions.py` & `eradiate-0.26.3rc1/src/eradiate/exceptions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/experiments/_atmosphere.py` & `eradiate-0.26.3rc1/src/eradiate/experiments/_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/experiments/_canopy.py` & `eradiate-0.26.3rc1/src/eradiate/experiments/_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/experiments/_canopy_atmosphere.py` & `eradiate-0.26.3rc1/src/eradiate/experiments/_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/experiments/_core.py` & `eradiate-0.26.3rc1/src/eradiate/experiments/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/experiments/_dem.py` & `eradiate-0.26.3rc1/src/eradiate/experiments/_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/experiments/_helpers.py` & `eradiate-0.26.3rc1/src/eradiate/experiments/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/frame.py` & `eradiate-0.26.3rc1/src/eradiate/frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/kernel/__init__.pyi` & `eradiate-0.26.3rc1/src/eradiate/kernel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/kernel/_bitmap.py` & `eradiate-0.26.3rc1/src/eradiate/kernel/_bitmap.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/kernel/_bsdf.py` & `eradiate-0.26.3rc1/src/eradiate/kernel/_bsdf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/kernel/_kernel_dict.py` & `eradiate-0.26.3rc1/src/eradiate/kernel/_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/kernel/_render.py` & `eradiate-0.26.3rc1/src/eradiate/kernel/_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/kernel/_versions.py` & `eradiate-0.26.3rc1/src/eradiate/kernel/_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Upon import, this module checks if the kernel dependencies are correctly set up.
 """
 
 from importlib.metadata import PackageNotFoundError, version
 
 # Internal constants
 REQUIRED_MITSUBA_VERSION = "3.4.1"
-REQUIRED_MITSUBA_PATCH_VERSION = "0.2.0"
+REQUIRED_MITSUBA_PATCH_VERSION = "0.2.1"
 
 
 def find_drjit():
     # Check if Dr.Jit and Mitsuba can be imported successfully
     try:
         __import__("drjit")
         return True
```

### Comparing `eradiate-0.26.2rc1/src/eradiate/kernel/gridvolume.py` & `eradiate-0.26.3rc1/src/eradiate/kernel/gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/kernel/logging.py` & `eradiate-0.26.3rc1/src/eradiate/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/kernel/transform.py` & `eradiate-0.26.3rc1/src/eradiate/kernel/transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/notebook/__init__.py` & `eradiate-0.26.3rc1/src/eradiate/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/notebook/tutorials.py` & `eradiate-0.26.3rc1/src/eradiate/notebook/tutorials.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/pipelines/__init__.py` & `eradiate-0.26.3rc1/src/eradiate/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/pipelines/core.py` & `eradiate-0.26.3rc1/src/eradiate/pipelines/core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/pipelines/definitions.py` & `eradiate-0.26.3rc1/src/eradiate/pipelines/definitions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/pipelines/logic.py` & `eradiate-0.26.3rc1/src/eradiate/pipelines/logic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/plot.py` & `eradiate-0.26.3rc1/src/eradiate/plot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/quad.py` & `eradiate-0.26.3rc1/src/eradiate/quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/radprops/_atmosphere.py` & `eradiate-0.26.3rc1/src/eradiate/radprops/_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/radprops/_core.py` & `eradiate-0.26.3rc1/src/eradiate/radprops/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/radprops/absorption.py` & `eradiate-0.26.3rc1/src/eradiate/radprops/absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/radprops/rayleigh.py` & `eradiate-0.26.3rc1/src/eradiate/radprops/rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/rng.py` & `eradiate-0.26.3rc1/src/eradiate/rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/__init__.pyi` & `eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_homogeneous.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_molecular.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_molecular.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_particle_dist.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/atmosphere/_particle_layer.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/atmosphere/_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/__init__.pyi` & `eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_canopies.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_canopies.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_canopy_loader.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_canopy_loader.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_discrete.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_rami_scenarios.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_rami_scenarios.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/biosphere/_tree.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/biosphere/_tree.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_black.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_black.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_checkerboard.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_hapke.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_hapke.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_lambertian.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_opacity_mask.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_opacity_mask.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_rpv.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/bsdfs/_rtls.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/bsdfs/_rtls.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/geometry.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/geometry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_astro_object.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_astro_object.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_constant.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_directional.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/illumination/_spot.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/illumination/_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/integrators/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/integrators/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/integrators/_path_tracers.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/integrators/_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/measure/__init__.pyi` & `eradiate-0.26.3rc1/src/eradiate/scenes/measure/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/measure/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/measure/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/measure/_distant.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/measure/_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/measure/_distant_flux.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/measure/_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/measure/_hemispherical_distant.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/measure/_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/measure/_multi_distant.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/measure/_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/measure/_perspective.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/measure/_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/measure/_radiancemeter.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/measure/_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/phase/_blend.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/phase/_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/phase/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/phase/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/phase/_hg.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/phase/_hg.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/phase/_rayleigh.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/phase/_rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/phase/_tabulated.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/phase/_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_buffermesh.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_cuboid.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_filemesh.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_rectangle.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/shapes/_sphere.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/shapes/_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_interpolated.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_multi_delta.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_multi_delta.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_solar_irradiance.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/spectra/_uniform.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/spectra/_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/surface/_basic.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/surface/_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/surface/_central_patch.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/surface/_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/surface/_core.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/surface/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/scenes/surface/_dem.py` & `eradiate-0.26.3rc1/src/eradiate/scenes/surface/_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/spectral/ckd.py` & `eradiate-0.26.3rc1/src/eradiate/spectral/ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/spectral/index.py` & `eradiate-0.26.3rc1/src/eradiate/spectral/index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/spectral/mono.py` & `eradiate-0.26.3rc1/src/eradiate/spectral/mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/srf_tools.py` & `eradiate-0.26.3rc1/src/eradiate/srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/test_tools/plugin.py` & `eradiate-0.26.3rc1/src/eradiate/test_tools/plugin.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/test_tools/regression.py` & `eradiate-0.26.3rc1/src/eradiate/test_tools/regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/test_tools/types.py` & `eradiate-0.26.3rc1/src/eradiate/test_tools/types.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/test_tools/util.py` & `eradiate-0.26.3rc1/src/eradiate/test_tools/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/units.py` & `eradiate-0.26.3rc1/src/eradiate/units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/units.txt` & `eradiate-0.26.3rc1/src/eradiate/units.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/util/deprecation.py` & `eradiate-0.26.3rc1/src/eradiate/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/util/misc.py` & `eradiate-0.26.3rc1/src/eradiate/util/misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/util/numpydoc.py` & `eradiate-0.26.3rc1/src/eradiate/util/numpydoc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/util/sys_info.py` & `eradiate-0.26.3rc1/src/eradiate/util/sys_info.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/validators.py` & `eradiate-0.26.3rc1/src/eradiate/validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/warp.py` & `eradiate-0.26.3rc1/src/eradiate/warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/xarray/_accessors.py` & `eradiate-0.26.3rc1/src/eradiate/xarray/_accessors.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/xarray/_helpers.py` & `eradiate-0.26.3rc1/src/eradiate/xarray/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate/xarray/interp.py` & `eradiate-0.26.3rc1/src/eradiate/xarray/interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate.egg-info/PKG-INFO` & `eradiate-0.26.3rc1/src/eradiate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.26.2rc1
+Version: 0.26.3rc1
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: eradiate-mitsuba==0.2.0
+Requires-Dist: eradiate-mitsuba==0.2.1
 Requires-Dist: aenum
 Requires-Dist: attrs>=22.2
 Requires-Dist: click
 Requires-Dist: dessinemoi>=23.1.0
 Requires-Dist: environ-config
 Requires-Dist: importlib_resources
 Requires-Dist: joseki>=2.6.0
@@ -30,15 +30,15 @@
 Requires-Dist: ruamel.yaml
 Requires-Dist: scipy
 Requires-Dist: sf-hamilton>=1.40
 Requires-Dist: shellingham!=1.5.1
 Requires-Dist: tqdm
 Requires-Dist: typer>=0.9.0
 Requires-Dist: xarray!=0.20.*,>=0.19
-Requires-Dist: eradiate-mitsuba==0.2.0
+Requires-Dist: eradiate-mitsuba==0.2.1
 Provides-Extra: recommended
 Requires-Dist: aabbtree; extra == "recommended"
 Requires-Dist: astropy; extra == "recommended"
 Requires-Dist: ipython; extra == "recommended"
 Requires-Dist: ipywidgets; extra == "recommended"
 Requires-Dist: jupyterlab; extra == "recommended"
 Requires-Dist: python-dateutil; extra == "recommended"
```

### Comparing `eradiate-0.26.2rc1/src/eradiate.egg-info/SOURCES.txt` & `eradiate-0.26.3rc1/src/eradiate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/src/eradiate.egg-info/requires.txt` & `eradiate-0.26.3rc1/src/eradiate.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-eradiate-mitsuba==0.2.0
+eradiate-mitsuba==0.2.1
 aenum
 attrs>=22.2
 click
 dessinemoi>=23.1.0
 environ-config
 importlib_resources
 joseki>=2.6.0
@@ -17,15 +17,15 @@
 ruamel.yaml
 scipy
 sf-hamilton>=1.40
 shellingham!=1.5.1
 tqdm
 typer>=0.9.0
 xarray!=0.20.*,>=0.19
-eradiate-mitsuba==0.2.0
+eradiate-mitsuba==0.2.1
 
 [recommended]
 aabbtree
 astropy
 ipython
 ipywidgets
 jupyterlab
```

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_blind_directory.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_blind_online.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_core.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_datasets.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_multi.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_safe_directory.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/data/test_safe_online.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/data/test_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_atmosphere.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_core.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_dem.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/experiments/test_helpers.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/experiments/test_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_gridvolume.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_logging.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_render.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/kernel/test_transform.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/kernel/test_transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/pipelines/conftest.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/pipelines/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/pipelines/test_logic.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/pipelines/test_logic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/test_absorption.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/test_absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/radprops/test_zgrid.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/radprops/test_zgrid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_hapke.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_hapke.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rtls.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rtls.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_target.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/measure/test_target.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_blend.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/phase/test_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_core.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_multi_delta.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_multi_delta.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_basic.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/surface/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_dem.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/surface/test_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/test_core.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/scenes/test_loader.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/scenes/test_loader.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/spectral/test_ckd.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/spectral/test_ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/spectral/test_index.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/spectral/test_index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/spectral/test_mono.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/spectral/test_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_config.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_config.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_factory.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_frame.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_mode.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_quad.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_rng.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_srf_tools.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_tools/test_regression.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_tools/test_regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_units.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_validators.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/test_warp.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/test_warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/util/test_deprecation.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/util/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/util/test_misc.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/util/test_misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/xarray/conftest.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/xarray/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/01_unit/xarray/test_interp.py` & `eradiate-0.26.3rc1/tests/01_eradiate/01_unit/xarray/test_interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/conftest.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_albedo.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_albedo.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_atmosphere_rpv.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_atmosphere_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_basic.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_ckd_basic.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_ckd_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_irradiance_scaling.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_irradiance_scaling.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_kernel_render_benchmark.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_kernel_render_benchmark.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_maximum_scene_size.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_maximum_scene_size.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_mdistant_insitu.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_mdistant_insitu.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_onedim_phase.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_onedim_phase.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_onedim_symmetry.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_onedim_symmetry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/02_system/test_spectral_loop.py` & `eradiate-0.26.3rc1/tests/01_eradiate/02_system/test_spectral_loop.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py` & `eradiate-0.26.3rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py` & `eradiate-0.26.3rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py` & `eradiate-0.26.3rc1/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/03_regression/romc/test_het01.py` & `eradiate-0.26.3rc1/tests/01_eradiate/03_regression/romc/test_het01.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/03_regression/romc/test_het04.py` & `eradiate-0.26.3rc1/tests/01_eradiate/03_regression/romc/test_het04.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/03_regression/romc/test_het06.py` & `eradiate-0.26.3rc1/tests/01_eradiate/03_regression/romc/test_het06.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/01_eradiate/conftest.py` & `eradiate-0.26.3rc1/tests/01_eradiate/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.26.2rc1/tests/conftest.py` & `eradiate-0.26.3rc1/tests/conftest.py`

 * *Files identical despite different names*

