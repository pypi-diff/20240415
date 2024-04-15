# Comparing `tmp/elastic-5.1.0.17.tar.gz` & `tmp/elastic-5.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elastic-5.1.0.17.tar", last modified: Thu Jul 12 10:37:24 2018, max compression
+gzip compressed data, was "elastic-5.2.0.0.tar", last modified: Mon Apr 15 20:29:17 2024, max compression
```

## Comparing `elastic-5.1.0.17.tar` & `elastic-5.2.0.0.tar`

### file list

```diff
@@ -1,151 +1,155 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/conda/
--rwxr-xr-x   0 travis    (2000) travis    (2000)      282 2018-07-12 10:32:09.000000 elastic-5.1.0.17/conda/anaconda_deploy.sh
--rw-r--r--   0 travis    (2000) travis    (2000)     1390 2018-07-12 10:32:09.000000 elastic-5.1.0.17/conda/meta.yaml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/docs/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/docs/notebook/
--rw-r--r--   0 travis    (2000) travis    (2000)    60989 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/notebook/lib-usage.ipynb
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/docs/source/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/docs/source/_static/
--rw-r--r--   0 travis    (2000) travis    (2000)     2238 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/_static/favicon.ico
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/docs/source/_templates/
--rw-r--r--   0 travis    (2000) travis    (2000)     1048 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/_templates/layout.html
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/docs/source/fig/
--rw-r--r--   0 travis    (2000) travis    (2000)     2238 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/favicon.ico
--rw-r--r--   0 travis    (2000) travis    (2000)     2252 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/favicon.png
--rw-r--r--   0 travis    (2000) travis    (2000)     5145 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/favicon.svg
--rw-r--r--   0 travis    (2000) travis    (2000)     7319 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot1.pdf
--rw-r--r--   0 travis    (2000) travis    (2000)    17836 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot1.png
--rw-r--r--   0 travis    (2000) travis    (2000)    24292 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot1.svg
--rw-r--r--   0 travis    (2000) travis    (2000)     5703 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot2.pdf
--rw-r--r--   0 travis    (2000) travis    (2000)    24303 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot2.png
--rw-r--r--   0 travis    (2000) travis    (2000)    18497 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot2.svg
--rw-r--r--   0 travis    (2000) travis    (2000)     7407 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot3.pdf
--rw-r--r--   0 travis    (2000) travis    (2000)    28926 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot3.png
--rw-r--r--   0 travis    (2000) travis    (2000)    27181 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot3.svg
--rw-r--r--   0 travis    (2000) travis    (2000)     7757 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot3a.pdf
--rw-r--r--   0 travis    (2000) travis    (2000)    34509 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot3a.png
--rw-r--r--   0 travis    (2000) travis    (2000)    36285 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot3a.svg
--rw-r--r--   0 travis    (2000) travis    (2000)     7419 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot3b.pdf
--rw-r--r--   0 travis    (2000) travis    (2000)    27897 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot3b.png
--rw-r--r--   0 travis    (2000) travis    (2000)    30417 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/fig/plot3b.svg
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/docs/source/lib-usage_files/
--rw-r--r--   0 travis    (2000) travis    (2000)    11186 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/lib-usage_files/lib-usage_12_1.png
--rw-r--r--   0 travis    (2000) travis    (2000)    18112 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/lib-usage_files/lib-usage_18_1.png
--rw-r--r--   0 travis    (2000) travis    (2000)     4947 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/lib-usage_files/lib-usage_9_1.png
--rw-r--r--   0 travis    (2000) travis    (2000)     6086 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/cli-usage.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     8465 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/conf.py
--rw-r--r--   0 travis    (2000) travis    (2000)     8304 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/conf.py.tmpl
--rw-r--r--   0 travis    (2000) travis    (2000)     1581 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/endmatter.rst
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/examples.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     2658 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/index.rst
--rw-r--r--   0 travis    (2000) travis    (2000)    15113 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/intro.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     9637 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/lib-usage.rst
--rw-r--r--   0 travis    (2000) travis    (2000)      654 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/source/modules.rst
--rw-r--r--   0 travis    (2000) travis    (2000)     4598 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/Makefile
--rw-r--r--   0 travis    (2000) travis    (2000)      186 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/_config.yml
--rw-r--r--   0 travis    (2000) travis    (2000)     2956 2018-07-12 10:32:09.000000 elastic-5.1.0.17/docs/index.md
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/elastic/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/elastic/cli/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-07-12 10:32:09.000000 elastic-5.1.0.17/elastic/cli/__init__.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)     5903 2018-07-12 10:32:09.000000 elastic-5.1.0.17/elastic/cli/elastic.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2543 2018-07-12 10:32:09.000000 elastic-5.1.0.17/elastic/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)    26474 2018-07-12 10:32:09.000000 elastic-5.1.0.17/elastic/elastic.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/elastic.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     3943 2018-07-12 10:37:24.000000 elastic-5.1.0.17/elastic.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)     2916 2018-07-12 10:37:24.000000 elastic-5.1.0.17/elastic.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-07-12 10:37:24.000000 elastic-5.1.0.17/elastic.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       75 2018-07-12 10:37:24.000000 elastic-5.1.0.17/elastic.egg-info/entry_points.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        6 2018-07-12 10:37:24.000000 elastic-5.1.0.17/elastic.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       16 2018-07-12 10:37:24.000000 elastic-5.1.0.17/elastic.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/examples/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/examples/scripts/
--rwxr-xr-x   0 travis    (2000) travis    (2000)      486 2018-07-12 10:32:09.000000 elastic-5.1.0.17/examples/scripts/check-job
--rwxr-xr-x   0 travis    (2000) travis    (2000)       48 2018-07-12 10:32:09.000000 elastic-5.1.0.17/examples/scripts/run-on-tsi
--rwxr-xr-x   0 travis    (2000) travis    (2000)     2106 2018-07-12 10:32:09.000000 elastic-5.1.0.17/examples/scripts/run-vasp5-lock
--rw-r--r--   0 travis    (2000) travis    (2000)      209 2018-07-12 10:32:09.000000 elastic-5.1.0.17/examples/scripts/run_vasp.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2896 2018-07-12 10:32:09.000000 elastic-5.1.0.17/examples/example1.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3252 2018-07-12 10:32:09.000000 elastic-5.1.0.17/examples/example2.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3222 2018-07-12 10:32:09.000000 elastic-5.1.0.17/examples/example3.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/parcalc/
--rw-r--r--   0 travis    (2000) travis    (2000)     1630 2018-07-12 10:32:09.000000 elastic-5.1.0.17/parcalc/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)    24638 2018-07-12 10:32:09.000000 elastic-5.1.0.17/parcalc/parcalc.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/test/
--rw-r--r--   0 travis    (2000) travis    (2000)     3526 2018-07-12 10:32:09.000000 elastic-5.1.0.17/test/test_elastic.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_000/
--rw-r--r--   0 travis    (2000) travis    (2000)    44183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_000/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_001/
--rw-r--r--   0 travis    (2000) travis    (2000)    46925 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_001/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_002/
--rw-r--r--   0 travis    (2000) travis    (2000)    46183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_002/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_003/
--rw-r--r--   0 travis    (2000) travis    (2000)    44183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_003/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_004/
--rw-r--r--   0 travis    (2000) travis    (2000)    46183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_004/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_005/
--rw-r--r--   0 travis    (2000) travis    (2000)    46183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_005/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_006/
--rw-r--r--   0 travis    (2000) travis    (2000)    48183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_006/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_007/
--rw-r--r--   0 travis    (2000) travis    (2000)    50184 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_007/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_008/
--rw-r--r--   0 travis    (2000) travis    (2000)    50926 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_008/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_009/
--rw-r--r--   0 travis    (2000) travis    (2000)    50926 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_009/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-cij_010/
--rw-r--r--   0 travis    (2000) travis    (2000)    50926 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-cij_010/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-eos_000/
--rw-r--r--   0 travis    (2000) travis    (2000)    44183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-eos_000/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-eos_001/
--rw-r--r--   0 travis    (2000) travis    (2000)    44183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-eos_001/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-eos_002/
--rw-r--r--   0 travis    (2000) travis    (2000)    44183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-eos_002/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-eos_003/
--rw-r--r--   0 travis    (2000) travis    (2000)    44183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-eos_003/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-eos_004/
--rw-r--r--   0 travis    (2000) travis    (2000)    44183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-eos_004/vasprun.xml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-07-12 10:37:24.000000 elastic-5.1.0.17/tests/data/calc-eos_005/
--rw-r--r--   0 travis    (2000) travis    (2000)    44183 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/calc-eos_005/vasprun.xml
--rw-r--r--   0 travis    (2000) travis    (2000)      193 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/INCAR
--rw-r--r--   0 travis    (2000) travis    (2000)       79 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/KPOINTS
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)   438201 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/POTCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      925 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/abinit
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_000.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_001.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_002.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_003.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_004.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_005.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_006.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_007.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_008.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_009.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/cij_010.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/eos_000.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/eos_001.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/eos_002.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/eos_003.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/eos_004.POSCAR
--rw-r--r--   0 travis    (2000) travis    (2000)      744 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/eos_005.POSCAR
--rwxr-xr-x   0 travis    (2000) travis    (2000)      319 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/data/run-calcs
--rwxr-xr-x   0 travis    (2000) travis    (2000)      190 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/runtest.sh
--rw-r--r--   0 travis    (2000) travis    (2000)     7656 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/test_01.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1406 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/test_02.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6441 2018-07-12 10:32:09.000000 elastic-5.1.0.17/tests/test_elastic.py
--rw-r--r--   0 travis    (2000) travis    (2000)       36 2018-07-12 10:32:09.000000 elastic-5.1.0.17/.bzrignore
--rw-r--r--   0 travis    (2000) travis    (2000)       61 2018-07-12 10:32:09.000000 elastic-5.1.0.17/.gitattributes
--rw-r--r--   0 travis    (2000) travis    (2000)      475 2018-07-12 10:32:09.000000 elastic-5.1.0.17/.gitignore
--rw-r--r--   0 travis    (2000) travis    (2000)     3011 2018-07-12 10:32:09.000000 elastic-5.1.0.17/.travis.yml
--rw-r--r--   0 travis    (2000) travis    (2000)      130 2018-07-12 10:32:09.000000 elastic-5.1.0.17/Contributors
--rw-r--r--   0 travis    (2000) travis    (2000)    35121 2018-07-12 10:32:09.000000 elastic-5.1.0.17/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)       76 2018-07-12 10:32:09.000000 elastic-5.1.0.17/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     2956 2018-07-12 10:32:09.000000 elastic-5.1.0.17/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)     1788 2018-07-12 10:32:09.000000 elastic-5.1.0.17/paper.bib
--rw-r--r--   0 travis    (2000) travis    (2000)     1266 2018-07-12 10:32:09.000000 elastic-5.1.0.17/paper.md
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-07-12 10:32:09.000000 elastic-5.1.0.17/requirements.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       80 2018-07-12 10:37:24.000000 elastic-5.1.0.17/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     1146 2018-07-12 10:32:09.000000 elastic-5.1.0.17/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3943 2018-07-12 10:37:24.000000 elastic-5.1.0.17/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 20:29:13.000000 elastic-5.2.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.796260 elastic-5.2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.804260 elastic-5.2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-15 20:29:13.000000 elastic-5.2.0.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 20:29:13.000000 elastic-5.2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 20:29:13.000000 elastic-5.2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 20:29:13.000000 elastic-5.2.0.0/Contributors
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-15 20:29:13.000000 elastic-5.2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 20:29:13.000000 elastic-5.2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 20:29:17.824260 elastic-5.2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 20:29:13.000000 elastic-5.2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.804260 elastic-5.2.0.0/conda/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      282 2024-04-15 20:29:13.000000 elastic-5.2.0.0/conda/anaconda_deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 20:29:13.000000 elastic-5.2.0.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.804260 elastic-5.2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.804260 elastic-5.2.0.0/docs/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)    60989 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/notebook/lib-usage.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.808260 elastic-5.2.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.808260 elastic-5.2.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.808260 elastic-5.2.0.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/cli-usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/conf.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/endmatter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/docs/source/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    24303 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    28926 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27181 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3a.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3a.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36285 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3b.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    27897 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3b.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/fig/plot3b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/lib-usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/docs/source/lib-usage_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_18_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_9_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-15 20:29:13.000000 elastic-5.2.0.0/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-15 20:29:13.000000 elastic-5.2.0.0/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/elastic/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:13.000000 elastic-5.2.0.0/elastic/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5857 2024-04-15 20:29:13.000000 elastic-5.2.0.0/elastic/cli/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26585 2024-04-15 20:29:13.000000 elastic-5.2.0.0/elastic/elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 20:29:17.000000 elastic-5.2.0.0/elastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.812260 elastic-5.2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/example1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/example3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.816260 elastic-5.2.0.0/examples/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/scripts/check-job
+-rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/scripts/run-on-tsi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/scripts/run-vasp5-lock
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 20:29:13.000000 elastic-5.2.0.0/examples/scripts/run_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-15 20:29:13.000000 elastic-5.2.0.0/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 20:29:13.000000 elastic-5.2.0.0/paper.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.816260 elastic-5.2.0.0/parcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-15 20:29:13.000000 elastic-5.2.0.0/parcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24638 2024-04-15 20:29:13.000000 elastic-5.2.0.0/parcalc/parcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-15 20:29:13.000000 elastic-5.2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:29:13.000000 elastic-5.2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:29:17.824260 elastic-5.2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-15 20:29:13.000000 elastic-5.2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.816260 elastic-5.2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-15 20:29:13.000000 elastic-5.2.0.0/test/test_elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.816260 elastic-5.2.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/INCAR
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)   438201 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/POTCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/abinit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_000/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_000/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_001/
+-rw-r--r--   0 runner    (1001) docker     (127)    46925 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_001/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_002/
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_002/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_003/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_003/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.820260 elastic-5.2.0.0/tests/data/calc-cij_004/
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_004/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_005/
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_005/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_006/
+-rw-r--r--   0 runner    (1001) docker     (127)    48183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_006/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_007/
+-rw-r--r--   0 runner    (1001) docker     (127)    50184 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_007/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_008/
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_008/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_009/
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_009/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-cij_010/
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-cij_010/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_000/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_000/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_001/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_001/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_002/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_002/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_003/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_003/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_004/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_004/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:29:17.824260 elastic-5.2.0.0/tests/data/calc-eos_005/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/calc-eos_005/vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_000.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_001.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_002.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_003.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_004.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_005.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_006.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_007.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_008.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_009.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/cij_010.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_000.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_001.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_002.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_003.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_004.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/eos_005.POSCAR
+-rwxr-xr-x   0 runner    (1001) docker     (127)      319 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/data/run-calcs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/runtest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/test_01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/test_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-15 20:29:13.000000 elastic-5.2.0.0/tests/test_elastic.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `elastic-5.1.0.17/conda/meta.yaml` & `elastic-5.2.0.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/notebook/lib-usage.ipynb` & `elastic-5.2.0.0/docs/notebook/lib-usage.ipynb`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/_static/favicon.ico` & `elastic-5.2.0.0/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/_templates/layout.html` & `elastic-5.2.0.0/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/favicon.ico` & `elastic-5.2.0.0/docs/source/fig/favicon.ico`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/favicon.png` & `elastic-5.2.0.0/docs/source/fig/favicon.png`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/favicon.svg` & `elastic-5.2.0.0/docs/source/fig/favicon.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot1.pdf` & `elastic-5.2.0.0/docs/source/fig/plot1.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot1.png` & `elastic-5.2.0.0/docs/source/fig/plot1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot1.svg` & `elastic-5.2.0.0/docs/source/fig/plot1.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot2.pdf` & `elastic-5.2.0.0/docs/source/fig/plot2.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot2.png` & `elastic-5.2.0.0/docs/source/fig/plot2.png`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot2.svg` & `elastic-5.2.0.0/docs/source/fig/plot2.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot3.pdf` & `elastic-5.2.0.0/docs/source/fig/plot3.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot3.png` & `elastic-5.2.0.0/docs/source/fig/plot3.png`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot3.svg` & `elastic-5.2.0.0/docs/source/fig/plot3.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot3a.pdf` & `elastic-5.2.0.0/docs/source/fig/plot3a.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot3a.png` & `elastic-5.2.0.0/docs/source/fig/plot3a.png`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot3a.svg` & `elastic-5.2.0.0/docs/source/fig/plot3a.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot3b.pdf` & `elastic-5.2.0.0/docs/source/fig/plot3b.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot3b.png` & `elastic-5.2.0.0/docs/source/fig/plot3b.png`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/fig/plot3b.svg` & `elastic-5.2.0.0/docs/source/fig/plot3b.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/lib-usage_files/lib-usage_12_1.png` & `elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_12_1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/lib-usage_files/lib-usage_18_1.png` & `elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_18_1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/lib-usage_files/lib-usage_9_1.png` & `elastic-5.2.0.0/docs/source/lib-usage_files/lib-usage_9_1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/cli-usage.rst` & `elastic-5.2.0.0/docs/source/cli-usage.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/conf.py` & `elastic-5.2.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/conf.py.tmpl` & `elastic-5.2.0.0/docs/source/conf.py.tmpl`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/endmatter.rst` & `elastic-5.2.0.0/docs/source/endmatter.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/index.rst` & `elastic-5.2.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/intro.rst` & `elastic-5.2.0.0/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/lib-usage.rst` & `elastic-5.2.0.0/docs/source/lib-usage.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/source/modules.rst` & `elastic-5.2.0.0/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/Makefile` & `elastic-5.2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/docs/index.md` & `elastic-5.2.0.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/elastic/cli/elastic.py` & `elastic-5.2.0.0/elastic/cli/elastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,23 @@
 of elastic library for direct use - without writing any python code.
 '''
 
 from __future__ import print_function, absolute_import, division
 import click
 import ase.io
 import elastic
-import pkg_resources
 from click import echo
 
 verbose = 0
 
 
 def banner():
     if verbose > 1:
         echo('Elastic ver. %s\n----------------------' %
-             pkg_resources.get_distribution("elastic").version)
+             elastic._version.version)
 
 
 def set_verbosity(v):
     global verbose
     verbose = v
```

### Comparing `elastic-5.1.0.17/elastic/__init__.py` & `elastic-5.2.0.0/elastic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,7 +62,10 @@
 
 '''
 
 from __future__ import print_function, division, absolute_import
 from .elastic import get_BM_EOS, get_elastic_tensor
 from .elastic import get_elementary_deformations, scan_volumes
 from .elastic import get_pressure, get_strain, BMEOS
+
+# To reach "elastic.__version__" attribute in other programs
+from ._version import __version__
```

### Comparing `elastic-5.1.0.17/elastic/elastic.py` & `elastic-5.2.0.0/elastic/elastic.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,30 +117,30 @@
 
 def tetragonal(u):
     '''
     Equation matrix generation for the tetragonal lattice.
     The order of constants is as follows:
 
     .. math::
-       C_{11}, C_{33}, C_{12}, C_{13}, C_{44}, C_{14}
+       C_{11}, C_{33}, C_{12}, C_{13}, C_{44}, C_{66}
 
     :param u: vector of deformations:
         [ :math:`u_{xx}, u_{yy}, u_{zz}, u_{yz}, u_{xz}, u_{xy}` ]
 
     :returns: Symmetry defined stress-strain equation matrix
     '''
 
     uxx, uyy, uzz, uyz, uxz, uxy = u[0], u[1], u[2], u[3], u[4], u[5]
     return array(
                 [[uxx,   0,    uyy,  uzz,      0,      0],
                  [uyy,   0,    uxx,  uzz,      0,      0],
                  [0,     uzz,  0,    uxx+uyy,  0,      0],
-                 [0,     0,    0,    0,        0,      2*uxy],
                  [0,     0,    0,    0,        2*uxz,  0],
-                 [0,     0,    0,    0,        2*uyz,  0]])
+                 [0,     0,    0,    0,        2*uyz,  0],
+                 [0,     0,    0,    0,        0,      2*uxy]])
 
 
 def orthorombic(u):
     '''
     Equation matrix generation for the orthorombic lattice.
     The order of constants is as follows:
 
@@ -290,15 +290,15 @@
             1: ('C_11', 'C_22', 'C_33', 'C_12', 'C_13', 'C_23',
                 'C_44', 'C_55', 'C_66', 'C_16', 'C_26', 'C_36',
                 'C_46', 'C_56', 'C_14', 'C_15', 'C_25', 'C_45'),
             2: ('C_11', 'C_22', 'C_33', 'C_12', 'C_13', 'C_23',
                 'C_44', 'C_55', 'C_66', 'C_16', 'C_26', 'C_36', 'C_45'),
             3: ('C_11', 'C_22', 'C_33', 'C_12', 'C_13', 'C_23', 'C_44',
                 'C_55', 'C_66'),
-            4: ('C_11', 'C_33', 'C_12', 'C_13', 'C_44', 'C_14'),
+            4: ('C_11', 'C_33', 'C_12', 'C_13', 'C_44', 'C_66'),
             5: ('C_11', 'C_33', 'C_12', 'C_13', 'C_44', 'C_14'),
             6: ('C_11', 'C_33', 'C_12', 'C_13', 'C_44'),
             7: ('C_11', 'C_12', 'C_44'),
             }
     return orders[get_lattice_type(cryst)[0]]
 
 
@@ -327,15 +327,17 @@
             [75,  "Orthorombic"],
             [143, "Tetragonal"],
             [168, "Trigonal"],
             [195, "Hexagonal"],
             [231, "Cubic"]
         ]
 
-    sg = spg.get_spacegroup(cryst)
+    sg = spg.get_spacegroup((cryst.get_cell(), 
+                             cryst.get_positions(), 
+                             cryst.numbers))
     m = re.match(r'([A-Z].*\b)\s*\(([0-9]*)\)', sg)
     sg_name = m.group(1)
     sg_nr = int(m.group(2))
 
     for n, l in enumerate(lattice_types):
         if sg_nr < l[0]:
             bravais = l[1]
```

### Comparing `elastic-5.1.0.17/elastic.egg-info/SOURCES.txt` & `elastic-5.2.0.0/elastic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.bzrignore
 .gitattributes
 .gitignore
-.travis.yml
+CHANGELOG.md
 Contributors
 LICENSE
 MANIFEST.in
 README.md
 paper.bib
 paper.md
+pyproject.toml
 requirements.txt
-setup.cfg
 setup.py
+.github/workflows/pypi.yml
 conda/anaconda_deploy.sh
 conda/meta.yaml
 docs/Makefile
 docs/_config.yml
 docs/index.md
 docs/notebook/lib-usage.ipynb
 docs/source/cli-usage.rst
@@ -46,14 +46,15 @@
 docs/source/fig/plot3b.pdf
 docs/source/fig/plot3b.png
 docs/source/fig/plot3b.svg
 docs/source/lib-usage_files/lib-usage_12_1.png
 docs/source/lib-usage_files/lib-usage_18_1.png
 docs/source/lib-usage_files/lib-usage_9_1.png
 elastic/__init__.py
+elastic/_version.py
 elastic/elastic.py
 elastic.egg-info/PKG-INFO
 elastic.egg-info/SOURCES.txt
 elastic.egg-info/dependency_links.txt
 elastic.egg-info/entry_points.txt
 elastic.egg-info/requires.txt
 elastic.egg-info/top_level.txt
```

### Comparing `elastic-5.1.0.17/examples/scripts/run-vasp5-lock` & `elastic-5.2.0.0/examples/scripts/run-vasp5-lock`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/examples/example1.py` & `elastic-5.2.0.0/examples/example1.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/examples/example2.py` & `elastic-5.2.0.0/examples/example2.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/examples/example3.py` & `elastic-5.2.0.0/examples/example3.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/parcalc/__init__.py` & `elastic-5.2.0.0/parcalc/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/parcalc/parcalc.py` & `elastic-5.2.0.0/parcalc/parcalc.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/test/test_elastic.py` & `elastic-5.2.0.0/test/test_elastic.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_000/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_000/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_001/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_002/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_002/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_003/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_003/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_004/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_004/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_005/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_005/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_006/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_006/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_007/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_007/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_008/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_008/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_009/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_009/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-cij_010/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-cij_010/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-eos_000/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-eos_000/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-eos_001/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-eos_001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-eos_002/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-eos_002/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-eos_003/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-eos_003/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-eos_004/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-eos_004/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/calc-eos_005/vasprun.xml` & `elastic-5.2.0.0/tests/data/calc-eos_005/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/POSCAR` & `elastic-5.2.0.0/tests/data/POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/POTCAR` & `elastic-5.2.0.0/tests/data/POTCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/abinit` & `elastic-5.2.0.0/tests/data/abinit`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_000.POSCAR` & `elastic-5.2.0.0/tests/data/cij_000.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_001.POSCAR` & `elastic-5.2.0.0/tests/data/cij_001.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_002.POSCAR` & `elastic-5.2.0.0/tests/data/cij_002.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_003.POSCAR` & `elastic-5.2.0.0/tests/data/cij_003.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_004.POSCAR` & `elastic-5.2.0.0/tests/data/cij_004.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_005.POSCAR` & `elastic-5.2.0.0/tests/data/cij_005.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_006.POSCAR` & `elastic-5.2.0.0/tests/data/cij_006.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_007.POSCAR` & `elastic-5.2.0.0/tests/data/cij_007.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_008.POSCAR` & `elastic-5.2.0.0/tests/data/cij_008.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_009.POSCAR` & `elastic-5.2.0.0/tests/data/cij_009.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/cij_010.POSCAR` & `elastic-5.2.0.0/tests/data/cij_010.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/eos_000.POSCAR` & `elastic-5.2.0.0/tests/data/eos_000.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/eos_001.POSCAR` & `elastic-5.2.0.0/tests/data/eos_001.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/eos_002.POSCAR` & `elastic-5.2.0.0/tests/data/eos_002.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/eos_003.POSCAR` & `elastic-5.2.0.0/tests/data/eos_003.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/eos_004.POSCAR` & `elastic-5.2.0.0/tests/data/eos_004.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/data/eos_005.POSCAR` & `elastic-5.2.0.0/tests/data/eos_005.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/test_01.py` & `elastic-5.2.0.0/tests/test_01.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/test_02.py` & `elastic-5.2.0.0/tests/test_02.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/tests/test_elastic.py` & `elastic-5.2.0.0/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/LICENSE` & `elastic-5.2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/README.md` & `elastic-5.2.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Elastic
 =======
 
-[![Build
-Status](https://travis-ci.org/jochym/Elastic.svg?branch=master)](https://travis-ci.org/jochym/Elastic)
-[![PVersion
-Badge](https://img.shields.io/pypi/v/elastic.svg)](https://pypi.org/project/elastic/)
-[![CVersion
-Badge](https://anaconda.org/conda-forge/elastic/badges/version.svg)](https://anaconda.org/conda-forge/elastic)
-[![Downloads
-Badge](https://anaconda.org/conda-forge/elastic/badges/downloads.svg)](https://anaconda.org/conda-forge/elastic)
-[![License
-Badge](https://anaconda.org/jochym/elastic/badges/license.svg)](https://anaconda.org/jochym/elastic)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/jochym/Elastic/pypi.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/elastic)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/elastic?label=PyPi)
+![Conda Version](https://img.shields.io/conda/vn/conda-forge/elastic)
+![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/elastic?label=forge)
+![GitHub License](https://img.shields.io/github/license/jochym/Elastic)
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.593721.svg)](https://doi.org/10.5281/zenodo.593721)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/9f348d724d564ce399beb009ab9a3654)](https://www.codacy.com/app/jochym/Elastic?utm_source=github.com&utm_medium=referral&utm_content=jochym/Elastic&utm_campaign=badger)
 [![Documentation Status](https://readthedocs.org/projects/elastic/badge/?version=latest)](https://elastic.readthedocs.io/en/latest/?badge=latest)
 
 Elastic is a set of python routines for calculation of elastic
 properties of crystals (elastic constants, equation of state, sound
 velocities, etc.). It is a third version of the in-house code I have
 written over few years and is implemented as a extension to the
 [ASE](https://wiki.fysik.dtu.dk/ase/) system. The code was a basis for
@@ -29,19 +24,14 @@
 The on-line documentation is placed on
 [ReadTheDocs](http://elastic.rtfd.org/) or [Elastic
 website](http://wolf.ifj.edu.pl/elastic/). You can obtain the
 [documentation as a PDF
 file](https://media.readthedocs.org/pdf/elastic/stable/elastic.pdf) as
 well.
 
-The docs are also published at: [Elastic over
-IPFS](https://ipfs.io/ipns/QmSHUr59SLvWEZq7URTDGgouVaq7vFJYG7HqtBgL4s6M2u/)
-
-The stable site hash is:
-/ipns/QmSHUr59SLvWEZq7URTDGgouVaq7vFJYG7HqtBgL4s6M2u/
 
 Installation
 ------------
 
 The installation is simple if you are using conda package menager:
 
     conda install -c conda-forge elastic
```

### Comparing `elastic-5.1.0.17/paper.bib` & `elastic-5.2.0.0/paper.bib`

 * *Files identical despite different names*

### Comparing `elastic-5.1.0.17/paper.md` & `elastic-5.2.0.0/paper.md`

 * *Files identical despite different names*

