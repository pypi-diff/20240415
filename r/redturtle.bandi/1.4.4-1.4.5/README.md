# Comparing `tmp/redturtle.bandi-1.4.4.tar.gz` & `tmp/redturtle.bandi-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.bandi-1.4.4.tar", last modified: Tue Feb 20 15:35:50 2024, max compression
+gzip compressed data, was "redturtle.bandi-1.4.5.tar", last modified: Mon Apr 15 09:48:30 2024, max compression
```

## Comparing `redturtle.bandi-1.4.4.tar` & `redturtle.bandi-1.4.5.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.035942 redturtle.bandi-1.4.4/
--rw-r--r--   0 daniele    (501) staff       (20)      317 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/MANIFEST.in
--rw-r--r--   0 daniele    (501) staff       (20)     6544 2024-02-20 15:35:50.035804 redturtle.bandi-1.4.4/PKG-INFO
--rw-r--r--   0 daniele    (501) staff       (20)     3254 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/README.rst
--rw-r--r--   0 daniele    (501) staff       (20)       96 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/buildout.cfg
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.999469 redturtle.bandi-1.4.4/docs/
--rw-r--r--   0 daniele    (501) staff       (20)     2047 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/docs/HISTORY.txt
--rw-r--r--   0 daniele    (501) staff       (20)     1463 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/docs/INSTALL.txt
--rw-r--r--   0 daniele    (501) staff       (20)    17987 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/docs/LICENSE.GPL
--rw-r--r--   0 daniele    (501) staff       (20)      726 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/docs/LICENSE.txt
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.999806 redturtle.bandi-1.4.4/redturtle/
--rw-r--r--   0 daniele    (501) staff       (20)      244 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/__init__.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.006052 redturtle.bandi-1.4.4/redturtle/bandi/
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.006794 redturtle.bandi-1.4.4/redturtle/bandi/Extensions/
--rw-r--r--   0 daniele    (501) staff       (20)      402 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/Extensions/Install.py
--rw-r--r--   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/Extensions/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)    10004 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/README.txt
--rw-r--r--   0 daniele    (501) staff       (20)      197 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/__init__.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.011400 redturtle.bandi-1.4.4/redturtle/bandi/browser/
--rw-r--r--   0 daniele    (501) staff       (20)        2 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)     8892 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/bando-right.pt
--rw-r--r--   0 daniele    (501) staff       (20)     8211 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/bando.pt
--rw-r--r--   0 daniele    (501) staff       (20)     9506 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/bando.py
--rw-r--r--   0 daniele    (501) staff       (20)     5702 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/collection.pt
--rw-r--r--   0 daniele    (501) staff       (20)     1893 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/collection.py
--rw-r--r--   0 daniele    (501) staff       (20)     4708 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/configure.zcml
--rw-r--r--   0 daniele    (501) staff       (20)      585 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/context.py
--rw-r--r--   0 daniele    (501) staff       (20)      389 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/controlpanel.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.012863 redturtle.bandi-1.4.4/redturtle/bandi/browser/css/
--rw-r--r--   0 daniele    (501) staff       (20)       48 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/css/Makefile
--rw-r--r--   0 daniele    (501) staff       (20)     4833 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/css/bandi.css
--rw-r--r--   0 daniele    (501) staff       (20)     1032 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/css/bandi.css.map
--rw-r--r--   0 daniele    (501) staff       (20)     5365 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/css/bandi.scss
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.014732 redturtle.bandi-1.4.4/redturtle/bandi/browser/images/
--rw-r--r--   0 daniele    (501) staff       (20)      252 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/images/bando.png
--rw-r--r--   0 daniele    (501) staff       (20)     1192 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/images/bando_closed.png
--rw-r--r--   0 daniele    (501) staff       (20)      811 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/images/bando_icon.svg
--rw-r--r--   0 daniele    (501) staff       (20)      351 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/images/bando_inprogress.png
--rw-r--r--   0 daniele    (501) staff       (20)     1199 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/images/bando_open.png
--rw-r--r--   0 daniele    (501) staff       (20)      621 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/images/folder_bando_deep.gif
--rw-r--r--   0 daniele    (501) staff       (20)     3973 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/migrator.py
--rw-r--r--   0 daniele    (501) staff       (20)     6811 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/search.pt
--rw-r--r--   0 daniele    (501) staff       (20)     5969 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/search.py
--rw-r--r--   0 daniele    (501) staff       (20)     9603 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/search_form.pt
--rw-r--r--   0 daniele    (501) staff       (20)      322 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/browser/searchbandi.js
--rw-r--r--   0 daniele    (501) staff       (20)     2762 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/configure.zcml
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.016050 redturtle.bandi-1.4.4/redturtle/bandi/content/
--rw-r--r--   0 daniele    (501) staff       (20)        2 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/content/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)      220 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/content/bando.py
--rw-r--r--   0 daniele    (501) staff       (20)      280 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/content/bandofolderdeepening.py
--rw-r--r--   0 daniele    (501) staff       (20)      152 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/content/configure.zcml
--rw-r--r--   0 daniele    (501) staff       (20)     1808 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/indexer.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.018215 redturtle.bandi-1.4.4/redturtle/bandi/interfaces/
--rw-r--r--   0 daniele    (501) staff       (20)      130 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/interfaces/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)      104 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/interfaces/bando.py
--rw-r--r--   0 daniele    (501) staff       (20)     4077 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/interfaces/bandoSchema.py
--rw-r--r--   0 daniele    (501) staff       (20)      218 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/interfaces/bandofolderdeepening.py
--rw-r--r--   0 daniele    (501) staff       (20)       95 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/interfaces/bandofolderdeepeningschema.py
--rw-r--r--   0 daniele    (501) staff       (20)      307 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/interfaces/browserlayer.py
--rw-r--r--   0 daniele    (501) staff       (20)     1797 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/interfaces/settings.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.019235 redturtle.bandi-1.4.4/redturtle/bandi/locales/
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.994251 redturtle.bandi-1.4.4/redturtle/bandi/locales/it/
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.019880 redturtle.bandi-1.4.4/redturtle/bandi/locales/it/LC_MESSAGES/
--rw-r--r--   0 daniele    (501) staff       (20)      997 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 daniele    (501) staff       (20)    14096 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/locales/it/LC_MESSAGES/redturtle.bandi.po
--rw-r--r--   0 daniele    (501) staff       (20)    11353 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/locales/redturtle.bandi.pot
--rw-r--r--   0 daniele    (501) staff       (20)     1561 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/locales/update.py
--rwxr-xr-x   0 daniele    (501) staff       (20)      482 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/locales/update.sh
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.021188 redturtle.bandi-1.4.4/redturtle/bandi/portlets/
--rw-r--r--   0 daniele    (501) staff       (20)        2 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/portlets/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)     3559 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/portlets/collection.pt
--rw-r--r--   0 daniele    (501) staff       (20)     9823 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/portlets/collection.py
--rw-r--r--   0 daniele    (501) staff       (20)      724 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/portlets/configure.zcml
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.995302 redturtle.bandi-1.4.4/redturtle/bandi/profiles/
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.025931 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/
--rw-r--r--   0 daniele    (501) staff       (20)      184 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/browserlayer.xml
--rw-r--r--   0 daniele    (501) staff       (20)     1006 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/catalog.xml
--rw-r--r--   0 daniele    (501) staff       (20)      587 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/controlpanel.xml
--rw-r--r--   0 daniele    (501) staff       (20)      313 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/diff_tool.xml
--rw-r--r--   0 daniele    (501) staff       (20)      728 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/factorytool.xml
--rw-r--r--   0 daniele    (501) staff       (20)       71 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/metadata.xml
--rw-r--r--   0 daniele    (501) staff       (20)      425 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/portlets.xml
--rw-r--r--   0 daniele    (501) staff       (20)      312 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/propertiestool.xml
--rw-r--r--   0 daniele    (501) staff       (20)       13 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/redturtle.bandi_various.txt
--rw-r--r--   0 daniele    (501) staff       (20)     6489 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/registry.xml
--rw-r--r--   0 daniele    (501) staff       (20)      244 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/repositorytool.xml
--rw-r--r--   0 daniele    (501) staff       (20)      738 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/rolemap.xml
--rw-r--r--   0 daniele    (501) staff       (20)      307 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/tinymce.xml
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.026823 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/types/
--rw-r--r--   0 daniele    (501) staff       (20)     3008 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/types/Bando.xml
--rw-r--r--   0 daniele    (501) staff       (20)     2593 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/types/Bando_Folder_Deepening.xml
--rw-r--r--   0 daniele    (501) staff       (20)      351 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/types/Collection.xml
--rw-r--r--   0 daniele    (501) staff       (20)      709 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/types.xml
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.027424 redturtle.bandi-1.4.4/redturtle/bandi/profiles/to_1100/
--rw-r--r--   0 daniele    (501) staff       (20)      779 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/to_1100/catalog.xml
--rw-r--r--   0 daniele    (501) staff       (20)     1093 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/to_1100/registry.xml
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.029667 redturtle.bandi-1.4.4/redturtle/bandi/profiles/uninstall/
--rw-r--r--   0 daniele    (501) staff       (20)      204 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 daniele    (501) staff       (20)      813 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/uninstall/catalog.xml
--rw-r--r--   0 daniele    (501) staff       (20)       47 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/uninstall/metadata.xml
--rw-r--r--   0 daniele    (501) staff       (20)      232 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/uninstall/portlets.xml
--rw-r--r--   0 daniele    (501) staff       (20)      265 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/uninstall/propertiestool.xml
--rw-r--r--   0 daniele    (501) staff       (20)      221 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/uninstall/registry.xml
--rw-r--r--   0 daniele    (501) staff       (20)      239 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/profiles/uninstall/types.xml
--rw-r--r--   0 daniele    (501) staff       (20)     1626 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/psheetvocabulary.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.030250 redturtle.bandi-1.4.4/redturtle/bandi/restapi/
--rw-r--r--   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/restapi/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)      315 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/restapi/configure.zcml
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.031182 redturtle.bandi-1.4.4/redturtle/bandi/restapi/deserializer/
--rw-r--r--   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/restapi/deserializer/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)      217 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/restapi/deserializer/configure.zcml
--rw-r--r--   0 daniele    (501) staff       (20)     2601 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/restapi/deserializer/dxfields.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.032046 redturtle.bandi-1.4.4/redturtle/bandi/restapi/services/
--rw-r--r--   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/restapi/services/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)      266 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/restapi/services/configure.zcml
--rw-r--r--   0 daniele    (501) staff       (20)      433 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/restapi/services/controlpanel.py
--rw-r--r--   0 daniele    (501) staff       (20)     1445 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/testing.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.033236 redturtle.bandi-1.4.4/redturtle/bandi/tests/
--rw-r--r--   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/tests/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)     3604 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/tests/test_bando_view.py
--rw-r--r--   0 daniele    (501) staff       (20)     2203 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/tests/test_collection_criteria.py
--rw-r--r--   0 daniele    (501) staff       (20)     2198 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/tests/test_setup.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.034424 redturtle.bandi-1.4.4/redturtle/bandi/tiles/
--rw-r--r--   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/tiles/__init__.py
--rw-r--r--   0 daniele    (501) staff       (20)     5060 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/tiles/bandi_render.pt
--rw-r--r--   0 daniele    (501) staff       (20)      364 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/tiles/bandi_render.py
--rw-r--r--   0 daniele    (501) staff       (20)      410 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/tiles/configure.zcml
--rw-r--r--   0 daniele    (501) staff       (20)     5450 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/upgrades.py
--rw-r--r--   0 daniele    (501) staff       (20)     1718 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/upgrades.zcml
--rw-r--r--   0 daniele    (501) staff       (20)     1963 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle/bandi/vocabularies.py
-drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-02-20 15:35:50.002886 redturtle.bandi-1.4.4/redturtle.bandi.egg-info/
--rw-r--r--   0 daniele    (501) staff       (20)     6544 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle.bandi.egg-info/PKG-INFO
--rw-r--r--   0 daniele    (501) staff       (20)     4554 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle.bandi.egg-info/SOURCES.txt
--rw-r--r--   0 daniele    (501) staff       (20)        1 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle.bandi.egg-info/dependency_links.txt
--rw-r--r--   0 daniele    (501) staff       (20)      120 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle.bandi.egg-info/entry_points.txt
--rw-r--r--   0 daniele    (501) staff       (20)       10 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle.bandi.egg-info/namespace_packages.txt
--rw-r--r--   0 daniele    (501) staff       (20)        1 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle.bandi.egg-info/not-zip-safe
--rw-r--r--   0 daniele    (501) staff       (20)      160 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle.bandi.egg-info/requires.txt
--rw-r--r--   0 daniele    (501) staff       (20)       10 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/redturtle.bandi.egg-info/top_level.txt
--rw-r--r--   0 daniele    (501) staff       (20)      321 2024-02-20 15:35:50.036469 redturtle.bandi-1.4.4/setup.cfg
--rw-r--r--   0 daniele    (501) staff       (20)     2306 2024-02-20 15:35:49.000000 redturtle.bandi-1.4.4/setup.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:30.000215 redturtle.bandi-1.4.5/
+-rw-r--r--   0 daniele    (501) staff       (20)      317 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/MANIFEST.in
+-rw-r--r--   0 daniele    (501) staff       (20)     6639 2024-04-15 09:48:30.000037 redturtle.bandi-1.4.5/PKG-INFO
+-rw-r--r--   0 daniele    (501) staff       (20)     3254 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/README.rst
+-rw-r--r--   0 daniele    (501) staff       (20)       96 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/buildout.cfg
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.957318 redturtle.bandi-1.4.5/docs/
+-rw-r--r--   0 daniele    (501) staff       (20)     2142 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/docs/HISTORY.txt
+-rw-r--r--   0 daniele    (501) staff       (20)     1463 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/docs/INSTALL.txt
+-rw-r--r--   0 daniele    (501) staff       (20)    17987 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/docs/LICENSE.GPL
+-rw-r--r--   0 daniele    (501) staff       (20)      726 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/docs/LICENSE.txt
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.957656 redturtle.bandi-1.4.5/redturtle/
+-rw-r--r--   0 daniele    (501) staff       (20)      244 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/__init__.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.964232 redturtle.bandi-1.4.5/redturtle/bandi/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.965008 redturtle.bandi-1.4.5/redturtle/bandi/Extensions/
+-rw-r--r--   0 daniele    (501) staff       (20)      402 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/Extensions/Install.py
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/Extensions/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)    10004 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/README.txt
+-rw-r--r--   0 daniele    (501) staff       (20)      197 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/__init__.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.970031 redturtle.bandi-1.4.5/redturtle/bandi/browser/
+-rw-r--r--   0 daniele    (501) staff       (20)        2 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     8892 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/bando-right.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     8211 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/bando.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     9506 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/bando.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5702 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/collection.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     1893 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/collection.py
+-rw-r--r--   0 daniele    (501) staff       (20)     4708 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)      585 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/context.py
+-rw-r--r--   0 daniele    (501) staff       (20)      389 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/controlpanel.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.971672 redturtle.bandi-1.4.5/redturtle/bandi/browser/css/
+-rw-r--r--   0 daniele    (501) staff       (20)       48 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/css/Makefile
+-rw-r--r--   0 daniele    (501) staff       (20)     4833 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/css/bandi.css
+-rw-r--r--   0 daniele    (501) staff       (20)     1032 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/css/bandi.css.map
+-rw-r--r--   0 daniele    (501) staff       (20)     5365 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/css/bandi.scss
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.973850 redturtle.bandi-1.4.5/redturtle/bandi/browser/images/
+-rw-r--r--   0 daniele    (501) staff       (20)      252 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/images/bando.png
+-rw-r--r--   0 daniele    (501) staff       (20)     1192 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/images/bando_closed.png
+-rw-r--r--   0 daniele    (501) staff       (20)      811 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/images/bando_icon.svg
+-rw-r--r--   0 daniele    (501) staff       (20)      351 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/images/bando_inprogress.png
+-rw-r--r--   0 daniele    (501) staff       (20)     1199 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/images/bando_open.png
+-rw-r--r--   0 daniele    (501) staff       (20)      621 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/images/folder_bando_deep.gif
+-rw-r--r--   0 daniele    (501) staff       (20)     3973 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/migrator.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6811 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/search.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     5969 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/search.py
+-rw-r--r--   0 daniele    (501) staff       (20)     9603 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/search_form.pt
+-rw-r--r--   0 daniele    (501) staff       (20)      322 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/browser/searchbandi.js
+-rw-r--r--   0 daniele    (501) staff       (20)     2846 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/configure.zcml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.975436 redturtle.bandi-1.4.5/redturtle/bandi/content/
+-rw-r--r--   0 daniele    (501) staff       (20)        2 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/content/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      220 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/content/bando.py
+-rw-r--r--   0 daniele    (501) staff       (20)      280 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/content/bandofolderdeepening.py
+-rw-r--r--   0 daniele    (501) staff       (20)      152 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/content/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     2217 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/indexer.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.978003 redturtle.bandi-1.4.5/redturtle/bandi/interfaces/
+-rw-r--r--   0 daniele    (501) staff       (20)      130 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/interfaces/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      104 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/interfaces/bando.py
+-rw-r--r--   0 daniele    (501) staff       (20)     4077 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/interfaces/bandoSchema.py
+-rw-r--r--   0 daniele    (501) staff       (20)      218 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/interfaces/bandofolderdeepening.py
+-rw-r--r--   0 daniele    (501) staff       (20)       95 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/interfaces/bandofolderdeepeningschema.py
+-rw-r--r--   0 daniele    (501) staff       (20)      307 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/interfaces/browserlayer.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1797 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/interfaces/settings.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.979104 redturtle.bandi-1.4.5/redturtle/bandi/locales/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.951972 redturtle.bandi-1.4.5/redturtle/bandi/locales/it/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.980242 redturtle.bandi-1.4.5/redturtle/bandi/locales/it/LC_MESSAGES/
+-rw-r--r--   0 daniele    (501) staff       (20)      997 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 daniele    (501) staff       (20)    14096 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/locales/it/LC_MESSAGES/redturtle.bandi.po
+-rw-r--r--   0 daniele    (501) staff       (20)    11353 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/locales/redturtle.bandi.pot
+-rw-r--r--   0 daniele    (501) staff       (20)     1561 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/locales/update.py
+-rwxr-xr-x   0 daniele    (501) staff       (20)      482 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/locales/update.sh
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.981937 redturtle.bandi-1.4.5/redturtle/bandi/portlets/
+-rw-r--r--   0 daniele    (501) staff       (20)        2 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/portlets/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3559 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/portlets/collection.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     9823 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/portlets/collection.py
+-rw-r--r--   0 daniele    (501) staff       (20)      724 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/portlets/configure.zcml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.953154 redturtle.bandi-1.4.5/redturtle/bandi/profiles/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.987644 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/
+-rw-r--r--   0 daniele    (501) staff       (20)      184 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/browserlayer.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     1050 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/catalog.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      587 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/controlpanel.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      313 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/diff_tool.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      728 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/factorytool.xml
+-rw-r--r--   0 daniele    (501) staff       (20)       71 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/metadata.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      425 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/portlets.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      312 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/propertiestool.xml
+-rw-r--r--   0 daniele    (501) staff       (20)       13 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/redturtle.bandi_various.txt
+-rw-r--r--   0 daniele    (501) staff       (20)     6489 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/registry.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      244 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/repositorytool.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      738 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/rolemap.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      307 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/tinymce.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.988758 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/types/
+-rw-r--r--   0 daniele    (501) staff       (20)     3008 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/types/Bando.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     2593 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/types/Bando_Folder_Deepening.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      351 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/types/Collection.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      709 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/types.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.989493 redturtle.bandi-1.4.5/redturtle/bandi/profiles/to_1100/
+-rw-r--r--   0 daniele    (501) staff       (20)      779 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/to_1100/catalog.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     1093 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/to_1100/registry.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.992565 redturtle.bandi-1.4.5/redturtle/bandi/profiles/uninstall/
+-rw-r--r--   0 daniele    (501) staff       (20)      204 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      813 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/uninstall/catalog.xml
+-rw-r--r--   0 daniele    (501) staff       (20)       47 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/uninstall/metadata.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      232 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/uninstall/portlets.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      265 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/uninstall/propertiestool.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      221 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/uninstall/registry.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      239 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/profiles/uninstall/types.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     1626 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/psheetvocabulary.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.993224 redturtle.bandi-1.4.5/redturtle/bandi/restapi/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/restapi/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      315 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/restapi/configure.zcml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.994340 redturtle.bandi-1.4.5/redturtle/bandi/restapi/deserializer/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/restapi/deserializer/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      217 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/restapi/deserializer/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     2601 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/restapi/deserializer/dxfields.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.995411 redturtle.bandi-1.4.5/redturtle/bandi/restapi/services/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/restapi/services/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      266 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/restapi/services/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)      433 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/restapi/services/controlpanel.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1445 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/testing.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.996957 redturtle.bandi-1.4.5/redturtle/bandi/tests/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/tests/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3604 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/tests/test_bando_view.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2203 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/tests/test_collection_criteria.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2198 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/tests/test_setup.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.998516 redturtle.bandi-1.4.5/redturtle/bandi/tiles/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/tiles/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5060 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/tiles/bandi_render.pt
+-rw-r--r--   0 daniele    (501) staff       (20)      364 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/tiles/bandi_render.py
+-rw-r--r--   0 daniele    (501) staff       (20)      410 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/tiles/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     5969 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/upgrades.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1933 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/upgrades.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     1963 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle/bandi/vocabularies.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-15 09:48:29.960811 redturtle.bandi-1.4.5/redturtle.bandi.egg-info/
+-rw-r--r--   0 daniele    (501) staff       (20)     6639 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle.bandi.egg-info/PKG-INFO
+-rw-r--r--   0 daniele    (501) staff       (20)     4554 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle.bandi.egg-info/SOURCES.txt
+-rw-r--r--   0 daniele    (501) staff       (20)        1 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle.bandi.egg-info/dependency_links.txt
+-rw-r--r--   0 daniele    (501) staff       (20)      120 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle.bandi.egg-info/entry_points.txt
+-rw-r--r--   0 daniele    (501) staff       (20)       10 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle.bandi.egg-info/namespace_packages.txt
+-rw-r--r--   0 daniele    (501) staff       (20)        1 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle.bandi.egg-info/not-zip-safe
+-rw-r--r--   0 daniele    (501) staff       (20)      160 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle.bandi.egg-info/requires.txt
+-rw-r--r--   0 daniele    (501) staff       (20)       10 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/redturtle.bandi.egg-info/top_level.txt
+-rw-r--r--   0 daniele    (501) staff       (20)      321 2024-04-15 09:48:30.001032 redturtle.bandi-1.4.5/setup.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     2306 2024-04-15 09:48:29.000000 redturtle.bandi-1.4.5/setup.py
```

### Comparing `redturtle.bandi-1.4.4/PKG-INFO` & `redturtle.bandi-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.bandi
-Version: 1.4.4
+Version: 1.4.5
 Summary: A product for announcements management based on rer.bandi
 Home-page: https://github.com/PloneGov-IT/redturtle.bandi
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.bandi
 Project-URL: Source, https://github.com/RedTurtle/redturtle.bandi
@@ -142,14 +142,21 @@
 .. image:: http://www.redturtle.net/redturtle_banner.png
    :alt: RedTurtle Technology Site
    :target: http://www.redturtle.net/
 
 Changelog
 =========
 
+1.4.5 (2024-04-15)
+------------------
+
+- Added "tipologia_bando_label" metadata.
+  [daniele]
+
+
 1.4.4 (2024-02-20)
 ------------------
 
 - Changed translation for states "Open" and "Closed".
   [daniele]
```

### Comparing `redturtle.bandi-1.4.4/README.rst` & `redturtle.bandi-1.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/docs/HISTORY.txt` & `redturtle.bandi-1.4.5/docs/HISTORY.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+1.4.5 (2024-04-15)
+------------------
+
+- Added "tipologia_bando_label" metadata.
+  [daniele]
+
+
 1.4.4 (2024-02-20)
 ------------------
 
 - Changed translation for states "Open" and "Closed".
   [daniele]
```

### Comparing `redturtle.bandi-1.4.4/docs/INSTALL.txt` & `redturtle.bandi-1.4.5/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/docs/LICENSE.GPL` & `redturtle.bandi-1.4.5/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/docs/LICENSE.txt` & `redturtle.bandi-1.4.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/README.txt` & `redturtle.bandi-1.4.5/redturtle/bandi/README.txt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/bando-right.pt` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/bando-right.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/bando.pt` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/bando.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/bando.py` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/bando.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/collection.pt` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/collection.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/collection.py` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/collection.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/configure.zcml` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/context.py` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/context.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/css/bandi.css` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/css/bandi.css`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/css/bandi.css.map` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/css/bandi.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/css/bandi.scss` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/css/bandi.scss`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/images/bando_closed.png` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/images/bando_closed.png`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/images/bando_icon.svg` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/images/bando_icon.svg`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/images/bando_open.png` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/images/bando_open.png`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/images/folder_bando_deep.gif` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/images/folder_bando_deep.gif`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/migrator.py` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/migrator.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/search.pt` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/search.py` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/search.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/browser/search_form.pt` & `redturtle.bandi-1.4.5/redturtle/bandi/browser/search_form.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/configure.zcml` & `redturtle.bandi-1.4.5/redturtle/bandi/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -76,9 +76,10 @@
 
   <!-- indexers -->
   <adapter name="destinatari_bando" factory=".indexer.destinatari_bando" />
   <adapter name="chiusura_procedimento_bando" factory=".indexer.chiusura_procedimento_bando" />
   <adapter name="scadenza_bando" factory=".indexer.scadenza_bando" />
   <adapter name="ente_bando" factory=".indexer.ente_bando" />
   <adapter name="tipologia_bando" factory=".indexer.tipologia_bando" />
+  <adapter name="tipologia_bando_label" factory=".indexer.tipologia_bando_label" />
   <adapter name="apertura_bando" factory=".indexer.apertura_bando" />
 </configure>
```

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/indexer.py` & `redturtle.bandi-1.4.5/redturtle/bandi/indexer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from DateTime import DateTime
 from plone.indexer.decorator import indexer
 from redturtle.bandi.interfaces.bando import IBando
+from redturtle.bandi.vocabularies import TipologiaBandoVocabulary
 
 # importo il datetime di python
 from datetime import datetime
 
 # funzione che riceve un date e torna un datetime con l'ora a zero
 
 
@@ -59,7 +60,19 @@
 def ente_bando(object, **kw):
     return getattr(object, "ente_bando", None)
 
 
 @indexer(IBando)
 def tipologia_bando(object, **kw):
     return getattr(object, "tipologia_bando", None)
+    
+
+@indexer(IBando)
+def tipologia_bando_label(object, **kw):
+    if not object.tipologia_bando:
+        return None
+    vocab = TipologiaBandoVocabulary().__call__(object)
+    try:
+        vocab.getTermByToken(object.tipologia_bando)
+    except LookupError:
+        return None
+    return vocab.getTermByToken(object.tipologia_bando).title
```

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/interfaces/bandoSchema.py` & `redturtle.bandi-1.4.5/redturtle/bandi/interfaces/bandoSchema.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/interfaces/settings.py` & `redturtle.bandi-1.4.5/redturtle/bandi/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/locales/it/LC_MESSAGES/plone.po` & `redturtle.bandi-1.4.5/redturtle/bandi/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/locales/it/LC_MESSAGES/redturtle.bandi.po` & `redturtle.bandi-1.4.5/redturtle/bandi/locales/it/LC_MESSAGES/redturtle.bandi.po`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/locales/redturtle.bandi.pot` & `redturtle.bandi-1.4.5/redturtle/bandi/locales/redturtle.bandi.pot`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/locales/update.py` & `redturtle.bandi-1.4.5/redturtle/bandi/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/portlets/collection.pt` & `redturtle.bandi-1.4.5/redturtle/bandi/portlets/collection.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/portlets/collection.py` & `redturtle.bandi-1.4.5/redturtle/bandi/portlets/collection.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/portlets/configure.zcml` & `redturtle.bandi-1.4.5/redturtle/bandi/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/catalog.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/catalog.xml`

 * *Files 4% similar despite different names*

#### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/catalog.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/catalog.xml`

```diff
@@ -19,8 +19,9 @@
     <indexed_attr value="ente_bando"/>
   </index>
   <column value="chiusura_procedimento_bando"/>
   <column value="apertura_bando"/>
   <column value="destinatari_bando"/>
   <column value="scadenza_bando"/>
   <column value="tipologia_bando"/>
+  <column value="tipologia_bando_label"/>
 </object>
```

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/controlpanel.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/factorytool.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/factorytool.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/registry.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/rolemap.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/types/Bando.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/types/Bando.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/types/Bando_Folder_Deepening.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/types/Bando_Folder_Deepening.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/default/types.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/to_1100/catalog.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/to_1100/catalog.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/to_1100/registry.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/to_1100/registry.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/profiles/uninstall/catalog.xml` & `redturtle.bandi-1.4.5/redturtle/bandi/profiles/uninstall/catalog.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/psheetvocabulary.py` & `redturtle.bandi-1.4.5/redturtle/bandi/psheetvocabulary.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/restapi/deserializer/dxfields.py` & `redturtle.bandi-1.4.5/redturtle/bandi/restapi/deserializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/testing.py` & `redturtle.bandi-1.4.5/redturtle/bandi/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/tests/test_bando_view.py` & `redturtle.bandi-1.4.5/redturtle/bandi/tests/test_bando_view.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/tests/test_collection_criteria.py` & `redturtle.bandi-1.4.5/redturtle/bandi/tests/test_collection_criteria.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/tests/test_setup.py` & `redturtle.bandi-1.4.5/redturtle/bandi/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/tiles/bandi_render.pt` & `redturtle.bandi-1.4.5/redturtle/bandi/tiles/bandi_render.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/upgrades.py` & `redturtle.bandi-1.4.5/redturtle/bandi/upgrades.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,7 +166,23 @@
         logger.info(
             "[{counter}/{tot}] - {bando}".format(
                 counter=counter + 1, tot=tot_results, bando=brain.getPath()
             )
         )
         bando = brain.getObject()
         bando.reindexObject(idxs=['scadenza_bando'])
+
+
+def migrate_to_2102(context):
+    update_catalog(context)
+
+    bandi = api.content.find(portal_type="Bando")
+    tot_results = len(bandi)
+    logger.info("### Fixing {tot} Bandi ###".format(tot=tot_results))
+    for counter, brain in enumerate(bandi):
+        logger.info(
+            "[{counter}/{tot}] - {bando}".format(
+                counter=counter + 1, tot=tot_results, bando=brain.getPath()
+            )
+        )
+        bando = brain.getObject()
+        bando.reindexObject(idxs=['tipologia_bando_label'])
```

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/upgrades.zcml` & `redturtle.bandi-1.4.5/redturtle/bandi/upgrades.zcml`

 * *Files 18% similar despite different names*

```diff
@@ -55,8 +55,16 @@
     title="Reindex Scadenza bando with new indexer version"
     description=""
     source="2100"
     destination="2101"
     handler=".upgrades.migrate_to_2101"
     profile="redturtle.bandi:default" />
 
+  <gs:upgradeStep
+    title="Add new metadata for tipologia_bando_label"
+    description=""
+    source="2101"
+    destination="2102"
+    handler=".upgrades.migrate_to_2102"
+    profile="redturtle.bandi:default" />
+
   </configure>
```

### Comparing `redturtle.bandi-1.4.4/redturtle/bandi/vocabularies.py` & `redturtle.bandi-1.4.5/redturtle/bandi/vocabularies.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/redturtle.bandi.egg-info/PKG-INFO` & `redturtle.bandi-1.4.5/redturtle.bandi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.bandi
-Version: 1.4.4
+Version: 1.4.5
 Summary: A product for announcements management based on rer.bandi
 Home-page: https://github.com/PloneGov-IT/redturtle.bandi
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.bandi
 Project-URL: Source, https://github.com/RedTurtle/redturtle.bandi
@@ -142,14 +142,21 @@
 .. image:: http://www.redturtle.net/redturtle_banner.png
    :alt: RedTurtle Technology Site
    :target: http://www.redturtle.net/
 
 Changelog
 =========
 
+1.4.5 (2024-04-15)
+------------------
+
+- Added "tipologia_bando_label" metadata.
+  [daniele]
+
+
 1.4.4 (2024-02-20)
 ------------------
 
 - Changed translation for states "Open" and "Closed".
   [daniele]
```

### Comparing `redturtle.bandi-1.4.4/redturtle.bandi.egg-info/SOURCES.txt` & `redturtle.bandi-1.4.5/redturtle.bandi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.4/setup.py` & `redturtle.bandi-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 This module contains the tool of redturtle.bandi
 """
 import os
 from setuptools import setup, find_packages
 
-version = "1.4.4"
+version = "1.4.5"
 
 setup(
     name="redturtle.bandi",
     version=version,
     description="A product for announcements management based on rer.bandi",
     long_description=open("README.rst").read()
     + "\n"
```

