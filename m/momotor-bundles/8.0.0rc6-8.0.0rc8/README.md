# Comparing `tmp/momotor-bundles-8.0.0rc6.tar.gz` & `tmp/momotor-bundles-8.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-bundles-8.0.0rc6.tar", last modified: Thu Jan 18 07:20:18 2024, max compression
+gzip compressed data, was "momotor-bundles-8.0.0rc8.tar", last modified: Fri Mar  8 06:57:33 2024, max compression
```

## Comparing `momotor-bundles-8.0.0rc6.tar` & `momotor-bundles-8.0.0rc8.tar`

### file list

```diff
@@ -1,224 +1,223 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/
--rw-rw-rw-   0 root         (0) root         (0)     2927 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3399 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/.idea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/.idea/inspectionProfiles/
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0 root         (0) root         (0)      282 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)     1325 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/.idea/momotor.lib.bundles.iml
--rw-rw-rw-   0 root         (0) root         (0)     1155 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/.xsdata.xml
--rw-rw-rw-   0 root         (0) root         (0)    28129 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3531 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1468 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/build.bat
--rwxrwxrwx   0 root         (0) root         (0)      100 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      764 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)     6988 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/_static/logo-text-negative.png
--rw-rw-rw-   0 root         (0) root         (0)     6887 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/_static/logo-text.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/docs/source/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/_templates/projectlinks.html
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/binding.rst
--rw-rw-rw-   0 root         (0) root         (0)     4688 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/bundles.rst
--rw-rw-rw-   0 root         (0) root         (0)     3783 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/constants.rst
--rw-rw-rw-   0 root         (0) root         (0)     3245 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/content.rst
--rw-rw-rw-   0 root         (0) root         (0)     3100 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/elements.rst
--rw-rw-rw-   0 root         (0) root         (0)      474 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)    16692 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/filters.rst
--rw-rw-rw-   0 root         (0) root         (0)     3791 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2869 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/docs/source/utils.rst
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/publish-docs.sh
--rw-rw-rw-   0 root         (0) root         (0)     2798 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/semver.sh
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20223 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/binding/
--rw-rw-rw-   0 root         (0) root         (0)     1772 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/binding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24652 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/binding/momotor_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/binding/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     3181 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/config.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7171 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/base.py
--rw-rw-rw-   0 root         (0) root         (0)    16087 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/checklets.py
--rw-rw-rw-   0 root         (0) root         (0)    28560 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/content.py
--rw-rw-rw-   0 root         (0) root         (0)    12940 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/files.py
--rw-rw-rw-   0 root         (0) root         (0)     9035 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     9901 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/options.py
--rw-rw-rw-   0 root         (0) root         (0)     7208 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/properties.py
--rw-rw-rw-   0 root         (0) root         (0)     1485 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/refs.py
--rw-rw-rw-   0 root         (0) root         (0)     5408 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     8878 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/result.py
--rw-rw-rw-   0 root         (0) root         (0)     5066 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/results.py
--rw-rw-rw-   0 root         (0) root         (0)    11933 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/steps.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/wildcard.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/mixins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/mixins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21212 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/mixins/attachments.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/mixins/id.py
--rw-rw-rw-   0 root         (0) root         (0)     1816 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/mixins/name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/handlers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/handlers/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/handlers/lxml.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/handlers/xml.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     3605 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/product.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/recipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/schema/
--rw-rw-rw-   0 root         (0) root         (0)    13856 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/schema/momotor-1.0.xsd
--rw-rw-rw-   0 root         (0) root         (0)     8836 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/schema/xml.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/serializers/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/serializers/writers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/serializers/writers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/serializers/writers/lxml.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/serializers/writers/xml.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/serializers/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/test.py
--rw-rw-rw-   0 root         (0) root         (0)     3905 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/testresult.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/typing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/typing/element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)      642 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     5242 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/assertion.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/detect.py
--rw-rw-rw-   0 root         (0) root         (0)     3383 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     4224 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/encoding.py
--rw-rw-rw-   0 root         (0) root         (0)    12987 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/grouping.py
--rw-rw-rw-   0 root         (0) root         (0)     2198 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/immutable.py
--rw-rw-rw-   0 root         (0) root         (0)     6215 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/keyedtuple.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/lxml.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/rglob.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/text.py
--rw-rw-rw-   0 root         (0) root         (0)     1881 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/zipwrapper.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-01-18 07:20:13.000000 momotor-bundles-8.0.0rc6/src/momotor/bundles/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor_bundles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3531 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor_bundles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5847 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor_bundles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor_bundles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      412 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor_bundles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/src/momotor_bundles.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/content.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/full-recipe/
--rw-rw-rw-   0 root         (0) root         (0)     1928 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/full-recipe/recipe.xml
--rw-rw-rw-   0 root         (0) root         (0)    35629 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/huge_product.zip
--rw-rw-rw-   0 root         (0) root         (0)      351 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/inline-trailing-whitespace.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/meta/
--rw-rw-rw-   0 root         (0) root         (0)      358 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/meta/invalid-description.xml
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/meta/recipe-with-meta.xml
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/meta/recipe-with-multiple-meta.xml
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/non-product-1.txt
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/non-product-2.zip
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/product-1.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/product-2/
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/product-2/product.xml
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/product-3.zip
--rw-rw-rw-   0 root         (0) root         (0)      252 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/recipe-1.xml
--rw-rw-rw-   0 root         (0) root         (0)     1421 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/resources.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/file-in-root.txt
--rw-rw-rw-   0 root         (0) root         (0)     1639 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/recipe.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/step1/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/step1/file-in-root.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/step1/subdir/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/step1/subdir/file-in-dir.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/subdir/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/subdir/file-in-dir.txt
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-files.zip
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-repository/
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-repository/recipe.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-repository/repo/
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-repository/repo/repofile.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-repository/repo/subdir/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-repository/repo/subdir/repofile.txt
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/files/with-repository.zip
--rw-rw-rw-   0 root         (0) root         (0)     2339 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_checklets.py
--rw-rw-rw-   0 root         (0) root         (0)    12241 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_content.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_detect.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_empty.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_files.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_hashes.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_huge_text.py
--rw-rw-rw-   0 root         (0) root         (0)     5156 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     2891 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_read_bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_resources.py
--rw-rw-rw-   0 root         (0) root         (0)     1319 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_result.py
--rw-rw-rw-   0 root         (0) root         (0)      930 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle/test_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2948 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/bundle_test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/create/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/create/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/create/files/missing_attachment/
--rw-rw-rw-   0 root         (0) root         (0)      293 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/create/files/missing_attachment/config.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/create/files/recipe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/create/files/recipe/checklet/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/create/files/recipe/checklet/generate-score/
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/create/files/recipe/checklet/generate-score/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/create/files/recipe/checklet/generate-score/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/create/files/recipe/checklet/generate-score/src/generate_score/
--rw-rw-rw-   0 root         (0) root         (0)     3505 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/create/files/recipe/checklet/generate-score/src/generate_score/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/create/files/recipe/recipe.xml
--rw-rw-rw-   0 root         (0) root         (0)     8531 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/create/test_attachments.py
--rw-rw-rw-   0 root         (0) root         (0)     7459 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/create/test_bundle_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     6121 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/create/test_xml_creation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/fromio/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/fromio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/fromio/files/
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/fromio/files/invalid.xml
--rw-rw-rw-   0 root         (0) root         (0)      351 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/fromio/files/valid.xml
--rw-rw-rw-   0 root         (0) root         (0)      969 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/fromio/files/valid_xslt.xml
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/fromio/test_fromio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/options/
--rw-rw-rw-   0 root         (0) root         (0)    16934 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/options/test_option_domains.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/recreate/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/recreate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/recreate/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/recreate/files/result1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/recreate/files/result1/files/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/recreate/files/result1/files/result.txt
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/recreate/files/result1/result.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/recreate/files/result2/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/recreate/files/result2/result.txt
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/recreate/files/result2/result.xml
--rw-rw-rw-   0 root         (0) root         (0)     4198 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/recreate/test_result_recreate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7390 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/utils/test_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2131 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/utils/test_rglob.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/utils/test_utils_encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     3167 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/utils/test_utils_keyedsequence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/warnings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 07:20:18.000000 momotor-bundles-8.0.0rc6/tests/warnings/files/
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/warnings/files/domnode.xml
--rw-rw-rw-   0 root         (0) root         (0)      973 2024-01-18 07:19:35.000000 momotor-bundles-8.0.0rc6/tests/warnings/test_warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/
+-rw-rw-rw-   0 root         (0) root         (0)     2927 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3399 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/.idea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/.idea/inspectionProfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/.idea/momotor.lib.bundles.iml
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/.xsdata.xml
+-rw-rw-rw-   0 root         (0) root         (0)    28129 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3535 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/build.bat
+-rwxrwxrwx   0 root         (0) root         (0)      100 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     6988 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/_static/logo-text-negative.png
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/_static/logo-text.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/docs/source/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/_templates/projectlinks.html
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/binding.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4688 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/bundles.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3783 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/constants.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3245 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/content.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3100 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/elements.rst
+-rw-rw-rw-   0 root         (0) root         (0)      474 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16692 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/filters.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3791 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2869 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/docs/source/utils.rst
+-rw-rw-rw-   0 root         (0) root         (0)      423 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/publish-docs.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2871 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/semver.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20223 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/binding/
+-rw-rw-rw-   0 root         (0) root         (0)     1772 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/binding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24652 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/binding/momotor_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/binding/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3181 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7171 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    16087 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/checklets.py
+-rw-rw-rw-   0 root         (0) root         (0)    28560 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/content.py
+-rw-rw-rw-   0 root         (0) root         (0)    12940 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     9035 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     7208 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/refs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5408 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     8878 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/result.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/results.py
+-rw-rw-rw-   0 root         (0) root         (0)    11933 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/wildcard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/mixins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21212 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/mixins/attachments.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/mixins/id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/mixins/name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/handlers/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/handlers/lxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/handlers/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/product.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/recipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2900 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/schema/
+-rw-rw-rw-   0 root         (0) root         (0)    13856 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/schema/momotor-1.0.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     8836 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/schema/xml.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/serializers/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/serializers/writers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/serializers/writers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/serializers/writers/lxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/serializers/writers/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/serializers/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/testresult.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/typing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/typing/element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)      642 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     5242 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/assertion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/detect.py
+-rw-rw-rw-   0 root         (0) root         (0)     3383 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)    12987 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/grouping.py
+-rw-rw-rw-   0 root         (0) root         (0)     2198 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/immutable.py
+-rw-rw-rw-   0 root         (0) root         (0)     6215 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/keyedtuple.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/lxml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/rglob.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/zipwrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-03-08 06:57:31.000000 momotor-bundles-8.0.0rc8/src/momotor/bundles/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor_bundles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3535 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor_bundles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5835 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor_bundles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor_bundles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      416 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor_bundles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/src/momotor_bundles.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/content.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/full-recipe/
+-rw-rw-rw-   0 root         (0) root         (0)     1928 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/full-recipe/recipe.xml
+-rw-rw-rw-   0 root         (0) root         (0)    35629 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/huge_product.zip
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/inline-trailing-whitespace.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/meta/
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/meta/invalid-description.xml
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/meta/recipe-with-meta.xml
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/meta/recipe-with-multiple-meta.xml
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/non-product-1.txt
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/non-product-2.zip
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/product-1.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/product-2/
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/product-2/product.xml
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/product-3.zip
+-rw-rw-rw-   0 root         (0) root         (0)      252 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/recipe-1.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/resources.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/file-in-root.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/recipe.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/step1/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/step1/file-in-root.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/step1/subdir/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/step1/subdir/file-in-dir.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/subdir/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/subdir/file-in-dir.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-files.zip
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-repository/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-repository/recipe.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-repository/repo/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-repository/repo/repofile.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-repository/repo/subdir/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-repository/repo/subdir/repofile.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/files/with-repository.zip
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_checklets.py
+-rw-rw-rw-   0 root         (0) root         (0)    12241 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_content.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_detect.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_empty.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_huge_text.py
+-rw-rw-rw-   0 root         (0) root         (0)     5156 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2891 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_read_bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_result.py
+-rw-rw-rw-   0 root         (0) root         (0)      930 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle/test_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2948 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/bundle_test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/create/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/create/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/create/files/missing_attachment/
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/create/files/missing_attachment/config.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/create/files/recipe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/create/files/recipe/checklet/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/create/files/recipe/checklet/generate-score/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/create/files/recipe/checklet/generate-score/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/create/files/recipe/checklet/generate-score/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/create/files/recipe/checklet/generate-score/src/generate_score/
+-rw-rw-rw-   0 root         (0) root         (0)     3505 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/create/files/recipe/checklet/generate-score/src/generate_score/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/create/files/recipe/recipe.xml
+-rw-rw-rw-   0 root         (0) root         (0)     8531 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/create/test_attachments.py
+-rw-rw-rw-   0 root         (0) root         (0)     7459 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/create/test_bundle_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6121 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/create/test_xml_creation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/fromio/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/fromio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/fromio/files/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/fromio/files/invalid.xml
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/fromio/files/valid.xml
+-rw-rw-rw-   0 root         (0) root         (0)      969 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/fromio/files/valid_xslt.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/fromio/test_fromio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/options/
+-rw-rw-rw-   0 root         (0) root         (0)    16934 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/options/test_option_domains.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/recreate/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/recreate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/recreate/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/recreate/files/result1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/recreate/files/result1/files/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/recreate/files/result1/files/result.txt
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/recreate/files/result1/result.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/recreate/files/result2/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/recreate/files/result2/result.txt
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/recreate/files/result2/result.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/recreate/test_result_recreate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7390 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/utils/test_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/utils/test_rglob.py
+-rw-rw-rw-   0 root         (0) root         (0)      838 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/utils/test_utils_encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3167 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/utils/test_utils_keyedsequence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/warnings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 06:57:33.000000 momotor-bundles-8.0.0rc8/tests/warnings/files/
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/warnings/files/domnode.xml
+-rw-rw-rw-   0 root         (0) root         (0)      973 2024-03-08 06:56:59.000000 momotor-bundles-8.0.0rc8/tests/warnings/test_warnings.py
```

### Comparing `momotor-bundles-8.0.0rc6/.gitignore` & `momotor-bundles-8.0.0rc8/.gitignore`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/.gitlab-ci.yml` & `momotor-bundles-8.0.0rc8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/.idea/momotor.lib.bundles.iml` & `momotor-bundles-8.0.0rc8/.idea/momotor.lib.bundles.iml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/.xsdata.xml` & `momotor-bundles-8.0.0rc8/.xsdata.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/CHANGELOG.md` & `momotor-bundles-8.0.0rc8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/LICENSE.txt` & `momotor-bundles-8.0.0rc8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/PKG-INFO` & `momotor-bundles-8.0.0rc8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momotor-bundles
-Version: 8.0.0rc6
+Version: 8.0.0rc8
 Summary: Momotor bundle reader, writer, tools
 Author-email: Erik Scheffers <e.t.j.scheffers@tue.nl>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://momotor.org
 Project-URL: Documentation, https://momotor.org/doc/engine/momotor-bundles/
 Project-URL: Repository, https://gitlab.tue.nl/momotor/engine-py3/momotor-bundles/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-bundles/issues
@@ -35,15 +35,15 @@
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints!=1.14.0; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: momotor-bundles[docs,lxml,test]; extra == "dev"
 Requires-Dist: xsdata[cli]==23.8.*; extra == "dev"
 Provides-Extra: build
-Requires-Dist: momotor-bundles[docs]; extra == "build"
+Requires-Dist: momotor-bundles[dev,docs]; extra == "build"
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: build[virtualenv]; extra == "build"
 Requires-Dist: python-semantic-release~=8.0; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 This package is a part of [Momotor](https://momotor.org/), a tool for automated processing of digital content.
```

### Comparing `momotor-bundles-8.0.0rc6/README.md` & `momotor-bundles-8.0.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/Makefile` & `momotor-bundles-8.0.0rc8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/make.bat` & `momotor-bundles-8.0.0rc8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/_static/logo-text-negative.png` & `momotor-bundles-8.0.0rc8/docs/source/_static/logo-text-negative.png`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/_static/logo-text.png` & `momotor-bundles-8.0.0rc8/docs/source/_static/logo-text.png`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/_templates/projectlinks.html` & `momotor-bundles-8.0.0rc8/docs/source/_templates/projectlinks.html`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/bundles.rst` & `momotor-bundles-8.0.0rc8/docs/source/bundles.rst`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/conf.py` & `momotor-bundles-8.0.0rc8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/content.rst` & `momotor-bundles-8.0.0rc8/docs/source/content.rst`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/elements.rst` & `momotor-bundles-8.0.0rc8/docs/source/elements.rst`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/filters.rst` & `momotor-bundles-8.0.0rc8/docs/source/filters.rst`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/index.rst` & `momotor-bundles-8.0.0rc8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/docs/source/utils.rst` & `momotor-bundles-8.0.0rc8/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/pyproject.toml` & `momotor-bundles-8.0.0rc8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     'furo',
 ]
 dev = [
     'momotor-bundles[lxml,test,docs]',
     'xsdata[cli]==23.8.*',
 ]
 build = [
-    'momotor-bundles[docs]',
+    'momotor-bundles[dev,docs]',
     'setuptools',
     'build[virtualenv]',
     'python-semantic-release~=8.0',
     'twine',
 ]
 
 [project.urls]
@@ -65,14 +65,17 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["momotor.*"]
 
+[tool.setuptools.package-data]
+"momotor.bundles.schema" = ["*.xsd"]
+
 [tool.setuptools.dynamic]
 version = { attr = "momotor.bundles.version.__VERSION__" }
 readme = { file = ["README.md"], content-type = "text/markdown" }
 
 [tool.pytest.ini_options]
 required_plugins = ["pytest-doctestplus"]
 norecursedirs = [".git", "files"]
```

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/base.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/base.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/binding/__init__.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/binding/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/binding/momotor_1_0.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/binding/momotor_1_0.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/config.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/config.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/base.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/base.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/checklets.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/checklets.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 class Checklet(
     NestedElement[CheckletComplexType, CheckletsComplexType],
     NameStrMixin,
     ResourcesMixin,
 ):
     """ A Checklet element encapsulating :py:class:`~momotor.bundles.binding.momotor_1_0.CheckletComplexType`
     """
-    DEFAULT_ENTRYPOINT: typing.ClassVar[str] = 'momotor.checklet'
+    _OLD_DEFAULT_ENTRYPOINT: typing.ClassVar[str] = 'momotor.checklet'
 
     __unset: typing.ClassVar = object()
 
     _extras: FilterableTuple[str] | None = __unset
     _version: str | None = __unset
     _entrypoint: str | None = __unset
     _repository: Repository | None = __unset
@@ -170,18 +170,18 @@
     def version(self, version: str | None):
         assert self._version is self.__unset, "Immutable attribute `version`"
         assert version is None or isinstance(version, str), "Invalid type for attribute `version`"
         self._version = version
 
     @typing.final
     @property
-    def entrypoint(self) -> str:
+    def entrypoint(self) -> typing.Optional[str]:
         """ `entrypoint` attribute: Override the default package entrypoint """
         assert self._entrypoint is not self.__unset, "Uninitialized attribute `entrypoint`"
-        return self._entrypoint or self.DEFAULT_ENTRYPOINT
+        return self._entrypoint
 
     @entrypoint.setter
     def entrypoint(self, entrypoint: str | None):
         assert self._entrypoint is self.__unset, "Immutable attribute `entrypoint`"
         assert entrypoint is None or isinstance(entrypoint, str), "Invalid type for attribute `entrypoint`"
         self._entrypoint = entrypoint
 
@@ -384,15 +384,15 @@
                 yield CheckletComplexType.PackageVersion(name=pv.name, version=pv.version)
 
     def _construct_node(self, *, args: BundleConstructionArguments) -> CheckletComplexType:
         return CheckletComplexType(
             name=self.name,
             extras=','.join(self.extras) if self.extras else None,
             version=self.version,
-            entrypoint=self.entrypoint if self.entrypoint != self.DEFAULT_ENTRYPOINT else None,
+            entrypoint=self.entrypoint if self.entrypoint != self._OLD_DEFAULT_ENTRYPOINT else None,
             repository=list(self._construct_repository_nodes(args=args)),
             link=list(self._construct_link_nodes(args=args)),
             index=list(),  # self._construct_index_nodes(args=args),
             package_version=list(self._construct_package_version_nodes(args=args)),
             resources=list(self._construct_resources_nodes(args=args)),
         )
```

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/content.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/content.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/files.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/files.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/meta.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/meta.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/options.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/options.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/properties.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/properties.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/refs.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/refs.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/resources.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/resources.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/result.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/result.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/results.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/results.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/steps.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/steps.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/elements/wildcard.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/elements/wildcard.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/exception.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/exception.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/mixins/attachments.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/mixins/attachments.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/mixins/id.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/mixins/id.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/mixins/name.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/mixins/name.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/config.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/config.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/handlers/lxml.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/handlers/lxml.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/handlers/xml.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/parsers/xml.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/parsers/xml.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/product.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/product.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/recipe.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/recipe.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/results.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/results.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/schema/momotor-1.0.xsd` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/schema/momotor-1.0.xsd`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/schema/xml.xsd` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/schema/xml.xsd`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/test.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/test.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/testresult.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/testresult.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/arguments.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/ascii.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/ascii.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/assertion.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/boolean.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/boolean.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/detect.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/detect.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/domain.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/domain.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/encoding.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/filters.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/filters.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/grouping.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/grouping.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/immutable.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/immutable.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/keyedtuple.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/keyedtuple.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/lxml.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/lxml.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/nodes.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/nodes.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/rglob.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/rglob.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/text.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/text.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/src/momotor/bundles/utils/zipwrapper.py` & `momotor-bundles-8.0.0rc8/src/momotor/bundles/utils/zipwrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,49 +18,57 @@
 
     :param path: The path to the zip file, or
     :param content: A :py:class:`bytes` or :py:class:`memoryview` containing the data of the zip file
     """
     path: pathlib.Path | None
     content: bytes | memoryview | None
     zip_file: zipfile.ZipFile | None
+    __nesting: int = 0
 
     def __init__(self, *, path: pathlib.Path | None = None, content: bytes | memoryview | None = None):
+        self.__init(path=path, content=content)
+
+    def __init(self, path: pathlib.Path | None, content: bytes | memoryview | None):
         self.path = path
         self.content = content
         self.zip_file = None
+        self.__nesting = 0
 
     def __enter__(self):
         if self.zip_file is None:
+            self.__nesting = 1
             self.zip_file = zipfile.ZipFile(self.path if self.path else BytesIO(self.content), 'r')
+        else:
+            self.__nesting += 1
 
         return self.zip_file
 
-    def __exit__(self, exc_type, exc_value, traceback):
-        pass
+    def __exit__(self, *args, **kwargs):
+        self.__nesting -= 1
+        if self.__nesting == 0:
+            self.close()
+
+    def __del__(self):
+        self.close()
 
     def close(self):
         """ Close the wrapped zip file """
         if self.zip_file:
             try:
                 self.zip_file.close()
             except OSError:
                 pass
-            self.zip_file = None
 
-    def __del__(self):
-        self.close()
+            self.__nesting = 0
+            self.zip_file = None
 
     def __getstate__(self):
-        if self.path:
+        if self.path is not None:
             return {'path': self.path}
-        else:
+        elif self.content is not None:
             return {'content': bytes(self.content)}
-
-    def __setstate__(self, state):
-        if 'path' in state:
-            self.path = state['path']
-            self.content = None
         else:
-            self.path = None
-            self.content = state['content']
+            return {}
 
-        self.zip_file = None
+    def __setstate__(self, state):
+        self.close()
+        self.__init(state.get('path'), state.get('content'))
```

### Comparing `momotor-bundles-8.0.0rc6/src/momotor_bundles.egg-info/PKG-INFO` & `momotor-bundles-8.0.0rc8/src/momotor_bundles.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momotor-bundles
-Version: 8.0.0rc6
+Version: 8.0.0rc8
 Summary: Momotor bundle reader, writer, tools
 Author-email: Erik Scheffers <e.t.j.scheffers@tue.nl>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://momotor.org
 Project-URL: Documentation, https://momotor.org/doc/engine/momotor-bundles/
 Project-URL: Repository, https://gitlab.tue.nl/momotor/engine-py3/momotor-bundles/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-bundles/issues
@@ -35,15 +35,15 @@
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints!=1.14.0; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: momotor-bundles[docs,lxml,test]; extra == "dev"
 Requires-Dist: xsdata[cli]==23.8.*; extra == "dev"
 Provides-Extra: build
-Requires-Dist: momotor-bundles[docs]; extra == "build"
+Requires-Dist: momotor-bundles[dev,docs]; extra == "build"
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: build[virtualenv]; extra == "build"
 Requires-Dist: python-semantic-release~=8.0; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 This package is a part of [Momotor](https://momotor.org/), a tool for automated processing of digital content.
```

### Comparing `momotor-bundles-8.0.0rc6/src/momotor_bundles.egg-info/SOURCES.txt` & `momotor-bundles-8.0.0rc8/src/momotor_bundles.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .gitignore
 .gitlab-ci.yml
 .xsdata.xml
 CHANGELOG.md
 LICENSE.txt
-MANIFEST.in
 README.md
 build.bat
 build.sh
 publish-docs.sh
 pyproject.toml
 semver.sh
 setup.py
```

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/files/content.xml` & `momotor-bundles-8.0.0rc8/tests/bundle/files/content.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/files/full-recipe/recipe.xml` & `momotor-bundles-8.0.0rc8/tests/bundle/files/full-recipe/recipe.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/files/huge_product.zip` & `momotor-bundles-8.0.0rc8/tests/bundle/files/huge_product.zip`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/files/meta/recipe-with-meta.xml` & `momotor-bundles-8.0.0rc8/tests/bundle/files/meta/recipe-with-meta.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/files/meta/recipe-with-multiple-meta.xml` & `momotor-bundles-8.0.0rc8/tests/bundle/files/meta/recipe-with-multiple-meta.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/files/resources.xml` & `momotor-bundles-8.0.0rc8/tests/bundle/files/resources.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/files/with-files/recipe.xml` & `momotor-bundles-8.0.0rc8/tests/bundle/files/with-files/recipe.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/files/with-files.zip` & `momotor-bundles-8.0.0rc8/tests/bundle/files/with-files.zip`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/files/with-repository.zip` & `momotor-bundles-8.0.0rc8/tests/bundle/files/with-repository.zip`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_checklets.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_checklets.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_content.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_content.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_detect.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_detect.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_files.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_files.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_hashes.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_hashes.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_meta.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_meta.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_read_bundle.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_read_bundle.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_repository.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_repository.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_resources.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_resources.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_result.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_result.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle/test_static.py` & `momotor-bundles-8.0.0rc8/tests/bundle/test_static.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/bundle_test_helpers.py` & `momotor-bundles-8.0.0rc8/tests/bundle_test_helpers.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/create/files/recipe/checklet/generate-score/setup.py` & `momotor-bundles-8.0.0rc8/tests/create/files/recipe/checklet/generate-score/setup.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/create/files/recipe/checklet/generate-score/src/generate_score/__init__.py` & `momotor-bundles-8.0.0rc8/tests/create/files/recipe/checklet/generate-score/src/generate_score/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/create/files/recipe/recipe.xml` & `momotor-bundles-8.0.0rc8/tests/create/files/recipe/recipe.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/create/test_attachments.py` & `momotor-bundles-8.0.0rc8/tests/create/test_attachments.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/create/test_bundle_creation.py` & `momotor-bundles-8.0.0rc8/tests/create/test_bundle_creation.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/create/test_xml_creation.py` & `momotor-bundles-8.0.0rc8/tests/create/test_xml_creation.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/fromio/files/valid_xslt.xml` & `momotor-bundles-8.0.0rc8/tests/fromio/files/valid_xslt.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/fromio/test_fromio.py` & `momotor-bundles-8.0.0rc8/tests/fromio/test_fromio.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/options/test_option_domains.py` & `momotor-bundles-8.0.0rc8/tests/options/test_option_domains.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/recreate/files/result1/result.xml` & `momotor-bundles-8.0.0rc8/tests/recreate/files/result1/result.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/recreate/files/result2/result.xml` & `momotor-bundles-8.0.0rc8/tests/recreate/files/result2/result.xml`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/recreate/test_result_recreate.py` & `momotor-bundles-8.0.0rc8/tests/recreate/test_result_recreate.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/utils/test_filters.py` & `momotor-bundles-8.0.0rc8/tests/utils/test_filters.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/utils/test_rglob.py` & `momotor-bundles-8.0.0rc8/tests/utils/test_rglob.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/utils/test_utils_encoding.py` & `momotor-bundles-8.0.0rc8/tests/utils/test_utils_encoding.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/utils/test_utils_keyedsequence.py` & `momotor-bundles-8.0.0rc8/tests/utils/test_utils_keyedsequence.py`

 * *Files identical despite different names*

### Comparing `momotor-bundles-8.0.0rc6/tests/warnings/test_warnings.py` & `momotor-bundles-8.0.0rc8/tests/warnings/test_warnings.py`

 * *Files identical despite different names*

