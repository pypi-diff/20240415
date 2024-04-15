# Comparing `tmp/elastic-5.2.0.0.tar.gz` & `tmp/elastic-5.2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elastic-5.2.0.0.tar", last modified: Mon Apr 15 20:29:17 2024, max compression
+gzip compressed data, was "elastic-5.2.1.0.tar", last modified: Mon Apr 15 20:51:54 2024, max compression
```

## Comparing `elastic-5.2.0.0.tar` & `elastic-5.2.1.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 20:29:13.000000 elastic-5.2.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.796260 elastic-5.2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.804260 elastic-5.2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-15 20:29:13.000000 elastic-5.2.0.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 20:29:13.000000 elastic-5.2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 20:29:13.000000 elastic-5.2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 20:29:13.000000 elastic-5.2.0.0/Contributors
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-15 20:29:13.000000 elastic-5.2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 20:29:13.000000 elastic-5.2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 20:29:17.824260 elastic-5.2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 20:29:13.000000 elastic-5.2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.804260 elastic-5.2.0.0/conda/
--rwxr-xr-x   0 runner    (1001) docker     (127)      282 2024-04-15 20:29:13.000000 elastic-5.2.0.0/conda/anaconda_deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 20:29:13.000000 elastic-5.2.0.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.804260 elastic-5.2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.804260 elastic-5.2.0.0/docs/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)    60989 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/notebook/lib-usage.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.808260 elastic-5.2.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.808260 elastic-5.2.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.808260 elastic-5.2.0.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/cli-usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/conf.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/endmatter.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/docs/source/fig/
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot1.png
--rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    24303 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    28926 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3.png
--rw-r--r--   0 runner    (1001) docker     (127)    27181 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3a.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3a.png
--rw-r--r--   0 runner    (1001) docker     (127)    36285 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3b.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    27897 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3b.png
--rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3b.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/lib-usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/docs/source/lib-usage_files/
--rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_12_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_18_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_9_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/elastic/
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-15 20:29:13.000000 elastic-5.2.0.0/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/elastic/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:13.000000 elastic-5.2.0.0/elastic/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5857 2024-04-15 20:29:13.000000 elastic-5.2.0.0/elastic/cli/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)    26585 2024-04-15 20:29:13.000000 elastic-5.2.0.0/elastic/elastic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/elastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/example1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/example2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/example3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.816260 elastic-5.2.0.0/examples/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/scripts/check-job
--rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/scripts/run-on-tsi
--rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/scripts/run-vasp5-lock
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/scripts/run_vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-15 20:29:13.000000 elastic-5.2.0.0/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 20:29:13.000000 elastic-5.2.0.0/paper.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.816260 elastic-5.2.0.0/parcalc/
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-15 20:29:13.000000 elastic-5.2.0.0/parcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24638 2024-04-15 20:29:13.000000 elastic-5.2.0.0/parcalc/parcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-15 20:29:13.000000 elastic-5.2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:29:13.000000 elastic-5.2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:29:17.824260 elastic-5.2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-15 20:29:13.000000 elastic-5.2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.816260 elastic-5.2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-15 20:29:13.000000 elastic-5.2.0.0/test/test_elastic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.816260 elastic-5.2.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/INCAR
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/KPOINTS
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)   438201 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/POTCAR
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/abinit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_000/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_000/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_001/
--rw-r--r--   0 runner    (1001) docker     (127)    46925 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_001/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_002/
--rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_002/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_003/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_003/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_004/
--rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_004/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_005/
--rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_005/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_006/
--rw-r--r--   0 runner    (1001) docker     (127)    48183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_006/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_007/
--rw-r--r--   0 runner    (1001) docker     (127)    50184 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_007/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_008/
--rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_008/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_009/
--rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_009/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_010/
--rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_010/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_000/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_000/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_001/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_001/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_002/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_002/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_003/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_003/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_004/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_004/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_005/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_005/vasprun.xml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_000.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_001.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_002.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_003.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_004.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_005.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_006.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_007.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_008.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_009.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_010.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_000.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_001.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_002.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_003.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_004.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_005.POSCAR
--rwxr-xr-x   0 runner    (1001) docker     (127)      319 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/run-calcs
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/runtest.sh
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/test_01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/test_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/test_elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.315086 elastic-5.2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 20:51:50.000000 elastic-5.2.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.287086 elastic-5.2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.295086 elastic-5.2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-15 20:51:50.000000 elastic-5.2.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 20:51:50.000000 elastic-5.2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 20:51:50.000000 elastic-5.2.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 20:51:50.000000 elastic-5.2.1.0/Contributors
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-15 20:51:50.000000 elastic-5.2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 20:51:50.000000 elastic-5.2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 20:51:54.315086 elastic-5.2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 20:51:50.000000 elastic-5.2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.295086 elastic-5.2.1.0/conda/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      282 2024-04-15 20:51:50.000000 elastic-5.2.1.0/conda/anaconda_deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 20:51:50.000000 elastic-5.2.1.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.295086 elastic-5.2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.295086 elastic-5.2.1.0/docs/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)    60989 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/notebook/lib-usage.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.295086 elastic-5.2.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.295086 elastic-5.2.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.295086 elastic-5.2.1.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/cli-usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/conf.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/endmatter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.299086 elastic-5.2.1.0/docs/source/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    24303 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot3.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    28926 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27181 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot3a.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot3a.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36285 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot3a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot3b.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    27897 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot3b.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/fig/plot3b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/lib-usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.303086 elastic-5.2.1.0/docs/source/lib-usage_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/lib-usage_files/lib-usage_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/lib-usage_files/lib-usage_18_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/lib-usage_files/lib-usage_9_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-15 20:51:50.000000 elastic-5.2.1.0/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.303086 elastic-5.2.1.0/elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-15 20:51:50.000000 elastic-5.2.1.0/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 20:51:54.000000 elastic-5.2.1.0/elastic/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.303086 elastic-5.2.1.0/elastic/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:50.000000 elastic-5.2.1.0/elastic/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5857 2024-04-15 20:51:50.000000 elastic-5.2.1.0/elastic/cli/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26585 2024-04-15 20:51:50.000000 elastic-5.2.1.0/elastic/elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.315086 elastic-5.2.1.0/elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 20:51:54.000000 elastic-5.2.1.0/elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-15 20:51:54.000000 elastic-5.2.1.0/elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:51:54.000000 elastic-5.2.1.0/elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 20:51:54.000000 elastic-5.2.1.0/elastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 20:51:54.000000 elastic-5.2.1.0/elastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 20:51:54.000000 elastic-5.2.1.0/elastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.303086 elastic-5.2.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-15 20:51:50.000000 elastic-5.2.1.0/examples/example1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 20:51:50.000000 elastic-5.2.1.0/examples/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-15 20:51:50.000000 elastic-5.2.1.0/examples/example3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.303086 elastic-5.2.1.0/examples/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-04-15 20:51:50.000000 elastic-5.2.1.0/examples/scripts/check-job
+-rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-15 20:51:50.000000 elastic-5.2.1.0/examples/scripts/run-on-tsi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-04-15 20:51:50.000000 elastic-5.2.1.0/examples/scripts/run-vasp5-lock
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 20:51:50.000000 elastic-5.2.1.0/examples/scripts/run_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-15 20:51:50.000000 elastic-5.2.1.0/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 20:51:50.000000 elastic-5.2.1.0/paper.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.303086 elastic-5.2.1.0/parcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-15 20:51:50.000000 elastic-5.2.1.0/parcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24638 2024-04-15 20:51:50.000000 elastic-5.2.1.0/parcalc/parcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-15 20:51:50.000000 elastic-5.2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:51:50.000000 elastic-5.2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:51:54.315086 elastic-5.2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-15 20:51:50.000000 elastic-5.2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.303086 elastic-5.2.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-15 20:51:50.000000 elastic-5.2.1.0/test/test_elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.307086 elastic-5.2.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/INCAR
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)   438201 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/POTCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/abinit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_000/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_000/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_001/
+-rw-r--r--   0 runner    (1001) docker     (127)    46925 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_001/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_002/
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_002/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_003/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_003/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_004/
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_004/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_005/
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_005/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_006/
+-rw-r--r--   0 runner    (1001) docker     (127)    48183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_006/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_007/
+-rw-r--r--   0 runner    (1001) docker     (127)    50184 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_007/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_008/
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_008/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_009/
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_009/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-cij_010/
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-cij_010/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-eos_000/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-eos_000/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-eos_001/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-eos_001/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.311086 elastic-5.2.1.0/tests/data/calc-eos_002/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-eos_002/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.315086 elastic-5.2.1.0/tests/data/calc-eos_003/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-eos_003/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.315086 elastic-5.2.1.0/tests/data/calc-eos_004/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-eos_004/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:51:54.315086 elastic-5.2.1.0/tests/data/calc-eos_005/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/calc-eos_005/vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_000.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_001.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_002.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_003.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_004.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_005.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_006.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_007.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_008.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_009.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/cij_010.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/eos_000.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/eos_001.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/eos_002.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/eos_003.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/eos_004.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/eos_005.POSCAR
+-rwxr-xr-x   0 runner    (1001) docker     (127)      319 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/data/run-calcs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/runtest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/test_01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/test_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-15 20:51:50.000000 elastic-5.2.1.0/tests/test_elastic.py
```

### Comparing `elastic-5.2.0.0/.github/workflows/pypi.yml` & `elastic-5.2.1.0/.github/workflows/pypi.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Test and publish to TestPyPI
+name: Build, test and publish to (test)PyPI
 on: push
 
 jobs:
   build:
     name: Build distribution
     runs-on: ubuntu-latest
```

### Comparing `elastic-5.2.0.0/LICENSE` & `elastic-5.2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/PKG-INFO` & `elastic-5.2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic
-Version: 5.2.0.0
+Version: 5.2.1.0
 Summary: Extension for ASE to calculate elastic constants
 Author-email: "Paweł T. Jochym" <Pawel.Jochym@ifj.edu.pl>, Georgios Tritsaris <gtritsaris@seas.harvard.edu>
 Maintainer-email: "Paweł T. Jochym" <Pawel.Jochym@ifj.edu.pl>
 License: GPLv3
 Project-URL: Homepage, https://wolf.ifj.edu.pl/elastic
 Project-URL: Documentation, http://elastic.rtfd.org/
 Project-URL: Repository, https://github.com/jochym/Elastic
```

### Comparing `elastic-5.2.0.0/README.md` & `elastic-5.2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/conda/meta.yaml` & `elastic-5.2.1.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/Makefile` & `elastic-5.2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/index.md` & `elastic-5.2.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/notebook/lib-usage.ipynb` & `elastic-5.2.1.0/docs/notebook/lib-usage.ipynb`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/_static/favicon.ico` & `elastic-5.2.1.0/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/_templates/layout.html` & `elastic-5.2.1.0/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/cli-usage.rst` & `elastic-5.2.1.0/docs/source/cli-usage.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/conf.py` & `elastic-5.2.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/conf.py.tmpl` & `elastic-5.2.1.0/docs/source/conf.py.tmpl`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/endmatter.rst` & `elastic-5.2.1.0/docs/source/endmatter.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/favicon.ico` & `elastic-5.2.1.0/docs/source/fig/favicon.ico`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/favicon.png` & `elastic-5.2.1.0/docs/source/fig/favicon.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/favicon.svg` & `elastic-5.2.1.0/docs/source/fig/favicon.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot1.pdf` & `elastic-5.2.1.0/docs/source/fig/plot1.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot1.png` & `elastic-5.2.1.0/docs/source/fig/plot1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot1.svg` & `elastic-5.2.1.0/docs/source/fig/plot1.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot2.pdf` & `elastic-5.2.1.0/docs/source/fig/plot2.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot2.png` & `elastic-5.2.1.0/docs/source/fig/plot2.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot2.svg` & `elastic-5.2.1.0/docs/source/fig/plot2.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot3.pdf` & `elastic-5.2.1.0/docs/source/fig/plot3.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot3.png` & `elastic-5.2.1.0/docs/source/fig/plot3.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot3.svg` & `elastic-5.2.1.0/docs/source/fig/plot3.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot3a.pdf` & `elastic-5.2.1.0/docs/source/fig/plot3a.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot3a.png` & `elastic-5.2.1.0/docs/source/fig/plot3a.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot3a.svg` & `elastic-5.2.1.0/docs/source/fig/plot3a.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot3b.pdf` & `elastic-5.2.1.0/docs/source/fig/plot3b.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot3b.png` & `elastic-5.2.1.0/docs/source/fig/plot3b.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/fig/plot3b.svg` & `elastic-5.2.1.0/docs/source/fig/plot3b.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/index.rst` & `elastic-5.2.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/intro.rst` & `elastic-5.2.1.0/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/lib-usage.rst` & `elastic-5.2.1.0/docs/source/lib-usage.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_12_1.png` & `elastic-5.2.1.0/docs/source/lib-usage_files/lib-usage_12_1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_18_1.png` & `elastic-5.2.1.0/docs/source/lib-usage_files/lib-usage_18_1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_9_1.png` & `elastic-5.2.1.0/docs/source/lib-usage_files/lib-usage_9_1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/docs/source/modules.rst` & `elastic-5.2.1.0/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/elastic/__init__.py` & `elastic-5.2.1.0/elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/elastic/cli/elastic.py` & `elastic-5.2.1.0/elastic/cli/elastic.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/elastic/elastic.py` & `elastic-5.2.1.0/elastic/elastic.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     uxx, uyy, uzz, uyz, uxz, uxy = u[0], u[1], u[2], u[3], u[4], u[5]
     return array(
                 [[   uxx,   0,    uyy,     uzz,     0   ],
                  [   uyy,   0,    uxx,     uzz,     0   ],
                  [     0, uzz,      0, uxx+uyy,     0   ],
                  [     0,   0,      0,       0, 2*uyz   ],
                  [     0,   0,      0,       0, 2*uxz   ],
-                 [ 2*uxy,   0, -2*uxy,       0,     0   ]])
+                 [   uxy,   0,   -uxy,       0,     0   ]])
 
 
 def monoclinic(u):
     '''Monoclinic group,
 
     The ordering of constants is:
```

### Comparing `elastic-5.2.0.0/elastic.egg-info/PKG-INFO` & `elastic-5.2.1.0/elastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic
-Version: 5.2.0.0
+Version: 5.2.1.0
 Summary: Extension for ASE to calculate elastic constants
 Author-email: "Paweł T. Jochym" <Pawel.Jochym@ifj.edu.pl>, Georgios Tritsaris <gtritsaris@seas.harvard.edu>
 Maintainer-email: "Paweł T. Jochym" <Pawel.Jochym@ifj.edu.pl>
 License: GPLv3
 Project-URL: Homepage, https://wolf.ifj.edu.pl/elastic
 Project-URL: Documentation, http://elastic.rtfd.org/
 Project-URL: Repository, https://github.com/jochym/Elastic
```

### Comparing `elastic-5.2.0.0/elastic.egg-info/SOURCES.txt` & `elastic-5.2.1.0/elastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/examples/example1.py` & `elastic-5.2.1.0/examples/example1.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/examples/example2.py` & `elastic-5.2.1.0/examples/example2.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/examples/example3.py` & `elastic-5.2.1.0/examples/example3.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/examples/scripts/run-vasp5-lock` & `elastic-5.2.1.0/examples/scripts/run-vasp5-lock`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/paper.bib` & `elastic-5.2.1.0/paper.bib`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/paper.md` & `elastic-5.2.1.0/paper.md`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/parcalc/__init__.py` & `elastic-5.2.1.0/parcalc/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/parcalc/parcalc.py` & `elastic-5.2.1.0/parcalc/parcalc.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/pyproject.toml` & `elastic-5.2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,35 +2,35 @@
     requires = ["setuptools", "setuptools-scm"]
     build-backend = "setuptools.build_meta"
 
 [project]
     dynamic = ["version"]
     name = "elastic"
     dependencies = [
-    "ase",
-    "spglib",
-    "numpy",
-    "scipy",
-    "click",
+        "ase",
+        "spglib",
+        "numpy",
+        "scipy",
+        "click",
     ]
     authors = [
-    {name = "Paweł T. Jochym", email = "Pawel.Jochym@ifj.edu.pl"},
-    {name = "Georgios Tritsaris", email = "gtritsaris@seas.harvard.edu"},
+        {name = "Paweł T. Jochym", email = "Pawel.Jochym@ifj.edu.pl"},
+        {name = "Georgios Tritsaris", email = "gtritsaris@seas.harvard.edu"},
     ]
     maintainers = [
-    {name = "Paweł T. Jochym", email = "Pawel.Jochym@ifj.edu.pl"},
+        {name = "Paweł T. Jochym", email = "Pawel.Jochym@ifj.edu.pl"},
     ]
     description = "Extension for ASE to calculate elastic constants"
     readme = "README.md"
     license = {text = "GPLv3"}
     keywords = ['science', 'physics', 'ase', 'elastic constants', 'crystals']
     classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-    "Programming Language :: Python :: 3",
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "Programming Language :: Python :: 3",
     ]
 
 [project.scripts]
     elastic = "elastic.cli.elastic:cli"
 
 [project.urls]
     Homepage = "https://wolf.ifj.edu.pl/elastic"
```

### Comparing `elastic-5.2.0.0/setup.py` & `elastic-5.2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/test/test_elastic.py` & `elastic-5.2.1.0/test/test_elastic.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/POSCAR` & `elastic-5.2.1.0/tests/data/POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/POTCAR` & `elastic-5.2.1.0/tests/data/POTCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/abinit` & `elastic-5.2.1.0/tests/data/abinit`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_000/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_000/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_001/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_002/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_002/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_003/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_003/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_004/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_004/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_005/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_005/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_006/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_006/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_007/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_007/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_008/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_008/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_009/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_009/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-cij_010/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-cij_010/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-eos_000/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-eos_000/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-eos_001/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-eos_001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-eos_002/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-eos_002/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-eos_003/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-eos_003/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-eos_004/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-eos_004/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/calc-eos_005/vasprun.xml` & `elastic-5.2.1.0/tests/data/calc-eos_005/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_000.POSCAR` & `elastic-5.2.1.0/tests/data/cij_000.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_001.POSCAR` & `elastic-5.2.1.0/tests/data/cij_001.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_002.POSCAR` & `elastic-5.2.1.0/tests/data/cij_002.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_003.POSCAR` & `elastic-5.2.1.0/tests/data/cij_003.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_004.POSCAR` & `elastic-5.2.1.0/tests/data/cij_004.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_005.POSCAR` & `elastic-5.2.1.0/tests/data/cij_005.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_006.POSCAR` & `elastic-5.2.1.0/tests/data/cij_006.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_007.POSCAR` & `elastic-5.2.1.0/tests/data/cij_007.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_008.POSCAR` & `elastic-5.2.1.0/tests/data/cij_008.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_009.POSCAR` & `elastic-5.2.1.0/tests/data/cij_009.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/cij_010.POSCAR` & `elastic-5.2.1.0/tests/data/cij_010.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/eos_000.POSCAR` & `elastic-5.2.1.0/tests/data/eos_000.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/eos_001.POSCAR` & `elastic-5.2.1.0/tests/data/eos_001.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/eos_002.POSCAR` & `elastic-5.2.1.0/tests/data/eos_002.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/eos_003.POSCAR` & `elastic-5.2.1.0/tests/data/eos_003.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/eos_004.POSCAR` & `elastic-5.2.1.0/tests/data/eos_004.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/data/eos_005.POSCAR` & `elastic-5.2.1.0/tests/data/eos_005.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/test_01.py` & `elastic-5.2.1.0/tests/test_01.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/test_02.py` & `elastic-5.2.1.0/tests/test_02.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.0.0/tests/test_elastic.py` & `elastic-5.2.1.0/tests/test_elastic.py`

 * *Files identical despite different names*
