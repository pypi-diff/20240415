# Comparing `tmp/tad_mctc-0.1.2.tar.gz` & `tmp/tad_mctc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_mctc-0.1.2.tar", last modified: Fri Apr 12 11:37:11 2024, max compression
+gzip compressed data, was "tad_mctc-0.1.3.tar", last modified: Mon Apr 15 10:38:59 2024, max compression
```

## Comparing `tad_mctc-0.1.2.tar` & `tad_mctc-0.1.3.tar`

### file list

```diff
@@ -1,108 +1,113 @@
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/
--rw-rw-r--   0 friede    (1000) friede    (1000)    11358 2024-03-28 13:09:56.000000 tad_mctc-0.1.2/LICENSE
--rw-rw-r--   0 friede    (1000) friede    (1000)     9497 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)     8658 2024-03-28 13:09:56.000000 tad_mctc-0.1.2/README.md
--rw-rw-r--   0 friede    (1000) friede    (1000)     1648 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/pyproject.toml
--rw-rw-r--   0 friede    (1000) friede    (1000)     1250 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/setup.cfg
--rw-rw-r--   0 friede    (1000) friede    (1000)      714 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/setup.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.162719 tad_mctc-0.1.2/src/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.162719 tad_mctc-0.1.2/src/tad_mctc/
--rw-rw-r--   0 friede    (1000) friede    (1000)     4302 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1590 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/_version.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.162719 tad_mctc-0.1.2/src/tad_mctc/autograd/
--rw-rw-r--   0 friede    (1000) friede    (1000)      921 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1455 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/batched.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4489 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/compat.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4188 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/gradcheck.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2691 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/hessian.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2058 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/internals.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2578 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/nonfunctorch.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/batch/
--rw-rw-r--   0 friede    (1000) friede    (1000)      817 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/batch/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1911 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/batch/agnostic.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3305 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/batch/mask.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5722 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/batch/pack.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5898 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/batch/unpack.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/convert/
--rw-rw-r--   0 friede    (1000) friede    (1000)      903 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/convert/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3963 2024-04-05 08:07:49.000000 tad_mctc-0.1.2/src/tad_mctc/convert/numpy.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1692 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/convert/pse.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3928 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/convert/pytorch.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2733 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/convert/tensor.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/data/
--rw-rw-r--   0 friede    (1000) friede    (1000)     1041 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1890 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/en.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3320 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/getters.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2421 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/mass.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    69463 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/molecules.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4440 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/pse.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4312 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/radii.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3607 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/zeff.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/exceptions/
--rw-rw-r--   0 friede    (1000) friede    (1000)      803 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/exceptions/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1143 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/exceptions/io.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      994 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/exceptions/molecule.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      944 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/exceptions/pytorch.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/io/
--rw-rw-r--   0 friede    (1000) friede    (1000)      750 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/__init__.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/io/checks/
--rw-rw-r--   0 friede    (1000) friede    (1000)      782 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/checks/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     6220 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/checks/molecule.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2251 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/checks/shape.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/io/read/
--rw-rw-r--   0 friede    (1000) friede    (1000)     1144 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2463 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/dotfiles.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     6505 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/frompath.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2834 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/orca.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3169 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/qcschema.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5446 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/reader.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2370 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/tblite.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5433 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/turbomole.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5472 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/xyz.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/io/write/
--rw-rw-r--   0 friede    (1000) friede    (1000)      770 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/write/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2240 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/write/turbomole.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2704 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/write/writer.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2446 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/write/xyz.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/math/
--rw-rw-r--   0 friede    (1000) friede    (1000)      746 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/math/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2251 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/math/einsum.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/molecule/
--rw-rw-r--   0 friede    (1000) friede    (1000)      793 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/molecule/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    13209 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/molecule/bond.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4014 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/molecule/geometry.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4546 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/molecule/property.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/src/tad_mctc/ncoord/
--rw-rw-r--   0 friede    (1000) friede    (1000)     2871 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5967 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/count.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5623 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/d3.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3731 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/d4.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1593 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/defaults.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4019 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/eeq.py
--rw-rw-r--   0 friede    (1000) friede    (1000)        0 2024-01-09 09:57:14.000000 tad_mctc-0.1.2/src/tad_mctc/py.typed
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/src/tad_mctc/storch/
--rw-rw-r--   0 friede    (1000) friede    (1000)     1113 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/storch/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4538 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/storch/distance.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4289 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/storch/elemental.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    30570 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/storch/linalg.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1343 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/storch/utils.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/src/tad_mctc/typing/
--rw-rw-r--   0 friede    (1000) friede    (1000)      920 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/typing/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1137 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/typing/builtin.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4777 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/typing/compat.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     8427 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/typing/pytorch.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/src/tad_mctc/units/
--rw-rw-r--   0 friede    (1000) friede    (1000)      841 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2025 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/codata.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3517 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/energy.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1463 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/length.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1682 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/mass.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      873 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/math.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2490 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/spectroscopy.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1047 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/time.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.162719 tad_mctc-0.1.2/src/tad_mctc.egg-info/
--rw-r--r--   0 friede    (1000) friede    (1000)     9497 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)     2617 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/SOURCES.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)        1 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/dependency_links.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)      238 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/requires.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)        9 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-15 10:38:59.477671 tad_mctc-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.457671 tad_mctc-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.461671 tad_mctc-0.1.3/src/tad_mctc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.461671 tad_mctc-0.1.3/src/tad_mctc/autograd/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/batched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/gradcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/nonfunctorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.461671 tad_mctc-0.1.3/src/tad_mctc/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/agnostic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.461671 tad_mctc-0.1.3/src/tad_mctc/batch/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/unpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/pse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69463 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/pse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/radii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/zeff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/exceptions/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/exceptions/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/exceptions/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/io/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/checks/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/checks/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/io/read/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/dotfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/frompath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/orca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/tblite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/turbomole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/io/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/write/turbomole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/write/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/write/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/math/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/math/einsum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/molecule/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/molecule/bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/molecule/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/molecule/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/ncoord/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/d3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/d4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/eeq.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/src/tad_mctc/storch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/elemental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30570 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/src/tad_mctc/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/typing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/typing/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/typing/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/src/tad_mctc/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/codata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/src/tad_mctc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/top_level.txt
```

### Comparing `tad_mctc-0.1.2/LICENSE` & `tad_mctc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/PKG-INFO` & `tad_mctc-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: tad_mctc
-Version: 0.1.2
-Summary: Torch Autodiff Utility
-Author: "Marvin Friede"
-License: Apache-2.0
-Classifier: Framework :: Pytest
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: tox
-License-File: LICENSE
-
 # Torch Autodiff Utility
 
 <table>
   <tr>
     <td>Compatibility:</td>
     <td>
       <img src="https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg" alt="Python Versions"/>
```

#### html2text {}

```diff
@@ -1,19 +1,8 @@
-Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.2 Summary: Torch Autodiff
-Utility Author: "Marvin Friede" License: Apache-2.0 Classifier: Framework ::
-Pytest Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Topic :: Scientific/Engineering
-Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: tox License-File: LICENSE #
-Torch Autodiff Utility
+# Torch Autodiff Utility
 Compatibility: [Python Versions][PyTorch Versions]
 Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
 Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
                _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
```

### Comparing `tad_mctc-0.1.2/pyproject.toml` & `tad_mctc-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/setup.py` & `tad_mctc-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/_version.py` & `tad_mctc-0.1.3/src/tad_mctc/_version.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,9 +46,9 @@
             f"versioning scheme of MAJOR.MINOR.PATCH ({s})."
         )
 
     version_numbers = [int(part) for part in s[:3]]
     return tuple(version_numbers)
 
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __tversion__ = version_tuple(torch.__version__)
```

### Comparing `tad_mctc-0.1.2/src/tad_mctc/autograd/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/autograd/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/autograd/batched.py` & `tad_mctc-0.1.3/src/tad_mctc/autograd/batched.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/autograd/compat.py` & `tad_mctc-0.1.3/src/tad_mctc/autograd/compat.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/autograd/gradcheck.py` & `tad_mctc-0.1.3/src/tad_mctc/autograd/gradcheck.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/autograd/hessian.py` & `tad_mctc-0.1.3/src/tad_mctc/autograd/hessian.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/autograd/internals.py` & `tad_mctc-0.1.3/src/tad_mctc/autograd/internals.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/autograd/nonfunctorch.py` & `tad_mctc-0.1.3/src/tad_mctc/autograd/nonfunctorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/batch/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/batch/agnostic.py` & `tad_mctc-0.1.3/src/tad_mctc/batch/agnostic.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/batch/mask.py` & `tad_mctc-0.1.3/src/tad_mctc/batch/mask/pairs.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,93 +20,75 @@
 
 Functions for creating masks that discern between padding and actual values.
 """
 from __future__ import annotations
 
 import torch
 
-from ..typing import Tensor
+from ...typing import Tensor
+from .atoms import real_atoms
 
-__all__ = ["real_atoms", "real_pairs", "real_triples"]
+__all__ = ["real_pairs"]
 
 
-@torch.jit.script
-def real_atoms(numbers: Tensor) -> Tensor:
+# scripting or tracing does not improve performance
+def real_pairs(numbers: Tensor, mask_diagonal: bool = True) -> Tensor:
     """
-    Create a mask for atoms, discerning padding and actual atoms.
-    Padding value is zero.
+    Create a mask for pairs of atoms from atomic numbers, discerning padding
+    and actual atoms. Padding value is zero.
 
     Parameters
     ----------
     numbers : Tensor
         Atomic numbers for all atoms.
+    mask_diagonal : bool, optional
+        Flag for also masking the diagonal, i.e., all pairs with the same
+        indices. Defaults to `True`, i.e., writing False to the diagonal.
 
     Returns
     -------
     Tensor
-        Mask for atoms that discerns padding and real atoms.
+        Mask for atom pairs that discerns padding and real atoms.
     """
-    return numbers != 0
+    if mask_diagonal is True:
+        return real_pairs_maskdiag(numbers)
+    return real_pairs_no_maskdiag(numbers)
 
 
-@torch.jit.script
-def real_pairs(numbers: Tensor, mask_diagonal: bool = True) -> Tensor:
+def real_pairs_maskdiag(numbers: Tensor) -> Tensor:
     """
     Create a mask for pairs of atoms from atomic numbers, discerning padding
     and actual atoms. Padding value is zero.
 
     Parameters
     ----------
     numbers : Tensor
         Atomic numbers for all atoms.
-    mask_diagonal : bool, optional
-        Flag for also masking the diagonal, i.e., all pairs with the same
-        indices. Defaults to `True`, i.e., writing False to the diagonal.
 
     Returns
     -------
     Tensor
         Mask for atom pairs that discerns padding and real atoms.
     """
     real = real_atoms(numbers)
     mask = real.unsqueeze(-2) * real.unsqueeze(-1)
-
-    if mask_diagonal is True:
-        mask *= ~torch.diag_embed(torch.ones_like(real))
+    mask *= ~torch.diag_embed(torch.ones_like(real))
     return mask
 
 
-@torch.jit.script
-def real_triples(
-    numbers: Tensor, mask_diagonal: bool = True, mask_self: bool = True
-) -> Tensor:
+def real_pairs_no_maskdiag(numbers: Tensor) -> Tensor:
     """
-    Create a mask for triples from atomic numbers. Padding value is zero.
+    Create a mask for pairs of atoms from atomic numbers, discerning padding
+    and actual atoms. Padding value is zero.
 
     Parameters
     ----------
     numbers : Tensor
         Atomic numbers for all atoms.
-    mask_diagonal : bool, optional
-        Flag for also masking the diagonal, i.e., all pairs with the same
-        indices. Defaults to `True`, i.e., writing False to the diagonal.
-    mask_self : bool, optional
-        Flag for also masking all triples where at least two indices are
-        identical. Defaults to `True`, i.e., writing `False`.
 
     Returns
     -------
     Tensor
-        Mask for triples.
+        Mask for atom pairs that discerns padding and real atoms.
     """
-    real = real_pairs(numbers, mask_diagonal=False)
-    mask = real.unsqueeze(-3) * real.unsqueeze(-2) * real.unsqueeze(-1)
-
-    if mask_diagonal is True:
-        mask *= ~torch.diag_embed(torch.ones_like(real))
-
-    if mask_self is True:
-        mask *= ~torch.diag_embed(torch.ones_like(real), offset=0, dim1=-3, dim2=-2)
-        mask *= ~torch.diag_embed(torch.ones_like(real), offset=0, dim1=-3, dim2=-1)
-        mask *= ~torch.diag_embed(torch.ones_like(real), offset=0, dim1=-2, dim2=-1)
-
-    return mask
+    real = real_atoms(numbers)
+    return real.unsqueeze(-2) * real.unsqueeze(-1)
```

### Comparing `tad_mctc-0.1.2/src/tad_mctc/batch/pack.py` & `tad_mctc-0.1.3/src/tad_mctc/batch/pack.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/batch/unpack.py` & `tad_mctc-0.1.3/src/tad_mctc/batch/unpack.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/convert/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/convert/numpy.py` & `tad_mctc-0.1.3/src/tad_mctc/convert/numpy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/convert/pse.py` & `tad_mctc-0.1.3/src/tad_mctc/convert/pse.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/convert/pytorch.py` & `tad_mctc-0.1.3/src/tad_mctc/convert/pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         Unknown device name is given.
     """
     if "cpu" in s:
         return torch.device("cpu")
 
     if "cuda" in s:
         if not torch.cuda.is_available():
-            raise KeyError(f"No CUDA devices available.")
+            raise KeyError("No CUDA devices available.")
         return torch.device("cuda", index=torch.cuda.current_device())
 
     raise KeyError(f"Unknown device '{s}' given.")
 
 
 def any_to_tensor(
     x: Any,
@@ -118,20 +118,20 @@
     """
     if isinstance(x, Tensor):
         return x.to(device=device, dtype=dtype)
 
     if isinstance(x, list):
         if all(isinstance(item, (float, int, bool)) for item in x):
             return torch.tensor(x, device=device, dtype=dtype)
-        else:
-            raise ValueError("List must contain only float, int, or bool types.")
+
+        raise ValueError("List must contain only float, int, or bool types.")
 
     if isinstance(x, (float, int, bool)):
         return torch.tensor(x, device=device, dtype=dtype)
 
     if isinstance(x, str):
         try:
             return torch.tensor(float(x), device=device, dtype=dtype)
-        except ValueError:
-            raise ValueError(f"Cannot convert string '{x}' to float")
+        except ValueError as e:
+            raise ValueError(f"Cannot convert string '{x}' to float") from e
 
     raise TypeError(f"Tensor-incompatible type '{type(x)}' of variable {x}.")
```

### Comparing `tad_mctc-0.1.2/src/tad_mctc/convert/tensor.py` & `tad_mctc-0.1.3/src/tad_mctc/convert/tensor.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/data/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/data/en.py` & `tad_mctc-0.1.3/src/tad_mctc/data/en.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/data/getters.py` & `tad_mctc-0.1.3/src/tad_mctc/data/getters.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/data/mass.py` & `tad_mctc-0.1.3/src/tad_mctc/data/mass.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/data/molecules.py` & `tad_mctc-0.1.3/src/tad_mctc/data/molecules.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/data/pse.py` & `tad_mctc-0.1.3/src/tad_mctc/data/pse.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/data/radii.py` & `tad_mctc-0.1.3/src/tad_mctc/data/radii.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/data/zeff.py` & `tad_mctc-0.1.3/src/tad_mctc/data/zeff.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/exceptions/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/exceptions/io.py` & `tad_mctc-0.1.3/src/tad_mctc/exceptions/io.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/exceptions/molecule.py` & `tad_mctc-0.1.3/src/tad_mctc/exceptions/molecule.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/exceptions/pytorch.py` & `tad_mctc-0.1.3/src/tad_mctc/exceptions/pytorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/checks/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/io/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/checks/molecule.py` & `tad_mctc-0.1.3/src/tad_mctc/io/checks/molecule.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/checks/shape.py` & `tad_mctc-0.1.3/src/tad_mctc/io/checks/shape.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/read/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/io/read/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/read/dotfiles.py` & `tad_mctc-0.1.3/src/tad_mctc/io/read/dotfiles.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/read/frompath.py` & `tad_mctc-0.1.3/src/tad_mctc/io/read/frompath.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/read/orca.py` & `tad_mctc-0.1.3/src/tad_mctc/io/read/orca.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/read/qcschema.py` & `tad_mctc-0.1.3/src/tad_mctc/io/read/qcschema.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/read/reader.py` & `tad_mctc-0.1.3/src/tad_mctc/io/read/reader.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/read/tblite.py` & `tad_mctc-0.1.3/src/tad_mctc/io/read/tblite.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/read/turbomole.py` & `tad_mctc-0.1.3/src/tad_mctc/io/read/turbomole.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/read/xyz.py` & `tad_mctc-0.1.3/src/tad_mctc/io/read/xyz.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/write/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/io/write/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/write/turbomole.py` & `tad_mctc-0.1.3/src/tad_mctc/io/write/turbomole.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/write/writer.py` & `tad_mctc-0.1.3/src/tad_mctc/io/write/writer.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/io/write/xyz.py` & `tad_mctc-0.1.3/src/tad_mctc/io/write/xyz.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/math/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/math/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/math/einsum.py` & `tad_mctc-0.1.3/src/tad_mctc/math/einsum.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         return _torch_einsum(*args, optimize=optimize)
 
 except ImportError:  # pragma: no cover
 
     @_wraps(torch.einsum)
     def einsum(*args: Any, optimize: Any = None) -> Tensor:
         if optimize is not None:
+            # pylint: disable=import-outside-toplevel
             from warnings import warn
 
             warn("Optimization not supported without 'opt_einsum' package.")
 
         return torch.einsum(*args)
 
     einsum_optimal = einsum_greedy = einsum
```

### Comparing `tad_mctc-0.1.2/src/tad_mctc/molecule/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/molecule/bond.py` & `tad_mctc-0.1.3/src/tad_mctc/molecule/bond.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/molecule/geometry.py` & `tad_mctc-0.1.3/src/tad_mctc/molecule/geometry.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/molecule/property.py` & `tad_mctc-0.1.3/src/tad_mctc/molecule/property.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/ncoord/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/ncoord/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/ncoord/count.py` & `tad_mctc-0.1.3/src/tad_mctc/ncoord/count.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/ncoord/d3.py` & `tad_mctc-0.1.3/src/tad_mctc/ncoord/d3.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/ncoord/d4.py` & `tad_mctc-0.1.3/src/tad_mctc/ncoord/d4.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/ncoord/defaults.py` & `tad_mctc-0.1.3/src/tad_mctc/ncoord/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/ncoord/eeq.py` & `tad_mctc-0.1.3/src/tad_mctc/ncoord/eeq.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/storch/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/storch/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/storch/distance.py` & `tad_mctc-0.1.3/src/tad_mctc/storch/distance.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 Functions for calculating the cartesian distance of two vectors.
 """
 from __future__ import annotations
 
 import torch
 
+from ..math import einsum
 from ..typing import Tensor
 from .elemental import sqrt as ssqrt
 
 __all__ = ["cdist"]
 
 
 def euclidean_dist_quadratic_expansion(x: Tensor, y: Tensor) -> Tensor:
@@ -62,21 +63,21 @@
     eps = torch.tensor(
         torch.finfo(x.dtype).eps,
         device=x.device,
         dtype=x.dtype,
     )
 
     # using einsum is slightly faster than `torch.pow(x, 2).sum(-1)`
-    xnorm = torch.einsum("...ij,...ij->...i", x, x)
-    ynorm = torch.einsum("...ij,...ij->...i", y, y)
+    xnorm = einsum("...ij,...ij->...i", x, x)
+    ynorm = einsum("...ij,...ij->...i", y, y)
 
     n = xnorm.unsqueeze(-1) + ynorm.unsqueeze(-2)
 
-    # x @ y.mT
-    prod = torch.einsum("...ik,...jk->...ij", x, y)
+    # "...ik,...jk->...ij"
+    prod = x @ y.mT
 
     # important: remove negative values that give NaN in backward
     return ssqrt(n - 2.0 * prod, eps=eps)
 
 
 def cdist_direct_expansion(x: Tensor, y: Tensor, p: int = 2) -> Tensor:
     """
```

### Comparing `tad_mctc-0.1.2/src/tad_mctc/storch/elemental.py` & `tad_mctc-0.1.3/src/tad_mctc/storch/elemental.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/storch/linalg.py` & `tad_mctc-0.1.3/src/tad_mctc/storch/linalg.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/storch/utils.py` & `tad_mctc-0.1.3/src/tad_mctc/storch/utils.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/typing/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/typing/builtin.py` & `tad_mctc-0.1.3/src/tad_mctc/typing/builtin.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,30 +19,28 @@
 ================
 
 This module contains all used built-in type annotations.
 """
 from typing import (
     IO,
     Any,
-    Callable,
     Iterable,
     Iterator,
     Literal,
     NoReturn,
     Protocol,
     TypedDict,
     TypeVar,
     overload,
     runtime_checkable,
 )
 
 __all__ = [
     "IO",
     "Any",
-    "Callable",
     "Iterable",
     "Iterator",
     "Literal",
     "NoReturn",
     "Protocol",
     "TypedDict",
     "TypeVar",
```

### Comparing `tad_mctc-0.1.2/src/tad_mctc/typing/compat.py` & `tad_mctc-0.1.3/src/tad_mctc/typing/compat.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/typing/pytorch.py` & `tad_mctc-0.1.3/src/tad_mctc/typing/pytorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/units/__init__.py` & `tad_mctc-0.1.3/src/tad_mctc/units/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/units/codata.py` & `tad_mctc-0.1.3/src/tad_mctc/units/codata.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/units/energy.py` & `tad_mctc-0.1.3/src/tad_mctc/units/energy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/units/length.py` & `tad_mctc-0.1.3/src/tad_mctc/units/length.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/units/mass.py` & `tad_mctc-0.1.3/src/tad_mctc/units/mass.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/units/math.py` & `tad_mctc-0.1.3/src/tad_mctc/units/math.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/units/spectroscopy.py` & `tad_mctc-0.1.3/src/tad_mctc/units/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc/units/time.py` & `tad_mctc-0.1.3/src/tad_mctc/units/time.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.2/src/tad_mctc.egg-info/PKG-INFO` & `tad_mctc-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,57 @@
 Metadata-Version: 2.1
-Name: tad-mctc
-Version: 0.1.2
+Name: tad_mctc
+Version: 0.1.3
 Summary: Torch Autodiff Utility
+Home-page: https://github.com/tad-mctc/tad-mctc
 Author: "Marvin Friede"
 License: Apache-2.0
+Project-URL: Documentation, https://tad-mctc.readthedocs.io
+Project-URL: Source, https://github.com/tad-mctc/tad-mctc
+Project-URL: Tracker, https://github.com/tad-mctc/tad-mctc/issues
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: opt-einsum
+Requires-Dist: scipy
+Requires-Dist: torch>=1.11
+Requires-Dist: typing-extensions
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: covdefaults; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-random-order; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 Provides-Extra: tox
-License-File: LICENSE
+Requires-Dist: covdefaults; extra == "tox"
+Requires-Dist: pytest; extra == "tox"
+Requires-Dist: pytest-cov; extra == "tox"
+Requires-Dist: pytest-random-order; extra == "tox"
+Requires-Dist: pytest-xdist; extra == "tox"
+Requires-Dist: scipy; extra == "tox"
 
 # Torch Autodiff Utility
 
 <table>
   <tr>
     <td>Compatibility:</td>
     <td>
```

#### html2text {}

```diff
@@ -1,19 +1,33 @@
-Metadata-Version: 2.1 Name: tad-mctc Version: 0.1.2 Summary: Torch Autodiff
-Utility Author: "Marvin Friede" License: Apache-2.0 Classifier: Framework ::
-Pytest Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Topic :: Scientific/Engineering
-Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: tox License-File: LICENSE #
-Torch Autodiff Utility
+Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.3 Summary: Torch Autodiff
+Utility Home-page: https://github.com/tad-mctc/tad-mctc Author: "Marvin Friede"
+License: Apache-2.0 Project-URL: Documentation, https://tad-mctc.readthedocs.io
+Project-URL: Source, https://github.com/tad-mctc/tad-mctc Project-URL: Tracker,
+https://github.com/tad-mctc/tad-mctc/issues Classifier: Framework :: Pytest
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering Classifier: Typing :: Typed
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: numpy Requires-Dist: opt-einsum Requires-Dist: scipy
+Requires-Dist: torch>=1.11 Requires-Dist: typing-extensions Provides-Extra: dev
+Requires-Dist: black; extra == "dev" Requires-Dist: covdefaults; extra == "dev"
+Requires-Dist: mypy; extra == "dev" Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pylint; extra == "dev" Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: pytest-random-order;
+extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" Requires-Dist:
+scipy; extra == "dev" Requires-Dist: tox; extra == "dev" Provides-Extra: tox
+Requires-Dist: covdefaults; extra == "tox" Requires-Dist: pytest; extra ==
+"tox" Requires-Dist: pytest-cov; extra == "tox" Requires-Dist: pytest-random-
+order; extra == "tox" Requires-Dist: pytest-xdist; extra == "tox" Requires-
+Dist: scipy; extra == "tox" # Torch Autodiff Utility
 Compatibility: [Python Versions][PyTorch Versions]
 Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
 Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
                _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
```

### Comparing `tad_mctc-0.1.2/src/tad_mctc.egg-info/SOURCES.txt` & `tad_mctc-0.1.3/src/tad_mctc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,21 @@
 src/tad_mctc/autograd/compat.py
 src/tad_mctc/autograd/gradcheck.py
 src/tad_mctc/autograd/hessian.py
 src/tad_mctc/autograd/internals.py
 src/tad_mctc/autograd/nonfunctorch.py
 src/tad_mctc/batch/__init__.py
 src/tad_mctc/batch/agnostic.py
-src/tad_mctc/batch/mask.py
 src/tad_mctc/batch/pack.py
 src/tad_mctc/batch/unpack.py
+src/tad_mctc/batch/mask/__init__.py
+src/tad_mctc/batch/mask/atoms.py
+src/tad_mctc/batch/mask/jit.py
+src/tad_mctc/batch/mask/pairs.py
+src/tad_mctc/batch/mask/triples.py
 src/tad_mctc/convert/__init__.py
 src/tad_mctc/convert/numpy.py
 src/tad_mctc/convert/pse.py
 src/tad_mctc/convert/pytorch.py
 src/tad_mctc/convert/tensor.py
 src/tad_mctc/data/__init__.py
 src/tad_mctc/data/en.py
```

