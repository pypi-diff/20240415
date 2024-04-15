# Comparing `tmp/imio.webspellchecker-1.0b6.tar.gz` & `tmp/imio.webspellchecker-1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.webspellchecker-1.0b6.tar", last modified: Thu Apr  4 12:49:42 2024, max compression
+gzip compressed data, was "imio.webspellchecker-1.0b7.tar", last modified: Mon Apr 15 13:49:56 2024, max compression
```

## Comparing `imio.webspellchecker-1.0b6.tar` & `imio.webspellchecker-1.0b7.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/
--rw-rw-r--   0 adu       (1000) adu       (1000)      826 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/CHANGES.md
--rw-rw-r--   0 adu       (1000) adu       (1000)       49 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/CONTRIBUTORS.md
--rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/LICENSE.GPL
--rw-rw-r--   0 adu       (1000) adu       (1000)      655 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/LICENSE.md
--rw-rw-r--   0 adu       (1000) adu       (1000)       60 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/MANIFEST.in
--rw-rw-r--   0 adu       (1000) adu       (1000)     4351 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)     2231 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/README.md
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/docs/
--rw-rw-r--   0 adu       (1000) adu       (1000)     7909 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/docs/conf.py
--rw-rw-r--   0 adu       (1000) adu       (1000)       83 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/docs/index.rst
--rw-rw-r--   0 adu       (1000) adu       (1000)      321 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/setup.cfg
--rw-rw-r--   0 adu       (1000) adu       (1000)     2181 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/setup.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/src/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/
--rw-rw-r--   0 adu       (1000) adu       (1000)       80 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/
--rw-rw-r--   0 adu       (1000) adu       (1000)      137 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1420 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)     5144 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/controlpanel.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/
--rw-rw-r--   0 adu       (1000) adu       (1000)      608 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/controlpanel-icon.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      626 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/p4-controlpanel-icon.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     2587 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/plone_spinner.svg
--rw-rw-r--   0 adu       (1000) adu       (1000)     5890 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/wsctheme.css
--rw-rw-r--   0 adu       (1000) adu       (1000)     1841 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/viewlet.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     2474 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/webspellchecker.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1028 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)      417 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/interfaces.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/
--rw-rw-r--   0 adu       (1000) adu       (1000)      611 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/README.rst
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/en/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/en/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)     3725 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/en/LC_MESSAGES/imio.webspellchecker.po
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/fr/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)     5838 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/fr/LC_MESSAGES/imio.webspellchecker.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     3900 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/imio.webspellchecker.pot
--rw-rw-r--   0 adu       (1000) adu       (1000)     1756 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/update.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)      497 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/update.sh
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.282364 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/
--rw-rw-r--   0 adu       (1000) adu       (1000)      186 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/browserlayer.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)       88 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      573 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/registry.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/
--rw-rw-r--   0 adu       (1000) adu       (1000)      682 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/controlpanel.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      339 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/cssregistry.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      172 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      240 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/registry.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/
--rw-rw-r--   0 adu       (1000) adu       (1000)      679 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/controlpanel.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      172 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      544 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/registry.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/testing/
--rw-rw-r--   0 adu       (1000) adu       (1000)      189 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/testing/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      726 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/testing/registry.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/uninstall/
--rw-rw-r--   0 adu       (1000) adu       (1000)      112 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)     1430 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)      661 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/setuphandlers.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1913 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/testing.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      445 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/testing.zcml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.290365 imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/
--rw-rw-r--   0 adu       (1000) adu       (1000)      745 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     2789 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/test_setup.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     6504 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/test_view.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      212 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/upgrades.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      389 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/upgrades.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)      738 2024-04-04 12:49:41.000000 imio.webspellchecker-1.0b6/src/imio/webspellchecker/vocabularies.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-04 12:49:42.286364 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/
--rw-rw-r--   0 adu       (1000) adu       (1000)     4351 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)     2626 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/SOURCES.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/dependency_links.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)      145 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/entry_points.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        5 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/namespace_packages.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/not-zip-safe
--rw-rw-r--   0 adu       (1000) adu       (1000)      131 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/requires.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        5 2024-04-04 12:49:42.000000 imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/top_level.txt
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.263631 imio.webspellchecker-1.0b7/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1108 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/CHANGES.md
+-rw-rw-r--   0 adu       (1000) adu       (1000)       49 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/CONTRIBUTORS.md
+-rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/LICENSE.GPL
+-rw-rw-r--   0 adu       (1000) adu       (1000)      655 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/LICENSE.md
+-rw-rw-r--   0 adu       (1000) adu       (1000)       60 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/MANIFEST.in
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4633 2024-04-15 13:49:56.263631 imio.webspellchecker-1.0b7/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2231 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/README.md
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.255631 imio.webspellchecker-1.0b7/docs/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7910 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/docs/conf.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)       83 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/docs/index.rst
+-rw-rw-r--   0 adu       (1000) adu       (1000)      363 2024-04-15 13:49:56.263631 imio.webspellchecker-1.0b7/setup.cfg
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2181 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/setup.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.255631 imio.webspellchecker-1.0b7/src/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.255631 imio.webspellchecker-1.0b7/src/imio/
+-rw-rw-r--   0 adu       (1000) adu       (1000)       80 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.259631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      137 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.259631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1420 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5162 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/controlpanel.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.259631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/static/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      608 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/static/controlpanel-icon.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      626 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/static/p4-controlpanel-icon.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2587 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/static/plone_spinner.svg
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5890 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/static/wsctheme.css
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1841 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/viewlet.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2474 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/webspellchecker.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3500 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/config.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1028 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      417 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/interfaces.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.259631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      611 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/README.rst
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.255631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/en/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.259631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3725 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/en/LC_MESSAGES/imio.webspellchecker.po
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.255631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/fr/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.259631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5838 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/fr/LC_MESSAGES/imio.webspellchecker.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3900 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/imio.webspellchecker.pot
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1756 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/update.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      497 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/update.sh
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.255631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.263631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/base/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      186 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/base/browserlayer.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)       88 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/base/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      573 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/base/registry.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.263631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone4/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      682 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone4/controlpanel.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      339 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone4/cssregistry.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      172 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone4/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      240 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone4/registry.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.263631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone6/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      679 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone6/controlpanel.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      172 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone6/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      544 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone6/registry.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.263631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/testing/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      189 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/testing/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      726 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/testing/registry.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.263631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/uninstall/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      112 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1430 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      661 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/setuphandlers.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1913 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/testing.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      445 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/testing.zcml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.263631 imio.webspellchecker-1.0b7/src/imio/webspellchecker/tests/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      745 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/tests/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2789 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/tests/test_setup.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5525 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/tests/test_view.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      212 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/upgrades.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      389 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/upgrades.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      738 2024-04-15 13:49:55.000000 imio.webspellchecker-1.0b7/src/imio/webspellchecker/vocabularies.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2024-04-15 13:49:56.259631 imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4633 2024-04-15 13:49:56.000000 imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2661 2024-04-15 13:49:56.000000 imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/SOURCES.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2024-04-15 13:49:56.000000 imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/dependency_links.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)      145 2024-04-15 13:49:56.000000 imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/entry_points.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        5 2024-04-15 13:49:56.000000 imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/namespace_packages.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2024-04-15 13:49:56.000000 imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/not-zip-safe
+-rw-rw-r--   0 adu       (1000) adu       (1000)      131 2024-04-15 13:49:56.000000 imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/requires.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        5 2024-04-15 13:49:56.000000 imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/top_level.txt
```

### Comparing `imio.webspellchecker-1.0b6/LICENSE.GPL` & `imio.webspellchecker-1.0b7/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/LICENSE.md` & `imio.webspellchecker-1.0b7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/PKG-INFO` & `imio.webspellchecker-1.0b7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.webspellchecker
-Version: 1.0b6
+Version: 1.0b7
 Summary: Integration of Webspellchecker's WProofReader with Plone, providing real-time spellchecking for various WYSIWYG editors.
 Home-page: https://github.com/collective/imio.webspellchecker
 Author: iMio
 Author-email: antoine.duchene@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.webspellchecker
 Project-URL: Source, https://github.com/imio/imio.webspellchecker
@@ -89,15 +89,25 @@
 
 - Antoine Duchêne, (iMio, scrl)
 
 
 # Changelog
 
 
-1.0b6 (2024-04-04)
+1.0b7 (2024-04-15)
+
+- Added helpers to `get` and `set` config registry values.
+  [gbastien]
+- Use `plone.app.vocabularies.PortalTypes` instead
+ `plone.app.vocabularies.UserFriendlyTypes` for `allowed_portal_types` and
+ `disallowed_portal_types` config parameters.
+  [gbastien]
+
+
+## 1.0b6 (2024-04-04)
 
 - Use proper type on the script tags.
   [aduchene]
 
 ## 1.0b5 (2024-03-29)
 
 - Use unicode for default values.
```

### Comparing `imio.webspellchecker-1.0b6/README.md` & `imio.webspellchecker-1.0b7/README.md`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/docs/conf.py` & `imio.webspellchecker-1.0b7/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys
 import os
+import sys
+
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration ------------------------------------------------
```

### Comparing `imio.webspellchecker-1.0b6/setup.py` & `imio.webspellchecker-1.0b7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.md").read(),
     ]
 )
 
 
 setup(
     name="imio.webspellchecker",
-    version="1.0b6",
+    version="1.0b7",
     description="Integration of Webspellchecker's WProofReader with Plone, "
     "providing real-time spellchecking for various WYSIWYG editors.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/configure.zcml` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/controlpanel.py` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/controlpanel.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,52 +71,54 @@
 
     allowed_portal_types = schema.List(
         title=_("Allowed portal types"),
         description=_(
             "Define the portal types where the webspellchecker will be active."
             "If this is left blank, the webspellchecker will be available on all portal types."
         ),
-        value_type=schema.Choice(vocabulary="plone.app.vocabularies.UserFriendlyTypes"),
+        value_type=schema.Choice(vocabulary="plone.app.vocabularies.PortalTypes"),
         required=False,
         missing_value=[],
         default=[],
     )
 
     disallowed_portal_types = schema.List(
         title=_("Disallowed portal types"),
         description=_(
             "Define the portal types where the webspellchecker should not be active."
             "If this is left blank, this setting will be ignored."
         ),
-        value_type=schema.Choice(vocabulary="plone.app.vocabularies.UserFriendlyTypes"),
+        value_type=schema.Choice(vocabulary="plone.app.vocabularies.PortalTypes"),
         required=False,
         missing_value=[],
         default=[],
     )
 
     # see https://webspellchecker.com/docs/api/wscbundle/AutoSearchMechanism.html
     enable_autosearch_in = schema.TextLine(
         title=_("Enable autosearch in"),
         description=_(
-            "The parameter allows enabling the autoSearch mechanism only for elements with provided class, id, data attribute name or HTML elements type. "
+            "The parameter allows enabling the autoSearch mechanism only for elements "
+            "with provided class, id, data attribute name or HTML elements type. "
             "Possible values are: <br>"
             " - '.class' - enable autoSearch for elements with a specified class. <br>"
             " - '#id' - enable autoSearch for elements with a specified id. <br>"
             " - '[data-attribute]' - enable autoSearch for elements with a specified data attribute name. <br>"
             " - 'textarea' - enable autoSearch for HTML elements (e.g. textarea, input)."
         ),
         required=False,
         default=u"",
         constraint=is_valid_json,
     )
 
     disable_autosearch_in = schema.TextLine(
         title=_("Disable autosearch in"),
         description=_(
-            "The parameter allows disabling the autoSearch mechanism by class, id, data attribute name and HTML elements."
+            "The parameter allows disabling the autoSearch mechanism by class, id, "
+            "data attribute name and HTML elements."
             "If enable_autosearch_in option is specified than this option will be ignored. Possible values are: <br>"
             " - '.class' - disable autoSearch for elements with a specified class. <br>"
             " - '#id' - disable autoSearch for elements with a specified id. <br>"
             " - '[data-attribute]' - disable autoSearch for elements with a specified data attribute name. <br>"
             " - 'textarea' - disable autoSearch for HTML elements (e.g. textarea, input)."
         ),
         required=False,
```

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/controlpanel-icon.png` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/static/controlpanel-icon.png`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/p4-controlpanel-icon.png` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/static/p4-controlpanel-icon.png`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/plone_spinner.svg` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/static/plone_spinner.svg`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/static/wsctheme.css` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/static/wsctheme.css`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/viewlet.py` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/viewlet.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/browser/webspellchecker.py` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/browser/webspellchecker.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/configure.zcml` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/README.rst` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/README.rst`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/en/LC_MESSAGES/imio.webspellchecker.po` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/en/LC_MESSAGES/imio.webspellchecker.po`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/fr/LC_MESSAGES/imio.webspellchecker.po` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/fr/LC_MESSAGES/imio.webspellchecker.po`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/imio.webspellchecker.pot` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/imio.webspellchecker.pot`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/locales/update.py` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/locales/update.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/base/registry.xml` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/base/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone4/controlpanel.xml` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone4/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/controlpanel.xml` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone6/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/plone6/registry.xml` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/plone6/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles/testing/registry.xml` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles/testing/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/profiles.zcml` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/setuphandlers.py` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/testing.py` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/testing.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/__init__.py` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/tests/test_setup.py` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio/webspellchecker/vocabularies.py` & `imio.webspellchecker-1.0b7/src/imio/webspellchecker/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/PKG-INFO` & `imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.webspellchecker
-Version: 1.0b6
+Version: 1.0b7
 Summary: Integration of Webspellchecker's WProofReader with Plone, providing real-time spellchecking for various WYSIWYG editors.
 Home-page: https://github.com/collective/imio.webspellchecker
 Author: iMio
 Author-email: antoine.duchene@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.webspellchecker
 Project-URL: Source, https://github.com/imio/imio.webspellchecker
@@ -89,15 +89,25 @@
 
 - Antoine Duchêne, (iMio, scrl)
 
 
 # Changelog
 
 
-1.0b6 (2024-04-04)
+1.0b7 (2024-04-15)
+
+- Added helpers to `get` and `set` config registry values.
+  [gbastien]
+- Use `plone.app.vocabularies.PortalTypes` instead
+ `plone.app.vocabularies.UserFriendlyTypes` for `allowed_portal_types` and
+ `disallowed_portal_types` config parameters.
+  [gbastien]
+
+
+## 1.0b6 (2024-04-04)
 
 - Use proper type on the script tags.
   [aduchene]
 
 ## 1.0b5 (2024-03-29)
 
 - Use unicode for default values.
```

### Comparing `imio.webspellchecker-1.0b6/src/imio.webspellchecker.egg-info/SOURCES.txt` & `imio.webspellchecker-1.0b7/src/imio.webspellchecker.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/imio.webspellchecker.egg-info/dependency_links.txt
 src/imio.webspellchecker.egg-info/entry_points.txt
 src/imio.webspellchecker.egg-info/namespace_packages.txt
 src/imio.webspellchecker.egg-info/not-zip-safe
 src/imio.webspellchecker.egg-info/requires.txt
 src/imio.webspellchecker.egg-info/top_level.txt
 src/imio/webspellchecker/__init__.py
+src/imio/webspellchecker/config.py
 src/imio/webspellchecker/configure.zcml
 src/imio/webspellchecker/interfaces.py
 src/imio/webspellchecker/profiles.zcml
 src/imio/webspellchecker/setuphandlers.py
 src/imio/webspellchecker/testing.py
 src/imio/webspellchecker/testing.zcml
 src/imio/webspellchecker/upgrades.py
```

