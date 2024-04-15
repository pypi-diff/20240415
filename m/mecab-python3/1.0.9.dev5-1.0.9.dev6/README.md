# Comparing `tmp/mecab-python3-1.0.9.dev5.tar.gz` & `tmp/mecab_python3-1.0.9.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecab-python3-1.0.9.dev5.tar", last modified: Sat Mar  9 04:28:19 2024, max compression
+gzip compressed data, was "mecab_python3-1.0.9.dev6.tar", last modified: Mon Apr 15 12:32:12 2024, max compression
```

## Comparing `mecab-python3-1.0.9.dev5.tar` & `mecab_python3-1.0.9.dev6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.967495 mecab-python3-1.0.9.dev5/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.959495 mecab-python3-1.0.9.dev5/.github/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1672 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/macos-build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.963495 mecab-python3-1.0.9.dev5/.github/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.955495 mecab-python3-1.0.9.dev5/.github/workflows/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.963495 mecab-python3-1.0.9.dev5/.github/workflows/actions/build-manylinux/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/actions/build-manylinux/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.963495 mecab-python3-1.0.9.dev5/.github/workflows/actions/build-wheels/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/actions/build-wheels/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.959495 mecab-python3-1.0.9.dev5/.github/workflows/actions_aarch64/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.963495 mecab-python3-1.0.9.dev5/.github/workflows/actions_aarch64/build_manylinux2014/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/actions_aarch64/build_manylinux2014/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.963495 mecab-python3-1.0.9.dev5/.github/workflows/actions_aarch64/build_wheels/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/actions_aarch64/build_wheels/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      617 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/build_mecab.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      872 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/manylinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/osx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/test_manylinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/BSD
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    17981 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/GPL
--rw-r--r--   0 runner    (1001) docker     (127)    26421 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/LGPL
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-03-09 04:28:19.967495 mecab-python3-1.0.9.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.963495 mecab-python3-1.0.9.dev5/debian/
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/debian/control
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/debian/docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.963495 mecab-python3-1.0.9.dev5/debian/source/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/debian/source/format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.963495 mecab-python3-1.0.9.dev5/debian/upstream/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/debian/upstream/metadata
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/debian/watch
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 04:28:19.967495 mecab-python3-1.0.9.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.959495 mecab-python3-1.0.9.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.963495 mecab-python3-1.0.9.dev5/src/MeCab/
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/src/MeCab/MeCab.i
--rw-r--r--   0 runner    (1001) docker     (127)   345029 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/src/MeCab/MeCab_wrap.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/src/MeCab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/src/MeCab/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.967495 mecab-python3-1.0.9.dev5/src/mecab_python3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-03-09 04:28:19.000000 mecab-python3-1.0.9.dev5/src/mecab_python3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-09 04:28:19.000000 mecab-python3-1.0.9.dev5/src/mecab_python3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 04:28:19.000000 mecab-python3-1.0.9.dev5/src/mecab_python3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-09 04:28:19.000000 mecab-python3-1.0.9.dev5/src/mecab_python3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-09 04:28:19.000000 mecab-python3-1.0.9.dev5/src/mecab_python3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-09 04:28:19.000000 mecab-python3-1.0.9.dev5/src/mecab_python3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 04:28:19.967495 mecab-python3-1.0.9.dev5/test/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/test/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-09 04:27:04.000000 mecab-python3-1.0.9.dev5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.360265 mecab_python3-1.0.9.dev6/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.352265 mecab_python3-1.0.9.dev6/.github/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1672 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/macos-build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.352265 mecab_python3-1.0.9.dev6/.github/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.348266 mecab_python3-1.0.9.dev6/.github/workflows/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.352265 mecab_python3-1.0.9.dev6/.github/workflows/actions/build-manylinux/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/actions/build-manylinux/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.352265 mecab_python3-1.0.9.dev6/.github/workflows/actions/build-wheels/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/actions/build-wheels/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.348266 mecab_python3-1.0.9.dev6/.github/workflows/actions_aarch64/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.352265 mecab_python3-1.0.9.dev6/.github/workflows/actions_aarch64/build_manylinux2014/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/actions_aarch64/build_manylinux2014/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.352265 mecab_python3-1.0.9.dev6/.github/workflows/actions_aarch64/build_wheels/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/actions_aarch64/build_wheels/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      617 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/build_mecab.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      872 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/manylinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/osx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/test_manylinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/BSD
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    17981 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/GPL
+-rw-r--r--   0 runner    (1001) docker     (127)    26421 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/LGPL
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-15 12:32:12.356265 mecab_python3-1.0.9.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.356265 mecab_python3-1.0.9.dev6/debian/
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/debian/control
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/debian/docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.356265 mecab_python3-1.0.9.dev6/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/debian/source/format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.356265 mecab_python3-1.0.9.dev6/debian/upstream/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/debian/upstream/metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/debian/watch
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 12:32:12.360265 mecab_python3-1.0.9.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.348266 mecab_python3-1.0.9.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.356265 mecab_python3-1.0.9.dev6/src/MeCab/
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/src/MeCab/MeCab.i
+-rw-r--r--   0 runner    (1001) docker     (127)   345029 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/src/MeCab/MeCab_wrap.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/src/MeCab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/src/MeCab/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.356265 mecab_python3-1.0.9.dev6/src/mecab_python3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-15 12:32:12.000000 mecab_python3-1.0.9.dev6/src/mecab_python3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 12:32:12.000000 mecab_python3-1.0.9.dev6/src/mecab_python3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:32:12.000000 mecab_python3-1.0.9.dev6/src/mecab_python3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 12:32:12.000000 mecab_python3-1.0.9.dev6/src/mecab_python3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 12:32:12.000000 mecab_python3-1.0.9.dev6/src/mecab_python3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 12:32:12.000000 mecab_python3-1.0.9.dev6/src/mecab_python3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:32:12.356265 mecab_python3-1.0.9.dev6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/test/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 12:30:29.000000 mecab_python3-1.0.9.dev6/tox.ini
```

### Comparing `mecab-python3-1.0.9.dev5/.github/macos-build.sh` & `mecab_python3-1.0.9.dev6/.github/macos-build.sh`

 * *Files 1% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 cd ../..
 mv src/.libs.combined src/.libs
 
 sudo make install
 cd ../..
 
 python -m pip install --upgrade setuptools wheel pip setuptools-scm
-python -m pip install cibuildwheel==2.14.1
+python -m pip install cibuildwheel==2.17.0
 
 # don't bother with pypy wheels
 export CIBW_SKIP="pp*"
 python -m cibuildwheel --platform macos --archs x86_64,arm64,universal2 --output-dir dist
```

### Comparing `mecab-python3-1.0.9.dev5/.github/workflows/build_mecab.sh` & `mecab_python3-1.0.9.dev6/.github/workflows/build_mecab.sh`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/.github/workflows/entrypoint.sh` & `mecab_python3-1.0.9.dev6/.github/workflows/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/.github/workflows/manylinux.yml` & `mecab_python3-1.0.9.dev6/.github/workflows/manylinux.yml`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 on: [push]
 
 jobs:
   build_sdist:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: |
           3.8
           3.9
           3.10
           3.11
           3.12
@@ -47,17 +47,17 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         arch: [x86_64, aarch64]
     env:
       arch: ${{ matrix.arch }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: |
           3.8
           3.9
           3.10
           3.11
           3.12
```

### Comparing `mecab-python3-1.0.9.dev5/.github/workflows/osx.yml` & `mecab_python3-1.0.9.dev6/.github/workflows/osx.yml`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 on: [push]
 
 jobs:
   build_osx:
     runs-on: macos-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: |
           3.8
           3.9
           3.10
           3.11
           3.12
```

### Comparing `mecab-python3-1.0.9.dev5/.github/workflows/test_manylinux.yml` & `mecab_python3-1.0.9.dev6/.github/workflows/test_manylinux.yml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   push:
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ 3.7, 3.8, 3.9, "3.10", "3.11" ]
+        python-version: [ 3.8, 3.9, "3.10", "3.11", "3.12 ]
     env:
       PYTHON: python${{ matrix.python-version }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - run: docker build -t mecab-py .
     - name: setup and test
       run: docker run -v $(pwd):/workdir -w /workdir mecab-py sh -c "export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/lib/ && $PYTHON -m pip install pytest wheel unidic-lite && $PYTHON -m pip install -e . && $PYTHON -m pytest"
```

### Comparing `mecab-python3-1.0.9.dev5/.github/workflows/windows.yml` & `mecab_python3-1.0.9.dev6/.github/workflows/windows.yml`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
           - python-version: "3.11"
             py-short: 311
             py-short2: 311
           - python-version: "3.12"
             py-short: 312
             py-short2: 312
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Cache mecab
       id: cache-mecab
       uses: actions/cache@v3
       with:
         path: C:/mecab
```

### Comparing `mecab-python3-1.0.9.dev5/BSD` & `mecab_python3-1.0.9.dev6/BSD`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/GPL` & `mecab_python3-1.0.9.dev6/GPL`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/LGPL` & `mecab_python3-1.0.9.dev6/LGPL`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/PKG-INFO` & `mecab_python3-1.0.9.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecab-python3
-Version: 1.0.9.dev5
+Version: 1.0.9.dev6
 Summary: Python wrapper for the MeCab morphological analyzer for Japanese
 Home-page: https://github.com/SamuraiT/mecab-python3
 Maintainer: Paul O'Leary McCann
 Maintainer-email: polm@dampfkraft.com
 License: BSD
 Classifier: Development Status :: 6 - Mature
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mecab-python3-1.0.9.dev5/README.md` & `mecab_python3-1.0.9.dev6/README.md`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/debian/changelog` & `mecab_python3-1.0.9.dev6/debian/changelog`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/debian/control` & `mecab_python3-1.0.9.dev6/debian/control`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/debian/copyright` & `mecab_python3-1.0.9.dev6/debian/copyright`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/setup.py` & `mecab_python3-1.0.9.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/src/MeCab/MeCab.i` & `mecab_python3-1.0.9.dev6/src/MeCab/MeCab.i`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/src/MeCab/MeCab_wrap.cpp` & `mecab_python3-1.0.9.dev6/src/MeCab/MeCab_wrap.cpp`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/src/MeCab/__init__.py` & `mecab_python3-1.0.9.dev6/src/MeCab/__init__.py`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/src/MeCab/cli.py` & `mecab_python3-1.0.9.dev6/src/MeCab/cli.py`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/src/mecab_python3.egg-info/PKG-INFO` & `mecab_python3-1.0.9.dev6/src/mecab_python3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecab-python3
-Version: 1.0.9.dev5
+Version: 1.0.9.dev6
 Summary: Python wrapper for the MeCab morphological analyzer for Japanese
 Home-page: https://github.com/SamuraiT/mecab-python3
 Maintainer: Paul O'Leary McCann
 Maintainer-email: polm@dampfkraft.com
 License: BSD
 Classifier: Development Status :: 6 - Mature
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mecab-python3-1.0.9.dev5/src/mecab_python3.egg-info/SOURCES.txt` & `mecab_python3-1.0.9.dev6/src/mecab_python3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/test/test_basic.py` & `mecab_python3-1.0.9.dev6/test/test_basic.py`

 * *Files identical despite different names*

### Comparing `mecab-python3-1.0.9.dev5/tox.ini` & `mecab_python3-1.0.9.dev6/tox.ini`

 * *Files identical despite different names*

