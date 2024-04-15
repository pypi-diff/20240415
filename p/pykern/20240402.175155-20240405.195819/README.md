# Comparing `tmp/pykern-20240402.175155.tar.gz` & `tmp/pykern-20240405.195819.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykern-20240402.175155.tar", last modified: Tue Apr  2 19:12:09 2024, max compression
+gzip compressed data, was "pykern-20240405.195819.tar", last modified: Tue Apr  9 14:46:27 2024, max compression
```

## Comparing `pykern-20240402.175155.tar` & `pykern-20240405.195819.tar`

### file list

```diff
@@ -1,463 +1,463 @@
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.996141 pykern-20240402.175155/
--rw-r-----   0 root         (0) root         (0)    11324 2018-02-06 22:51:04.000000 pykern-20240402.175155/LICENSE
--rw-r-----   0 root         (0) root         (0)      182 2024-03-19 18:50:32.000000 pykern-20240402.175155/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1741 2024-04-02 19:12:09.996141 pykern-20240402.175155/PKG-INFO
--rw-r-----   0 root         (0) root         (0)      264 2024-03-20 14:13:19.000000 pykern-20240402.175155/README.md
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.920140 pykern-20240402.175155/docs/
--rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240402.175155/docs/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.921140 pykern-20240402.175155/docs/_static/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/docs/_static/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.921140 pykern-20240402.175155/docs/_templates/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/docs/_templates/.gitignore
--rw-r-----   0 root         (0) root         (0)      365 2018-02-06 22:51:04.000000 pykern-20240402.175155/docs/index.rst
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.927140 pykern-20240402.175155/pykern/
--rw-r-----   0 root         (0) root         (0)      354 2024-03-20 14:13:19.000000 pykern-20240402.175155/pykern/__init__.py
--rw-r-----   0 root         (0) root         (0)    17824 2023-10-20 20:51:58.000000 pykern-20240402.175155/pykern/fconf.py
--rw-r-----   0 root         (0) root         (0)     1029 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/mpi.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.929140 pykern-20240402.175155/pykern/package_data/
--rw-r-----   0 root         (0) root         (0)     9727 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/docs-conf.py.format
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.930140 pykern-20240402.175155/pykern/package_data/projex/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.898140 pykern-20240402.175155/pykern/package_data/projex/.github/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.932140 pykern-20240402.175155/pykern/package_data/projex/.github/workflows/
--rw-r-----   0 root         (0) root         (0)      281 2022-07-20 23:21:19.000000 pykern-20240402.175155/pykern/package_data/projex/.github/workflows/python-ci.yml.jinja
--rw-r-----   0 root         (0) root         (0)      221 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/README.md.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.933140 pykern-20240402.175155/pykern/package_data/projex/docs/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.933140 pykern-20240402.175155/pykern/package_data/projex/docs/_static/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/docs/_static/dot-gitignore.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.933140 pykern-20240402.175155/pykern/package_data/projex/docs/_templates/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/docs/_templates/dot-gitignore.jinja
--rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/docs/dot-gitignore.jinja
--rw-r-----   0 root         (0) root         (0)      207 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/docs/index.rst.jinja
--rw-r-----   0 root         (0) root         (0)      772 2022-02-12 15:07:54.000000 pykern-20240402.175155/pykern/package_data/projex/dot-gitignore.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.934140 pykern-20240402.175155/pykern/package_data/projex/projex/
--rw-r-----   0 root         (0) root         (0)      296 2022-10-24 20:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/projex/__init__.py.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.934140 pykern-20240402.175155/pykern/package_data/projex/projex/package_data/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/projex/package_data/dot-gitignore.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.934140 pykern-20240402.175155/pykern/package_data/projex/projex/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/projex/pkcli/__init__.py.jinja
--rw-r-----   0 root         (0) root         (0)      298 2022-10-24 20:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/projex/projex_console.py.jinja
--rw-r-----   0 root         (0) root         (0)      578 2022-10-24 20:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/setup.py.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.935140 pykern-20240402.175155/pykern/package_data/projex/tests/
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/tests/dot-gitignore.jinja
--rw-r-----   0 root         (0) root         (0)      228 2022-10-24 20:51:04.000000 pykern-20240402.175155/pykern/package_data/projex/tests/import_test.py.jinja
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.932140 pykern-20240402.175155/pykern/package_data/projex-licenses/
--rw-r-----   0 root         (0) root         (0)    34520 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex-licenses/agpl-3.0.txt
--rw-r-----   0 root         (0) root         (0)    11358 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex-licenses/apache2.jinja
--rw-r-----   0 root         (0) root         (0)    18092 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex-licenses/gpl2.jinja
--rw-r-----   0 root         (0) root         (0)    35147 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex-licenses/gpl3.jinja
--rw-r-----   0 root         (0) root         (0)    25383 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex-licenses/lgpl2.jinja
--rw-r-----   0 root         (0) root         (0)     7651 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex-licenses/lgpl3.jinja
--rw-r-----   0 root         (0) root         (0)     1085 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex-licenses/mit.jinja
--rw-r-----   0 root         (0) root         (0)      191 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/projex-licenses/proprietary.jinja
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240402.175155/pykern/package_data/test.yml
--rw-r-----   0 root         (0) root         (0)     1169 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pkarray.py
--rw-r-----   0 root         (0) root         (0)     2845 2024-03-15 14:11:15.000000 pykern-20240402.175155/pykern/pkasyncio.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.937140 pykern-20240402.175155/pykern/pkcli/
--rw-r-----   0 root         (0) root         (0)    10485 2024-03-15 14:11:15.000000 pykern-20240402.175155/pykern/pkcli/__init__.py
--rw-r-----   0 root         (0) root         (0)     4170 2024-03-20 14:13:19.000000 pykern-20240402.175155/pykern/pkcli/ci.py
--rw-r-----   0 root         (0) root         (0)     1763 2022-12-28 15:07:11.000000 pykern-20240402.175155/pykern/pkcli/fmt.py
--rw-r-----   0 root         (0) root         (0)    20449 2024-03-15 14:11:15.000000 pykern-20240402.175155/pykern/pkcli/github.py
--rw-r-----   0 root         (0) root         (0)    12793 2022-10-31 19:53:53.000000 pykern-20240402.175155/pykern/pkcli/github_orgmode.py
--rw-r-----   0 root         (0) root         (0)     2849 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pkcli/pkexample.py
--rw-r-----   0 root         (0) root         (0)     4773 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pkcli/projex.py
--rw-r-----   0 root         (0) root         (0)     3039 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pkcli/rsmanifest.py
--rw-r-----   0 root         (0) root         (0)     6686 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pkcli/sim.py
--rw-r-----   0 root         (0) root         (0)     7417 2024-03-28 17:40:02.000000 pykern-20240402.175155/pykern/pkcli/test.py
--rw-r-----   0 root         (0) root         (0)    12437 2024-03-21 14:11:12.000000 pykern-20240402.175155/pykern/pkcollections.py
--rw-r-----   0 root         (0) root         (0)     3686 2023-09-13 14:10:24.000000 pykern-20240402.175155/pykern/pkcompat.py
--rw-r-----   0 root         (0) root         (0)    24232 2023-10-20 20:51:58.000000 pykern-20240402.175155/pykern/pkconfig.py
--rw-r-----   0 root         (0) root         (0)     1221 2024-03-28 17:40:02.000000 pykern-20240402.175155/pykern/pkconst.py
--rw-r-----   0 root         (0) root         (0)    22756 2024-01-19 15:11:21.000000 pykern-20240402.175155/pykern/pkdebug.py
--rw-r-----   0 root         (0) root         (0)     4591 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pkexample.py
--rw-r-----   0 root         (0) root         (0)     8826 2024-01-19 15:11:21.000000 pykern-20240402.175155/pykern/pkinspect.py
--rw-r-----   0 root         (0) root         (0)    10253 2024-02-01 15:11:17.000000 pykern-20240402.175155/pykern/pkio.py
--rw-r-----   0 root         (0) root         (0)     1857 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pkjinja.py
--rw-r-----   0 root         (0) root         (0)     2302 2024-01-12 21:32:37.000000 pykern-20240402.175155/pykern/pkjson.py
--rw-r-----   0 root         (0) root         (0)     1427 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pkplatform.py
--rw-r-----   0 root         (0) root         (0)     3214 2024-03-28 17:40:02.000000 pykern-20240402.175155/pykern/pkresource.py
--rw-r-----   0 root         (0) root         (0)      774 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pkrunpy.py
--rw-r-----   0 root         (0) root         (0)    22115 2024-03-28 17:40:02.000000 pykern-20240402.175155/pykern/pksetup.py
--rw-r-----   0 root         (0) root         (0)     4287 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pksubprocess.py
--rw-r-----   0 root         (0) root         (0)    25421 2024-03-20 14:13:19.000000 pykern-20240402.175155/pykern/pkunit.py
--rw-r-----   0 root         (0) root         (0)     2578 2022-07-12 14:07:33.000000 pykern-20240402.175155/pykern/pkyaml.py
--rw-r-----   0 root         (0) root         (0)      421 2022-06-24 14:08:21.000000 pykern-20240402.175155/pykern/pykern_console.py
--rw-r-----   0 root         (0) root         (0)      180 2024-03-20 14:13:19.000000 pykern-20240402.175155/pykern/pytest_plugin.py
--rw-r-----   0 root         (0) root         (0)      404 2022-09-26 20:14:13.000000 pykern-20240402.175155/pykern/quest.py
--rw-r-----   0 root         (0) root         (0)     3756 2024-03-15 14:11:15.000000 pykern-20240402.175155/pykern/util.py
--rw-r-----   0 root         (0) root         (0)    23884 2023-09-25 14:09:48.000000 pykern-20240402.175155/pykern/xlsx.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.995140 pykern-20240402.175155/pykern.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1741 2024-04-02 19:12:09.000000 pykern-20240402.175155/pykern.egg-info/PKG-INFO
--rw-r-----   0 root         (0) root         (0)    11319 2024-04-02 19:12:09.000000 pykern-20240402.175155/pykern.egg-info/SOURCES.txt
--rw-r-----   0 root         (0) root         (0)        1 2024-04-02 19:12:09.000000 pykern-20240402.175155/pykern.egg-info/dependency_links.txt
--rw-r-----   0 root         (0) root         (0)       54 2024-04-02 19:12:09.000000 pykern-20240402.175155/pykern.egg-info/entry_points.txt
--rw-r-----   0 root         (0) root         (0)      376 2024-04-02 19:12:09.000000 pykern-20240402.175155/pykern.egg-info/requires.txt
--rw-r-----   0 root         (0) root         (0)        7 2024-04-02 19:12:09.000000 pykern-20240402.175155/pykern.egg-info/top_level.txt
--rw-r-----   0 root         (0) root         (0)     1455 2024-04-02 19:05:05.000000 pykern-20240402.175155/pyproject.toml
--rw-r-----   0 root         (0) root         (0)       38 2024-04-02 19:12:09.996141 pykern-20240402.175155/setup.cfg
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.946140 pykern-20240402.175155/tests/
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/.gitignore
--rw-r-----   0 root         (0) root         (0)      554 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/conftest.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.900140 pykern-20240402.175155/tests/fconf_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.947140 pykern-20240402.175155/tests/fconf_data/1.in/
--rw-r-----   0 root         (0) root         (0)      450 2022-07-18 15:54:21.000000 pykern-20240402.175155/tests/fconf_data/1.in/0.py
--rw-r-----   0 root         (0) root         (0)      883 2022-07-18 15:54:21.000000 pykern-20240402.175155/tests/fconf_data/1.in/1.yml
--rw-r-----   0 root         (0) root         (0)       57 2022-07-07 14:08:03.000000 pykern-20240402.175155/tests/fconf_data/1.in/2.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.947140 pykern-20240402.175155/tests/fconf_data/1.out/
--rw-r-----   0 root         (0) root         (0)     1647 2022-07-18 15:54:21.000000 pykern-20240402.175155/tests/fconf_data/1.out/res.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.947140 pykern-20240402.175155/tests/fconf_data/2.in/
--rw-r-----   0 root         (0) root         (0)      139 2022-07-07 14:08:03.000000 pykern-20240402.175155/tests/fconf_data/2.in/1.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.948140 pykern-20240402.175155/tests/fconf_data/2.out/
--rw-r-----   0 root         (0) root         (0)      374 2022-07-07 14:08:03.000000 pykern-20240402.175155/tests/fconf_data/2.out/res.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.948140 pykern-20240402.175155/tests/fconf_data/3.in/
--rw-r-----   0 root         (0) root         (0)       71 2022-07-07 14:08:03.000000 pykern-20240402.175155/tests/fconf_data/3.in/0.py
--rw-r-----   0 root         (0) root         (0)       71 2022-07-07 14:08:03.000000 pykern-20240402.175155/tests/fconf_data/3.in/1.py
--rw-r-----   0 root         (0) root         (0)       11 2022-07-07 14:08:03.000000 pykern-20240402.175155/tests/fconf_data/3.in/2.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.949140 pykern-20240402.175155/tests/fconf_data/3.out/
--rw-r-----   0 root         (0) root         (0)      118 2022-07-07 14:08:03.000000 pykern-20240402.175155/tests/fconf_data/3.out/res.json
--rw-r-----   0 root         (0) root         (0)      602 2022-07-07 14:08:03.000000 pykern-20240402.175155/tests/fconf_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.949140 pykern-20240402.175155/tests/mpi_data/
--rw-r-----   0 root         (0) root         (0)      925 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/mpi_data/p1.py
--rw-r-----   0 root         (0) root         (0)     1307 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/mpi_test.py
--rw-r-----   0 root         (0) root         (0)      885 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkarray_test.py
--rw-r-----   0 root         (0) root         (0)     2633 2024-01-19 15:11:21.000000 pykern-20240402.175155/tests/pkasyncio_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.952140 pykern-20240402.175155/tests/pkcli/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.902140 pykern-20240402.175155/tests/pkcli/ci1_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.952140 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.952140 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/.x/
--rw-r-----   0 root         (0) root         (0)       61 2022-06-29 14:08:01.000000 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/.x/x.py
--rw-r-----   0 root         (0) root         (0)       34 2022-06-29 14:08:01.000000 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/setup.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.953140 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/somepkg/
--rw-r-----   0 root         (0) root         (0)        8 2022-06-29 14:08:01.000000 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/somepkg/has_print.py
--rw-r-----   0 root         (0) root         (0)       14 2022-06-29 14:08:01.000000 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/somepkg/ok.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.953140 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/somepkg/package_data/
--rw-r-----   0 root         (0) root         (0)       50 2022-06-29 14:08:01.000000 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/somepkg/package_data/not_checked.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.902140 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/tests/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.953140 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/tests/test_data/
--rw-r-----   0 root         (0) root         (0)       50 2022-06-29 14:08:01.000000 pykern-20240402.175155/tests/pkcli/ci1_data/1.in/tests/test_data/not_checked.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.953140 pykern-20240402.175155/tests/pkcli/ci1_data/1.out/
--rw-r-----   0 root         (0) root         (0)       45 2022-10-22 14:07:30.000000 pykern-20240402.175155/tests/pkcli/ci1_data/1.out/pkexcept
--rw-r-----   0 root         (0) root         (0)      428 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkcli/ci1_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.905140 pykern-20240402.175155/tests/pkcli/ci_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.953140 pykern-20240402.175155/tests/pkcli/ci_data/check_eof_newline-1.in/
--rw-r-----   0 root         (0) root         (0)       36 2022-11-17 18:34:08.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_eof_newline-1.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.954140 pykern-20240402.175155/tests/pkcli/ci_data/check_eof_newline-1.out/
--rw-r-----   0 root         (0) root         (0)       24 2022-11-17 18:34:08.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_eof_newline-1.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.954140 pykern-20240402.175155/tests/pkcli/ci_data/check_eof_newline-2.in/
--rw-r-----   0 root         (0) root         (0)       45 2022-11-17 18:34:08.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_eof_newline-2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.954140 pykern-20240402.175155/tests/pkcli/ci_data/check_eof_newline-2.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:08.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_eof_newline-2.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.954140 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-1.in/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.955140 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-1.in/run/
--rw-r-----   0 root         (0) root         (0)       27 2022-11-17 18:34:08.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-1.in/run/ignored.py
--rw-r-----   0 root         (0) root         (0)      191 2022-11-17 18:34:08.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-1.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.955140 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-1.out/
--rw-r-----   0 root         (0) root         (0)      148 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-1.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.955140 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-2.in/
--rw-r-----   0 root         (0) root         (0)      208 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.955140 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-2.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-2.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.956140 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-3.in/
--rw-r-----   0 root         (0) root         (0)       87 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-3.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.956140 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-3.out/
--rw-r-----   0 root         (0) root         (0)       82 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-3.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.956140 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-4.in/
--rw-r-----   0 root         (0) root         (0)       10 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-4.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.956140 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-4.out/
--rw-r-----   0 root         (0) root         (0)       31 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/check_prints-4.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.957140 pykern-20240402.175155/tests/pkcli/ci_data/run-1.in/
--rw-r-----   0 root         (0) root         (0)       20 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/run-1.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.957140 pykern-20240402.175155/tests/pkcli/ci_data/run-1.out/
--rw-r-----   0 root         (0) root         (0)       14 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/run-1.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.957140 pykern-20240402.175155/tests/pkcli/ci_data/run-2.in/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.957140 pykern-20240402.175155/tests/pkcli/ci_data/run-2.in/tests/
--rw-r-----   0 root         (0) root         (0)       23 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/run-2.in/tests/x_test.py
--rw-r-----   0 root         (0) root         (0)       23 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/run-2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.958140 pykern-20240402.175155/tests/pkcli/ci_data/run-2.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_data/run-2.out/pkexcept
--rw-r-----   0 root         (0) root         (0)      400 2022-11-17 18:34:09.000000 pykern-20240402.175155/tests/pkcli/ci_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.906140 pykern-20240402.175155/tests/pkcli/fmt_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.958140 pykern-20240402.175155/tests/pkcli/fmt_data/check1.in/
--rw-r-----   0 root         (0) root         (0)       44 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/check1.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.958140 pykern-20240402.175155/tests/pkcli/fmt_data/check1.out/
--rw-r-----   0 root         (0) root         (0)       39 2022-12-28 15:07:11.000000 pykern-20240402.175155/tests/pkcli/fmt_data/check1.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.958140 pykern-20240402.175155/tests/pkcli/fmt_data/check2.in/
--rw-r-----   0 root         (0) root         (0)       56 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/check2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.959140 pykern-20240402.175155/tests/pkcli/fmt_data/check2.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-06-18 14:08:41.000000 pykern-20240402.175155/tests/pkcli/fmt_data/check2.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.959140 pykern-20240402.175155/tests/pkcli/fmt_data/diff.in/
--rw-r-----   0 root         (0) root         (0)      245 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/diff.in/file1.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.959140 pykern-20240402.175155/tests/pkcli/fmt_data/diff.out/
--rw-r-----   0 root         (0) root         (0)        5 2022-06-18 14:08:41.000000 pykern-20240402.175155/tests/pkcli/fmt_data/diff.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.959140 pykern-20240402.175155/tests/pkcli/fmt_data/diff2.in/
--rw-r-----   0 root         (0) root         (0)      368 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/diff2.in/x.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.960140 pykern-20240402.175155/tests/pkcli/fmt_data/diff2.out/
--rw-r-----   0 root         (0) root         (0)       14 2022-06-18 14:08:41.000000 pykern-20240402.175155/tests/pkcli/fmt_data/diff2.out/pkexcept
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.960140 pykern-20240402.175155/tests/pkcli/fmt_data/fmt_dir.in/
--rw-r-----   0 root         (0) root         (0)      170 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/fmt_dir.in/file1.py
--rw-r-----   0 root         (0) root         (0)      483 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/fmt_dir.in/y.py
--rw-r-----   0 root         (0) root         (0)      244 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/fmt_dir.in/z.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.961140 pykern-20240402.175155/tests/pkcli/fmt_data/fmt_dir.out/
--rw-r-----   0 root         (0) root         (0)      245 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/fmt_dir.out/file1.py
--rw-r-----   0 root         (0) root         (0)      584 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/fmt_dir.out/y.py
--rw-r-----   0 root         (0) root         (0)      324 2022-06-14 14:07:59.000000 pykern-20240402.175155/tests/pkcli/fmt_data/fmt_dir.out/z.py
--rw-r-----   0 root         (0) root         (0)      798 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkcli/fmt_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.907140 pykern-20240402.175155/tests/pkcli/github_orgmode_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.961140 pykern-20240402.175155/tests/pkcli/github_orgmode_data/assignee_issues-1.in/
--rw-r-----   0 root         (0) root         (0)    20455 2022-10-11 14:09:00.000000 pykern-20240402.175155/tests/pkcli/github_orgmode_data/assignee_issues-1.in/repo.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.962140 pykern-20240402.175155/tests/pkcli/github_orgmode_data/assignee_issues-1.out/
--rw-r-----   0 root         (0) root         (0)     1301 2022-10-15 14:08:58.000000 pykern-20240402.175155/tests/pkcli/github_orgmode_data/assignee_issues-1.out/assignee_issues.org
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.962140 pykern-20240402.175155/tests/pkcli/github_orgmode_data/from_issues-1.in/
--rw-r-----   0 root         (0) root         (0)    21657 2022-10-11 14:09:00.000000 pykern-20240402.175155/tests/pkcli/github_orgmode_data/from_issues-1.in/repo.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.962140 pykern-20240402.175155/tests/pkcli/github_orgmode_data/from_issues-1.out/
--rw-r-----   0 root         (0) root         (0)     1056 2022-10-15 14:08:58.000000 pykern-20240402.175155/tests/pkcli/github_orgmode_data/from_issues-1.out/radiasoft-test-pykern-github-orgmode.org
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.963140 pykern-20240402.175155/tests/pkcli/github_orgmode_data/to_issues-1.in/
--rw-r-----   0 root         (0) root         (0)     2922 2022-10-11 14:09:00.000000 pykern-20240402.175155/tests/pkcli/github_orgmode_data/to_issues-1.in/repo.json
--rw-r-----   0 root         (0) root         (0)     1264 2022-10-11 14:09:00.000000 pykern-20240402.175155/tests/pkcli/github_orgmode_data/to_issues-1.in/to_issues-1.org
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.963140 pykern-20240402.175155/tests/pkcli/github_orgmode_data/to_issues-1.out/
--rw-r-----   0 root         (0) root         (0)      933 2022-10-11 14:09:00.000000 pykern-20240402.175155/tests/pkcli/github_orgmode_data/to_issues-1.out/res.json
--rw-r-----   0 root         (0) root         (0)     2312 2022-10-31 19:53:53.000000 pykern-20240402.175155/tests/pkcli/github_orgmode_test.py
--rw-r-----   0 root         (0) root         (0)     4988 2024-03-15 14:11:15.000000 pykern-20240402.175155/tests/pkcli/github_test.py
--rw-r-----   0 root         (0) root         (0)     2923 2023-08-16 14:09:51.000000 pykern-20240402.175155/tests/pkcli/projex_test.py
--rw-r-----   0 root         (0) root         (0)     1995 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkcli/rsmanifest_test.py
--rw-r-----   0 root         (0) root         (0)     1816 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkcli/sim_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.908140 pykern-20240402.175155/tests/pkcli/test1_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.963140 pykern-20240402.175155/tests/pkcli/test1_data/tests/
--rw-r-----   0 root         (0) root         (0)      293 2023-04-05 14:10:34.000000 pykern-20240402.175155/tests/pkcli/test1_data/tests/always_test.py
--rw-r-----   0 root         (0) root         (0)      461 2023-04-05 14:10:34.000000 pykern-20240402.175155/tests/pkcli/test1_data/tests/twice_test.py
--rw-r-----   0 root         (0) root         (0)      653 2023-04-05 14:10:34.000000 pykern-20240402.175155/tests/pkcli/test1_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.908140 pykern-20240402.175155/tests/pkcli/test2_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.964140 pykern-20240402.175155/tests/pkcli/test2_data/1.in/
--rw-r-----   0 root         (0) root         (0)      338 2023-10-16 19:47:54.000000 pykern-20240402.175155/tests/pkcli/test2_data/1.in/coroutine_test.py
--rw-r-----   0 root         (0) root         (0)      739 2023-10-16 19:47:54.000000 pykern-20240402.175155/tests/pkcli/test2_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.908140 pykern-20240402.175155/tests/pkcli/test_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.964140 pykern-20240402.175155/tests/pkcli/test_data/tests/
--rw-r-----   0 root         (0) root         (0)      277 2019-12-04 23:50:51.000000 pykern-20240402.175155/tests/pkcli/test_data/tests/1_test.py
--rw-r-----   0 root         (0) root         (0)      282 2019-12-04 23:50:51.000000 pykern-20240402.175155/tests/pkcli/test_data/tests/2_test.py
--rw-r-----   0 root         (0) root         (0)      327 2024-02-13 15:11:30.000000 pykern-20240402.175155/tests/pkcli/test_data/tests/3_test.py
--rw-r-----   0 root         (0) root         (0)     2463 2024-02-13 15:11:30.000000 pykern-20240402.175155/tests/pkcli/test_test.py
--rw-r-----   0 root         (0) root         (0)      597 2022-06-30 14:07:51.000000 pykern-20240402.175155/tests/pkcli1_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.909140 pykern-20240402.175155/tests/pkcli_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.965140 pykern-20240402.175155/tests/pkcli_data/arghparsing/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/arghparsing/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.965140 pykern-20240402.175155/tests/pkcli_data/arghparsing/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/arghparsing/pkcli/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.965140 pykern-20240402.175155/tests/pkcli_data/command_info.in/
--rw-r-----   0 root         (0) root         (0)      140 2022-10-04 14:08:26.000000 pykern-20240402.175155/tests/pkcli_data/command_info.in/example_pkcli_module.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.965140 pykern-20240402.175155/tests/pkcli_data/command_info.out/
--rw-r-----   0 root         (0) root         (0)       17 2022-10-04 14:08:26.000000 pykern-20240402.175155/tests/pkcli_data/command_info.out/example_stderr.out
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.966140 pykern-20240402.175155/tests/pkcli_data/package1/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/package1/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.966140 pykern-20240402.175155/tests/pkcli_data/package1/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/package1/pkcli/__init__.py
--rw-r-----   0 root         (0) root         (0)      366 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/package1/pkcli/conf1.py
--rw-r-----   0 root         (0) root         (0)      178 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/package1/pkcli/conf2.py
--rw-r-----   0 root         (0) root         (0)      219 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/package1/pkcli/conf3.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.967140 pykern-20240402.175155/tests/pkcli_data/package2/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/package2/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.967140 pykern-20240402.175155/tests/pkcli_data/package2/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/package2/pkcli/__init__.py
--rw-r-----   0 root         (0) root         (0)      310 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/package2/pkcli/argh_test.py
--rw-r-----   0 root         (0) root         (0)      195 2023-12-07 23:37:10.000000 pykern-20240402.175155/tests/pkcli_data/package2/pkcli/some_mod.py
--rw-r-----   0 root         (0) root         (0)     4879 2024-03-15 14:11:15.000000 pykern-20240402.175155/tests/pkcli_test.py
--rw-r-----   0 root         (0) root         (0)     6378 2023-06-17 14:08:55.000000 pykern-20240402.175155/tests/pkcollections_test.py
--rw-r-----   0 root         (0) root         (0)     2276 2023-09-13 14:10:24.000000 pykern-20240402.175155/tests/pkcompat_test.py
--rw-r-----   0 root         (0) root         (0)     1862 2023-03-14 17:59:06.000000 pykern-20240402.175155/tests/pkconfig1_test.py
--rw-r-----   0 root         (0) root         (0)     1175 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkconfig2_test.py
--rw-r-----   0 root         (0) root         (0)      868 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkconfig3_test.py
--rw-r-----   0 root         (0) root         (0)      754 2023-04-14 17:14:13.000000 pykern-20240402.175155/tests/pkconfig4_test.py
--rw-r-----   0 root         (0) root         (0)     1588 2023-04-14 17:14:13.000000 pykern-20240402.175155/tests/pkconfig5_test.py
--rw-r-----   0 root         (0) root         (0)      623 2023-04-14 17:14:13.000000 pykern-20240402.175155/tests/pkconfig6_test.py
--rw-r-----   0 root         (0) root         (0)      617 2023-04-14 17:14:13.000000 pykern-20240402.175155/tests/pkconfig7_test.py
--rw-r-----   0 root         (0) root         (0)      350 2023-04-23 14:08:30.000000 pykern-20240402.175155/tests/pkconfig8_test.py
--rw-r-----   0 root         (0) root         (0)      421 2023-10-20 20:51:58.000000 pykern-20240402.175155/tests/pkconfig9_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.910140 pykern-20240402.175155/tests/pkconfig_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.968140 pykern-20240402.175155/tests/pkconfig_data/p1/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkconfig_data/p1/__init__.py
--rw-r-----   0 root         (0) root         (0)      214 2023-10-20 20:51:58.000000 pykern-20240402.175155/tests/pkconfig_data/p1/append_error.py
--rw-r-----   0 root         (0) root         (0)      469 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkconfig_data/p1/base_pkconfig.py
--rw-r-----   0 root         (0) root         (0)     1984 2020-01-08 19:20:36.000000 pykern-20240402.175155/tests/pkconfig_data/p1/m1.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.969140 pykern-20240402.175155/tests/pkconfig_data/p1/s1/
--rw-r-----   0 root         (0) root         (0)        2 2019-11-17 13:40:26.000000 pykern-20240402.175155/tests/pkconfig_data/p1/s1/__init__.py
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkconfig_data/p1/s1/m11.py
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkconfig_data/p1/s1/m12.py
--rw-r-----   0 root         (0) root         (0)    10382 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkdebug1_test.py
--rw-r-----   0 root         (0) root         (0)     1870 2023-08-16 14:09:51.000000 pykern-20240402.175155/tests/pkdebug2_test.py
--rw-r-----   0 root         (0) root         (0)     1737 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkexample_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.910140 pykern-20240402.175155/tests/pkinspect_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.970140 pykern-20240402.175155/tests/pkinspect_data/p1/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkinspect_data/p1/__init__.py
--rw-r-----   0 root         (0) root         (0)      326 2021-02-16 00:17:58.000000 pykern-20240402.175155/tests/pkinspect_data/p1/m1.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.970140 pykern-20240402.175155/tests/pkinspect_data/p1/p2/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkinspect_data/p1/p2/__init__.py
--rw-r-----   0 root         (0) root         (0)       35 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkinspect_data/p1/p2/m2.py
--rw-r-----   0 root         (0) root         (0)     3979 2024-01-19 15:11:21.000000 pykern-20240402.175155/tests/pkinspect_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.971140 pykern-20240402.175155/tests/pkio_data/
--rw-r-----   0 root         (0) root         (0)   239616 2024-02-01 15:11:17.000000 pykern-20240402.175155/tests/pkio_data/binary.dat
--rw-r-----   0 root         (0) root         (0)       18 2024-02-01 15:11:17.000000 pykern-20240402.175155/tests/pkio_data/text.dat
--rw-r-----   0 root         (0) root         (0)     7132 2024-03-15 14:11:15.000000 pykern-20240402.175155/tests/pkio_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.971140 pykern-20240402.175155/tests/pkjinja_data/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkjinja_data/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.971140 pykern-20240402.175155/tests/pkjinja_data/package_data/
--rw-r-----   0 root         (0) root         (0)       12 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkjinja_data/package_data/t1.jinja
--rw-r-----   0 root         (0) root         (0)      211 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkjinja_data/t1.py
--rw-r-----   0 root         (0) root         (0)      997 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkjinja_test.py
--rw-r-----   0 root         (0) root         (0)     1617 2023-10-17 17:55:03.000000 pykern-20240402.175155/tests/pkjson_test.py
--rw-r-----   0 root         (0) root         (0)     1415 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkplatform_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.972140 pykern-20240402.175155/tests/pkresource_data/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkresource_data/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.972140 pykern-20240402.175155/tests/pkresource_data/package_data/
--rw-r-----   0 root         (0) root         (0)       14 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkresource_data/package_data/somefile
--rw-r-----   0 root         (0) root         (0)      189 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkresource_data/t1.py
--rw-r-----   0 root         (0) root         (0)     1309 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkresource_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.972140 pykern-20240402.175155/tests/pkrunpy_data/
--rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkrunpy_data/f1.py
--rw-r-----   0 root         (0) root         (0)      533 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pkrunpy_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.913140 pykern-20240402.175155/tests/pksetup_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.974141 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/
--rw-r-----   0 root         (0) root         (0)      738 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/.gitignore
--rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/LICENSE
--rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/README.md
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.974141 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/docs/
--rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/docs/index.rst
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.974141 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/examples/
--rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/examples/example1.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.975140 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/pksetupunit1/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/pksetupunit1/__init__.py
--rw-r-----   0 root         (0) root         (0)      350 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/pksetupunit1/base_pkconfig.py
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/pksetupunit1/mod1.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.975140 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/pksetupunit1/package_data/
--rw-r-----   0 root         (0) root         (0)       10 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/pksetupunit1/package_data/data1
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.976140 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/__init__.py
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/mod2.py
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/requirements.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.976140 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/scripts/
--rw-r-----   0 root         (0) root         (0)       25 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/scripts/script1
--rw-r-----   0 root         (0) root         (0)      295 2019-05-06 20:05:16.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/setup.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.976140 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/tests/
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/tests/.gitignore
--rw-r-----   0 root         (0) root         (0)       99 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/tests/mod1_test.py
--rw-r-----   0 root         (0) root         (0)      181 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit1/tests/mod2_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.978140 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/
--rw-r-----   0 root         (0) root         (0)      756 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/.gitignore
--rw-r-----   0 root         (0) root         (0)      134 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/.travis.yml
--rw-r-----   0 root         (0) root         (0)    22102 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/LICENSE
--rw-r-----   0 root         (0) root         (0)      302 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/README.md
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.978140 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/docs/
--rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/docs/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.979140 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/docs/_static/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/docs/_static/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.979140 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/docs/_templates/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/docs/_templates/.gitignore
--rw-r-----   0 root         (0) root         (0)      227 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/docs/index.rst
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.980141 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/pksetupunit2/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/pksetupunit2/__init__.py
--rw-r-----   0 root         (0) root         (0)      350 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/pksetupunit2/base_pkconfig.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.980141 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/pksetupunit2/package_data/
--rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/pksetupunit2/package_data/.gitignore
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.980141 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/pksetupunit2/pkcli/
--rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/pksetupunit2/pkcli/__init__.py
--rw-r-----   0 root         (0) root         (0)      466 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/pksetupunit2/pksetupunit2_console.py
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/requirements.txt
--rw-r-----   0 root         (0) root         (0)     1051 2019-05-06 20:05:16.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/setup.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.981140 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/tests/
--rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/tests/.gitignore
--rw-r-----   0 root         (0) root         (0)      321 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pksetup_data/pksetupunit2/tests/simple_test.py
--rw-r-----   0 root         (0) root         (0)     5098 2023-04-04 14:10:19.000000 pykern-20240402.175155/tests/pksetup_test.py
--rw-r-----   0 root         (0) root         (0)     3892 2022-06-24 14:08:21.000000 pykern-20240402.175155/tests/pksubprocess_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.916140 pykern-20240402.175155/tests/pkunit1_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.981140 pykern-20240402.175155/tests/pkunit1_data/bytes-1.in/
--rw-r-----   0 root         (0) root         (0)       42 2023-04-14 14:08:36.000000 pykern-20240402.175155/tests/pkunit1_data/bytes-1.in/dot.gif
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.981140 pykern-20240402.175155/tests/pkunit1_data/bytes-1.out/
--rw-r-----   0 root         (0) root         (0)       42 2023-04-14 14:08:36.000000 pykern-20240402.175155/tests/pkunit1_data/bytes-1.out/dot.gif
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.982140 pykern-20240402.175155/tests/pkunit1_data/conformance-1.in/
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/conformance-1.in/in.txt
--rw-r-----   0 root         (0) root         (0)      102 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/conformance-1.in/res.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.982140 pykern-20240402.175155/tests/pkunit1_data/conformance-1.out/
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/conformance-1.out/in.txt
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/conformance-1.out/out.txt
--rw-r-----   0 root         (0) root         (0)      102 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/conformance-1.out/res.json
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.983141 pykern-20240402.175155/tests/pkunit1_data/conformance-2.in/
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/conformance-2.in/in.txt
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/conformance-2.in/out.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.983141 pykern-20240402.175155/tests/pkunit1_data/conformance-2.out/
--rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/conformance-2.out/in.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.983141 pykern-20240402.175155/tests/pkunit1_data/curly_brackets.in/
--rw-r-----   0 root         (0) root         (0)       13 2022-09-20 14:07:49.000000 pykern-20240402.175155/tests/pkunit1_data/curly_brackets.in/sample.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.984140 pykern-20240402.175155/tests/pkunit1_data/curly_brackets.out/
--rw-r-----   0 root         (0) root         (0)        9 2022-09-20 14:07:49.000000 pykern-20240402.175155/tests/pkunit1_data/curly_brackets.out/sample.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.984140 pykern-20240402.175155/tests/pkunit1_data/deviance-1.in/
--rw-r-----   0 root         (0) root         (0)        0 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/deviance-1.in/not-used.txt
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.984140 pykern-20240402.175155/tests/pkunit1_data/deviance-1.out/
--rw-r-----   0 root         (0) root         (0)        9 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/pkunit1_data/deviance-1.out/out.txt
--rw-r-----   0 root         (0) root         (0)     1449 2023-04-14 14:08:36.000000 pykern-20240402.175155/tests/pkunit1_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.990141 pykern-20240402.175155/tests/pkunit_data/
--rw-r-----   0 root         (0) root         (0)       24 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/actual_abs_ok.ndiff
--rw-r-----   0 root         (0) root         (0)       48 2022-12-08 15:07:12.000000 pykern-20240402.175155/tests/pkunit_data/actual_conformance_2.ndiff
--rw-r-----   0 root         (0) root         (0)       53 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/actual_default_conformance.ndiff
--rw-r-----   0 root         (0) root         (0)       53 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/actual_default_conformance_1.ndiff
--rw-r-----   0 root         (0) root         (0)       15 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/actual_rel_ok.ndiff
--rw-r-----   0 root         (0) root         (0)       21 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/actual_rel_ok_2.ndiff
--rw-r-----   0 root         (0) root         (0)       15 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkunit_data/assert1.json
--rw-r-----   0 root         (0) root         (0)       88 2022-08-23 22:15:42.000000 pykern-20240402.175155/tests/pkunit_data/different.bin
--rw-r-----   0 root         (0) root         (0)      543 2022-05-16 23:38:16.000000 pykern-20240402.175155/tests/pkunit_data/example.csv
--rw-r-----   0 root         (0) root         (0)     5425 2022-05-16 23:38:16.000000 pykern-20240402.175155/tests/pkunit_data/example.xlsx
--rw-r-----   0 root         (0) root         (0)       24 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/expect_abs_ok.ndiff
--rw-r-----   0 root         (0) root         (0)       48 2022-12-08 15:07:12.000000 pykern-20240402.175155/tests/pkunit_data/expect_conformance_2.ndiff
--rw-r-----   0 root         (0) root         (0)       52 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/expect_default_conformance.ndiff
--rw-r-----   0 root         (0) root         (0)       51 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/expect_default_conformance_1.ndiff
--rw-r-----   0 root         (0) root         (0)       15 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/expect_rel_ok.ndiff
--rw-r-----   0 root         (0) root         (0)       21 2023-03-17 14:08:25.000000 pykern-20240402.175155/tests/pkunit_data/expect_rel_ok_2.ndiff
--rw-r-----   0 root         (0) root         (0)       20 2022-04-08 21:30:14.000000 pykern-20240402.175155/tests/pkunit_data/file_eq1.json
--rw-r-----   0 root         (0) root         (0)        0 2022-04-08 21:30:14.000000 pykern-20240402.175155/tests/pkunit_data/file_eq2.txt
--rw-r-----   0 root         (0) root         (0)       14 2022-04-08 21:30:14.000000 pykern-20240402.175155/tests/pkunit_data/file_eq3.txt
--rw-r-----   0 root         (0) root         (0)       67 2022-08-25 16:28:29.000000 pykern-20240402.175155/tests/pkunit_data/ignore_lines.in
--rw-r-----   0 root         (0) root         (0)       68 2022-08-25 16:28:29.000000 pykern-20240402.175155/tests/pkunit_data/ignore_lines.out
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.916140 pykern-20240402.175155/tests/pkunit_data/import1/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.990141 pykern-20240402.175155/tests/pkunit_data/import1/p1/
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkunit_data/import1/p1/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.916140 pykern-20240402.175155/tests/pkunit_data/import2/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.990141 pykern-20240402.175155/tests/pkunit_data/import2/p1/
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkunit_data/import2/p1/__init__.py
--rw-r-----   0 root         (0) root         (0)      100 2022-08-23 22:15:42.000000 pykern-20240402.175155/tests/pkunit_data/in.bin
--rw-r-----   0 root         (0) root         (0)      100 2022-08-23 22:15:42.000000 pykern-20240402.175155/tests/pkunit_data/out.bin
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkunit_data/t1.yml
--rw-r-----   0 root         (0) root         (0)     8413 2023-10-30 22:15:18.000000 pykern-20240402.175155/tests/pkunit_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.990141 pykern-20240402.175155/tests/pkyaml_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.991140 pykern-20240402.175155/tests/pkyaml_data/1.in/
--rw-r-----   0 root         (0) root         (0)       65 2022-07-12 14:07:33.000000 pykern-20240402.175155/tests/pkyaml_data/1.in/in.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.991140 pykern-20240402.175155/tests/pkyaml_data/1.out/
--rw-r-----   0 root         (0) root         (0)       62 2022-07-12 14:07:33.000000 pykern-20240402.175155/tests/pkyaml_data/1.out/out.yml
--rw-r-----   0 root         (0) root         (0)       27 2020-09-03 15:51:30.000000 pykern-20240402.175155/tests/pkyaml_data/dump1.yml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.991140 pykern-20240402.175155/tests/pkyaml_data/p1/
--rw-r-----   0 root         (0) root         (0)       61 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkyaml_data/p1/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.991140 pykern-20240402.175155/tests/pkyaml_data/p1/package_data/
--rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240402.175155/tests/pkyaml_data/p1/package_data/conf2.yml
--rw-r-----   0 root         (0) root         (0)     1275 2022-07-12 14:07:33.000000 pykern-20240402.175155/tests/pkyaml_test.py
--rw-r-----   0 root         (0) root         (0)     1163 2024-02-01 15:11:17.000000 pykern-20240402.175155/tests/util_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.919140 pykern-20240402.175155/tests/xlsx_data/
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.992140 pykern-20240402.175155/tests/xlsx_data/1.in/
--rw-r-----   0 root         (0) root         (0)      903 2022-08-02 14:08:07.000000 pykern-20240402.175155/tests/xlsx_data/1.in/case.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.992140 pykern-20240402.175155/tests/xlsx_data/1.out/
--rw-r-----   0 root         (0) root         (0)       58 2022-08-02 14:08:07.000000 pykern-20240402.175155/tests/xlsx_data/1.out/case1.csv
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.992140 pykern-20240402.175155/tests/xlsx_data/1.out/xl/
--rw-r-----   0 root         (0) root         (0)      281 2022-08-02 14:08:07.000000 pykern-20240402.175155/tests/xlsx_data/1.out/xl/sharedStrings.xml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.992140 pykern-20240402.175155/tests/xlsx_data/1.out/xl/worksheets/
--rw-r-----   0 root         (0) root         (0)     1250 2022-08-02 14:08:07.000000 pykern-20240402.175155/tests/xlsx_data/1.out/xl/worksheets/sheet1.xml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.993141 pykern-20240402.175155/tests/xlsx_data/2.in/
--rw-r-----   0 root         (0) root         (0)     1057 2022-08-10 14:07:21.000000 pykern-20240402.175155/tests/xlsx_data/2.in/case.py
--rw-r-----   0 root         (0) root         (0)     6288 2022-08-02 14:08:07.000000 pykern-20240402.175155/tests/xlsx_data/2.in/case2.xlsx
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.993141 pykern-20240402.175155/tests/xlsx_data/2.out/
--rw-r-----   0 root         (0) root         (0)       90 2022-08-10 14:07:21.000000 pykern-20240402.175155/tests/xlsx_data/2.out/case2#0.csv
--rw-r-----   0 root         (0) root         (0)        9 2022-06-03 23:08:48.000000 pykern-20240402.175155/tests/xlsx_data/2.out/case2#1.csv
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.994140 pykern-20240402.175155/tests/xlsx_data/2.out/xl/
--rw-r-----   0 root         (0) root         (0)      338 2022-08-10 14:07:21.000000 pykern-20240402.175155/tests/xlsx_data/2.out/xl/sharedStrings.xml
--rw-r-----   0 root         (0) root         (0)     1656 2023-03-14 17:59:06.000000 pykern-20240402.175155/tests/xlsx_data/2.out/xl/styles.xml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.994140 pykern-20240402.175155/tests/xlsx_data/2.out/xl/worksheets/
--rw-r-----   0 root         (0) root         (0)     1830 2023-01-16 15:07:03.000000 pykern-20240402.175155/tests/xlsx_data/2.out/xl/worksheets/sheet1.xml
--rw-r-----   0 root         (0) root         (0)      795 2022-06-03 23:08:48.000000 pykern-20240402.175155/tests/xlsx_data/2.out/xl/worksheets/sheet2.xml
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.995140 pykern-20240402.175155/tests/xlsx_data/3.in/
--rw-r-----   0 root         (0) root         (0)      484 2022-08-02 14:08:07.000000 pykern-20240402.175155/tests/xlsx_data/3.in/case.py
-drwxr-x---   0 root         (0) root         (0)        0 2024-04-02 19:12:09.995140 pykern-20240402.175155/tests/xlsx_data/3.out/
--rw-r-----   0 root         (0) root         (0)       38 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/xlsx_data/3.out/pkexcept
--rw-r-----   0 root         (0) root         (0)     1114 2022-08-06 14:07:18.000000 pykern-20240402.175155/tests/xlsx_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.433140 pykern-20240405.195819/
+-rw-r-----   0 root         (0) root         (0)    11324 2018-02-06 22:51:04.000000 pykern-20240405.195819/LICENSE
+-rw-r-----   0 root         (0) root         (0)      182 2024-03-19 18:50:32.000000 pykern-20240405.195819/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-04-09 14:46:27.433140 pykern-20240405.195819/PKG-INFO
+-rw-r-----   0 root         (0) root         (0)      264 2024-03-20 14:13:19.000000 pykern-20240405.195819/README.md
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.356140 pykern-20240405.195819/docs/
+-rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240405.195819/docs/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.356140 pykern-20240405.195819/docs/_static/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/docs/_static/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.357140 pykern-20240405.195819/docs/_templates/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/docs/_templates/.gitignore
+-rw-r-----   0 root         (0) root         (0)      365 2018-02-06 22:51:04.000000 pykern-20240405.195819/docs/index.rst
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.363140 pykern-20240405.195819/pykern/
+-rw-r-----   0 root         (0) root         (0)      354 2024-03-20 14:13:19.000000 pykern-20240405.195819/pykern/__init__.py
+-rw-r-----   0 root         (0) root         (0)    17824 2023-10-20 20:51:58.000000 pykern-20240405.195819/pykern/fconf.py
+-rw-r-----   0 root         (0) root         (0)     1029 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/mpi.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.365140 pykern-20240405.195819/pykern/package_data/
+-rw-r-----   0 root         (0) root         (0)     9727 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/docs-conf.py.format
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.366140 pykern-20240405.195819/pykern/package_data/projex/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.333140 pykern-20240405.195819/pykern/package_data/projex/.github/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.368140 pykern-20240405.195819/pykern/package_data/projex/.github/workflows/
+-rw-r-----   0 root         (0) root         (0)      281 2022-07-20 23:21:19.000000 pykern-20240405.195819/pykern/package_data/projex/.github/workflows/python-ci.yml.jinja
+-rw-r-----   0 root         (0) root         (0)      221 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/README.md.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.369140 pykern-20240405.195819/pykern/package_data/projex/docs/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.369140 pykern-20240405.195819/pykern/package_data/projex/docs/_static/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/docs/_static/dot-gitignore.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.369140 pykern-20240405.195819/pykern/package_data/projex/docs/_templates/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/docs/_templates/dot-gitignore.jinja
+-rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/docs/dot-gitignore.jinja
+-rw-r-----   0 root         (0) root         (0)      207 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/docs/index.rst.jinja
+-rw-r-----   0 root         (0) root         (0)      772 2022-02-12 15:07:54.000000 pykern-20240405.195819/pykern/package_data/projex/dot-gitignore.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.370140 pykern-20240405.195819/pykern/package_data/projex/projex/
+-rw-r-----   0 root         (0) root         (0)      296 2022-10-24 20:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/projex/__init__.py.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.370140 pykern-20240405.195819/pykern/package_data/projex/projex/package_data/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/projex/package_data/dot-gitignore.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.370140 pykern-20240405.195819/pykern/package_data/projex/projex/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/projex/pkcli/__init__.py.jinja
+-rw-r-----   0 root         (0) root         (0)      298 2022-10-24 20:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/projex/projex_console.py.jinja
+-rw-r-----   0 root         (0) root         (0)      578 2022-10-24 20:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/setup.py.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.371140 pykern-20240405.195819/pykern/package_data/projex/tests/
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/tests/dot-gitignore.jinja
+-rw-r-----   0 root         (0) root         (0)      228 2022-10-24 20:51:04.000000 pykern-20240405.195819/pykern/package_data/projex/tests/import_test.py.jinja
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.368140 pykern-20240405.195819/pykern/package_data/projex-licenses/
+-rw-r-----   0 root         (0) root         (0)    34520 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex-licenses/agpl-3.0.txt
+-rw-r-----   0 root         (0) root         (0)    11358 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex-licenses/apache2.jinja
+-rw-r-----   0 root         (0) root         (0)    18092 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex-licenses/gpl2.jinja
+-rw-r-----   0 root         (0) root         (0)    35147 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex-licenses/gpl3.jinja
+-rw-r-----   0 root         (0) root         (0)    25383 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex-licenses/lgpl2.jinja
+-rw-r-----   0 root         (0) root         (0)     7651 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex-licenses/lgpl3.jinja
+-rw-r-----   0 root         (0) root         (0)     1085 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex-licenses/mit.jinja
+-rw-r-----   0 root         (0) root         (0)      191 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/projex-licenses/proprietary.jinja
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240405.195819/pykern/package_data/test.yml
+-rw-r-----   0 root         (0) root         (0)     1169 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pkarray.py
+-rw-r-----   0 root         (0) root         (0)     2845 2024-03-15 14:11:15.000000 pykern-20240405.195819/pykern/pkasyncio.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.373140 pykern-20240405.195819/pykern/pkcli/
+-rw-r-----   0 root         (0) root         (0)    10485 2024-03-15 14:11:15.000000 pykern-20240405.195819/pykern/pkcli/__init__.py
+-rw-r-----   0 root         (0) root         (0)     4170 2024-03-20 14:13:19.000000 pykern-20240405.195819/pykern/pkcli/ci.py
+-rw-r-----   0 root         (0) root         (0)     1763 2022-12-28 15:07:11.000000 pykern-20240405.195819/pykern/pkcli/fmt.py
+-rw-r-----   0 root         (0) root         (0)    20449 2024-03-15 14:11:15.000000 pykern-20240405.195819/pykern/pkcli/github.py
+-rw-r-----   0 root         (0) root         (0)    12793 2022-10-31 19:53:53.000000 pykern-20240405.195819/pykern/pkcli/github_orgmode.py
+-rw-r-----   0 root         (0) root         (0)     2849 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pkcli/pkexample.py
+-rw-r-----   0 root         (0) root         (0)     4773 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pkcli/projex.py
+-rw-r-----   0 root         (0) root         (0)     3039 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pkcli/rsmanifest.py
+-rw-r-----   0 root         (0) root         (0)     6686 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pkcli/sim.py
+-rw-r-----   0 root         (0) root         (0)     7427 2024-04-06 14:13:17.000000 pykern-20240405.195819/pykern/pkcli/test.py
+-rw-r-----   0 root         (0) root         (0)    13807 2024-04-03 20:20:06.000000 pykern-20240405.195819/pykern/pkcollections.py
+-rw-r-----   0 root         (0) root         (0)     3686 2023-09-13 14:10:24.000000 pykern-20240405.195819/pykern/pkcompat.py
+-rw-r-----   0 root         (0) root         (0)    24232 2023-10-20 20:51:58.000000 pykern-20240405.195819/pykern/pkconfig.py
+-rw-r-----   0 root         (0) root         (0)     1221 2024-03-28 17:40:02.000000 pykern-20240405.195819/pykern/pkconst.py
+-rw-r-----   0 root         (0) root         (0)    22756 2024-01-19 15:11:21.000000 pykern-20240405.195819/pykern/pkdebug.py
+-rw-r-----   0 root         (0) root         (0)     4591 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pkexample.py
+-rw-r-----   0 root         (0) root         (0)     8826 2024-01-19 15:11:21.000000 pykern-20240405.195819/pykern/pkinspect.py
+-rw-r-----   0 root         (0) root         (0)    10253 2024-02-01 15:11:17.000000 pykern-20240405.195819/pykern/pkio.py
+-rw-r-----   0 root         (0) root         (0)     1857 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pkjinja.py
+-rw-r-----   0 root         (0) root         (0)     2302 2024-01-12 21:32:37.000000 pykern-20240405.195819/pykern/pkjson.py
+-rw-r-----   0 root         (0) root         (0)     1427 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pkplatform.py
+-rw-r-----   0 root         (0) root         (0)     3214 2024-03-28 17:40:02.000000 pykern-20240405.195819/pykern/pkresource.py
+-rw-r-----   0 root         (0) root         (0)      774 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pkrunpy.py
+-rw-r-----   0 root         (0) root         (0)    22115 2024-03-28 17:40:02.000000 pykern-20240405.195819/pykern/pksetup.py
+-rw-r-----   0 root         (0) root         (0)     4287 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pksubprocess.py
+-rw-r-----   0 root         (0) root         (0)    25421 2024-03-20 14:13:19.000000 pykern-20240405.195819/pykern/pkunit.py
+-rw-r-----   0 root         (0) root         (0)     2578 2022-07-12 14:07:33.000000 pykern-20240405.195819/pykern/pkyaml.py
+-rw-r-----   0 root         (0) root         (0)      421 2022-06-24 14:08:21.000000 pykern-20240405.195819/pykern/pykern_console.py
+-rw-r-----   0 root         (0) root         (0)      180 2024-03-20 14:13:19.000000 pykern-20240405.195819/pykern/pytest_plugin.py
+-rw-r-----   0 root         (0) root         (0)      404 2022-09-26 20:14:13.000000 pykern-20240405.195819/pykern/quest.py
+-rw-r-----   0 root         (0) root         (0)     3756 2024-03-15 14:11:15.000000 pykern-20240405.195819/pykern/util.py
+-rw-r-----   0 root         (0) root         (0)    23884 2023-09-25 14:09:48.000000 pykern-20240405.195819/pykern/xlsx.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.432140 pykern-20240405.195819/pykern.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-04-09 14:46:27.000000 pykern-20240405.195819/pykern.egg-info/PKG-INFO
+-rw-r-----   0 root         (0) root         (0)    11319 2024-04-09 14:46:27.000000 pykern-20240405.195819/pykern.egg-info/SOURCES.txt
+-rw-r-----   0 root         (0) root         (0)        1 2024-04-09 14:46:27.000000 pykern-20240405.195819/pykern.egg-info/dependency_links.txt
+-rw-r-----   0 root         (0) root         (0)       54 2024-04-09 14:46:27.000000 pykern-20240405.195819/pykern.egg-info/entry_points.txt
+-rw-r-----   0 root         (0) root         (0)      376 2024-04-09 14:46:27.000000 pykern-20240405.195819/pykern.egg-info/requires.txt
+-rw-r-----   0 root         (0) root         (0)        7 2024-04-09 14:46:27.000000 pykern-20240405.195819/pykern.egg-info/top_level.txt
+-rw-r-----   0 root         (0) root         (0)     1455 2024-04-02 19:05:05.000000 pykern-20240405.195819/pyproject.toml
+-rw-r-----   0 root         (0) root         (0)       38 2024-04-09 14:46:27.433140 pykern-20240405.195819/setup.cfg
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.382140 pykern-20240405.195819/tests/
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/.gitignore
+-rw-r-----   0 root         (0) root         (0)      554 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/conftest.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.336140 pykern-20240405.195819/tests/fconf_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.383140 pykern-20240405.195819/tests/fconf_data/1.in/
+-rw-r-----   0 root         (0) root         (0)      450 2022-07-18 15:54:21.000000 pykern-20240405.195819/tests/fconf_data/1.in/0.py
+-rw-r-----   0 root         (0) root         (0)      883 2022-07-18 15:54:21.000000 pykern-20240405.195819/tests/fconf_data/1.in/1.yml
+-rw-r-----   0 root         (0) root         (0)       57 2022-07-07 14:08:03.000000 pykern-20240405.195819/tests/fconf_data/1.in/2.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.383140 pykern-20240405.195819/tests/fconf_data/1.out/
+-rw-r-----   0 root         (0) root         (0)     1647 2022-07-18 15:54:21.000000 pykern-20240405.195819/tests/fconf_data/1.out/res.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.383140 pykern-20240405.195819/tests/fconf_data/2.in/
+-rw-r-----   0 root         (0) root         (0)      139 2022-07-07 14:08:03.000000 pykern-20240405.195819/tests/fconf_data/2.in/1.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.384140 pykern-20240405.195819/tests/fconf_data/2.out/
+-rw-r-----   0 root         (0) root         (0)      374 2022-07-07 14:08:03.000000 pykern-20240405.195819/tests/fconf_data/2.out/res.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.385140 pykern-20240405.195819/tests/fconf_data/3.in/
+-rw-r-----   0 root         (0) root         (0)       71 2022-07-07 14:08:03.000000 pykern-20240405.195819/tests/fconf_data/3.in/0.py
+-rw-r-----   0 root         (0) root         (0)       71 2022-07-07 14:08:03.000000 pykern-20240405.195819/tests/fconf_data/3.in/1.py
+-rw-r-----   0 root         (0) root         (0)       11 2022-07-07 14:08:03.000000 pykern-20240405.195819/tests/fconf_data/3.in/2.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.385140 pykern-20240405.195819/tests/fconf_data/3.out/
+-rw-r-----   0 root         (0) root         (0)      118 2022-07-07 14:08:03.000000 pykern-20240405.195819/tests/fconf_data/3.out/res.json
+-rw-r-----   0 root         (0) root         (0)      602 2022-07-07 14:08:03.000000 pykern-20240405.195819/tests/fconf_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.385140 pykern-20240405.195819/tests/mpi_data/
+-rw-r-----   0 root         (0) root         (0)      925 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/mpi_data/p1.py
+-rw-r-----   0 root         (0) root         (0)     1307 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/mpi_test.py
+-rw-r-----   0 root         (0) root         (0)      885 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkarray_test.py
+-rw-r-----   0 root         (0) root         (0)     2633 2024-01-19 15:11:21.000000 pykern-20240405.195819/tests/pkasyncio_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.388140 pykern-20240405.195819/tests/pkcli/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.337140 pykern-20240405.195819/tests/pkcli/ci1_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.388140 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.388140 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/.x/
+-rw-r-----   0 root         (0) root         (0)       61 2022-06-29 14:08:01.000000 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/.x/x.py
+-rw-r-----   0 root         (0) root         (0)       34 2022-06-29 14:08:01.000000 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/setup.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.389140 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/somepkg/
+-rw-r-----   0 root         (0) root         (0)        8 2022-06-29 14:08:01.000000 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/somepkg/has_print.py
+-rw-r-----   0 root         (0) root         (0)       14 2022-06-29 14:08:01.000000 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/somepkg/ok.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.389140 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/somepkg/package_data/
+-rw-r-----   0 root         (0) root         (0)       50 2022-06-29 14:08:01.000000 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/somepkg/package_data/not_checked.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.337140 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/tests/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.389140 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/tests/test_data/
+-rw-r-----   0 root         (0) root         (0)       50 2022-06-29 14:08:01.000000 pykern-20240405.195819/tests/pkcli/ci1_data/1.in/tests/test_data/not_checked.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.389140 pykern-20240405.195819/tests/pkcli/ci1_data/1.out/
+-rw-r-----   0 root         (0) root         (0)       45 2022-10-22 14:07:30.000000 pykern-20240405.195819/tests/pkcli/ci1_data/1.out/pkexcept
+-rw-r-----   0 root         (0) root         (0)      428 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkcli/ci1_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.340140 pykern-20240405.195819/tests/pkcli/ci_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.390140 pykern-20240405.195819/tests/pkcli/ci_data/check_eof_newline-1.in/
+-rw-r-----   0 root         (0) root         (0)       36 2022-11-17 18:34:08.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_eof_newline-1.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.390140 pykern-20240405.195819/tests/pkcli/ci_data/check_eof_newline-1.out/
+-rw-r-----   0 root         (0) root         (0)       24 2022-11-17 18:34:08.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_eof_newline-1.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.390140 pykern-20240405.195819/tests/pkcli/ci_data/check_eof_newline-2.in/
+-rw-r-----   0 root         (0) root         (0)       45 2022-11-17 18:34:08.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_eof_newline-2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.390140 pykern-20240405.195819/tests/pkcli/ci_data/check_eof_newline-2.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:08.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_eof_newline-2.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.391140 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-1.in/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.391140 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-1.in/run/
+-rw-r-----   0 root         (0) root         (0)       27 2022-11-17 18:34:08.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-1.in/run/ignored.py
+-rw-r-----   0 root         (0) root         (0)      191 2022-11-17 18:34:08.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-1.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.391140 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-1.out/
+-rw-r-----   0 root         (0) root         (0)      148 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-1.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.391140 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-2.in/
+-rw-r-----   0 root         (0) root         (0)      208 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.392140 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-2.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-2.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.392140 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-3.in/
+-rw-r-----   0 root         (0) root         (0)       87 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-3.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.392140 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-3.out/
+-rw-r-----   0 root         (0) root         (0)       82 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-3.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.392140 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-4.in/
+-rw-r-----   0 root         (0) root         (0)       10 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-4.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.393140 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-4.out/
+-rw-r-----   0 root         (0) root         (0)       31 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/check_prints-4.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.393140 pykern-20240405.195819/tests/pkcli/ci_data/run-1.in/
+-rw-r-----   0 root         (0) root         (0)       20 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/run-1.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.393140 pykern-20240405.195819/tests/pkcli/ci_data/run-1.out/
+-rw-r-----   0 root         (0) root         (0)       14 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/run-1.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.393140 pykern-20240405.195819/tests/pkcli/ci_data/run-2.in/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.394140 pykern-20240405.195819/tests/pkcli/ci_data/run-2.in/tests/
+-rw-r-----   0 root         (0) root         (0)       23 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/run-2.in/tests/x_test.py
+-rw-r-----   0 root         (0) root         (0)       23 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/run-2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.394140 pykern-20240405.195819/tests/pkcli/ci_data/run-2.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_data/run-2.out/pkexcept
+-rw-r-----   0 root         (0) root         (0)      400 2022-11-17 18:34:09.000000 pykern-20240405.195819/tests/pkcli/ci_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.342140 pykern-20240405.195819/tests/pkcli/fmt_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.394140 pykern-20240405.195819/tests/pkcli/fmt_data/check1.in/
+-rw-r-----   0 root         (0) root         (0)       44 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/check1.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.394140 pykern-20240405.195819/tests/pkcli/fmt_data/check1.out/
+-rw-r-----   0 root         (0) root         (0)       39 2022-12-28 15:07:11.000000 pykern-20240405.195819/tests/pkcli/fmt_data/check1.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.395140 pykern-20240405.195819/tests/pkcli/fmt_data/check2.in/
+-rw-r-----   0 root         (0) root         (0)       56 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/check2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.395140 pykern-20240405.195819/tests/pkcli/fmt_data/check2.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-06-18 14:08:41.000000 pykern-20240405.195819/tests/pkcli/fmt_data/check2.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.395140 pykern-20240405.195819/tests/pkcli/fmt_data/diff.in/
+-rw-r-----   0 root         (0) root         (0)      245 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/diff.in/file1.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.395140 pykern-20240405.195819/tests/pkcli/fmt_data/diff.out/
+-rw-r-----   0 root         (0) root         (0)        5 2022-06-18 14:08:41.000000 pykern-20240405.195819/tests/pkcli/fmt_data/diff.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.396140 pykern-20240405.195819/tests/pkcli/fmt_data/diff2.in/
+-rw-r-----   0 root         (0) root         (0)      368 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/diff2.in/x.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.396140 pykern-20240405.195819/tests/pkcli/fmt_data/diff2.out/
+-rw-r-----   0 root         (0) root         (0)       14 2022-06-18 14:08:41.000000 pykern-20240405.195819/tests/pkcli/fmt_data/diff2.out/pkexcept
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.397140 pykern-20240405.195819/tests/pkcli/fmt_data/fmt_dir.in/
+-rw-r-----   0 root         (0) root         (0)      170 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/fmt_dir.in/file1.py
+-rw-r-----   0 root         (0) root         (0)      483 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/fmt_dir.in/y.py
+-rw-r-----   0 root         (0) root         (0)      244 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/fmt_dir.in/z.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.397140 pykern-20240405.195819/tests/pkcli/fmt_data/fmt_dir.out/
+-rw-r-----   0 root         (0) root         (0)      245 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/fmt_dir.out/file1.py
+-rw-r-----   0 root         (0) root         (0)      584 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/fmt_dir.out/y.py
+-rw-r-----   0 root         (0) root         (0)      324 2022-06-14 14:07:59.000000 pykern-20240405.195819/tests/pkcli/fmt_data/fmt_dir.out/z.py
+-rw-r-----   0 root         (0) root         (0)      798 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkcli/fmt_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.343140 pykern-20240405.195819/tests/pkcli/github_orgmode_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.398140 pykern-20240405.195819/tests/pkcli/github_orgmode_data/assignee_issues-1.in/
+-rw-r-----   0 root         (0) root         (0)    20455 2022-10-11 14:09:00.000000 pykern-20240405.195819/tests/pkcli/github_orgmode_data/assignee_issues-1.in/repo.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.398140 pykern-20240405.195819/tests/pkcli/github_orgmode_data/assignee_issues-1.out/
+-rw-r-----   0 root         (0) root         (0)     1301 2022-10-15 14:08:58.000000 pykern-20240405.195819/tests/pkcli/github_orgmode_data/assignee_issues-1.out/assignee_issues.org
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.398140 pykern-20240405.195819/tests/pkcli/github_orgmode_data/from_issues-1.in/
+-rw-r-----   0 root         (0) root         (0)    21657 2022-10-11 14:09:00.000000 pykern-20240405.195819/tests/pkcli/github_orgmode_data/from_issues-1.in/repo.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.398140 pykern-20240405.195819/tests/pkcli/github_orgmode_data/from_issues-1.out/
+-rw-r-----   0 root         (0) root         (0)     1056 2022-10-15 14:08:58.000000 pykern-20240405.195819/tests/pkcli/github_orgmode_data/from_issues-1.out/radiasoft-test-pykern-github-orgmode.org
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.399140 pykern-20240405.195819/tests/pkcli/github_orgmode_data/to_issues-1.in/
+-rw-r-----   0 root         (0) root         (0)     2922 2022-10-11 14:09:00.000000 pykern-20240405.195819/tests/pkcli/github_orgmode_data/to_issues-1.in/repo.json
+-rw-r-----   0 root         (0) root         (0)     1264 2022-10-11 14:09:00.000000 pykern-20240405.195819/tests/pkcli/github_orgmode_data/to_issues-1.in/to_issues-1.org
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.399140 pykern-20240405.195819/tests/pkcli/github_orgmode_data/to_issues-1.out/
+-rw-r-----   0 root         (0) root         (0)      933 2022-10-11 14:09:00.000000 pykern-20240405.195819/tests/pkcli/github_orgmode_data/to_issues-1.out/res.json
+-rw-r-----   0 root         (0) root         (0)     2312 2022-10-31 19:53:53.000000 pykern-20240405.195819/tests/pkcli/github_orgmode_test.py
+-rw-r-----   0 root         (0) root         (0)     4988 2024-03-15 14:11:15.000000 pykern-20240405.195819/tests/pkcli/github_test.py
+-rw-r-----   0 root         (0) root         (0)     2923 2023-08-16 14:09:51.000000 pykern-20240405.195819/tests/pkcli/projex_test.py
+-rw-r-----   0 root         (0) root         (0)     1995 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkcli/rsmanifest_test.py
+-rw-r-----   0 root         (0) root         (0)     1816 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkcli/sim_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.343140 pykern-20240405.195819/tests/pkcli/test1_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.400140 pykern-20240405.195819/tests/pkcli/test1_data/tests/
+-rw-r-----   0 root         (0) root         (0)      293 2023-04-05 14:10:34.000000 pykern-20240405.195819/tests/pkcli/test1_data/tests/always_test.py
+-rw-r-----   0 root         (0) root         (0)      461 2023-04-05 14:10:34.000000 pykern-20240405.195819/tests/pkcli/test1_data/tests/twice_test.py
+-rw-r-----   0 root         (0) root         (0)      653 2023-04-05 14:10:34.000000 pykern-20240405.195819/tests/pkcli/test1_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.344140 pykern-20240405.195819/tests/pkcli/test2_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.400140 pykern-20240405.195819/tests/pkcli/test2_data/1.in/
+-rw-r-----   0 root         (0) root         (0)      338 2023-10-16 19:47:54.000000 pykern-20240405.195819/tests/pkcli/test2_data/1.in/coroutine_test.py
+-rw-r-----   0 root         (0) root         (0)      685 2024-04-06 14:13:17.000000 pykern-20240405.195819/tests/pkcli/test2_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.344140 pykern-20240405.195819/tests/pkcli/test_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.401140 pykern-20240405.195819/tests/pkcli/test_data/tests/
+-rw-r-----   0 root         (0) root         (0)      277 2019-12-04 23:50:51.000000 pykern-20240405.195819/tests/pkcli/test_data/tests/1_test.py
+-rw-r-----   0 root         (0) root         (0)      282 2019-12-04 23:50:51.000000 pykern-20240405.195819/tests/pkcli/test_data/tests/2_test.py
+-rw-r-----   0 root         (0) root         (0)      327 2024-02-13 15:11:30.000000 pykern-20240405.195819/tests/pkcli/test_data/tests/3_test.py
+-rw-r-----   0 root         (0) root         (0)     2463 2024-02-13 15:11:30.000000 pykern-20240405.195819/tests/pkcli/test_test.py
+-rw-r-----   0 root         (0) root         (0)      597 2022-06-30 14:07:51.000000 pykern-20240405.195819/tests/pkcli1_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.345140 pykern-20240405.195819/tests/pkcli_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.401140 pykern-20240405.195819/tests/pkcli_data/arghparsing/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/arghparsing/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.401140 pykern-20240405.195819/tests/pkcli_data/arghparsing/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/arghparsing/pkcli/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.401140 pykern-20240405.195819/tests/pkcli_data/command_info.in/
+-rw-r-----   0 root         (0) root         (0)      140 2022-10-04 14:08:26.000000 pykern-20240405.195819/tests/pkcli_data/command_info.in/example_pkcli_module.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.402140 pykern-20240405.195819/tests/pkcli_data/command_info.out/
+-rw-r-----   0 root         (0) root         (0)       17 2022-10-04 14:08:26.000000 pykern-20240405.195819/tests/pkcli_data/command_info.out/example_stderr.out
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.402140 pykern-20240405.195819/tests/pkcli_data/package1/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/package1/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.403140 pykern-20240405.195819/tests/pkcli_data/package1/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/package1/pkcli/__init__.py
+-rw-r-----   0 root         (0) root         (0)      366 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/package1/pkcli/conf1.py
+-rw-r-----   0 root         (0) root         (0)      178 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/package1/pkcli/conf2.py
+-rw-r-----   0 root         (0) root         (0)      219 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/package1/pkcli/conf3.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.403140 pykern-20240405.195819/tests/pkcli_data/package2/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/package2/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.404140 pykern-20240405.195819/tests/pkcli_data/package2/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/package2/pkcli/__init__.py
+-rw-r-----   0 root         (0) root         (0)      310 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/package2/pkcli/argh_test.py
+-rw-r-----   0 root         (0) root         (0)      195 2023-12-07 23:37:10.000000 pykern-20240405.195819/tests/pkcli_data/package2/pkcli/some_mod.py
+-rw-r-----   0 root         (0) root         (0)     4879 2024-03-15 14:11:15.000000 pykern-20240405.195819/tests/pkcli_test.py
+-rw-r-----   0 root         (0) root         (0)     7300 2024-04-03 20:20:06.000000 pykern-20240405.195819/tests/pkcollections_test.py
+-rw-r-----   0 root         (0) root         (0)     2276 2023-09-13 14:10:24.000000 pykern-20240405.195819/tests/pkcompat_test.py
+-rw-r-----   0 root         (0) root         (0)     1862 2023-03-14 17:59:06.000000 pykern-20240405.195819/tests/pkconfig1_test.py
+-rw-r-----   0 root         (0) root         (0)     1175 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkconfig2_test.py
+-rw-r-----   0 root         (0) root         (0)      868 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkconfig3_test.py
+-rw-r-----   0 root         (0) root         (0)      754 2023-04-14 17:14:13.000000 pykern-20240405.195819/tests/pkconfig4_test.py
+-rw-r-----   0 root         (0) root         (0)     1588 2023-04-14 17:14:13.000000 pykern-20240405.195819/tests/pkconfig5_test.py
+-rw-r-----   0 root         (0) root         (0)      623 2023-04-14 17:14:13.000000 pykern-20240405.195819/tests/pkconfig6_test.py
+-rw-r-----   0 root         (0) root         (0)      617 2023-04-14 17:14:13.000000 pykern-20240405.195819/tests/pkconfig7_test.py
+-rw-r-----   0 root         (0) root         (0)      350 2023-04-23 14:08:30.000000 pykern-20240405.195819/tests/pkconfig8_test.py
+-rw-r-----   0 root         (0) root         (0)      421 2023-10-20 20:51:58.000000 pykern-20240405.195819/tests/pkconfig9_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.345140 pykern-20240405.195819/tests/pkconfig_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.405140 pykern-20240405.195819/tests/pkconfig_data/p1/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkconfig_data/p1/__init__.py
+-rw-r-----   0 root         (0) root         (0)      214 2023-10-20 20:51:58.000000 pykern-20240405.195819/tests/pkconfig_data/p1/append_error.py
+-rw-r-----   0 root         (0) root         (0)      469 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkconfig_data/p1/base_pkconfig.py
+-rw-r-----   0 root         (0) root         (0)     1984 2020-01-08 19:20:36.000000 pykern-20240405.195819/tests/pkconfig_data/p1/m1.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.405140 pykern-20240405.195819/tests/pkconfig_data/p1/s1/
+-rw-r-----   0 root         (0) root         (0)        2 2019-11-17 13:40:26.000000 pykern-20240405.195819/tests/pkconfig_data/p1/s1/__init__.py
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkconfig_data/p1/s1/m11.py
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkconfig_data/p1/s1/m12.py
+-rw-r-----   0 root         (0) root         (0)    10382 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkdebug1_test.py
+-rw-r-----   0 root         (0) root         (0)     1870 2023-08-16 14:09:51.000000 pykern-20240405.195819/tests/pkdebug2_test.py
+-rw-r-----   0 root         (0) root         (0)     1737 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkexample_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.346140 pykern-20240405.195819/tests/pkinspect_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.406140 pykern-20240405.195819/tests/pkinspect_data/p1/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkinspect_data/p1/__init__.py
+-rw-r-----   0 root         (0) root         (0)      326 2021-02-16 00:17:58.000000 pykern-20240405.195819/tests/pkinspect_data/p1/m1.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.406140 pykern-20240405.195819/tests/pkinspect_data/p1/p2/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkinspect_data/p1/p2/__init__.py
+-rw-r-----   0 root         (0) root         (0)       35 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkinspect_data/p1/p2/m2.py
+-rw-r-----   0 root         (0) root         (0)     3979 2024-01-19 15:11:21.000000 pykern-20240405.195819/tests/pkinspect_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.407140 pykern-20240405.195819/tests/pkio_data/
+-rw-r-----   0 root         (0) root         (0)   239616 2024-02-01 15:11:17.000000 pykern-20240405.195819/tests/pkio_data/binary.dat
+-rw-r-----   0 root         (0) root         (0)       18 2024-02-01 15:11:17.000000 pykern-20240405.195819/tests/pkio_data/text.dat
+-rw-r-----   0 root         (0) root         (0)     7132 2024-03-15 14:11:15.000000 pykern-20240405.195819/tests/pkio_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.408140 pykern-20240405.195819/tests/pkjinja_data/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkjinja_data/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.408140 pykern-20240405.195819/tests/pkjinja_data/package_data/
+-rw-r-----   0 root         (0) root         (0)       12 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkjinja_data/package_data/t1.jinja
+-rw-r-----   0 root         (0) root         (0)      211 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkjinja_data/t1.py
+-rw-r-----   0 root         (0) root         (0)      997 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkjinja_test.py
+-rw-r-----   0 root         (0) root         (0)     1617 2023-10-17 17:55:03.000000 pykern-20240405.195819/tests/pkjson_test.py
+-rw-r-----   0 root         (0) root         (0)     1415 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkplatform_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.408140 pykern-20240405.195819/tests/pkresource_data/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkresource_data/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.409140 pykern-20240405.195819/tests/pkresource_data/package_data/
+-rw-r-----   0 root         (0) root         (0)       14 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkresource_data/package_data/somefile
+-rw-r-----   0 root         (0) root         (0)      189 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkresource_data/t1.py
+-rw-r-----   0 root         (0) root         (0)     1309 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkresource_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.409140 pykern-20240405.195819/tests/pkrunpy_data/
+-rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkrunpy_data/f1.py
+-rw-r-----   0 root         (0) root         (0)      533 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pkrunpy_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.349140 pykern-20240405.195819/tests/pksetup_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.410140 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/
+-rw-r-----   0 root         (0) root         (0)      738 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/.gitignore
+-rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/LICENSE
+-rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/README.md
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.410140 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/docs/
+-rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/docs/index.rst
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.411140 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/examples/
+-rw-r-----   0 root         (0) root         (0)        4 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/examples/example1.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.411140 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/pksetupunit1/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/pksetupunit1/__init__.py
+-rw-r-----   0 root         (0) root         (0)      350 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/pksetupunit1/base_pkconfig.py
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/pksetupunit1/mod1.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.412140 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/pksetupunit1/package_data/
+-rw-r-----   0 root         (0) root         (0)       10 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/pksetupunit1/package_data/data1
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.412140 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/__init__.py
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/pksetupunit1/pkg1/mod2.py
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/requirements.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.412140 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/scripts/
+-rw-r-----   0 root         (0) root         (0)       25 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/scripts/script1
+-rw-r-----   0 root         (0) root         (0)      295 2019-05-06 20:05:16.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/setup.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.413140 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/tests/
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/tests/.gitignore
+-rw-r-----   0 root         (0) root         (0)       99 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/tests/mod1_test.py
+-rw-r-----   0 root         (0) root         (0)      181 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit1/tests/mod2_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.415140 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/
+-rw-r-----   0 root         (0) root         (0)      756 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/.gitignore
+-rw-r-----   0 root         (0) root         (0)      134 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/.travis.yml
+-rw-r-----   0 root         (0) root         (0)    22102 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/LICENSE
+-rw-r-----   0 root         (0) root         (0)      302 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/README.md
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.415140 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/docs/
+-rw-r-----   0 root         (0) root         (0)       48 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/docs/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.415140 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/docs/_static/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/docs/_static/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.416140 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/docs/_templates/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/docs/_templates/.gitignore
+-rw-r-----   0 root         (0) root         (0)      227 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/docs/index.rst
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.416140 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/pksetupunit2/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/pksetupunit2/__init__.py
+-rw-r-----   0 root         (0) root         (0)      350 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/pksetupunit2/base_pkconfig.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.417140 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/pksetupunit2/package_data/
+-rw-r-----   0 root         (0) root         (0)        0 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/pksetupunit2/package_data/.gitignore
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.417140 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/pksetupunit2/pkcli/
+-rw-r-----   0 root         (0) root         (0)        2 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/pksetupunit2/pkcli/__init__.py
+-rw-r-----   0 root         (0) root         (0)      466 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/pksetupunit2/pksetupunit2_console.py
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/requirements.txt
+-rw-r-----   0 root         (0) root         (0)     1051 2019-05-06 20:05:16.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/setup.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.417140 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/tests/
+-rw-r-----   0 root         (0) root         (0)        7 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/tests/.gitignore
+-rw-r-----   0 root         (0) root         (0)      321 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pksetup_data/pksetupunit2/tests/simple_test.py
+-rw-r-----   0 root         (0) root         (0)     5098 2023-04-04 14:10:19.000000 pykern-20240405.195819/tests/pksetup_test.py
+-rw-r-----   0 root         (0) root         (0)     3892 2022-06-24 14:08:21.000000 pykern-20240405.195819/tests/pksubprocess_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.351140 pykern-20240405.195819/tests/pkunit1_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.418140 pykern-20240405.195819/tests/pkunit1_data/bytes-1.in/
+-rw-r-----   0 root         (0) root         (0)       42 2023-04-14 14:08:36.000000 pykern-20240405.195819/tests/pkunit1_data/bytes-1.in/dot.gif
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.418140 pykern-20240405.195819/tests/pkunit1_data/bytes-1.out/
+-rw-r-----   0 root         (0) root         (0)       42 2023-04-14 14:08:36.000000 pykern-20240405.195819/tests/pkunit1_data/bytes-1.out/dot.gif
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.418140 pykern-20240405.195819/tests/pkunit1_data/conformance-1.in/
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/conformance-1.in/in.txt
+-rw-r-----   0 root         (0) root         (0)      102 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/conformance-1.in/res.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.419140 pykern-20240405.195819/tests/pkunit1_data/conformance-1.out/
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/conformance-1.out/in.txt
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/conformance-1.out/out.txt
+-rw-r-----   0 root         (0) root         (0)      102 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/conformance-1.out/res.json
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.420140 pykern-20240405.195819/tests/pkunit1_data/conformance-2.in/
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/conformance-2.in/in.txt
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/conformance-2.in/out.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.420140 pykern-20240405.195819/tests/pkunit1_data/conformance-2.out/
+-rw-r-----   0 root         (0) root         (0)       14 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/conformance-2.out/in.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.420140 pykern-20240405.195819/tests/pkunit1_data/curly_brackets.in/
+-rw-r-----   0 root         (0) root         (0)       13 2022-09-20 14:07:49.000000 pykern-20240405.195819/tests/pkunit1_data/curly_brackets.in/sample.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.420140 pykern-20240405.195819/tests/pkunit1_data/curly_brackets.out/
+-rw-r-----   0 root         (0) root         (0)        9 2022-09-20 14:07:49.000000 pykern-20240405.195819/tests/pkunit1_data/curly_brackets.out/sample.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.421140 pykern-20240405.195819/tests/pkunit1_data/deviance-1.in/
+-rw-r-----   0 root         (0) root         (0)        0 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/deviance-1.in/not-used.txt
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.421140 pykern-20240405.195819/tests/pkunit1_data/deviance-1.out/
+-rw-r-----   0 root         (0) root         (0)        9 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/pkunit1_data/deviance-1.out/out.txt
+-rw-r-----   0 root         (0) root         (0)     1449 2023-04-14 14:08:36.000000 pykern-20240405.195819/tests/pkunit1_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.427140 pykern-20240405.195819/tests/pkunit_data/
+-rw-r-----   0 root         (0) root         (0)       24 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/actual_abs_ok.ndiff
+-rw-r-----   0 root         (0) root         (0)       48 2022-12-08 15:07:12.000000 pykern-20240405.195819/tests/pkunit_data/actual_conformance_2.ndiff
+-rw-r-----   0 root         (0) root         (0)       53 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/actual_default_conformance.ndiff
+-rw-r-----   0 root         (0) root         (0)       53 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/actual_default_conformance_1.ndiff
+-rw-r-----   0 root         (0) root         (0)       15 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/actual_rel_ok.ndiff
+-rw-r-----   0 root         (0) root         (0)       21 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/actual_rel_ok_2.ndiff
+-rw-r-----   0 root         (0) root         (0)       15 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkunit_data/assert1.json
+-rw-r-----   0 root         (0) root         (0)       88 2022-08-23 22:15:42.000000 pykern-20240405.195819/tests/pkunit_data/different.bin
+-rw-r-----   0 root         (0) root         (0)      543 2022-05-16 23:38:16.000000 pykern-20240405.195819/tests/pkunit_data/example.csv
+-rw-r-----   0 root         (0) root         (0)     5425 2022-05-16 23:38:16.000000 pykern-20240405.195819/tests/pkunit_data/example.xlsx
+-rw-r-----   0 root         (0) root         (0)       24 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/expect_abs_ok.ndiff
+-rw-r-----   0 root         (0) root         (0)       48 2022-12-08 15:07:12.000000 pykern-20240405.195819/tests/pkunit_data/expect_conformance_2.ndiff
+-rw-r-----   0 root         (0) root         (0)       52 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/expect_default_conformance.ndiff
+-rw-r-----   0 root         (0) root         (0)       51 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/expect_default_conformance_1.ndiff
+-rw-r-----   0 root         (0) root         (0)       15 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/expect_rel_ok.ndiff
+-rw-r-----   0 root         (0) root         (0)       21 2023-03-17 14:08:25.000000 pykern-20240405.195819/tests/pkunit_data/expect_rel_ok_2.ndiff
+-rw-r-----   0 root         (0) root         (0)       20 2022-04-08 21:30:14.000000 pykern-20240405.195819/tests/pkunit_data/file_eq1.json
+-rw-r-----   0 root         (0) root         (0)        0 2022-04-08 21:30:14.000000 pykern-20240405.195819/tests/pkunit_data/file_eq2.txt
+-rw-r-----   0 root         (0) root         (0)       14 2022-04-08 21:30:14.000000 pykern-20240405.195819/tests/pkunit_data/file_eq3.txt
+-rw-r-----   0 root         (0) root         (0)       67 2022-08-25 16:28:29.000000 pykern-20240405.195819/tests/pkunit_data/ignore_lines.in
+-rw-r-----   0 root         (0) root         (0)       68 2022-08-25 16:28:29.000000 pykern-20240405.195819/tests/pkunit_data/ignore_lines.out
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.352140 pykern-20240405.195819/tests/pkunit_data/import1/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.427140 pykern-20240405.195819/tests/pkunit_data/import1/p1/
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkunit_data/import1/p1/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.352140 pykern-20240405.195819/tests/pkunit_data/import2/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.427140 pykern-20240405.195819/tests/pkunit_data/import2/p1/
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkunit_data/import2/p1/__init__.py
+-rw-r-----   0 root         (0) root         (0)      100 2022-08-23 22:15:42.000000 pykern-20240405.195819/tests/pkunit_data/in.bin
+-rw-r-----   0 root         (0) root         (0)      100 2022-08-23 22:15:42.000000 pykern-20240405.195819/tests/pkunit_data/out.bin
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkunit_data/t1.yml
+-rw-r-----   0 root         (0) root         (0)     8413 2023-10-30 22:15:18.000000 pykern-20240405.195819/tests/pkunit_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.427140 pykern-20240405.195819/tests/pkyaml_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.428140 pykern-20240405.195819/tests/pkyaml_data/1.in/
+-rw-r-----   0 root         (0) root         (0)       65 2022-07-12 14:07:33.000000 pykern-20240405.195819/tests/pkyaml_data/1.in/in.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.428140 pykern-20240405.195819/tests/pkyaml_data/1.out/
+-rw-r-----   0 root         (0) root         (0)       62 2022-07-12 14:07:33.000000 pykern-20240405.195819/tests/pkyaml_data/1.out/out.yml
+-rw-r-----   0 root         (0) root         (0)       27 2020-09-03 15:51:30.000000 pykern-20240405.195819/tests/pkyaml_data/dump1.yml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.428140 pykern-20240405.195819/tests/pkyaml_data/p1/
+-rw-r-----   0 root         (0) root         (0)       61 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkyaml_data/p1/__init__.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.428140 pykern-20240405.195819/tests/pkyaml_data/p1/package_data/
+-rw-r-----   0 root         (0) root         (0)       11 2018-02-06 22:51:04.000000 pykern-20240405.195819/tests/pkyaml_data/p1/package_data/conf2.yml
+-rw-r-----   0 root         (0) root         (0)     1275 2022-07-12 14:07:33.000000 pykern-20240405.195819/tests/pkyaml_test.py
+-rw-r-----   0 root         (0) root         (0)     1163 2024-02-01 15:11:17.000000 pykern-20240405.195819/tests/util_test.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.355140 pykern-20240405.195819/tests/xlsx_data/
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.429140 pykern-20240405.195819/tests/xlsx_data/1.in/
+-rw-r-----   0 root         (0) root         (0)      903 2022-08-02 14:08:07.000000 pykern-20240405.195819/tests/xlsx_data/1.in/case.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.429140 pykern-20240405.195819/tests/xlsx_data/1.out/
+-rw-r-----   0 root         (0) root         (0)       58 2022-08-02 14:08:07.000000 pykern-20240405.195819/tests/xlsx_data/1.out/case1.csv
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.429140 pykern-20240405.195819/tests/xlsx_data/1.out/xl/
+-rw-r-----   0 root         (0) root         (0)      281 2022-08-02 14:08:07.000000 pykern-20240405.195819/tests/xlsx_data/1.out/xl/sharedStrings.xml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.429140 pykern-20240405.195819/tests/xlsx_data/1.out/xl/worksheets/
+-rw-r-----   0 root         (0) root         (0)     1250 2022-08-02 14:08:07.000000 pykern-20240405.195819/tests/xlsx_data/1.out/xl/worksheets/sheet1.xml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.430140 pykern-20240405.195819/tests/xlsx_data/2.in/
+-rw-r-----   0 root         (0) root         (0)     1057 2022-08-10 14:07:21.000000 pykern-20240405.195819/tests/xlsx_data/2.in/case.py
+-rw-r-----   0 root         (0) root         (0)     6288 2022-08-02 14:08:07.000000 pykern-20240405.195819/tests/xlsx_data/2.in/case2.xlsx
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.430140 pykern-20240405.195819/tests/xlsx_data/2.out/
+-rw-r-----   0 root         (0) root         (0)       90 2022-08-10 14:07:21.000000 pykern-20240405.195819/tests/xlsx_data/2.out/case2#0.csv
+-rw-r-----   0 root         (0) root         (0)        9 2022-06-03 23:08:48.000000 pykern-20240405.195819/tests/xlsx_data/2.out/case2#1.csv
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.431140 pykern-20240405.195819/tests/xlsx_data/2.out/xl/
+-rw-r-----   0 root         (0) root         (0)      338 2022-08-10 14:07:21.000000 pykern-20240405.195819/tests/xlsx_data/2.out/xl/sharedStrings.xml
+-rw-r-----   0 root         (0) root         (0)     1656 2023-03-14 17:59:06.000000 pykern-20240405.195819/tests/xlsx_data/2.out/xl/styles.xml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.431140 pykern-20240405.195819/tests/xlsx_data/2.out/xl/worksheets/
+-rw-r-----   0 root         (0) root         (0)     1830 2023-01-16 15:07:03.000000 pykern-20240405.195819/tests/xlsx_data/2.out/xl/worksheets/sheet1.xml
+-rw-r-----   0 root         (0) root         (0)      795 2022-06-03 23:08:48.000000 pykern-20240405.195819/tests/xlsx_data/2.out/xl/worksheets/sheet2.xml
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.432140 pykern-20240405.195819/tests/xlsx_data/3.in/
+-rw-r-----   0 root         (0) root         (0)      484 2022-08-02 14:08:07.000000 pykern-20240405.195819/tests/xlsx_data/3.in/case.py
+drwxr-x---   0 root         (0) root         (0)        0 2024-04-09 14:46:27.432140 pykern-20240405.195819/tests/xlsx_data/3.out/
+-rw-r-----   0 root         (0) root         (0)       38 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/xlsx_data/3.out/pkexcept
+-rw-r-----   0 root         (0) root         (0)     1114 2022-08-06 14:07:18.000000 pykern-20240405.195819/tests/xlsx_test.py
```

### Comparing `pykern-20240402.175155/LICENSE` & `pykern-20240405.195819/LICENSE`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/PKG-INFO` & `pykern-20240405.195819/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykern
-Version: 20240402.175155
+Version: 20240405.195819
 Summary: Python application support library
 Author-email: RadiaSoft LLC <pip@pykern.org>
 Project-URL: Homepage, http://pykern.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pykern-20240402.175155/pykern/fconf.py` & `pykern-20240405.195819/pykern/fconf.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/mpi.py` & `pykern-20240405.195819/pykern/mpi.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/docs-conf.py.format` & `pykern-20240405.195819/pykern/package_data/docs-conf.py.format`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/projex/dot-gitignore.jinja` & `pykern-20240405.195819/pykern/package_data/projex/dot-gitignore.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/projex/setup.py.jinja` & `pykern-20240405.195819/pykern/package_data/projex/setup.py.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/projex-licenses/agpl-3.0.txt` & `pykern-20240405.195819/pykern/package_data/projex-licenses/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/projex-licenses/apache2.jinja` & `pykern-20240405.195819/pykern/package_data/projex-licenses/apache2.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/projex-licenses/gpl2.jinja` & `pykern-20240405.195819/pykern/package_data/projex-licenses/gpl2.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/projex-licenses/gpl3.jinja` & `pykern-20240405.195819/pykern/package_data/projex-licenses/gpl3.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/projex-licenses/lgpl2.jinja` & `pykern-20240405.195819/pykern/package_data/projex-licenses/lgpl2.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/projex-licenses/lgpl3.jinja` & `pykern-20240405.195819/pykern/package_data/projex-licenses/lgpl3.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/package_data/projex-licenses/mit.jinja` & `pykern-20240405.195819/pykern/package_data/projex-licenses/mit.jinja`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkarray.py` & `pykern-20240405.195819/pykern/pkarray.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkasyncio.py` & `pykern-20240405.195819/pykern/pkasyncio.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/__init__.py` & `pykern-20240405.195819/pykern/pkcli/__init__.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/ci.py` & `pykern-20240405.195819/pykern/pkcli/ci.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/fmt.py` & `pykern-20240405.195819/pykern/pkcli/fmt.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/github.py` & `pykern-20240405.195819/pykern/pkcli/github.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/github_orgmode.py` & `pykern-20240405.195819/pykern/pkcli/github_orgmode.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/pkexample.py` & `pykern-20240405.195819/pykern/pkcli/pkexample.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/projex.py` & `pykern-20240405.195819/pykern/pkcli/projex.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/rsmanifest.py` & `pykern-20240405.195819/pykern/pkcli/rsmanifest.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/sim.py` & `pykern-20240405.195819/pykern/pkcli/sim.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkcli/test.py` & `pykern-20240405.195819/pykern/pkcli/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 import os
 import pykern.pkcli
 import re
 import sys
 
 
 SUITE_D = "tests"
-_COROUTINE_NEVER_AWAITED = re.compile("RuntimeWarning: coroutine .+ was never awaited")
+_COROUTINE_NEVER_AWAITED = re.compile(
+    "(.+ coroutine \S+ was never awaited.*)", flags=re.MULTILINE
+)
 _TEST_SKIPPED = re.compile(r"^.+\s+SKIPPED\s+\(.+\)$", flags=re.MULTILINE)
-_FAILED_ON_WARNINGS = "\n*** FAILED due to warnings. See warnings summary ***\n"
 _TEST_PY = re.compile(r"_test\.py$")
 
 
 _cfg = pkconfig.init(
     ignore_warnings=(False, bool, "override pytest's output of all warnings"),
     max_failures=(5, int, "maximum number of test failures before exit"),
     restartable=(
@@ -207,16 +208,17 @@
             )
             v = _env(restartable)
             try:
                 pksubprocess.check_call_with_signals(c, output=output, env=v)
             except Exception as e:
                 return _except(e, output, restartable)
             o = pkio.read_text(output)
-            if _COROUTINE_NEVER_AWAITED.search(o):
-                pkio.write_text(output, o + _FAILED_ON_WARNINGS)
+            if m := re.findall(_COROUTINE_NEVER_AWAITED, o):
+                with pkio.py_path(output).open(mode="a") as f:
+                    f.write("".join(f"ERROR: {x}\n" for x in m))
                 return _fail(output)
             if _TEST_SKIPPED.search(o):
                 return "\n".join(["pass"] + _skipped(o))
             return "pass"
 
         def _skipped(ouput):
             return _TEST_SKIPPED.findall(ouput)
```

### Comparing `pykern-20240402.175155/pykern/pkcollections.py` & `pykern-20240405.195819/pykern/pkcollections.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,43 +207,74 @@
             if k not in d:
                 d[k] = PKDict()
             d = d[k]
         d[q[-1]] = value
         return self
 
     def pksetdefault(self, *args, **kwargs):
-        """Get value or set it, possibly after evaluating arg.
+        """Set values for keys if key not already in self
 
-        Must pass an even number of args or kwargs, but not both. Each pair
-        is interpreted as (key, value).
+        Accepts args or kwargs, but not both.
+        `args` must be an even number and are interpreted in (key, value) order.
+        `kwargs` are accepted as key=value.
 
-        If self does not have `key`, then it will be set. If `value` is a callable,
-        it will be called to get the value to set.
 
-        Values will be called if they are callable
+        If self does not have `key`, then it will be set to
+        `value`. If `key` is already in self, its value is not changed.
+         If `value` is a callable, it will be called, and
+        `key` will be set to the returned value.
 
         Args:
-            key (object): value to get or set
+            key (object): key that will be assigned `value` if not already set
             value (object): if callable, will be called, else verbatim
         Returns:
             object: self
         """
-        assert not (args and kwargs), "one of args or kwargs must be set, but not both"
+        if args and kwargs:
+            raise AssertionError("one of args or kwargs must be set, but not both")
         if args:
-            assert (
-                len(args) % 2 == 0
-            ), "args must be an even number (pairs of key, value)"
+            if len(args) % 2 != 0:
+                raise AssertionError(
+                    "args must be an even number (pairs of key, value)"
+                )
             i = zip(args[0::2], args[1::2])
         else:
             i = kwargs.items()
         for k, v in i:
-            if k not in self:
-                self[k] = v() if callable(v) else v
+            self.__pksetdefault_one(k, v)
         return self
 
+    def pksetdefault1(self, *args, **kwargs):
+        """Get value if exists else set
+
+        Accepts one key and one value, either as two positional args
+        (``key, value``); or one keyword arg (``key=value``).
+
+
+        If self does not have `key`, then it will be set to
+        `value`. If `value` is a callable, it will be called, and
+        `key` will be set to the returned value.
+
+        Args:
+            key (object): value to get or set
+            value (object): if callable, will be called, else verbatim
+        Returns:
+            object: ``self[key]``; either `value` if just set, or preexisting value
+
+        """
+        if args and kwargs:
+            raise AssertionError("one of args or kwargs must be set, but not both")
+        if args:
+            if len(args) == 2:
+                return self.__pksetdefault_one(*args)
+        elif len(kwargs) == 1:
+            for k, v in kwargs.items():
+                return self.__pksetdefault_one(k, v)
+        raise AssertionError("must pass exactly one key and value")
+
     def pkunchecked_nested_get(self, qualifiers, default=None):
         """Split key on dots or iterable and return nested get calls
 
         If `qualifiers` is a str, will split on dots. Otherwise, will be iterated.
 
         If the element does not exist or is not indexable, fails silently and returns `default`.
 
@@ -261,14 +292,19 @@
             return default
 
     def pkupdate(self, *args, **kwargs):
         """Call `dict.update` and return ``self``."""
         super(PKDict, self).update(*args, **kwargs)
         return self
 
+    def __pksetdefault_one(self, key, value):
+        if key not in self:
+            self[key] = value() if callable(value) else value
+        return self[key]
+
 
 class PKDictNameError(NameError):
     """Raised when a key matches a builtin attribute in `dict`."""
 
     pass
```

### Comparing `pykern-20240402.175155/pykern/pkcompat.py` & `pykern-20240405.195819/pykern/pkcompat.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkconfig.py` & `pykern-20240405.195819/pykern/pkconfig.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkconst.py` & `pykern-20240405.195819/pykern/pkconst.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkdebug.py` & `pykern-20240405.195819/pykern/pkdebug.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkexample.py` & `pykern-20240405.195819/pykern/pkexample.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkinspect.py` & `pykern-20240405.195819/pykern/pkinspect.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkio.py` & `pykern-20240405.195819/pykern/pkio.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkjinja.py` & `pykern-20240405.195819/pykern/pkjinja.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkjson.py` & `pykern-20240405.195819/pykern/pkjson.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkplatform.py` & `pykern-20240405.195819/pykern/pkplatform.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkresource.py` & `pykern-20240405.195819/pykern/pkresource.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkrunpy.py` & `pykern-20240405.195819/pykern/pkrunpy.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pksetup.py` & `pykern-20240405.195819/pykern/pksetup.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pksubprocess.py` & `pykern-20240405.195819/pykern/pksubprocess.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkunit.py` & `pykern-20240405.195819/pykern/pkunit.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/pkyaml.py` & `pykern-20240405.195819/pykern/pkyaml.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/util.py` & `pykern-20240405.195819/pykern/util.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern/xlsx.py` & `pykern-20240405.195819/pykern/xlsx.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pykern.egg-info/PKG-INFO` & `pykern-20240405.195819/pykern.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykern
-Version: 20240402.175155
+Version: 20240405.195819
 Summary: Python application support library
 Author-email: RadiaSoft LLC <pip@pykern.org>
 Project-URL: Homepage, http://pykern.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pykern-20240402.175155/pykern.egg-info/SOURCES.txt` & `pykern-20240405.195819/pykern.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/pyproject.toml` & `pykern-20240405.195819/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/conftest.py` & `pykern-20240405.195819/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/fconf_data/1.in/1.yml` & `pykern-20240405.195819/tests/fconf_data/1.in/1.yml`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/fconf_data/1.out/res.json` & `pykern-20240405.195819/tests/fconf_data/1.out/res.json`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/fconf_test.py` & `pykern-20240405.195819/tests/fconf_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/mpi_data/p1.py` & `pykern-20240405.195819/tests/mpi_data/p1.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/mpi_test.py` & `pykern-20240405.195819/tests/mpi_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkarray_test.py` & `pykern-20240405.195819/tests/pkarray_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkasyncio_test.py` & `pykern-20240405.195819/tests/pkasyncio_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/fmt_data/fmt_dir.out/y.py` & `pykern-20240405.195819/tests/pkcli/fmt_data/fmt_dir.out/y.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/fmt_test.py` & `pykern-20240405.195819/tests/pkcli/fmt_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/github_orgmode_data/assignee_issues-1.in/repo.json` & `pykern-20240405.195819/tests/pkcli/github_orgmode_data/assignee_issues-1.in/repo.json`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/github_orgmode_data/assignee_issues-1.out/assignee_issues.org` & `pykern-20240405.195819/tests/pkcli/github_orgmode_data/assignee_issues-1.out/assignee_issues.org`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/github_orgmode_data/from_issues-1.in/repo.json` & `pykern-20240405.195819/tests/pkcli/github_orgmode_data/from_issues-1.in/repo.json`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/github_orgmode_data/from_issues-1.out/radiasoft-test-pykern-github-orgmode.org` & `pykern-20240405.195819/tests/pkcli/github_orgmode_data/from_issues-1.out/radiasoft-test-pykern-github-orgmode.org`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/github_orgmode_data/to_issues-1.in/repo.json` & `pykern-20240405.195819/tests/pkcli/github_orgmode_data/to_issues-1.in/repo.json`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/github_orgmode_data/to_issues-1.in/to_issues-1.org` & `pykern-20240405.195819/tests/pkcli/github_orgmode_data/to_issues-1.in/to_issues-1.org`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/github_orgmode_data/to_issues-1.out/res.json` & `pykern-20240405.195819/tests/pkcli/github_orgmode_data/to_issues-1.out/res.json`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/github_orgmode_test.py` & `pykern-20240405.195819/tests/pkcli/github_orgmode_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/github_test.py` & `pykern-20240405.195819/tests/pkcli/github_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/projex_test.py` & `pykern-20240405.195819/tests/pkcli/projex_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/rsmanifest_test.py` & `pykern-20240405.195819/tests/pkcli/rsmanifest_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/sim_test.py` & `pykern-20240405.195819/tests/pkcli/sim_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/test1_test.py` & `pykern-20240405.195819/tests/pkcli/test1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli/test_test.py` & `pykern-20240405.195819/tests/pkcli/test_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli1_test.py` & `pykern-20240405.195819/tests/pkcli1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcli_test.py` & `pykern-20240405.195819/tests/pkcli_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkcollections_test.py` & `pykern-20240405.195819/tests/pkcollections_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,40 +78,14 @@
     del n["items"]
     pkok(list(n.items()) == [], "items() should be deletable")
     # specific string is generated so match exactly
     with pkexcept("'PKDict' object has no attribute 'missing_attribute'"):
         n.missing_attribute()
     with pkexcept(KeyError):
         n["missing key"]
-    pkeq(13, n.pksetdefault("d1", lambda: 13).d1)
-    pkeq(13, n.pksetdefault("d1", "already set").d1)
-    pkeq(n, n.pksetdefault("d1", "already set", "d2", 2, "d3", 3, "d4", 4))
-    pkeq(2, n.d2)
-    pkeq(3, n.d3)
-    pkeq(4, n.d4)
-    for i in "already set", 2, 3, 4:
-        with pkexcept(KeyError):
-            n[i]
-    with pkexcept(AssertionError):
-        n.pksetdefault("a", "b", "c")
-    n = PKDict()
-    pkeq(13, n.pksetdefault(d1=13).d1)
-    pkeq(13, n.pksetdefault(d1="already set").d1)
-    pkeq(n, n.pksetdefault(d1="already set", d2=2, d3=3, d4=4))
-    pkeq(2, n.d2)
-    pkeq(3, n.d3)
-    pkeq(4, n.d4)
-    for i in "already set", 2, 3, 4:
-        with pkexcept(KeyError):
-            n[i]
-    # ok to call empty kwargs
-    n.pksetdefault()
-    pkeq(4, n.pkdel("d4"))
-    pkeq(None, n.pkdel("d4"))
-    pkeq("x", n.pkdel("d4", "x"))
 
 
 def test_dict_copy():
     from pykern.pkcollections import PKDict
     import copy
     from pykern.pkunit import pkeq, pkne
 
@@ -120,14 +94,24 @@
     pkne(id(n), id(m))
     pkeq(id(n.b), id(n.b))
     m = copy.deepcopy(n)
     pkne(id(n), id(m))
     pkeq(id(n.b), id(n.b))
 
 
+def test_dict_pkdel():
+    from pykern.pkcollections import PKDict
+    from pykern.pkunit import pkok, pkeq, pkexcept
+
+    n = PKDict(d4=4)
+    pkeq(4, n.pkdel("d4"))
+    pkeq(None, n.pkdel("d4"))
+    pkeq("x", n.pkdel("d4", "x"))
+
+
 def test_dict_pknested_get():
     from pykern.pkcollections import PKDict
     from pykern.pkunit import pkeq, pkexcept
 
     n = PKDict(one=PKDict(two=1.2), simple=1)
     pkeq(1, n.pknested_get("simple"))
     pkeq(1, n.pknested_get(["simple"]))
@@ -151,14 +135,63 @@
     n = PKDict(one=PKDict())
     n.pknested_set("one.two", 2)
     n.pknested_set("other", 3)
     pkeq(2, n.pknested_get("one.two"))
     pkeq(3, n.pknested_get(["other"]))
 
 
+def test_dict_pksetdefault():
+    from pykern.pkcollections import PKDict
+    from pykern.pkunit import pkok, pkeq, pkexcept
+
+    n = PKDict()
+    pkeq(13, n.pksetdefault("d1", lambda: 13).d1)
+    pkeq(13, n.pksetdefault("d1", "already set").d1)
+    pkeq(n, n.pksetdefault("d1", "already set", "d2", 2, "d3", 3, "d4", 4))
+    pkeq(2, n.d2)
+    pkeq(3, n.d3)
+    pkeq(4, n.d4)
+    for i in "already set", 2, 3, 4:
+        with pkexcept(KeyError):
+            n[i]
+    with pkexcept(AssertionError):
+        n.pksetdefault("a", "b", "c")
+    n = PKDict()
+    pkeq(13, n.pksetdefault(d1=13).d1)
+    pkeq(13, n.pksetdefault(d1="already set").d1)
+    pkeq(n, n.pksetdefault(d1="already set", d2=2, d3=3, d4=4))
+    pkeq(2, n.d2)
+    pkeq(3, n.d3)
+    pkeq(4, n.d4)
+    for i in "already set", 2, 3, 4:
+        with pkexcept(KeyError):
+            n[i]
+    # ok to call empty kwargs
+    n.pksetdefault()
+
+
+def test_dict_pksetdefault1():
+    from pykern.pkcollections import PKDict
+    from pykern.pkunit import pkok, pkeq, pkexcept
+
+    n = PKDict()
+    pkeq(13, n.pksetdefault1("d1", lambda: 13))
+    pkeq(13, n.pksetdefault1("d1", "already set"))
+    pkeq("value", n.pksetdefault1(key1="value"))
+    pkeq("other", n.pksetdefault1(key2=lambda: "other"))
+    for a, k, r in (
+        (("d2", 2, "d3", 3), dict(), "too many args"),
+        ((), dict(d2=2, d3=3), "too many kwargs"),
+        ((), dict(), "no args"),
+        (("d3",), dict(), "one arg"),
+    ):
+        with pkexcept(AssertionError, r):
+            n.pksetdefault1(*a, **k)
+
+
 def test_dict_pkupdate():
     from pykern.pkcollections import PKDict
     from pykern.pkunit import pkeq
 
     d = PKDict()
     pkeq(id(d), id(d.pkupdate(a=1)))
     pkeq(1, d.a)
```

### Comparing `pykern-20240402.175155/tests/pkcompat_test.py` & `pykern-20240405.195819/tests/pkcompat_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkconfig1_test.py` & `pykern-20240405.195819/tests/pkconfig1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkconfig2_test.py` & `pykern-20240405.195819/tests/pkconfig2_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkconfig3_test.py` & `pykern-20240405.195819/tests/pkconfig3_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkconfig4_test.py` & `pykern-20240405.195819/tests/pkconfig4_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkconfig5_test.py` & `pykern-20240405.195819/tests/pkconfig5_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkconfig6_test.py` & `pykern-20240405.195819/tests/pkconfig6_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkconfig7_test.py` & `pykern-20240405.195819/tests/pkconfig7_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkconfig_data/p1/m1.py` & `pykern-20240405.195819/tests/pkconfig_data/p1/m1.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkdebug1_test.py` & `pykern-20240405.195819/tests/pkdebug1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkdebug2_test.py` & `pykern-20240405.195819/tests/pkdebug2_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkexample_test.py` & `pykern-20240405.195819/tests/pkexample_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkinspect_test.py` & `pykern-20240405.195819/tests/pkinspect_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkio_data/binary.dat` & `pykern-20240405.195819/tests/pkio_data/binary.dat`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkio_test.py` & `pykern-20240405.195819/tests/pkio_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkjinja_test.py` & `pykern-20240405.195819/tests/pkjinja_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkjson_test.py` & `pykern-20240405.195819/tests/pkjson_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkplatform_test.py` & `pykern-20240405.195819/tests/pkplatform_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkresource_test.py` & `pykern-20240405.195819/tests/pkresource_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkrunpy_test.py` & `pykern-20240405.195819/tests/pkrunpy_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pksetup_data/pksetupunit1/.gitignore` & `pykern-20240405.195819/tests/pksetup_data/pksetupunit1/.gitignore`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pksetup_data/pksetupunit2/.gitignore` & `pykern-20240405.195819/tests/pksetup_data/pksetupunit2/.gitignore`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pksetup_data/pksetupunit2/LICENSE` & `pykern-20240405.195819/tests/pksetup_data/pksetupunit2/LICENSE`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pksetup_data/pksetupunit2/setup.py` & `pykern-20240405.195819/tests/pksetup_data/pksetupunit2/setup.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pksetup_test.py` & `pykern-20240405.195819/tests/pksetup_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pksubprocess_test.py` & `pykern-20240405.195819/tests/pksubprocess_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkunit1_test.py` & `pykern-20240405.195819/tests/pkunit1_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkunit_data/example.csv` & `pykern-20240405.195819/tests/pkunit_data/example.csv`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkunit_data/example.xlsx` & `pykern-20240405.195819/tests/pkunit_data/example.xlsx`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkunit_test.py` & `pykern-20240405.195819/tests/pkunit_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/pkyaml_test.py` & `pykern-20240405.195819/tests/pkyaml_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/util_test.py` & `pykern-20240405.195819/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/xlsx_data/1.in/case.py` & `pykern-20240405.195819/tests/xlsx_data/1.in/case.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/xlsx_data/1.out/xl/worksheets/sheet1.xml` & `pykern-20240405.195819/tests/xlsx_data/1.out/xl/worksheets/sheet1.xml`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/xlsx_data/2.in/case.py` & `pykern-20240405.195819/tests/xlsx_data/2.in/case.py`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/xlsx_data/2.in/case2.xlsx` & `pykern-20240405.195819/tests/xlsx_data/2.in/case2.xlsx`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/xlsx_data/2.out/xl/styles.xml` & `pykern-20240405.195819/tests/xlsx_data/2.out/xl/styles.xml`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/xlsx_data/2.out/xl/worksheets/sheet1.xml` & `pykern-20240405.195819/tests/xlsx_data/2.out/xl/worksheets/sheet1.xml`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/xlsx_data/2.out/xl/worksheets/sheet2.xml` & `pykern-20240405.195819/tests/xlsx_data/2.out/xl/worksheets/sheet2.xml`

 * *Files identical despite different names*

### Comparing `pykern-20240402.175155/tests/xlsx_test.py` & `pykern-20240405.195819/tests/xlsx_test.py`

 * *Files identical despite different names*

