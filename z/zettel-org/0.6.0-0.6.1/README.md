# Comparing `tmp/zettel-org-0.6.0.tar.gz` & `tmp/zettel_org-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zettel-org-0.6.0.tar", last modified: Sun Mar 31 16:57:09 2024, max compression
+gzip compressed data, was "zettel_org-0.6.1.tar", last modified: Sun Apr 14 23:01:45 2024, max compression
```

## Comparing `zettel-org-0.6.0.tar` & `zettel_org-0.6.1.tar`

### file list

```diff
@@ -1,147 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.891691 zettel-org-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.875692 zettel-org-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.879691 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.879691 zettel-org-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-31 16:57:01.000000 zettel-org-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-31 16:57:01.000000 zettel-org-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-31 16:57:01.000000 zettel-org-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-03-31 16:57:01.000000 zettel-org-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-31 16:57:01.000000 zettel-org-0.6.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-31 16:57:01.000000 zettel-org-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10731 2024-03-31 16:57:09.891691 zettel-org-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-03-31 16:57:01.000000 zettel-org-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.879691 zettel-org-0.6.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2320 2024-03-31 16:57:01.000000 zettel-org-0.6.0/bin/build_zorg_grammars
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-03-31 16:57:01.000000 zettel-org-0.6.0/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-03-31 16:57:01.000000 zettel-org-0.6.0/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-03-31 16:57:01.000000 zettel-org-0.6.0/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-03-31 16:57:01.000000 zettel-org-0.6.0/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.879691 zettel-org-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.879691 zettel-org-0.6.0/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.879691 zettel-org-0.6.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.879691 zettel-org-0.6.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.879691 zettel-org-0.6.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-31 16:57:01.000000 zettel-org-0.6.0/docs/source/zorg.rst
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-31 16:57:01.000000 zettel-org-0.6.0/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.871692 zettel-org-0.6.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.883691 zettel-org-0.6.0/examples/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-31 16:57:01.000000 zettel-org-0.6.0/examples/zorg_file/20240323.zo
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-31 16:57:01.000000 zettel-org-0.6.0/examples/zorg_file/basic.zo
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-31 16:57:01.000000 zettel-org-0.6.0/examples/zorg_file/multiblocks.zo
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-31 16:57:01.000000 zettel-org-0.6.0/examples/zorg_file/priority.zo
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-31 16:57:01.000000 zettel-org-0.6.0/examples/zorg_file/property.zo
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-31 16:57:01.000000 zettel-org-0.6.0/examples/zorg_file/scrambled_prj_notes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-31 16:57:01.000000 zettel-org-0.6.0/examples/zorg_file/subnotes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-31 16:57:01.000000 zettel-org-0.6.0/examples/zorg_file/subsections.zo
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-31 16:57:01.000000 zettel-org-0.6.0/examples/zorg_file/tags.zo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.883691 zettel-org-0.6.0/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-03-31 16:57:01.000000 zettel-org-0.6.0/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-31 16:57:01.000000 zettel-org-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-31 16:57:01.000000 zettel-org-0.6.0/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-03-31 16:57:01.000000 zettel-org-0.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-31 16:57:01.000000 zettel-org-0.6.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-31 16:57:01.000000 zettel-org-0.6.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.883691 zettel-org-0.6.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-31 16:57:01.000000 zettel-org-0.6.0/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-31 16:57:09.891691 zettel-org-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-03-31 16:57:01.000000 zettel-org-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.871692 zettel-org-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.891691 zettel-org-0.6.0/src/zettel_org.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10731 2024-03-31 16:57:09.000000 zettel-org-0.6.0/src/zettel_org.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-31 16:57:09.000000 zettel-org-0.6.0/src/zettel_org.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 16:57:09.000000 zettel-org-0.6.0/src/zettel_org.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-31 16:57:09.000000 zettel-org-0.6.0/src/zettel_org.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 16:57:06.000000 zettel-org-0.6.0/src/zettel_org.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-31 16:57:09.000000 zettel-org-0.6.0/src/zettel_org.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-31 16:57:09.000000 zettel-org-0.6.0/src/zettel_org.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.887691 zettel-org-0.6.0/src/zorg/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/file_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.887691 zettel-org-0.6.0/src/zorg/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.887691 zettel-org-0.6.0/src/zorg/grammar/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFile.g4
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFile.interp
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFile.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFileLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFileListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   105089 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/grammar/zorg_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.887691 zettel-org-0.6.0/src/zorg/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/runners/_run_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/runners/_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/runners/_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/runners/_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/runners/_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/runners/_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/sql_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-31 16:57:01.000000 zettel-org-0.6.0/src/zorg/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-31 16:57:01.000000 zettel-org-0.6.0/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.891691 zettel-org-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.891691 zettel-org-0.6.0/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    65905 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/__snapshots__/test_run_compile.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/__snapshots__/test_run_edit.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/__snapshots__/test_run_template.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:57:09.891691 zettel-org-0.6.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/data/day_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/data/done_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/data/habit_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/data/hello.zot
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/data/links.zo
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/test_file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/test_run_action_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/test_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/test_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tests/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-31 16:57:01.000000 zettel-org-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.169851 zettel_org-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.149852 zettel_org-0.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.153852 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.153852 zettel_org-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 23:01:32.000000 zettel_org-0.6.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-14 23:01:32.000000 zettel_org-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-14 23:01:32.000000 zettel_org-0.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-14 23:01:32.000000 zettel_org-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-14 23:01:32.000000 zettel_org-0.6.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-14 23:01:32.000000 zettel_org-0.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-14 23:01:45.169851 zettel_org-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-14 23:01:32.000000 zettel_org-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.153852 zettel_org-0.6.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2662 2024-04-14 23:01:32.000000 zettel_org-0.6.1/bin/build_zorg_grammars
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-14 23:01:32.000000 zettel_org-0.6.1/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-14 23:01:32.000000 zettel_org-0.6.1/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-14 23:01:32.000000 zettel_org-0.6.1/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-04-14 23:01:32.000000 zettel_org-0.6.1/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.153852 zettel_org-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.153852 zettel_org-0.6.1/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.153852 zettel_org-0.6.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.153852 zettel_org-0.6.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.153852 zettel_org-0.6.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-14 23:01:32.000000 zettel_org-0.6.1/docs/source/zorg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 23:01:32.000000 zettel_org-0.6.1/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.145851 zettel_org-0.6.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.157852 zettel_org-0.6.1/examples/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-14 23:01:32.000000 zettel_org-0.6.1/examples/zorg_file/20240323.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-14 23:01:32.000000 zettel_org-0.6.1/examples/zorg_file/basic.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-14 23:01:32.000000 zettel_org-0.6.1/examples/zorg_file/multiblocks.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-14 23:01:32.000000 zettel_org-0.6.1/examples/zorg_file/priority.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-14 23:01:32.000000 zettel_org-0.6.1/examples/zorg_file/property.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-14 23:01:32.000000 zettel_org-0.6.1/examples/zorg_file/scrambled_prj_notes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-14 23:01:32.000000 zettel_org-0.6.1/examples/zorg_file/subnotes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-14 23:01:32.000000 zettel_org-0.6.1/examples/zorg_file/subsections.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 23:01:32.000000 zettel_org-0.6.1/examples/zorg_file/tags_and_ids.zo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.157852 zettel_org-0.6.1/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-14 23:01:32.000000 zettel_org-0.6.1/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-14 23:01:32.000000 zettel_org-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-14 23:01:32.000000 zettel_org-0.6.1/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-14 23:01:32.000000 zettel_org-0.6.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-14 23:01:32.000000 zettel_org-0.6.1/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-14 23:01:32.000000 zettel_org-0.6.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.157852 zettel_org-0.6.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 23:01:32.000000 zettel_org-0.6.1/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-14 23:01:45.169851 zettel_org-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-14 23:01:32.000000 zettel_org-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.145851 zettel_org-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.169851 zettel_org-0.6.1/src/zettel_org.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-14 23:01:45.000000 zettel_org-0.6.1/src/zettel_org.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-14 23:01:45.000000 zettel_org-0.6.1/src/zettel_org.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:01:45.000000 zettel_org-0.6.1/src/zettel_org.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 23:01:45.000000 zettel_org-0.6.1/src/zettel_org.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:01:41.000000 zettel_org-0.6.1/src/zettel_org.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-14 23:01:45.000000 zettel_org-0.6.1/src/zettel_org.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-14 23:01:45.000000 zettel_org-0.6.1/src/zettel_org.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.157852 zettel_org-0.6.1/src/zorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.157852 zettel_org-0.6.1/src/zorg/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.161852 zettel_org-0.6.1/src/zorg/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/runners/_run_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/runners/_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/runners/_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/runners/_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/runners/_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/app/runners/_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.161852 zettel_org-0.6.1/src/zorg/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.161852 zettel_org-0.6.1/src/zorg/domain/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/domain/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/domain/messages/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/domain/messages/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/domain/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.161852 zettel_org-0.6.1/src/zorg/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.161852 zettel_org-0.6.1/src/zorg/grammar/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFile.g4
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFile.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFile.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFileLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFileListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118898 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/grammar/zorg_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.165851 zettel_org-0.6.1/src/zorg/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/service/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/service/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/service/file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/service/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/service/messagebus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/service/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/service/zid_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.165851 zettel_org-0.6.1/src/zorg/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.165851 zettel_org-0.6.1/src/zorg/storage/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/file/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/file/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.165851 zettel_org-0.6.1/src/zorg/storage/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/sql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/sql/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/sql/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-14 23:01:32.000000 zettel_org-0.6.1/src/zorg/storage/sql/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-14 23:01:32.000000 zettel_org-0.6.1/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.165851 zettel_org-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.165851 zettel_org-0.6.1/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    70292 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/__snapshots__/test_run_compile.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/__snapshots__/test_run_db.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/__snapshots__/test_run_edit.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/__snapshots__/test_run_template.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:01:45.169851 zettel_org-0.6.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/data/day_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/data/done_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/data/habit_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/data/hello.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/data/links.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/test_file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/test_run_action_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/test_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/test_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/test_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tests/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-14 23:01:32.000000 zettel_org-0.6.1/tox.ini
```

### Comparing `zettel-org-0.6.0/.cruft.json` & `zettel_org-0.6.1/.cruft.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'9bf66fb22364c3bd192f79ca59ddfa59c7f02657'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "fa0499ecbf36aa3124fad11b92826161d5e424f0",
+    "commit": "9bf66fb22364c3bd192f79ca59ddfa59c7f02657",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/python-boltons/cc-python",
             "author": "Bryan M Bugyi",
             "email": "bryanbugyi34@gmail.com",
             "git_org_name": "bbugyi200",
             "git_repo_name": "zorg",
```

### Comparing `zettel-org-0.6.0/.github/labels.yml` & `zettel_org-0.6.1/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/.github/workflows/ci.yml` & `zettel_org-0.6.1/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,17 @@
           chmod +x ~/.docker/cli-plugins/docker-compose
 
       - name: Unit tests
         run: |
           make test
 
       - name: Publish coverage to codecov.io.
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v4
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
         if: ${{ !env.ACT }}
         with:
           fail_ci_if_error: true
           files: ./coverage.xml
           verbose: true
   lint:
     runs-on: [ubuntu-latest]
@@ -97,11 +99,11 @@
       - name: Build docs and publish them back to the master branch if necessary.
         if: github.repository == 'bbugyi200/zorg' && github.ref == 'refs/heads/master'
         run: |
           ./bin/publish_docs
 
       - name: Publish distribution to PyPI
         if: github.repository == 'bbugyi200/zorg' && startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           skip_existing: true
```

### Comparing `zettel-org-0.6.0/.gitignore` & `zettel_org-0.6.1/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -119,7 +119,10 @@
 *.rej
 
 # pyright config file
 pyrightconfig.json
 
 # local sqlite databases
 *.db
+
+# zorg data files live here
+.zorg/
```

### Comparing `zettel-org-0.6.0/.pylintrc` & `zettel_org-0.6.1/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -295,8 +295,8 @@
 int-import-graph=
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtin.Exception
```

### Comparing `zettel-org-0.6.0/.readthedocs.yml` & `zettel_org-0.6.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/CHANGELOG.md` & `zettel_org-0.6.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,27 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.6.0...HEAD)
+## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.6.1...HEAD)
 
 No notable changes have been made.
 
 
+## [0.6.1](https://github.com/bbugyi200/zorg/compare/0.6.0...0.6.1) - 2024-04-10
+
+### Added
+
+* Add `zorg db create` command that creates a sqlite database and updates all
+  `*.zo` files by adding ZIDs to the notes they contain.
+
+
 ## [0.6.0](https://github.com/bbugyi200/zorg/compare/0.5.1...0.6.0) - 2024-03-31
 
 ### Changed
 
 * *BREAKING CHANGE*: Stop injecting `one_day` template variable.
 * Several improvements to the grammar used by `zorg compile`.
 * A lot of changes were made to the grammar and application logic that powers
```

### Comparing `zettel-org-0.6.0/CONTRIBUTING.md` & `zettel_org-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/Dockerfile` & `zettel_org-0.6.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/Makefile` & `zettel_org-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/PKG-INFO` & `zettel_org-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.6.0
+Version: 0.6.1
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,21 +14,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: antlr4-python3-runtime~=4.13
-Requires-Dist: bolton-clack~=0.3.10
+Requires-Dist: bolton-clack~=0.3.12
 Requires-Dist: bolton-eris~=0.2.3
 Requires-Dist: bolton-logrus~=0.1.1
 Requires-Dist: bolton-typist~=0.2.0
 Requires-Dist: jinja2
-Requires-Dist: potoroo~=0.4.1
+Requires-Dist: potoroo~=0.6.0
 Requires-Dist: sqlmodel~=0.0.16
+Requires-Dist: tqdm~=4.66
 Requires-Dist: vimala~=0.2.0
 
 # zorg
 
 **The zettel note manager of the future.**
 
 _project status badges:_
@@ -86,15 +87,15 @@
 <!-- [[[[[kooky.cog
 import subprocess
 
 popen = subprocess.Popen(["zorg", "--help"], stdout=subprocess.PIPE)
 stdout, _ = popen.communicate()
 print("```", stdout.decode().strip(), "```", sep="\n")
 
-for cmd in ['action', 'action open', 'compile', 'db', 'db info', 'edit', 'template', 'template init', 'template render']:
+for cmd in ['action', 'action open', 'compile', 'db', 'db create', 'db reindex', 'edit', 'template', 'template init', 'template render']:
     popen = subprocess.Popen(["zorg"] + cmd.split() + ["--help"], stdout=subprocess.PIPE)
     stdout, _ = popen.communicate()
     print(f"\n### `zorg {cmd} --help`\n")
     print("```", stdout.decode().strip(), "```", sep="\n")
 ]]]]] -->
 ```
 usage: zorg [-h] [-c CONFIG_FILE] [-L [FILE[:LEVEL][@FORMAT]]] [-v]
@@ -183,32 +184,48 @@
 options:
   -h, --help  show this help message and exit
 ```
 
 ### `zorg db --help`
 
 ```
-usage: zorg db [-h] {info} ...
+usage: zorg db [-h] {create,reindex} ...
 
 Commands for managing Zorg's SQL database.
 
 options:
-  -h, --help  show this help message and exit
+  -h, --help        show this help message and exit
 
 subcommands:
-  {info}
-    info      Display some useful stats related to your Zorg notes and todos.
+  {create,reindex}
+    create          Create zorg's backend database from scratch.
+    reindex         Reindex any changed files by adding them to the database.
+```
+
+### `zorg db create --help`
+
 ```
+usage: zorg db create [-h]
 
-### `zorg db info --help`
+Create zorg's backend database from scratch.
 
+options:
+  -h, --help  show this help message and exit
 ```
-usage: zorg db info [-h]
 
-Display some useful stats related to your Zorg notes and todos.
+### `zorg db reindex --help`
+
+```
+usage: zorg db reindex [-h] [paths ...]
+
+Reindex any changed files by adding them to the database.
+
+positional arguments:
+  paths       Reindex these specific paths. If this argument is not provided,
+              we use a hashing approach to check which files have changed.
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ### `zorg edit --help`
```

### Comparing `zettel-org-0.6.0/README.md` & `zettel_org-0.6.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 <!-- [[[[[kooky.cog
 import subprocess
 
 popen = subprocess.Popen(["zorg", "--help"], stdout=subprocess.PIPE)
 stdout, _ = popen.communicate()
 print("```", stdout.decode().strip(), "```", sep="\n")
 
-for cmd in ['action', 'action open', 'compile', 'db', 'db info', 'edit', 'template', 'template init', 'template render']:
+for cmd in ['action', 'action open', 'compile', 'db', 'db create', 'db reindex', 'edit', 'template', 'template init', 'template render']:
     popen = subprocess.Popen(["zorg"] + cmd.split() + ["--help"], stdout=subprocess.PIPE)
     stdout, _ = popen.communicate()
     print(f"\n### `zorg {cmd} --help`\n")
     print("```", stdout.decode().strip(), "```", sep="\n")
 ]]]]] -->
 ```
 usage: zorg [-h] [-c CONFIG_FILE] [-L [FILE[:LEVEL][@FORMAT]]] [-v]
@@ -154,32 +154,48 @@
 options:
   -h, --help  show this help message and exit
 ```
 
 ### `zorg db --help`
 
 ```
-usage: zorg db [-h] {info} ...
+usage: zorg db [-h] {create,reindex} ...
 
 Commands for managing Zorg's SQL database.
 
 options:
-  -h, --help  show this help message and exit
+  -h, --help        show this help message and exit
 
 subcommands:
-  {info}
-    info      Display some useful stats related to your Zorg notes and todos.
+  {create,reindex}
+    create          Create zorg's backend database from scratch.
+    reindex         Reindex any changed files by adding them to the database.
+```
+
+### `zorg db create --help`
+
 ```
+usage: zorg db create [-h]
 
-### `zorg db info --help`
+Create zorg's backend database from scratch.
 
+options:
+  -h, --help  show this help message and exit
 ```
-usage: zorg db info [-h]
 
-Display some useful stats related to your Zorg notes and todos.
+### `zorg db reindex --help`
+
+```
+usage: zorg db reindex [-h] [paths ...]
+
+Reindex any changed files by adding them to the database.
+
+positional arguments:
+  paths       Reindex these specific paths. If this argument is not provided,
+              we use a hashing approach to check which files have changed.
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ### `zorg edit --help`
```

### Comparing `zettel-org-0.6.0/bin/build_zorg_grammars` & `zettel_org-0.6.1/bin/build_zorg_grammars`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 # 1) Uses ANTLR to generate Python modules (e.g. parsers, lexers,
 #    listeners) from FOOBAR.g4 files.
 #
 # 2) Iterates over and attempts to parse all FOOBAR example files.
 #
 # Usage
 # -----
-# build_zorg_grammars [-v]
+# build_zorg_grammars [-v] [ZO_NAME]
+#
+# Positional Arguments:
+# ---------------------
+# ZO_NAME
+#     The name of a *.zo file without the extension or parent dir. If provided,
+#     will only parse example files that match ZO_NAME.
 #
 # Optional Arguments
 # ------------------
 #     -v | --verbose
 #         Enable more verbose output (e.g. print tokens).
 
 readonly BIN="$(dirname "$0")"
@@ -35,23 +41,31 @@
   if [[ "$1" == "-v" || "$1" == "--verbose" ]]; then
     shift
     VERBOSE=1
     parse_cmds+=('-tokens')
     log::debug "Verbose mode enabled!"
   fi
 
+  if [[ -n "${1}" ]]; then
+      ZO_NAME="$1"
+      shift
+  fi
+
   for dir in $(find src/zorg/grammar -maxdepth 1 -mindepth 1 -type d | xargs -I_ basename _); do
     if [[ "${dir}" == "_"* ]]; then
       log::debug "Skipping the %s directory." "${dir}"
       continue
     fi
 
     log::info "Generating %s parser using antlr4." $dir
     antlr4 -Dlanguage=Python3 src/zorg/grammar/$dir/*.g4
     for f in examples/$dir/*.zo; do
+      if [[ "${f}" != *"${ZO_NAME}"* ]]; then
+        continue
+      fi
       log::info "Contructing syntax tree from %s example file." $f
       echo "##### $f" >> $TMP_ERROR_FILE
       antlr4-parse src/zorg/grammar/$dir/*.g4 prog "${parse_cmds[@]}" $f 3>&1 1>&2 2>&3 | tee /dev/stderr >> $TMP_ERROR_FILE
       echo >> $TMP_ERROR_FILE
     done
 
     remove_header $TMP_ERROR_FILE > $TMP_ERROR_FILE_NO_HEADERS
```

### Comparing `zettel-org-0.6.0/bin/check_cc` & `zettel_org-0.6.1/bin/check_cc`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/bin/publish_docs` & `zettel_org-0.6.1/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/bin/quick-lints` & `zettel_org-0.6.1/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/bin/render_all_cogs` & `zettel_org-0.6.1/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/docs/Makefile` & `zettel_org-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/docs/make.bat` & `zettel_org-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/docs/source/conf.py` & `zettel_org-0.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/examples/zorg_file/20240323.zo` & `zettel_org-0.6.1/examples/zorg_file/20240323.zo`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/examples/zorg_file/scrambled_prj_notes.zo` & `zettel_org-0.6.1/examples/zorg_file/scrambled_prj_notes.zo`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/lib/bugyi.sh` & `zettel_org-0.6.1/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/requirements-dev.in` & `zettel_org-0.6.1/requirements-dev.in`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 cogapp ~= 3.3
 flake8
 isort
 mypy
 pydocstyle[toml]
 pylint
 
+### Types
+types-tqdm ~= 4.66
+
 ### Docs
 m2r2 != 0.3.3  # since this version requires docutils>=0.19 (see https://github.com/CrossNox/m2r2/compare/v0.3.2...v0.3.3)
 sphinx
 sphinx-rtd-theme
 sphinx-autodoc-typehints
 
 ### Misc
```

### Comparing `zettel-org-0.6.0/requirements-dev.txt` & `zettel_org-0.6.1/requirements-dev.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     # via cookiecutter
 astroid==3.1.0
     # via pylint
 babel==2.14.0
     # via sphinx
 binaryornot==0.4.4
     # via cookiecutter
-black==24.3.0
+black==24.4.0
     # via -r requirements-dev.in
-bolton-clack==0.3.10
+bolton-clack==0.3.12
     # via
     #   -r requirements.in
     #   zettel-org
 bolton-eris==0.2.3
     # via
     #   -r requirements.in
     #   bolton-clack
@@ -69,15 +69,15 @@
     # via requests
 click==8.1.7
     # via
     #   black
     #   cookiecutter
     #   cruft
     #   pip-tools
-    #   typer-slim
+    #   typer
 cogapp==3.4.1
     # via -r requirements-dev.in
 cookiecutter==2.6.0
     # via cruft
 coverage[toml]==7.4.4
     # via pytest-cov
 cruft[pyproject]==2.15.0
@@ -89,29 +89,29 @@
 docutils==0.20.1
     # via
     #   m2r2
     #   sphinx
     #   sphinx-rtd-theme
 exceptiongroup==1.2.0
     # via pytest
-filelock==3.13.3
+filelock==3.13.4
     # via
     #   tox
     #   virtualenv
 flake8==7.0.0
     # via -r requirements-dev.in
 freezegun==1.4.0
     # via -r requirements-dev.in
 gitdb==4.0.11
     # via gitpython
 gitpython==3.1.43
     # via cruft
 greenlet==3.0.3
     # via sqlalchemy
-idna==3.6
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
 install-jdk==1.1.0
     # via antlr4-tools
@@ -162,28 +162,28 @@
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.4.0
     # via
     #   pytest
     #   tox
-potoroo==0.4.1
+potoroo==0.6.0
     # via
     #   -r requirements.in
     #   zettel-org
 py==1.11.0
     # via tox
 pycodestyle==2.11.1
     # via flake8
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   bolton-clack
     #   pydantic-settings
     #   sqlmodel
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via bolton-clack
 pydocstyle[toml]==6.3.0
     # via -r requirements-dev.in
 pyflakes==3.2.0
     # via flake8
@@ -222,19 +222,19 @@
 requests==2.31.0
     # via
     #   cookiecutter
     #   sphinx
 rich==13.7.1
     # via
     #   cookiecutter
-    #   typer-slim
+    #   typer
 setuptools-scm==8.0.4
     # via -r requirements-dev.in
 shellingham==1.5.4
-    # via typer-slim
+    # via typer
 six==1.16.0
     # via
     #   python-dateutil
     #   tox
 smmap==5.0.1
     # via gitdb
 snowballstemmer==2.2.0
@@ -243,15 +243,15 @@
     #   sphinx
 sphinx==7.2.6
     # via
     #   -r requirements-dev.in
     #   sphinx-autodoc-typehints
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.0.1
     # via -r requirements-dev.in
 sphinx-rtd-theme==2.0.0
     # via -r requirements-dev.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
@@ -296,45 +296,45 @@
     # via pylint
 tox==3.28.0
     # via
     #   -r requirements-dev.in
     #   tox-pyenv
 tox-pyenv==1.1.0
     # via -r requirements-dev.in
-typer==0.12.0
-    # via cruft
-typer-cli==0.12.0
-    # via typer
-typer-slim[standard]==0.12.0
+tqdm==4.66.2
     # via
-    #   typer
-    #   typer-cli
+    #   -r requirements.in
+    #   zettel-org
+typer==0.12.3
+    # via cruft
 types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.10.0
+types-tqdm==4.66.0.20240106
+    # via -r requirements-dev.in
+typing-extensions==4.11.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pydantic-core
     #   setuptools-scm
     #   sqlalchemy
-    #   typer-slim
+    #   typer
 urllib3==2.2.1
     # via requests
 vimala==0.2.0
     # via
     #   -r requirements.in
     #   zettel-org
 virtualenv==20.25.1
     # via tox
 wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0
     # via pip-tools
-setuptools==69.2.0
+setuptools==69.5.1
     # via
     #   pip-tools
     #   setuptools-scm
```

### Comparing `zettel-org-0.6.0/requirements.txt` & `zettel_org-0.6.1/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    "make update-requirements"
 #
 annotated-types==0.6.0
     # via pydantic
 antlr4-python3-runtime==4.13.1
     # via -r requirements.in
-bolton-clack==0.3.10
+bolton-clack==0.3.12
     # via -r requirements.in
 bolton-eris==0.2.3
     # via
     #   -r requirements.in
     #   bolton-clack
     #   bolton-proctor
     #   potoroo
@@ -36,35 +36,37 @@
     #   vimala
 greenlet==3.0.3
     # via sqlalchemy
 jinja2==3.1.3
     # via -r requirements.in
 markupsafe==2.1.5
     # via jinja2
-potoroo==0.4.1
+potoroo==0.6.0
     # via -r requirements.in
-pydantic==2.6.4
+pydantic==2.7.0
     # via
     #   bolton-clack
     #   pydantic-settings
     #   sqlmodel
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pydantic-settings==2.2.1
     # via bolton-clack
 python-dotenv==1.0.1
     # via pydantic-settings
 pyyaml==6.0.1
     # via bolton-clack
 sqlalchemy==2.0.29
     # via sqlmodel
 sqlmodel==0.0.16
     # via -r requirements.in
 structlog==24.1.0
     # via bolton-logrus
-typing-extensions==4.10.0
+tqdm==4.66.2
+    # via -r requirements.in
+typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
     #   sqlalchemy
 vimala==0.2.0
     # via -r requirements.in
```

### Comparing `zettel-org-0.6.0/setup.cfg` & `zettel_org-0.6.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 show_error_context = True
 warn_redundant_casts = True
 warn_return_any = True
 warn_unreachable = True
 warn_unused_configs = True
 warn_unused_ignores = True
 
-[mypy-zorg.compiler]
+[mypy-zorg.service.compiler]
 disallow_untyped_calls = False
 
 [mypy-zorg.grammar.*]
 follow_imports = silent
 
 [mypy-antlr4.*,pluggy.*,setuptools.*]
 ignore_missing_imports = True
```

### Comparing `zettel-org-0.6.0/setup.py` & `zettel_org-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DESCRIPTION = "The zettel note manager of the future."
 SUPPORTED_PYTHON_VERSIONS = [
     (3, 9),
     (3, 10),
     (3, 11),
     (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.6.0"}
+USE_SCM_VERSION = {"fallback_version": "0.6.1"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
@@ -90,15 +90,15 @@
     + [
         f"Programming Language :: Python :: {pretty_pyver}"
         for pretty_pyver in PRETTY_PYTHON_VERSIONS
     ],
     description=DESCRIPTION,
     entry_points={
         "console_scripts": [
-            "zorg = zorg.__main__:main",
+            "zorg = zorg.app.__main__:main",
         ]
     },
     include_package_data=True,
     install_requires=install_requires(),
     license="MIT license",
     long_description=long_description(),
     long_description_content_type="text/markdown",
```

### Comparing `zettel-org-0.6.0/src/zettel_org.egg-info/PKG-INFO` & `zettel_org-0.6.1/src/zettel_org.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.6.0
+Version: 0.6.1
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,21 +14,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: antlr4-python3-runtime~=4.13
-Requires-Dist: bolton-clack~=0.3.10
+Requires-Dist: bolton-clack~=0.3.12
 Requires-Dist: bolton-eris~=0.2.3
 Requires-Dist: bolton-logrus~=0.1.1
 Requires-Dist: bolton-typist~=0.2.0
 Requires-Dist: jinja2
-Requires-Dist: potoroo~=0.4.1
+Requires-Dist: potoroo~=0.6.0
 Requires-Dist: sqlmodel~=0.0.16
+Requires-Dist: tqdm~=4.66
 Requires-Dist: vimala~=0.2.0
 
 # zorg
 
 **The zettel note manager of the future.**
 
 _project status badges:_
@@ -86,15 +87,15 @@
 <!-- [[[[[kooky.cog
 import subprocess
 
 popen = subprocess.Popen(["zorg", "--help"], stdout=subprocess.PIPE)
 stdout, _ = popen.communicate()
 print("```", stdout.decode().strip(), "```", sep="\n")
 
-for cmd in ['action', 'action open', 'compile', 'db', 'db info', 'edit', 'template', 'template init', 'template render']:
+for cmd in ['action', 'action open', 'compile', 'db', 'db create', 'db reindex', 'edit', 'template', 'template init', 'template render']:
     popen = subprocess.Popen(["zorg"] + cmd.split() + ["--help"], stdout=subprocess.PIPE)
     stdout, _ = popen.communicate()
     print(f"\n### `zorg {cmd} --help`\n")
     print("```", stdout.decode().strip(), "```", sep="\n")
 ]]]]] -->
 ```
 usage: zorg [-h] [-c CONFIG_FILE] [-L [FILE[:LEVEL][@FORMAT]]] [-v]
@@ -183,32 +184,48 @@
 options:
   -h, --help  show this help message and exit
 ```
 
 ### `zorg db --help`
 
 ```
-usage: zorg db [-h] {info} ...
+usage: zorg db [-h] {create,reindex} ...
 
 Commands for managing Zorg's SQL database.
 
 options:
-  -h, --help  show this help message and exit
+  -h, --help        show this help message and exit
 
 subcommands:
-  {info}
-    info      Display some useful stats related to your Zorg notes and todos.
+  {create,reindex}
+    create          Create zorg's backend database from scratch.
+    reindex         Reindex any changed files by adding them to the database.
+```
+
+### `zorg db create --help`
+
 ```
+usage: zorg db create [-h]
 
-### `zorg db info --help`
+Create zorg's backend database from scratch.
 
+options:
+  -h, --help  show this help message and exit
 ```
-usage: zorg db info [-h]
 
-Display some useful stats related to your Zorg notes and todos.
+### `zorg db reindex --help`
+
+```
+usage: zorg db reindex [-h] [paths ...]
+
+Reindex any changed files by adding them to the database.
+
+positional arguments:
+  paths       Reindex these specific paths. If this argument is not provided,
+              we use a hashing approach to check which files have changed.
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ### `zorg edit --help`
```

### Comparing `zettel-org-0.6.0/src/zettel_org.egg-info/SOURCES.txt` & `zettel_org-0.6.1/src/zettel_org.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -59,65 +59,82 @@
 examples/zorg_file/basic.zo
 examples/zorg_file/multiblocks.zo
 examples/zorg_file/priority.zo
 examples/zorg_file/property.zo
 examples/zorg_file/scrambled_prj_notes.zo
 examples/zorg_file/subnotes.zo
 examples/zorg_file/subsections.zo
-examples/zorg_file/tags.zo
+examples/zorg_file/tags_and_ids.zo
 lib/bugyi.sh
 scripts/README.md
 src/zettel_org.egg-info/PKG-INFO
 src/zettel_org.egg-info/SOURCES.txt
 src/zettel_org.egg-info/dependency_links.txt
 src/zettel_org.egg-info/entry_points.txt
 src/zettel_org.egg-info/not-zip-safe
 src/zettel_org.egg-info/requires.txt
 src/zettel_org.egg-info/top_level.txt
 src/zorg/__init__.py
-src/zorg/__main__.py
-src/zorg/common.py
-src/zorg/compiler.py
-src/zorg/config.py
-src/zorg/db.py
-src/zorg/file_groups.py
-src/zorg/models.py
 src/zorg/py.typed
-src/zorg/repo.py
-src/zorg/session.py
-src/zorg/sql_models.py
-src/zorg/templates.py
-src/zorg/types.py
+src/zorg/app/__init__.py
+src/zorg/app/__main__.py
+src/zorg/app/config.py
+src/zorg/app/runners/__init__.py
+src/zorg/app/runners/_run_action.py
+src/zorg/app/runners/_run_compile.py
+src/zorg/app/runners/_run_db.py
+src/zorg/app/runners/_run_edit.py
+src/zorg/app/runners/_run_template.py
+src/zorg/app/runners/_runners.py
+src/zorg/domain/__init__.py
+src/zorg/domain/models.py
+src/zorg/domain/types.py
+src/zorg/domain/messages/__init__.py
+src/zorg/domain/messages/commands.py
+src/zorg/domain/messages/events.py
 src/zorg/grammar/__init__.py
 src/zorg/grammar/zorg_file/ZorgFile.g4
 src/zorg/grammar/zorg_file/ZorgFile.interp
 src/zorg/grammar/zorg_file/ZorgFile.tokens
 src/zorg/grammar/zorg_file/ZorgFileLexer.interp
 src/zorg/grammar/zorg_file/ZorgFileLexer.py
 src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
 src/zorg/grammar/zorg_file/ZorgFileListener.py
 src/zorg/grammar/zorg_file/ZorgFileParser.py
 src/zorg/grammar/zorg_file/__init__.py
-src/zorg/runners/__init__.py
-src/zorg/runners/_run_action.py
-src/zorg/runners/_run_compile.py
-src/zorg/runners/_run_db.py
-src/zorg/runners/_run_edit.py
-src/zorg/runners/_run_template.py
-src/zorg/runners/_runners.py
+src/zorg/service/__init__.py
+src/zorg/service/common.py
+src/zorg/service/compiler.py
+src/zorg/service/file_groups.py
+src/zorg/service/handlers.py
+src/zorg/service/messagebus.py
+src/zorg/service/templates.py
+src/zorg/service/zid_manager.py
+src/zorg/storage/__init__.py
+src/zorg/storage/file/__init__.py
+src/zorg/storage/file/repo.py
+src/zorg/storage/file/session.py
+src/zorg/storage/sql/__init__.py
+src/zorg/storage/sql/converters.py
+src/zorg/storage/sql/engine.py
+src/zorg/storage/sql/models.py
+src/zorg/storage/sql/repo.py
+src/zorg/storage/sql/session.py
 tests/__init__.py
 tests/common.py
 tests/conftest.py
 tests/test_config.py
 tests/test_file_groups.py
 tests/test_run_action_open.py
 tests/test_run_compile.py
+tests/test_run_db.py
 tests/test_run_edit.py
 tests/test_run_template.py
 tests/__snapshots__/test_run_compile.ambr
+tests/__snapshots__/test_run_db.ambr
 tests/__snapshots__/test_run_edit.ambr
 tests/__snapshots__/test_run_template.ambr
 tests/data/day_log.zot
 tests/data/done_log.zot
 tests/data/habit_log.zot
 tests/data/hello.zot
 tests/data/links.zo
```

### Comparing `zettel-org-0.6.0/src/zorg/common.py` & `zettel_org-0.6.1/src/zorg/service/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime as dt
 from pathlib import Path
 import re
 from typing import Any, Iterable
 
 from typist import PathLike
 
-from .types import VarMapType
+from ..domain.types import VarMapType
 
 
 def process_var_map(var_map: VarMapType) -> dict[str, Any]:
     """Processes and potentially adds to {var_map}."""
     new_var_map = {}
     for k, v in var_map.items():
         new_var_map[k] = _var_map_value(v)
```

### Comparing `zettel-org-0.6.0/src/zorg/compiler.py` & `zettel_org-0.6.1/src/zorg/service/compiler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,60 @@
-"""Contains the ZorgFileCompiler class."""
+"""Contains service logic used to compile zorg files."""
 
 from dataclasses import dataclass, field
 import datetime as dt
+from functools import partial
+from pathlib import Path
 from typing import Any, Literal, Optional
 
 import antlr4
+from antlr4.error.ErrorListener import ErrorListener
 from logrus import Logger
+from typist import assert_never
 
-from .grammar.zorg_file.ZorgFileListener import ZorgFileListener
-from .grammar.zorg_file.ZorgFileParser import ZorgFileParser
-from .models import ZorgFile, ZorgNote, ZorgTodo
-from .types import TodoPriorityType
+from ..domain.models import TodoPayload, ZorgFile, ZorgNote
+from ..domain.types import TodoPriorityType, TodoStatus, TodoStatusPrefixChar
+from ..grammar.zorg_file.ZorgFileLexer import ZorgFileLexer
+from ..grammar.zorg_file.ZorgFileListener import ZorgFileListener
+from ..grammar.zorg_file.ZorgFileParser import ZorgFileParser
 
 
 TagName = Literal["areas", "contexts", "people", "projects"]
 
 logger = Logger(__name__)
 
 
-class ZorgFileCompiler(ZorgFileListener):
+class _ErrorManager(ErrorListener):
+    """Keeps track of zorg file syntax errors."""
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.errors: list[str] = []
+
+    def syntaxError(
+        self,
+        recognizer: Any,
+        offendingSymbol: str,
+        line: int,
+        column: int,
+        msg: str,
+        e: Any,
+    ) -> None:  # noqa: D102
+        del recognizer, offendingSymbol, e
+        self.errors.append(f"Line {line}:{column} {msg}")
+
+
+class _ZorgFileCompiler(ZorgFileListener):
     """Listener that compiles zorg files into zorc files."""
 
-    def __init__(self, zorg_file: ZorgFile) -> None:
+    def __init__(
+        self, zorg_file: ZorgFile, error_manager: _ErrorManager
+    ) -> None:
         self.zorg_file = zorg_file
+        self.error_manager = error_manager
 
         self._s = _ZorgFileCompilerState()
 
     def enterArea(self, ctx: ZorgFileParser.AreaContext) -> None:  # noqa: D102
         self._add_tags(ctx, "areas")
 
     def enterBase_note(
@@ -37,18 +65,33 @@
 
     def enterContext(
         self, ctx: ZorgFileParser.ContextContext
     ) -> None:  # noqa: D102
         self._add_tags(ctx, "contexts")
 
     def enterDate(self, ctx: ZorgFileParser.DateContext) -> None:  # noqa: D102
-        if self._s.in_note and self._s.ids_in_note == 1:
-            self._s.note_date = dt.datetime.strptime(
-                ctx.DATE().getText(), "%Y-%m-%d"
-            )
+        get_date = partial(
+            dt.datetime.strptime, ctx.DATE().getText(), "%Y-%m-%d"
+        )
+        if (
+            self._s.in_note
+            and self._s.ids_in_note == 1
+            and self._s.note_date is None
+        ):
+            self._s.note_date = get_date()
+        elif self._s.in_h4_header:
+            self._s.h4_date = get_date()
+        elif self._s.in_h3_header:
+            self._s.h3_date = get_date()
+        elif self._s.in_h2_header:
+            self._s.h2_date = get_date()
+        elif self._s.in_h1_header:
+            self._s.h1_date = get_date()
+        elif self._s.in_first_comment:
+            self._s.file_date = get_date()
 
     def enterH1_header(
         self, ctx: ZorgFileParser.H1_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h1_header = True
 
@@ -66,14 +109,18 @@
 
     def enterH4_header(
         self, ctx: ZorgFileParser.H4_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h4_header = True
 
+    def enterHead(self, ctx: ZorgFileParser.HeadContext) -> None:  # noqa: D102
+        del ctx
+        self._s.in_head = True
+
     def enterId(self, ctx: ZorgFileParser.IdContext) -> None:  # noqa: D102
         del ctx
         if self._s.in_note:
             self._s.ids_in_note += 1
 
     def enterItem(self, ctx: ZorgFileParser.ItemContext) -> None:  # noqa: D102
         del ctx
@@ -97,30 +144,32 @@
         self, ctx: ZorgFileParser.ProjectContext
     ) -> None:  # noqa: D102
         self._add_tags(ctx, "projects")
 
     def enterPriority(
         self, ctx: ZorgFileParser.PriorityContext
     ) -> None:  # noqa: D102
-        self._s.priority = ctx.ID().getText()[0].upper()
+        self._s.todo_priority = ctx.ID().getText()[0].upper()
 
     def enterProperty(
         self, ctx: ZorgFileParser.PropertyContext
     ) -> None:  # noqa: D102
         key, value = ctx.ID().getText(), ctx.id_group().getText()
-        if self._s.in_h1_header:
-            self._s.h1_properties[key] = value
+        if self._s.in_head:
+            self._s.file_props[key] = value
+        elif self._s.in_h1_header:
+            self._s.h1_props[key] = value
         elif self._s.in_h2_header:
-            self._s.h2_properties[key] = value
+            self._s.h2_props[key] = value
         elif self._s.in_h3_header:
-            self._s.h3_properties[key] = value
+            self._s.h3_props[key] = value
         elif self._s.in_h4_header:
-            self._s.h4_properties[key] = value
+            self._s.h4_props[key] = value
         elif self._s.in_note:
-            self._s.note_properties[key] = value
+            self._s.note_props[key] = value
 
     def enterSubnote(
         self, ctx: ZorgFileParser.SubnoteContext
     ) -> None:  # noqa: D102
         del ctx
         if not self._s.in_subnote:
             self._s.parent_id = self._s.next_id - 1
@@ -137,91 +186,163 @@
         self._reset_note_context()
 
     def enterTodo(self, ctx: ZorgFileParser.TodoContext) -> None:  # noqa: D102
         self._s.in_note = True
         self._s.parent_id = None
         del ctx
 
+    def enterTodo_prefix(
+        self, ctx: ZorgFileParser.Todo_prefixContext
+    ) -> None:  # noqa: D102
+        status = TodoStatus.OPEN
+        if self._s.in_note:
+            ch: TodoStatusPrefixChar = ctx.getText()[0]
+            if ch == "o":
+                status = TodoStatus.OPEN
+            elif ch == "x":
+                status = TodoStatus.CLOSED
+            elif ch == "~":
+                status = TodoStatus.CANCELED
+            elif ch == "<":
+                status = TodoStatus.BLOCKED
+            elif ch == ">":
+                status = TodoStatus.PARENT
+            else:
+                assert_never(ch)
+
+            self._s.todo_status = status
+
+    def enterZid(self, ctx: ZorgFileParser.ZidContext) -> None:  # noqa: D102
+        zid = ctx.getText()
+        self._s.zid = zid
+        zorg_id_date = f"20{zid.split('#')[0]}"
+        self._s.note_date = dt.datetime.strptime(zorg_id_date, "%Y%m%d")
+
     def exitBase_todo(
         self, ctx: ZorgFileParser.Base_todoContext
     ) -> None:  # noqa: D102
         self._s.in_note = False
-        kwargs = self._get_note_kwargs({"priority": self._s.priority})
-        todo = ZorgTodo(ctx.item_body().getText(), **kwargs)
-        self.zorg_file.todos.append(todo)
-        # Reset priority back to default.
-        self._s.priority = "C"
+        kwargs = self._get_note_kwargs(
+            ctx,
+            {
+                "todo_payload": TodoPayload(
+                    priority=self._s.todo_priority, status=self._s.todo_status
+                ),
+            },
+        )
+        id_note_body = ctx.id_note_body()
+        if id_note_body is None:
+            logger.warning("Skipping todo with no note body")
+        elif id_note_body.getText().strip() == "":
+            logger.warning("Skipping todo with empty note body")
+        elif self.error_manager.errors:
+            logger.warning(
+                "Skipping note since zorg file has errors.",
+                file_path=str(self.zorg_file.path),
+            )
+            self.zorg_file.has_errors = True
+        else:
+            todo = ZorgNote(id_note_body.getText(), **kwargs)
+            self.zorg_file.notes.append(todo)
+
+        # Reset todo priority and status back to defaults.
+        self._s.todo_priority = "C"
+        self._s.todo_status = TodoStatus.OPEN
 
     def exitH1_header(
         self, ctx: ZorgFileParser.H1_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h1_header = False
 
     def exitH1_section(
         self, ctx: ZorgFileParser.H1_headerContext
     ) -> None:  # noqa: D102
         del ctx
-        self._s.h1_section_tags = _get_default_tags_map()
-        self._s.h1_properties = {}
+        self._s.h1_tags = _get_default_tags_map()
+        self._s.h1_date = None
+        self._s.h1_props = {}
 
     def exitH2_header(
         self, ctx: ZorgFileParser.H2_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h2_header = False
 
     def exitH2_section(
         self, ctx: ZorgFileParser.H2_headerContext
     ) -> None:  # noqa: D102
         del ctx
-        self._s.h2_section_tags = _get_default_tags_map()
-        self._s.h2_properties = {}
+        self._s.h2_tags = _get_default_tags_map()
+        self._s.h2_date = None
+        self._s.h2_props = {}
 
     def exitH3_header(
         self, ctx: ZorgFileParser.H3_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h3_header = False
 
     def exitH3_section(
         self, ctx: ZorgFileParser.H3_headerContext
     ) -> None:  # noqa: D102
         del ctx
-        self._s.h3_section_tags = _get_default_tags_map()
-        self._s.h3_properties = {}
+        self._s.h3_tags = _get_default_tags_map()
+        self._s.h3_date = None
+        self._s.h3_props = {}
 
     def exitH4_header(
         self, ctx: ZorgFileParser.H4_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h4_header = False
 
     def exitH4_section(
         self, ctx: ZorgFileParser.H4_headerContext
     ) -> None:  # noqa: D102
         del ctx
-        self._s.h4_section_tags = _get_default_tags_map()
-        self._s.h4_properties = {}
+        self._s.h4_tags = _get_default_tags_map()
+        self._s.h4_date = None
+        self._s.h4_props = {}
+
+    def exitHead(self, ctx: ZorgFileParser.HeadContext) -> None:  # noqa: D102
+        del ctx
+        self._s.in_head = False
 
     def exitComment(
         self, ctx: ZorgFileParser.CommentContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_first_comment = False
 
     def exitBase_note(
         self, ctx: ZorgFileParser.Base_noteContext
     ) -> None:  # noqa: D102
         self._s.in_note = False
         extra_kwargs = {}
         if self._s.parent_id is not None:
             extra_kwargs["parent_note_id"] = self._s.parent_id
-        kwargs = self._get_note_kwargs(extra_kwargs)
-        note = ZorgNote(ctx.item_body().getText(), **kwargs)
+        kwargs = self._get_note_kwargs(ctx, extra_kwargs)
+        body: str = ctx.id_note_body().getText().strip()
+        if body == "":
+            logger.warning(
+                "Skipping note with empty body",
+                file_path=str(self.zorg_file.path),
+            )
+            return
+
+        if self.error_manager.errors:
+            logger.warning(
+                "Skipping note since zorg file has errors.",
+                file_path=str(self.zorg_file.path),
+            )
+            self.zorg_file.has_errors = True
+            return
+
+        note = ZorgNote(body, **kwargs)
         self.zorg_file.notes.append(note)
 
     def exitItem(self, ctx: ZorgFileParser.ItemContext) -> None:  # noqa: D102
         del ctx
         self._s.in_subnote = False
 
     def exitSubnote(
@@ -232,36 +353,39 @@
 
     def exitSubsubnote(
         self, ctx: ZorgFileParser.SubsubnoteContext
     ) -> None:  # noqa: D102
         del ctx
 
     def _get_note_kwargs(
-        self, extra_kwargs: dict[str, Any] = None
+        self,
+        ctx: antlr4.ParserRuleContext,
+        extra_kwargs: dict[str, Any] = None,
     ) -> dict[str, Any]:
         if extra_kwargs is None:
             extra_kwargs = {}
         kwargs: dict[str, Any] = {
             "areas": self._s.areas,
             "contexts": self._s.contexts,
-            "ident": self._s.next_id,
+            "create_date": self._s.create_date,
+            "line_no": ctx.start.line,
             "links": self._s.note_links,
             "people": self._s.people,
             "projects": self._s.projects,
             "properties": self._s.properties,
+            "zid": self._s.zid,
         }
         self._s.next_id += 1
-        if self._s.note_date is not None:
-            kwargs["create_date"] = self._s.note_date
         return kwargs | extra_kwargs
 
     def _reset_note_context(self) -> None:
+        self._s.zid = None
         self._s.ids_in_note = 0
         self._s.note_tags = _get_default_tags_map()
-        self._s.note_properties = {}
+        self._s.note_props = {}
         self._s.note_links = []
         self._s.note_date = None
 
     def _add_tags(
         self, ctx: antlr4.ParserRuleContext, tag_name: TagName
     ) -> None:
         text = ctx.children[1].getText()
@@ -271,128 +395,159 @@
                 tag_name=tag_name,
                 ID=text,
             )
             return
         if self._s.in_first_comment:
             self._s.file_tags[tag_name].append(text)
         elif self._s.in_h1_header:
-            self._s.h1_section_tags[tag_name].append(text)
+            self._s.h1_tags[tag_name].append(text)
         elif self._s.in_h2_header:
-            self._s.h2_section_tags[tag_name].append(text)
+            self._s.h2_tags[tag_name].append(text)
         elif self._s.in_h3_header:
-            self._s.h3_section_tags[tag_name].append(text)
+            self._s.h3_tags[tag_name].append(text)
         elif self._s.in_h4_header:
-            self._s.h4_section_tags[tag_name].append(text)
+            self._s.h4_tags[tag_name].append(text)
         elif self._s.in_note:
             self._s.note_tags[tag_name].append(text)
 
 
+def walk_zorg_file(zo_path: Path, verbose: bool = False) -> ZorgFile:
+    """Create a new _ZorgFileCompiler and walk through notes in {zorg_file}."""
+    zorg_file = ZorgFile(zo_path)
+    stream = antlr4.FileStream(zorg_file.path, errors="ignore")
+    lexer = ZorgFileLexer(stream)
+    tokens = antlr4.CommonTokenStream(lexer)
+    parser = ZorgFileParser(tokens)
+    if not verbose:
+        parser.removeErrorListeners()
+    error_manager = _ErrorManager()
+    parser.addErrorListener(error_manager)
+    tree = parser.prog()
+    compiler = _ZorgFileCompiler(zorg_file, error_manager)
+    walker = antlr4.ParseTreeWalker()
+    walker.walk(compiler, tree)
+    return zorg_file
+
+
 def _get_default_tags_map() -> dict[TagName, list[str]]:
     return {"areas": [], "projects": [], "contexts": [], "people": []}
 
 
 @dataclass
 class _ZorgFileCompilerState:
     """Serves as a data store while parsing zorg files."""
 
+    zid: Optional[str] = None
+
     ids_in_note: int = 0
 
+    # TODO(bugyi): Figure out a better way to track parent/child relationship
     next_id: int = 1
     parent_id: Optional[int] = None
 
     in_first_comment: bool = True
+    in_head: bool = False
     in_h1_header: bool = False
     in_h2_header: bool = False
     in_h3_header: bool = False
     in_h4_header: bool = False
     in_note: bool = False
     in_subnote: bool = False
     in_subsubnote: bool = False
 
     file_tags: dict[TagName, list[str]] = field(
         default_factory=_get_default_tags_map
     )
-    h1_section_tags: dict[TagName, list[str]] = field(
+    h1_tags: dict[TagName, list[str]] = field(
         default_factory=_get_default_tags_map
     )
-    h2_section_tags: dict[TagName, list[str]] = field(
+    h2_tags: dict[TagName, list[str]] = field(
         default_factory=_get_default_tags_map
     )
-    h3_section_tags: dict[TagName, list[str]] = field(
+    h3_tags: dict[TagName, list[str]] = field(
         default_factory=_get_default_tags_map
     )
-    h4_section_tags: dict[TagName, list[str]] = field(
+    h4_tags: dict[TagName, list[str]] = field(
         default_factory=_get_default_tags_map
     )
     note_tags: dict[TagName, list[str]] = field(
         default_factory=_get_default_tags_map
     )
 
-    h1_properties: dict[str, Any] = field(default_factory=lambda: {})
-    h2_properties: dict[str, Any] = field(default_factory=lambda: {})
-    h3_properties: dict[str, Any] = field(default_factory=lambda: {})
-    h4_properties: dict[str, Any] = field(default_factory=lambda: {})
-    note_properties: dict[str, Any] = field(default_factory=lambda: {})
+    file_props: dict[str, Any] = field(default_factory=lambda: {})
+    h1_props: dict[str, Any] = field(default_factory=lambda: {})
+    h2_props: dict[str, Any] = field(default_factory=lambda: {})
+    h3_props: dict[str, Any] = field(default_factory=lambda: {})
+    h4_props: dict[str, Any] = field(default_factory=lambda: {})
+    note_props: dict[str, Any] = field(default_factory=lambda: {})
 
     note_links: list[str] = field(default_factory=lambda: [])
+
+    file_date: Optional[dt.date] = None
+    h1_date: Optional[dt.date] = None
+    h2_date: Optional[dt.date] = None
+    h3_date: Optional[dt.date] = None
+    h4_date: Optional[dt.date] = None
     note_date: Optional[dt.date] = None
 
-    priority: TodoPriorityType = "C"
+    todo_priority: TodoPriorityType = "C"
+    todo_status: TodoStatus = TodoStatus.OPEN
 
     @property
     def areas(self) -> list[str]:
         """Area tags that are currently in-scope."""
         return self._get_current_tags("areas")
 
     @property
     def contexts(self) -> list[str]:
         """Context tags that are currently in-scope."""
         return self._get_current_tags("contexts")
 
     @property
     def projects(self) -> list[str]:
         """Project tags that are currently in-scope."""
-        project: Optional[str] = None
-        for tag_map in [
-            self.file_tags,
-            self.h1_section_tags,
-            self.h2_section_tags,
-            self.h3_section_tags,
-            self.h4_section_tags,
-            self.note_tags,
-        ]:
-            project_list = tag_map["projects"]
-            if not project_list:
-                continue
-            inner_project = project_list[0]
-            if project is None:
-                project = inner_project
-            elif project != inner_project:
-                project = f"{project}/{inner_project}"
-
-        return [] if project is None else [project]
+        return self._get_current_tags("projects")
 
     @property
     def people(self) -> list[str]:
         """People tags that are currently in-scope."""
         return self._get_current_tags("people")
 
     @property
     def properties(self) -> dict[str, Any]:
         """Properties that are currently in-scope."""
         return (
-            self.h1_properties
-            | self.h2_properties
-            | self.h3_properties
-            | self.h4_properties
-            | self.note_properties
+            self.file_props
+            | self.h1_props
+            | self.h2_props
+            | self.h3_props
+            | self.h4_props
+            | self.note_props
         )
 
+    @property
+    def create_date(self) -> dt.date:
+        """Create date based on file header, sections, zorg IDs, etc...."""
+        if self.note_date:
+            return self.note_date
+        elif self.h4_date:
+            return self.h4_date
+        elif self.h3_date:
+            return self.h3_date
+        elif self.h2_date:
+            return self.h2_date
+        elif self.h1_date:
+            return self.h1_date
+        elif self.file_date:
+            return self.file_date
+        else:
+            return dt.date.today()
+
     def _get_current_tags(self, tag_name: TagName) -> list[str]:
         tags = []
         tags.extend(self.file_tags[tag_name])
-        tags.extend(self.h1_section_tags[tag_name])
-        tags.extend(self.h2_section_tags[tag_name])
-        tags.extend(self.h3_section_tags[tag_name])
-        tags.extend(self.h4_section_tags[tag_name])
+        tags.extend(self.h1_tags[tag_name])
+        tags.extend(self.h2_tags[tag_name])
+        tags.extend(self.h3_tags[tag_name])
+        tags.extend(self.h4_tags[tag_name])
         tags.extend(self.note_tags[tag_name])
-        return tags
+        return sorted(set(tags))
```

### Comparing `zettel-org-0.6.0/src/zorg/config.py` & `zettel_org-0.6.1/src/zorg/app/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 """Clack config for zorg."""
 
 from __future__ import annotations
 
 import itertools as it
 from pathlib import Path
-from typing import Any, Literal, Optional, Sequence
+from typing import Any, Final, Literal, Optional, Sequence
 
 import clack
 from logrus import Logger
 
-from . import common
-from .types import FileGroupMapType, TemplatePatternMapType, VarMapType
+from .. import APP_NAME
+from ..domain.types import FileGroupMapType, TemplatePatternMapType, VarMapType
+from ..service import common
 
 
-Command = Literal["compile", "edit", "info", "init", "open", "render"]
+Command = Literal[
+    "compile", "create", "edit", "init", "open", "reindex", "render"
+]
 
-logger = Logger(__name__)
+_logger = Logger(__name__)
+
+_DEFAULT_ZETTEL_DIR: Final[Path] = Path.home() / "org"
 
 
 class Config(clack.Config):
     """Shared clack configuration class."""
 
     command: Command
 
     # ----- ARGUMENTS
-    zettel_dir: Path = Path.home() / "org"
+    zettel_dir: Path = _DEFAULT_ZETTEL_DIR
 
     # ----- CONFIG
+    database_url: str = "sqlite:///" + str(
+        _DEFAULT_ZETTEL_DIR / f".zorg/{APP_NAME}.db"
+    )
     template_pattern_map: TemplatePatternMapType = {}
 
 
 class OpenActionConfig(Config):
     """Clack config for the 'action' command."""
 
     command: Literal["open"]
@@ -45,18 +53,27 @@
 
     command: Literal["compile"]
 
     # ----- ARGUMENTS
     zo_path: Path
 
 
-class DbInfoConfig(Config):
-    """Clack config for the 'db info' command."""
+class DbCreateConfig(Config):
+    """Clack config for the 'db create' command."""
+
+    command: Literal["create"]
+
+
+class DbReindexConfig(Config):
+    """Clack config for the 'db reindex' command."""
+
+    command: Literal["reindex"]
 
-    command: Literal["info"]
+    # ----- Arguments
+    paths: list[Path] = []
 
 
 class EditConfig(Config):
     """Clack config for the 'edit' command."""
 
     command: Literal["edit"]
 
@@ -91,22 +108,22 @@
 
 
 def clack_parser(argv: Sequence[str]) -> dict[str, Any]:
     """Parser we pass to the `main_factory()` `parser` kwarg."""
     # HACK: Make 'edit' the default sub-command.
     argv_after_opts = list(it.dropwhile(lambda x: x.startswith("-"), argv[1:]))
     if not argv_after_opts:
-        logger.debug(
+        _logger.debug(
             "Inferring 'edit' command since no subcommand was specified."
         )
         argv = list(argv) + ["edit"]
     elif argv_after_opts[0].startswith("@"):
         argv_opts = list(it.takewhile(lambda x: x.startswith("-"), argv[1:]))
         argv = [argv[0]] + argv_opts + ["edit"] + argv_after_opts
-        logger.debug(
+        _logger.debug(
             "Inferring 'edit' command since we found a file group name.",
             file_group_name=argv_after_opts[0],
             new_args=argv[1:],
         )
 
     parser = clack.Parser(description="The zettel note manager of the future.")
     # --- Global Options
@@ -155,18 +172,32 @@
     )
 
     # --- 'db' command
     db_parser = new_command(
         "db", help="Commands for managing Zorg's SQL database."
     )
     new_db_command = clack.new_command_factory(db_parser)
-    # --- 'db info' command
+    # --- 'db create' command
     new_db_command(
-        "info",
-        help="Display some useful stats related to your Zorg notes and todos.",
+        "create",
+        help="Create zorg's backend database from scratch.",
+    )
+    # --- 'db reindex' command
+    db_reindex_parser = new_db_command(
+        "reindex",
+        help="Reindex any changed files by adding them to the database.",
+    )
+    db_reindex_parser.add_argument(
+        "paths",
+        type=Path,
+        nargs="*",
+        help=(
+            "Reindex these specific paths. If this argument is not provided,"
+            " we use a hashing approach to check which files have changed."
+        ),
     )
 
     # --- 'edit' command
     edit_parser = new_command(
         "edit",
         help=(
             "Generate new day logs from templates and open the main day log in"
@@ -230,15 +261,15 @@
     _process_zo_paths(kwargs)
 
     return kwargs
 
 
 def _process_zo_paths(kwargs: dict[str, Any]) -> None:
     if kwargs["command"] == "edit" and "zo_paths" not in kwargs:
-        logger.debug(
+        _logger.debug(
             "The 'edit' command was invoked, but no file paths were specified."
             " Auto-adding the @default file group paths.",
             kwargs=kwargs,
         )
         kwargs["zo_paths"] = [Path("@default")]
```

### Comparing `zettel-org-0.6.0/src/zorg/db.py` & `zettel_org-0.6.1/src/zorg/storage/sql/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from sqlalchemy.future import Engine
 from sqlmodel import SQLModel, create_engine as sqlmodel_create_engine
 
 
 @cache
 def create_cached_engine(url: str, /, **kwargs: Any) -> Engine:
     """Helper function for creating a new (if necessary) sqlalchemy engine."""
-    engine = create_engine(url, **kwargs)
+    engine = _create_engine(url, **kwargs)
     return engine
 
 
-def create_engine(url: str, /, **kwargs: Any) -> Engine:
+def _create_engine(url: str, /, **kwargs: Any) -> Engine:
     """Wrapper around sqlmodel.create_engine() that makes sure tables exist."""
     engine = sqlmodel_create_engine(url, **kwargs)
     SQLModel.metadata.create_all(engine)
     return engine
```

### Comparing `zettel-org-0.6.0/src/zorg/file_groups.py` & `zettel_org-0.6.1/src/zorg/service/file_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 from pathlib import Path
 from typing import Iterable, Sequence
 
 from typist import PathLike
 
-from .types import FileGroupMapType
+from ..domain.types import FileGroupMapType
 
 
 # TODO(bugyi): See if you can reduce complexity between this and _paths_from_file_group()
 def expand_file_group_paths(
     zo_paths: Iterable[PathLike],
     *,
     file_group_map: FileGroupMapType,
```

### Comparing `zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFile.interp` & `zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFile.interp`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 '*****'
 null
 'o'
 'x'
 null
 null
 null
+null
+null
 '  -'
 '    -'
 null
 '-'
 '.'
 '/'
 '_'
@@ -43,14 +45,16 @@
 null
 null
 NL
 LOWER_O
 LOWER_X
 ID
 DATE
+TIME
+ZID
 NUM_ID
 TWO_SPACE_DASH
 FOUR_SPACE_DASH
 SYMBOL
 DASH
 DOT
 FSLASH
@@ -72,30 +76,35 @@
 
 rule names:
 prog
 head
 comment
 block
 item
-todo
-priority
+footnote
 note
 base_note
-base_todo
+id_note_body
+note_body
 subnote
 subsubnote
-item_body
-footnote
+todo
+base_todo
+todo_prefix
+x_or_tilde
+priority
+zid
 space_atoms
 space_atom
 atom
 property
 id_group
 id
 date
+time
 any_symbol
 non_tag_symbol
 id_symbol
 tag_symbol
 tag
 area
 context
@@ -108,11 +117,12 @@
 h2_section
 h3_section
 h4_section
 h1_header
 h2_header
 h3_header
 h4_header
+eol
 
 
 atn:
-[4, 1, 33, 407, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 1, 0, 1, 0, 4, 0, 85, 8, 0, 11, 0, 12, 0, 86, 1, 0, 5, 0, 90, 8, 0, 10, 0, 12, 0, 93, 9, 0, 1, 0, 5, 0, 96, 8, 0, 10, 0, 12, 0, 99, 9, 0, 1, 0, 5, 0, 102, 8, 0, 10, 0, 12, 0, 105, 9, 0, 3, 0, 107, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 112, 8, 1, 11, 1, 12, 1, 113, 1, 2, 1, 2, 3, 2, 118, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 123, 8, 3, 11, 3, 12, 3, 124, 1, 3, 5, 3, 128, 8, 3, 10, 3, 12, 3, 131, 9, 3, 1, 4, 1, 4, 1, 4, 1, 4, 3, 4, 137, 8, 4, 1, 5, 1, 5, 5, 5, 141, 8, 5, 10, 5, 12, 5, 144, 9, 5, 1, 6, 1, 6, 1, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 7, 5, 7, 154, 8, 7, 10, 7, 12, 7, 157, 9, 7, 1, 8, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 3, 9, 165, 8, 9, 1, 9, 1, 9, 1, 9, 1, 10, 1, 10, 1, 10, 5, 10, 173, 8, 10, 10, 10, 12, 10, 176, 9, 10, 1, 11, 1, 11, 1, 11, 1, 12, 1, 12, 1, 12, 4, 12, 184, 8, 12, 11, 12, 12, 12, 185, 1, 12, 5, 12, 189, 8, 12, 10, 12, 12, 12, 192, 9, 12, 1, 13, 1, 13, 1, 13, 1, 13, 1, 14, 4, 14, 199, 8, 14, 11, 14, 12, 14, 200, 1, 15, 1, 15, 1, 15, 3, 15, 206, 8, 15, 1, 15, 1, 15, 5, 15, 210, 8, 15, 10, 15, 12, 15, 213, 9, 15, 1, 15, 1, 15, 3, 15, 217, 8, 15, 1, 15, 1, 15, 1, 15, 5, 15, 222, 8, 15, 10, 15, 12, 15, 225, 9, 15, 3, 15, 227, 8, 15, 1, 15, 3, 15, 230, 8, 15, 1, 16, 1, 16, 1, 16, 1, 16, 1, 16, 1, 16, 3, 16, 238, 8, 16, 1, 17, 1, 17, 1, 17, 1, 17, 1, 17, 1, 18, 1, 18, 4, 18, 247, 8, 18, 11, 18, 12, 18, 248, 1, 18, 1, 18, 5, 18, 253, 8, 18, 10, 18, 12, 18, 256, 9, 18, 1, 19, 1, 19, 1, 19, 1, 19, 1, 19, 3, 19, 263, 8, 19, 1, 20, 1, 20, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 3, 21, 272, 8, 21, 1, 22, 1, 22, 1, 23, 1, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 25, 1, 25, 3, 25, 284, 8, 25, 1, 26, 1, 26, 1, 26, 1, 27, 1, 27, 1, 27, 1, 28, 1, 28, 1, 28, 1, 29, 1, 29, 1, 29, 1, 30, 1, 30, 1, 30, 1, 30, 1, 30, 4, 30, 303, 8, 30, 11, 30, 12, 30, 304, 1, 30, 1, 30, 1, 30, 4, 30, 310, 8, 30, 11, 30, 12, 30, 311, 1, 30, 1, 30, 3, 30, 316, 8, 30, 1, 31, 1, 31, 1, 31, 1, 31, 1, 32, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 5, 33, 328, 8, 33, 10, 33, 12, 33, 331, 9, 33, 1, 33, 3, 33, 334, 8, 33, 1, 33, 5, 33, 337, 8, 33, 10, 33, 12, 33, 340, 9, 33, 1, 34, 1, 34, 5, 34, 344, 8, 34, 10, 34, 12, 34, 347, 9, 34, 1, 34, 3, 34, 350, 8, 34, 1, 34, 5, 34, 353, 8, 34, 10, 34, 12, 34, 356, 9, 34, 1, 35, 1, 35, 5, 35, 360, 8, 35, 10, 35, 12, 35, 363, 9, 35, 1, 35, 3, 35, 366, 8, 35, 1, 35, 5, 35, 369, 8, 35, 10, 35, 12, 35, 372, 9, 35, 1, 36, 1, 36, 5, 36, 376, 8, 36, 10, 36, 12, 36, 379, 9, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 1, 38, 1, 38, 1, 39, 1, 39, 1, 39, 1, 39, 1, 40, 1, 40, 1, 40, 1, 40, 1, 40, 1, 40, 1, 40, 0, 0, 41, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 0, 4, 3, 0, 8, 9, 30, 30, 32, 33, 4, 0, 15, 15, 19, 19, 22, 23, 30, 33, 2, 0, 16, 18, 20, 20, 1, 0, 24, 27, 427, 0, 82, 1, 0, 0, 0, 2, 111, 1, 0, 0, 0, 4, 115, 1, 0, 0, 0, 6, 122, 1, 0, 0, 0, 8, 136, 1, 0, 0, 0, 10, 138, 1, 0, 0, 0, 12, 145, 1, 0, 0, 0, 14, 150, 1, 0, 0, 0, 16, 158, 1, 0, 0, 0, 18, 161, 1, 0, 0, 0, 20, 169, 1, 0, 0, 0, 22, 177, 1, 0, 0, 0, 24, 180, 1, 0, 0, 0, 26, 193, 1, 0, 0, 0, 28, 198, 1, 0, 0, 0, 30, 202, 1, 0, 0, 0, 32, 237, 1, 0, 0, 0, 34, 239, 1, 0, 0, 0, 36, 244, 1, 0, 0, 0, 38, 262, 1, 0, 0, 0, 40, 264, 1, 0, 0, 0, 42, 271, 1, 0, 0, 0, 44, 273, 1, 0, 0, 0, 46, 275, 1, 0, 0, 0, 48, 277, 1, 0, 0, 0, 50, 283, 1, 0, 0, 0, 52, 285, 1, 0, 0, 0, 54, 288, 1, 0, 0, 0, 56, 291, 1, 0, 0, 0, 58, 294, 1, 0, 0, 0, 60, 315, 1, 0, 0, 0, 62, 317, 1, 0, 0, 0, 64, 321, 1, 0, 0, 0, 66, 325, 1, 0, 0, 0, 68, 341, 1, 0, 0, 0, 70, 357, 1, 0, 0, 0, 72, 373, 1, 0, 0, 0, 74, 380, 1, 0, 0, 0, 76, 392, 1, 0, 0, 0, 78, 396, 1, 0, 0, 0, 80, 400, 1, 0, 0, 0, 82, 106, 3, 2, 1, 0, 83, 85, 5, 7, 0, 0, 84, 83, 1, 0, 0, 0, 85, 86, 1, 0, 0, 0, 86, 84, 1, 0, 0, 0, 86, 87, 1, 0, 0, 0, 87, 91, 1, 0, 0, 0, 88, 90, 3, 6, 3, 0, 89, 88, 1, 0, 0, 0, 90, 93, 1, 0, 0, 0, 91, 89, 1, 0, 0, 0, 91, 92, 1, 0, 0, 0, 92, 97, 1, 0, 0, 0, 93, 91, 1, 0, 0, 0, 94, 96, 3, 68, 34, 0, 95, 94, 1, 0, 0, 0, 96, 99, 1, 0, 0, 0, 97, 95, 1, 0, 0, 0, 97, 98, 1, 0, 0, 0, 98, 103, 1, 0, 0, 0, 99, 97, 1, 0, 0, 0, 100, 102, 3, 66, 33, 0, 101, 100, 1, 0, 0, 0, 102, 105, 1, 0, 0, 0, 103, 101, 1, 0, 0, 0, 103, 104, 1, 0, 0, 0, 104, 107, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 106, 84, 1, 0, 0, 0, 106, 107, 1, 0, 0, 0, 107, 108, 1, 0, 0, 0, 108, 109, 5, 0, 0, 1, 109, 1, 1, 0, 0, 0, 110, 112, 3, 4, 2, 0, 111, 110, 1, 0, 0, 0, 112, 113, 1, 0, 0, 0, 113, 111, 1, 0, 0, 0, 113, 114, 1, 0, 0, 0, 114, 3, 1, 0, 0, 0, 115, 117, 5, 24, 0, 0, 116, 118, 3, 28, 14, 0, 117, 116, 1, 0, 0, 0, 117, 118, 1, 0, 0, 0, 118, 119, 1, 0, 0, 0, 119, 120, 5, 7, 0, 0, 120, 5, 1, 0, 0, 0, 121, 123, 3, 8, 4, 0, 122, 121, 1, 0, 0, 0, 123, 124, 1, 0, 0, 0, 124, 122, 1, 0, 0, 0, 124, 125, 1, 0, 0, 0, 125, 129, 1, 0, 0, 0, 126, 128, 5, 7, 0, 0, 127, 126, 1, 0, 0, 0, 128, 131, 1, 0, 0, 0, 129, 127, 1, 0, 0, 0, 129, 130, 1, 0, 0, 0, 130, 7, 1, 0, 0, 0, 131, 129, 1, 0, 0, 0, 132, 137, 3, 10, 5, 0, 133, 137, 3, 14, 7, 0, 134, 137, 3, 26, 13, 0, 135, 137, 3, 4, 2, 0, 136, 132, 1, 0, 0, 0, 136, 133, 1, 0, 0, 0, 136, 134, 1, 0, 0, 0, 136, 135, 1, 0, 0, 0, 137, 9, 1, 0, 0, 0, 138, 142, 3, 18, 9, 0, 139, 141, 3, 20, 10, 0, 140, 139, 1, 0, 0, 0, 141, 144, 1, 0, 0, 0, 142, 140, 1, 0, 0, 0, 142, 143, 1, 0, 0, 0, 143, 11, 1, 0, 0, 0, 144, 142, 1, 0, 0, 0, 145, 146, 5, 1, 0, 0, 146, 147, 5, 24, 0, 0, 147, 148, 5, 10, 0, 0, 148, 149, 5, 2, 0, 0, 149, 13, 1, 0, 0, 0, 150, 151, 5, 16, 0, 0, 151, 155, 3, 16, 8, 0, 152, 154, 3, 20, 10, 0, 153, 152, 1, 0, 0, 0, 154, 157, 1, 0, 0, 0, 155, 153, 1, 0, 0, 0, 155, 156, 1, 0, 0, 0, 156, 15, 1, 0, 0, 0, 157, 155, 1, 0, 0, 0, 158, 159, 3, 24, 12, 0, 159, 160, 5, 7, 0, 0, 160, 17, 1, 0, 0, 0, 161, 164, 7, 0, 0, 0, 162, 163, 5, 21, 0, 0, 163, 165, 3, 12, 6, 0, 164, 162, 1, 0, 0, 0, 164, 165, 1, 0, 0, 0, 165, 166, 1, 0, 0, 0, 166, 167, 3, 24, 12, 0, 167, 168, 5, 7, 0, 0, 168, 19, 1, 0, 0, 0, 169, 170, 5, 13, 0, 0, 170, 174, 3, 16, 8, 0, 171, 173, 3, 22, 11, 0, 172, 171, 1, 0, 0, 0, 173, 176, 1, 0, 0, 0, 174, 172, 1, 0, 0, 0, 174, 175, 1, 0, 0, 0, 175, 21, 1, 0, 0, 0, 176, 174, 1, 0, 0, 0, 177, 178, 5, 14, 0, 0, 178, 179, 3, 16, 8, 0, 179, 23, 1, 0, 0, 0, 180, 190, 3, 28, 14, 0, 181, 183, 5, 7, 0, 0, 182, 184, 5, 21, 0, 0, 183, 182, 1, 0, 0, 0, 184, 185, 1, 0, 0, 0, 185, 183, 1, 0, 0, 0, 185, 186, 1, 0, 0, 0, 186, 187, 1, 0, 0, 0, 187, 189, 3, 28, 14, 0, 188, 181, 1, 0, 0, 0, 189, 192, 1, 0, 0, 0, 190, 188, 1, 0, 0, 0, 190, 191, 1, 0, 0, 0, 191, 25, 1, 0, 0, 0, 192, 190, 1, 0, 0, 0, 193, 194, 3, 64, 32, 0, 194, 195, 5, 20, 0, 0, 195, 196, 3, 28, 14, 0, 196, 27, 1, 0, 0, 0, 197, 199, 3, 30, 15, 0, 198, 197, 1, 0, 0, 0, 199, 200, 1, 0, 0, 0, 200, 198, 1, 0, 0, 0, 200, 201, 1, 0, 0, 0, 201, 29, 1, 0, 0, 0, 202, 205, 5, 21, 0, 0, 203, 204, 5, 28, 0, 0, 204, 206, 3, 44, 22, 0, 205, 203, 1, 0, 0, 0, 205, 206, 1, 0, 0, 0, 206, 211, 1, 0, 0, 0, 207, 210, 3, 44, 22, 0, 208, 210, 5, 29, 0, 0, 209, 207, 1, 0, 0, 0, 209, 208, 1, 0, 0, 0, 210, 213, 1, 0, 0, 0, 211, 209, 1, 0, 0, 0, 211, 212, 1, 0, 0, 0, 212, 216, 1, 0, 0, 0, 213, 211, 1, 0, 0, 0, 214, 217, 3, 32, 16, 0, 215, 217, 3, 60, 30, 0, 216, 214, 1, 0, 0, 0, 216, 215, 1, 0, 0, 0, 216, 217, 1, 0, 0, 0, 217, 226, 1, 0, 0, 0, 218, 223, 3, 42, 21, 0, 219, 222, 3, 42, 21, 0, 220, 222, 3, 38, 19, 0, 221, 219, 1, 0, 0, 0, 221, 220, 1, 0, 0, 0, 222, 225, 1, 0, 0, 0, 223, 221, 1, 0, 0, 0, 223, 224, 1, 0, 0, 0, 224, 227, 1, 0, 0, 0, 225, 223, 1, 0, 0, 0, 226, 218, 1, 0, 0, 0, 226, 227, 1, 0, 0, 0, 227, 229, 1, 0, 0, 0, 228, 230, 3, 64, 32, 0, 229, 228, 1, 0, 0, 0, 229, 230, 1, 0, 0, 0, 230, 31, 1, 0, 0, 0, 231, 238, 3, 48, 24, 0, 232, 238, 3, 50, 25, 0, 233, 238, 3, 62, 31, 0, 234, 238, 3, 34, 17, 0, 235, 238, 3, 36, 18, 0, 236, 238, 3, 64, 32, 0, 237, 231, 1, 0, 0, 0, 237, 232, 1, 0, 0, 0, 237, 233, 1, 0, 0, 0, 237, 234, 1, 0, 0, 0, 237, 235, 1, 0, 0, 0, 237, 236, 1, 0, 0, 0, 238, 33, 1, 0, 0, 0, 239, 240, 5, 10, 0, 0, 240, 241, 5, 20, 0, 0, 241, 242, 5, 20, 0, 0, 242, 243, 3, 36, 18, 0, 243, 35, 1, 0, 0, 0, 244, 254, 3, 38, 19, 0, 245, 247, 3, 46, 23, 0, 246, 245, 1, 0, 0, 0, 247, 248, 1, 0, 0, 0, 248, 246, 1, 0, 0, 0, 248, 249, 1, 0, 0, 0, 249, 250, 1, 0, 0, 0, 250, 251, 3, 38, 19, 0, 251, 253, 1, 0, 0, 0, 252, 246, 1, 0, 0, 0, 253, 256, 1, 0, 0, 0, 254, 252, 1, 0, 0, 0, 254, 255, 1, 0, 0, 0, 255, 37, 1, 0, 0, 0, 256, 254, 1, 0, 0, 0, 257, 263, 5, 10, 0, 0, 258, 263, 5, 12, 0, 0, 259, 263, 3, 40, 20, 0, 260, 263, 5, 8, 0, 0, 261, 263, 5, 9, 0, 0, 262, 257, 1, 0, 0, 0, 262, 258, 1, 0, 0, 0, 262, 259, 1, 0, 0, 0, 262, 260, 1, 0, 0, 0, 262, 261, 1, 0, 0, 0, 263, 39, 1, 0, 0, 0, 264, 265, 5, 11, 0, 0, 265, 41, 1, 0, 0, 0, 266, 272, 5, 28, 0, 0, 267, 272, 5, 29, 0, 0, 268, 272, 3, 44, 22, 0, 269, 272, 3, 48, 24, 0, 270, 272, 3, 46, 23, 0, 271, 266, 1, 0, 0, 0, 271, 267, 1, 0, 0, 0, 271, 268, 1, 0, 0, 0, 271, 269, 1, 0, 0, 0, 271, 270, 1, 0, 0, 0, 272, 43, 1, 0, 0, 0, 273, 274, 7, 1, 0, 0, 274, 45, 1, 0, 0, 0, 275, 276, 7, 2, 0, 0, 276, 47, 1, 0, 0, 0, 277, 278, 7, 3, 0, 0, 278, 49, 1, 0, 0, 0, 279, 284, 3, 52, 26, 0, 280, 284, 3, 54, 27, 0, 281, 284, 3, 56, 28, 0, 282, 284, 3, 58, 29, 0, 283, 279, 1, 0, 0, 0, 283, 280, 1, 0, 0, 0, 283, 281, 1, 0, 0, 0, 283, 282, 1, 0, 0, 0, 284, 51, 1, 0, 0, 0, 285, 286, 5, 24, 0, 0, 286, 287, 5, 10, 0, 0, 287, 53, 1, 0, 0, 0, 288, 289, 5, 25, 0, 0, 289, 290, 5, 10, 0, 0, 290, 55, 1, 0, 0, 0, 291, 292, 5, 27, 0, 0, 292, 293, 5, 10, 0, 0, 293, 57, 1, 0, 0, 0, 294, 295, 5, 26, 0, 0, 295, 296, 5, 10, 0, 0, 296, 59, 1, 0, 0, 0, 297, 302, 5, 28, 0, 0, 298, 303, 3, 32, 16, 0, 299, 303, 3, 12, 6, 0, 300, 303, 5, 3, 0, 0, 301, 303, 5, 4, 0, 0, 302, 298, 1, 0, 0, 0, 302, 299, 1, 0, 0, 0, 302, 300, 1, 0, 0, 0, 302, 301, 1, 0, 0, 0, 303, 304, 1, 0, 0, 0, 304, 302, 1, 0, 0, 0, 304, 305, 1, 0, 0, 0, 305, 306, 1, 0, 0, 0, 306, 316, 5, 28, 0, 0, 307, 309, 5, 29, 0, 0, 308, 310, 3, 32, 16, 0, 309, 308, 1, 0, 0, 0, 310, 311, 1, 0, 0, 0, 311, 309, 1, 0, 0, 0, 311, 312, 1, 0, 0, 0, 312, 313, 1, 0, 0, 0, 313, 314, 5, 29, 0, 0, 314, 316, 1, 0, 0, 0, 315, 297, 1, 0, 0, 0, 315, 307, 1, 0, 0, 0, 316, 61, 1, 0, 0, 0, 317, 318, 5, 3, 0, 0, 318, 319, 3, 36, 18, 0, 319, 320, 5, 4, 0, 0, 320, 63, 1, 0, 0, 0, 321, 322, 5, 1, 0, 0, 322, 323, 3, 36, 18, 0, 323, 324, 5, 2, 0, 0, 324, 65, 1, 0, 0, 0, 325, 329, 3, 74, 37, 0, 326, 328, 3, 6, 3, 0, 327, 326, 1, 0, 0, 0, 328, 331, 1, 0, 0, 0, 329, 327, 1, 0, 0, 0, 329, 330, 1, 0, 0, 0, 330, 338, 1, 0, 0, 0, 331, 329, 1, 0, 0, 0, 332, 334, 5, 7, 0, 0, 333, 332, 1, 0, 0, 0, 333, 334, 1, 0, 0, 0, 334, 335, 1, 0, 0, 0, 335, 337, 3, 68, 34, 0, 336, 333, 1, 0, 0, 0, 337, 340, 1, 0, 0, 0, 338, 336, 1, 0, 0, 0, 338, 339, 1, 0, 0, 0, 339, 67, 1, 0, 0, 0, 340, 338, 1, 0, 0, 0, 341, 345, 3, 76, 38, 0, 342, 344, 3, 6, 3, 0, 343, 342, 1, 0, 0, 0, 344, 347, 1, 0, 0, 0, 345, 343, 1, 0, 0, 0, 345, 346, 1, 0, 0, 0, 346, 354, 1, 0, 0, 0, 347, 345, 1, 0, 0, 0, 348, 350, 5, 7, 0, 0, 349, 348, 1, 0, 0, 0, 349, 350, 1, 0, 0, 0, 350, 351, 1, 0, 0, 0, 351, 353, 3, 70, 35, 0, 352, 349, 1, 0, 0, 0, 353, 356, 1, 0, 0, 0, 354, 352, 1, 0, 0, 0, 354, 355, 1, 0, 0, 0, 355, 69, 1, 0, 0, 0, 356, 354, 1, 0, 0, 0, 357, 361, 3, 78, 39, 0, 358, 360, 3, 6, 3, 0, 359, 358, 1, 0, 0, 0, 360, 363, 1, 0, 0, 0, 361, 359, 1, 0, 0, 0, 361, 362, 1, 0, 0, 0, 362, 370, 1, 0, 0, 0, 363, 361, 1, 0, 0, 0, 364, 366, 5, 7, 0, 0, 365, 364, 1, 0, 0, 0, 365, 366, 1, 0, 0, 0, 366, 367, 1, 0, 0, 0, 367, 369, 3, 72, 36, 0, 368, 365, 1, 0, 0, 0, 369, 372, 1, 0, 0, 0, 370, 368, 1, 0, 0, 0, 370, 371, 1, 0, 0, 0, 371, 71, 1, 0, 0, 0, 372, 370, 1, 0, 0, 0, 373, 377, 3, 80, 40, 0, 374, 376, 3, 6, 3, 0, 375, 374, 1, 0, 0, 0, 376, 379, 1, 0, 0, 0, 377, 375, 1, 0, 0, 0, 377, 378, 1, 0, 0, 0, 378, 73, 1, 0, 0, 0, 379, 377, 1, 0, 0, 0, 380, 381, 5, 24, 0, 0, 381, 382, 5, 24, 0, 0, 382, 383, 5, 24, 0, 0, 383, 384, 5, 24, 0, 0, 384, 385, 5, 24, 0, 0, 385, 386, 5, 24, 0, 0, 386, 387, 5, 24, 0, 0, 387, 388, 5, 24, 0, 0, 388, 389, 5, 24, 0, 0, 389, 390, 3, 28, 14, 0, 390, 391, 5, 7, 0, 0, 391, 75, 1, 0, 0, 0, 392, 393, 5, 5, 0, 0, 393, 394, 3, 28, 14, 0, 394, 395, 5, 7, 0, 0, 395, 77, 1, 0, 0, 0, 396, 397, 5, 6, 0, 0, 397, 398, 3, 28, 14, 0, 398, 399, 5, 7, 0, 0, 399, 79, 1, 0, 0, 0, 400, 401, 5, 16, 0, 0, 401, 402, 5, 16, 0, 0, 402, 403, 5, 16, 0, 0, 403, 404, 3, 28, 14, 0, 404, 405, 5, 7, 0, 0, 405, 81, 1, 0, 0, 0, 45, 86, 91, 97, 103, 106, 113, 117, 124, 129, 136, 142, 155, 164, 174, 185, 190, 200, 205, 209, 211, 216, 221, 223, 226, 229, 237, 248, 254, 262, 271, 283, 302, 304, 311, 315, 329, 333, 338, 345, 349, 354, 361, 365, 370, 377]
+[4, 1, 35, 468, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 1, 0, 1, 0, 4, 0, 97, 8, 0, 11, 0, 12, 0, 98, 1, 0, 5, 0, 102, 8, 0, 10, 0, 12, 0, 105, 9, 0, 1, 0, 5, 0, 108, 8, 0, 10, 0, 12, 0, 111, 9, 0, 1, 0, 5, 0, 114, 8, 0, 10, 0, 12, 0, 117, 9, 0, 3, 0, 119, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 124, 8, 1, 11, 1, 12, 1, 125, 1, 2, 1, 2, 3, 2, 130, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 135, 8, 3, 11, 3, 12, 3, 136, 1, 3, 5, 3, 140, 8, 3, 10, 3, 12, 3, 143, 9, 3, 1, 4, 1, 4, 1, 4, 1, 4, 3, 4, 149, 8, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 1, 6, 1, 6, 5, 6, 159, 8, 6, 10, 6, 12, 6, 162, 9, 6, 1, 7, 1, 7, 1, 7, 1, 8, 1, 8, 3, 8, 169, 8, 8, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 4, 9, 176, 8, 9, 11, 9, 12, 9, 177, 1, 9, 5, 9, 181, 8, 9, 10, 9, 12, 9, 184, 9, 9, 1, 10, 1, 10, 1, 10, 5, 10, 189, 8, 10, 10, 10, 12, 10, 192, 9, 10, 1, 11, 1, 11, 1, 11, 1, 12, 1, 12, 5, 12, 199, 8, 12, 10, 12, 12, 12, 202, 9, 12, 1, 13, 1, 13, 1, 13, 3, 13, 207, 8, 13, 1, 13, 1, 13, 1, 13, 1, 14, 1, 14, 1, 14, 1, 14, 3, 14, 216, 8, 14, 1, 15, 1, 15, 1, 15, 3, 15, 221, 8, 15, 1, 16, 1, 16, 1, 16, 1, 16, 1, 16, 1, 17, 1, 17, 1, 18, 4, 18, 231, 8, 18, 11, 18, 12, 18, 232, 1, 19, 1, 19, 1, 19, 3, 19, 238, 8, 19, 1, 19, 1, 19, 5, 19, 242, 8, 19, 10, 19, 12, 19, 245, 9, 19, 1, 19, 1, 19, 3, 19, 249, 8, 19, 1, 19, 1, 19, 1, 19, 5, 19, 254, 8, 19, 10, 19, 12, 19, 257, 9, 19, 3, 19, 259, 8, 19, 1, 19, 3, 19, 262, 8, 19, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 3, 20, 270, 8, 20, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 22, 1, 22, 4, 22, 279, 8, 22, 11, 22, 12, 22, 280, 1, 22, 1, 22, 5, 22, 285, 8, 22, 10, 22, 12, 22, 288, 9, 22, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 3, 23, 296, 8, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 26, 1, 26, 1, 26, 3, 26, 307, 8, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 30, 1, 30, 3, 30, 319, 8, 30, 1, 31, 1, 31, 1, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 1, 35, 1, 35, 4, 35, 338, 8, 35, 11, 35, 12, 35, 339, 1, 35, 1, 35, 1, 35, 4, 35, 345, 8, 35, 11, 35, 12, 35, 346, 1, 35, 1, 35, 3, 35, 351, 8, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 5, 38, 363, 8, 38, 10, 38, 12, 38, 366, 9, 38, 1, 38, 5, 38, 369, 8, 38, 10, 38, 12, 38, 372, 9, 38, 1, 38, 3, 38, 375, 8, 38, 1, 38, 5, 38, 378, 8, 38, 10, 38, 12, 38, 381, 9, 38, 1, 39, 1, 39, 5, 39, 385, 8, 39, 10, 39, 12, 39, 388, 9, 39, 1, 39, 5, 39, 391, 8, 39, 10, 39, 12, 39, 394, 9, 39, 1, 39, 3, 39, 397, 8, 39, 1, 39, 5, 39, 400, 8, 39, 10, 39, 12, 39, 403, 9, 39, 1, 40, 1, 40, 5, 40, 407, 8, 40, 10, 40, 12, 40, 410, 9, 40, 1, 40, 5, 40, 413, 8, 40, 10, 40, 12, 40, 416, 9, 40, 1, 40, 3, 40, 419, 8, 40, 1, 40, 5, 40, 422, 8, 40, 10, 40, 12, 40, 425, 9, 40, 1, 41, 1, 41, 5, 41, 429, 8, 41, 10, 41, 12, 41, 432, 9, 41, 1, 41, 5, 41, 435, 8, 41, 10, 41, 12, 41, 438, 9, 41, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 42, 1, 43, 1, 43, 1, 43, 1, 43, 1, 44, 1, 44, 1, 44, 1, 44, 1, 45, 1, 45, 1, 45, 1, 45, 1, 45, 1, 45, 1, 46, 1, 46, 1, 46, 0, 0, 47, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 0, 5, 2, 0, 9, 9, 32, 32, 4, 0, 17, 17, 21, 21, 24, 25, 32, 35, 2, 0, 18, 20, 22, 22, 1, 0, 26, 29, 1, 1, 7, 7, 492, 0, 94, 1, 0, 0, 0, 2, 123, 1, 0, 0, 0, 4, 127, 1, 0, 0, 0, 6, 134, 1, 0, 0, 0, 8, 148, 1, 0, 0, 0, 10, 150, 1, 0, 0, 0, 12, 155, 1, 0, 0, 0, 14, 163, 1, 0, 0, 0, 16, 168, 1, 0, 0, 0, 18, 172, 1, 0, 0, 0, 20, 185, 1, 0, 0, 0, 22, 193, 1, 0, 0, 0, 24, 196, 1, 0, 0, 0, 26, 203, 1, 0, 0, 0, 28, 215, 1, 0, 0, 0, 30, 217, 1, 0, 0, 0, 32, 222, 1, 0, 0, 0, 34, 227, 1, 0, 0, 0, 36, 230, 1, 0, 0, 0, 38, 234, 1, 0, 0, 0, 40, 269, 1, 0, 0, 0, 42, 271, 1, 0, 0, 0, 44, 276, 1, 0, 0, 0, 46, 295, 1, 0, 0, 0, 48, 297, 1, 0, 0, 0, 50, 299, 1, 0, 0, 0, 52, 306, 1, 0, 0, 0, 54, 308, 1, 0, 0, 0, 56, 310, 1, 0, 0, 0, 58, 312, 1, 0, 0, 0, 60, 318, 1, 0, 0, 0, 62, 320, 1, 0, 0, 0, 64, 323, 1, 0, 0, 0, 66, 326, 1, 0, 0, 0, 68, 329, 1, 0, 0, 0, 70, 350, 1, 0, 0, 0, 72, 352, 1, 0, 0, 0, 74, 356, 1, 0, 0, 0, 76, 360, 1, 0, 0, 0, 78, 382, 1, 0, 0, 0, 80, 404, 1, 0, 0, 0, 82, 426, 1, 0, 0, 0, 84, 439, 1, 0, 0, 0, 86, 451, 1, 0, 0, 0, 88, 455, 1, 0, 0, 0, 90, 459, 1, 0, 0, 0, 92, 465, 1, 0, 0, 0, 94, 118, 3, 2, 1, 0, 95, 97, 5, 7, 0, 0, 96, 95, 1, 0, 0, 0, 97, 98, 1, 0, 0, 0, 98, 96, 1, 0, 0, 0, 98, 99, 1, 0, 0, 0, 99, 103, 1, 0, 0, 0, 100, 102, 3, 6, 3, 0, 101, 100, 1, 0, 0, 0, 102, 105, 1, 0, 0, 0, 103, 101, 1, 0, 0, 0, 103, 104, 1, 0, 0, 0, 104, 109, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 106, 108, 3, 78, 39, 0, 107, 106, 1, 0, 0, 0, 108, 111, 1, 0, 0, 0, 109, 107, 1, 0, 0, 0, 109, 110, 1, 0, 0, 0, 110, 115, 1, 0, 0, 0, 111, 109, 1, 0, 0, 0, 112, 114, 3, 76, 38, 0, 113, 112, 1, 0, 0, 0, 114, 117, 1, 0, 0, 0, 115, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 119, 1, 0, 0, 0, 117, 115, 1, 0, 0, 0, 118, 96, 1, 0, 0, 0, 118, 119, 1, 0, 0, 0, 119, 120, 1, 0, 0, 0, 120, 121, 5, 0, 0, 1, 121, 1, 1, 0, 0, 0, 122, 124, 3, 4, 2, 0, 123, 122, 1, 0, 0, 0, 124, 125, 1, 0, 0, 0, 125, 123, 1, 0, 0, 0, 125, 126, 1, 0, 0, 0, 126, 3, 1, 0, 0, 0, 127, 129, 5, 26, 0, 0, 128, 130, 3, 36, 18, 0, 129, 128, 1, 0, 0, 0, 129, 130, 1, 0, 0, 0, 130, 131, 1, 0, 0, 0, 131, 132, 5, 7, 0, 0, 132, 5, 1, 0, 0, 0, 133, 135, 3, 8, 4, 0, 134, 133, 1, 0, 0, 0, 135, 136, 1, 0, 0, 0, 136, 134, 1, 0, 0, 0, 136, 137, 1, 0, 0, 0, 137, 141, 1, 0, 0, 0, 138, 140, 5, 7, 0, 0, 139, 138, 1, 0, 0, 0, 140, 143, 1, 0, 0, 0, 141, 139, 1, 0, 0, 0, 141, 142, 1, 0, 0, 0, 142, 7, 1, 0, 0, 0, 143, 141, 1, 0, 0, 0, 144, 149, 3, 24, 12, 0, 145, 149, 3, 12, 6, 0, 146, 149, 3, 10, 5, 0, 147, 149, 3, 4, 2, 0, 148, 144, 1, 0, 0, 0, 148, 145, 1, 0, 0, 0, 148, 146, 1, 0, 0, 0, 148, 147, 1, 0, 0, 0, 149, 9, 1, 0, 0, 0, 150, 151, 3, 74, 37, 0, 151, 152, 5, 22, 0, 0, 152, 153, 3, 36, 18, 0, 153, 154, 5, 7, 0, 0, 154, 11, 1, 0, 0, 0, 155, 156, 5, 18, 0, 0, 156, 160, 3, 14, 7, 0, 157, 159, 3, 20, 10, 0, 158, 157, 1, 0, 0, 0, 159, 162, 1, 0, 0, 0, 160, 158, 1, 0, 0, 0, 160, 161, 1, 0, 0, 0, 161, 13, 1, 0, 0, 0, 162, 160, 1, 0, 0, 0, 163, 164, 3, 16, 8, 0, 164, 165, 5, 7, 0, 0, 165, 15, 1, 0, 0, 0, 166, 167, 5, 23, 0, 0, 167, 169, 3, 34, 17, 0, 168, 166, 1, 0, 0, 0, 168, 169, 1, 0, 0, 0, 169, 170, 1, 0, 0, 0, 170, 171, 3, 18, 9, 0, 171, 17, 1, 0, 0, 0, 172, 182, 3, 36, 18, 0, 173, 175, 5, 7, 0, 0, 174, 176, 5, 23, 0, 0, 175, 174, 1, 0, 0, 0, 176, 177, 1, 0, 0, 0, 177, 175, 1, 0, 0, 0, 177, 178, 1, 0, 0, 0, 178, 179, 1, 0, 0, 0, 179, 181, 3, 36, 18, 0, 180, 173, 1, 0, 0, 0, 181, 184, 1, 0, 0, 0, 182, 180, 1, 0, 0, 0, 182, 183, 1, 0, 0, 0, 183, 19, 1, 0, 0, 0, 184, 182, 1, 0, 0, 0, 185, 186, 5, 15, 0, 0, 186, 190, 3, 14, 7, 0, 187, 189, 3, 22, 11, 0, 188, 187, 1, 0, 0, 0, 189, 192, 1, 0, 0, 0, 190, 188, 1, 0, 0, 0, 190, 191, 1, 0, 0, 0, 191, 21, 1, 0, 0, 0, 192, 190, 1, 0, 0, 0, 193, 194, 5, 16, 0, 0, 194, 195, 3, 14, 7, 0, 195, 23, 1, 0, 0, 0, 196, 200, 3, 26, 13, 0, 197, 199, 3, 20, 10, 0, 198, 197, 1, 0, 0, 0, 199, 202, 1, 0, 0, 0, 200, 198, 1, 0, 0, 0, 200, 201, 1, 0, 0, 0, 201, 25, 1, 0, 0, 0, 202, 200, 1, 0, 0, 0, 203, 206, 3, 28, 14, 0, 204, 205, 5, 23, 0, 0, 205, 207, 3, 32, 16, 0, 206, 204, 1, 0, 0, 0, 206, 207, 1, 0, 0, 0, 207, 208, 1, 0, 0, 0, 208, 209, 3, 16, 8, 0, 209, 210, 5, 7, 0, 0, 210, 27, 1, 0, 0, 0, 211, 216, 5, 8, 0, 0, 212, 216, 3, 30, 15, 0, 213, 216, 5, 34, 0, 0, 214, 216, 5, 35, 0, 0, 215, 211, 1, 0, 0, 0, 215, 212, 1, 0, 0, 0, 215, 213, 1, 0, 0, 0, 215, 214, 1, 0, 0, 0, 216, 29, 1, 0, 0, 0, 217, 220, 7, 0, 0, 0, 218, 219, 5, 22, 0, 0, 219, 221, 3, 50, 25, 0, 220, 218, 1, 0, 0, 0, 220, 221, 1, 0, 0, 0, 221, 31, 1, 0, 0, 0, 222, 223, 5, 1, 0, 0, 223, 224, 5, 26, 0, 0, 224, 225, 5, 10, 0, 0, 225, 226, 5, 2, 0, 0, 226, 33, 1, 0, 0, 0, 227, 228, 5, 13, 0, 0, 228, 35, 1, 0, 0, 0, 229, 231, 3, 38, 19, 0, 230, 229, 1, 0, 0, 0, 231, 232, 1, 0, 0, 0, 232, 230, 1, 0, 0, 0, 232, 233, 1, 0, 0, 0, 233, 37, 1, 0, 0, 0, 234, 237, 5, 23, 0, 0, 235, 236, 5, 30, 0, 0, 236, 238, 3, 54, 27, 0, 237, 235, 1, 0, 0, 0, 237, 238, 1, 0, 0, 0, 238, 243, 1, 0, 0, 0, 239, 242, 3, 54, 27, 0, 240, 242, 5, 31, 0, 0, 241, 239, 1, 0, 0, 0, 241, 240, 1, 0, 0, 0, 242, 245, 1, 0, 0, 0, 243, 241, 1, 0, 0, 0, 243, 244, 1, 0, 0, 0, 244, 248, 1, 0, 0, 0, 245, 243, 1, 0, 0, 0, 246, 249, 3, 40, 20, 0, 247, 249, 3, 70, 35, 0, 248, 246, 1, 0, 0, 0, 248, 247, 1, 0, 0, 0, 248, 249, 1, 0, 0, 0, 249, 258, 1, 0, 0, 0, 250, 255, 3, 52, 26, 0, 251, 254, 3, 52, 26, 0, 252, 254, 3, 46, 23, 0, 253, 251, 1, 0, 0, 0, 253, 252, 1, 0, 0, 0, 254, 257, 1, 0, 0, 0, 255, 253, 1, 0, 0, 0, 255, 256, 1, 0, 0, 0, 256, 259, 1, 0, 0, 0, 257, 255, 1, 0, 0, 0, 258, 250, 1, 0, 0, 0, 258, 259, 1, 0, 0, 0, 259, 261, 1, 0, 0, 0, 260, 262, 3, 74, 37, 0, 261, 260, 1, 0, 0, 0, 261, 262, 1, 0, 0, 0, 262, 39, 1, 0, 0, 0, 263, 270, 3, 58, 29, 0, 264, 270, 3, 60, 30, 0, 265, 270, 3, 72, 36, 0, 266, 270, 3, 42, 21, 0, 267, 270, 3, 44, 22, 0, 268, 270, 3, 74, 37, 0, 269, 263, 1, 0, 0, 0, 269, 264, 1, 0, 0, 0, 269, 265, 1, 0, 0, 0, 269, 266, 1, 0, 0, 0, 269, 267, 1, 0, 0, 0, 269, 268, 1, 0, 0, 0, 270, 41, 1, 0, 0, 0, 271, 272, 5, 10, 0, 0, 272, 273, 5, 22, 0, 0, 273, 274, 5, 22, 0, 0, 274, 275, 3, 44, 22, 0, 275, 43, 1, 0, 0, 0, 276, 286, 3, 46, 23, 0, 277, 279, 3, 56, 28, 0, 278, 277, 1, 0, 0, 0, 279, 280, 1, 0, 0, 0, 280, 278, 1, 0, 0, 0, 280, 281, 1, 0, 0, 0, 281, 282, 1, 0, 0, 0, 282, 283, 3, 46, 23, 0, 283, 285, 1, 0, 0, 0, 284, 278, 1, 0, 0, 0, 285, 288, 1, 0, 0, 0, 286, 284, 1, 0, 0, 0, 286, 287, 1, 0, 0, 0, 287, 45, 1, 0, 0, 0, 288, 286, 1, 0, 0, 0, 289, 296, 5, 10, 0, 0, 290, 296, 5, 14, 0, 0, 291, 296, 3, 48, 24, 0, 292, 296, 3, 50, 25, 0, 293, 296, 5, 8, 0, 0, 294, 296, 5, 9, 0, 0, 295, 289, 1, 0, 0, 0, 295, 290, 1, 0, 0, 0, 295, 291, 1, 0, 0, 0, 295, 292, 1, 0, 0, 0, 295, 293, 1, 0, 0, 0, 295, 294, 1, 0, 0, 0, 296, 47, 1, 0, 0, 0, 297, 298, 5, 11, 0, 0, 298, 49, 1, 0, 0, 0, 299, 300, 5, 12, 0, 0, 300, 51, 1, 0, 0, 0, 301, 307, 5, 30, 0, 0, 302, 307, 5, 31, 0, 0, 303, 307, 3, 54, 27, 0, 304, 307, 3, 58, 29, 0, 305, 307, 3, 56, 28, 0, 306, 301, 1, 0, 0, 0, 306, 302, 1, 0, 0, 0, 306, 303, 1, 0, 0, 0, 306, 304, 1, 0, 0, 0, 306, 305, 1, 0, 0, 0, 307, 53, 1, 0, 0, 0, 308, 309, 7, 1, 0, 0, 309, 55, 1, 0, 0, 0, 310, 311, 7, 2, 0, 0, 311, 57, 1, 0, 0, 0, 312, 313, 7, 3, 0, 0, 313, 59, 1, 0, 0, 0, 314, 319, 3, 62, 31, 0, 315, 319, 3, 64, 32, 0, 316, 319, 3, 66, 33, 0, 317, 319, 3, 68, 34, 0, 318, 314, 1, 0, 0, 0, 318, 315, 1, 0, 0, 0, 318, 316, 1, 0, 0, 0, 318, 317, 1, 0, 0, 0, 319, 61, 1, 0, 0, 0, 320, 321, 5, 26, 0, 0, 321, 322, 5, 10, 0, 0, 322, 63, 1, 0, 0, 0, 323, 324, 5, 27, 0, 0, 324, 325, 5, 10, 0, 0, 325, 65, 1, 0, 0, 0, 326, 327, 5, 29, 0, 0, 327, 328, 5, 10, 0, 0, 328, 67, 1, 0, 0, 0, 329, 330, 5, 28, 0, 0, 330, 331, 5, 10, 0, 0, 331, 69, 1, 0, 0, 0, 332, 337, 5, 30, 0, 0, 333, 338, 3, 40, 20, 0, 334, 338, 3, 32, 16, 0, 335, 338, 5, 3, 0, 0, 336, 338, 5, 4, 0, 0, 337, 333, 1, 0, 0, 0, 337, 334, 1, 0, 0, 0, 337, 335, 1, 0, 0, 0, 337, 336, 1, 0, 0, 0, 338, 339, 1, 0, 0, 0, 339, 337, 1, 0, 0, 0, 339, 340, 1, 0, 0, 0, 340, 341, 1, 0, 0, 0, 341, 351, 5, 30, 0, 0, 342, 344, 5, 31, 0, 0, 343, 345, 3, 40, 20, 0, 344, 343, 1, 0, 0, 0, 345, 346, 1, 0, 0, 0, 346, 344, 1, 0, 0, 0, 346, 347, 1, 0, 0, 0, 347, 348, 1, 0, 0, 0, 348, 349, 5, 31, 0, 0, 349, 351, 1, 0, 0, 0, 350, 332, 1, 0, 0, 0, 350, 342, 1, 0, 0, 0, 351, 71, 1, 0, 0, 0, 352, 353, 5, 3, 0, 0, 353, 354, 3, 44, 22, 0, 354, 355, 5, 4, 0, 0, 355, 73, 1, 0, 0, 0, 356, 357, 5, 1, 0, 0, 357, 358, 3, 44, 22, 0, 358, 359, 5, 2, 0, 0, 359, 75, 1, 0, 0, 0, 360, 364, 3, 84, 42, 0, 361, 363, 5, 7, 0, 0, 362, 361, 1, 0, 0, 0, 363, 366, 1, 0, 0, 0, 364, 362, 1, 0, 0, 0, 364, 365, 1, 0, 0, 0, 365, 370, 1, 0, 0, 0, 366, 364, 1, 0, 0, 0, 367, 369, 3, 6, 3, 0, 368, 367, 1, 0, 0, 0, 369, 372, 1, 0, 0, 0, 370, 368, 1, 0, 0, 0, 370, 371, 1, 0, 0, 0, 371, 379, 1, 0, 0, 0, 372, 370, 1, 0, 0, 0, 373, 375, 5, 7, 0, 0, 374, 373, 1, 0, 0, 0, 374, 375, 1, 0, 0, 0, 375, 376, 1, 0, 0, 0, 376, 378, 3, 78, 39, 0, 377, 374, 1, 0, 0, 0, 378, 381, 1, 0, 0, 0, 379, 377, 1, 0, 0, 0, 379, 380, 1, 0, 0, 0, 380, 77, 1, 0, 0, 0, 381, 379, 1, 0, 0, 0, 382, 386, 3, 86, 43, 0, 383, 385, 5, 7, 0, 0, 384, 383, 1, 0, 0, 0, 385, 388, 1, 0, 0, 0, 386, 384, 1, 0, 0, 0, 386, 387, 1, 0, 0, 0, 387, 392, 1, 0, 0, 0, 388, 386, 1, 0, 0, 0, 389, 391, 3, 6, 3, 0, 390, 389, 1, 0, 0, 0, 391, 394, 1, 0, 0, 0, 392, 390, 1, 0, 0, 0, 392, 393, 1, 0, 0, 0, 393, 401, 1, 0, 0, 0, 394, 392, 1, 0, 0, 0, 395, 397, 5, 7, 0, 0, 396, 395, 1, 0, 0, 0, 396, 397, 1, 0, 0, 0, 397, 398, 1, 0, 0, 0, 398, 400, 3, 80, 40, 0, 399, 396, 1, 0, 0, 0, 400, 403, 1, 0, 0, 0, 401, 399, 1, 0, 0, 0, 401, 402, 1, 0, 0, 0, 402, 79, 1, 0, 0, 0, 403, 401, 1, 0, 0, 0, 404, 408, 3, 88, 44, 0, 405, 407, 5, 7, 0, 0, 406, 405, 1, 0, 0, 0, 407, 410, 1, 0, 0, 0, 408, 406, 1, 0, 0, 0, 408, 409, 1, 0, 0, 0, 409, 414, 1, 0, 0, 0, 410, 408, 1, 0, 0, 0, 411, 413, 3, 6, 3, 0, 412, 411, 1, 0, 0, 0, 413, 416, 1, 0, 0, 0, 414, 412, 1, 0, 0, 0, 414, 415, 1, 0, 0, 0, 415, 423, 1, 0, 0, 0, 416, 414, 1, 0, 0, 0, 417, 419, 5, 7, 0, 0, 418, 417, 1, 0, 0, 0, 418, 419, 1, 0, 0, 0, 419, 420, 1, 0, 0, 0, 420, 422, 3, 82, 41, 0, 421, 418, 1, 0, 0, 0, 422, 425, 1, 0, 0, 0, 423, 421, 1, 0, 0, 0, 423, 424, 1, 0, 0, 0, 424, 81, 1, 0, 0, 0, 425, 423, 1, 0, 0, 0, 426, 430, 3, 90, 45, 0, 427, 429, 5, 7, 0, 0, 428, 427, 1, 0, 0, 0, 429, 432, 1, 0, 0, 0, 430, 428, 1, 0, 0, 0, 430, 431, 1, 0, 0, 0, 431, 436, 1, 0, 0, 0, 432, 430, 1, 0, 0, 0, 433, 435, 3, 6, 3, 0, 434, 433, 1, 0, 0, 0, 435, 438, 1, 0, 0, 0, 436, 434, 1, 0, 0, 0, 436, 437, 1, 0, 0, 0, 437, 83, 1, 0, 0, 0, 438, 436, 1, 0, 0, 0, 439, 440, 5, 26, 0, 0, 440, 441, 5, 26, 0, 0, 441, 442, 5, 26, 0, 0, 442, 443, 5, 26, 0, 0, 443, 444, 5, 26, 0, 0, 444, 445, 5, 26, 0, 0, 445, 446, 5, 26, 0, 0, 446, 447, 5, 26, 0, 0, 447, 448, 5, 26, 0, 0, 448, 449, 3, 36, 18, 0, 449, 450, 3, 92, 46, 0, 450, 85, 1, 0, 0, 0, 451, 452, 5, 5, 0, 0, 452, 453, 3, 36, 18, 0, 453, 454, 3, 92, 46, 0, 454, 87, 1, 0, 0, 0, 455, 456, 5, 6, 0, 0, 456, 457, 3, 36, 18, 0, 457, 458, 3, 92, 46, 0, 458, 89, 1, 0, 0, 0, 459, 460, 5, 18, 0, 0, 460, 461, 5, 18, 0, 0, 461, 462, 5, 18, 0, 0, 462, 463, 3, 36, 18, 0, 463, 464, 3, 92, 46, 0, 464, 91, 1, 0, 0, 0, 465, 466, 7, 4, 0, 0, 466, 93, 1, 0, 0, 0, 52, 98, 103, 109, 115, 118, 125, 129, 136, 141, 148, 160, 168, 177, 182, 190, 200, 206, 215, 220, 232, 237, 241, 243, 248, 253, 255, 258, 261, 269, 280, 286, 295, 306, 318, 337, 339, 346, 350, 364, 370, 374, 379, 386, 392, 396, 401, 408, 414, 418, 423, 430, 436]
```

### Comparing `zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFileLexer.interp` & `zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFileLexer.interp`

 * *Files 25% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 '*****'
 null
 'o'
 'x'
 null
 null
 null
+null
+null
 '  -'
 '    -'
 null
 '-'
 '.'
 '/'
 '_'
@@ -43,14 +45,16 @@
 null
 null
 NL
 LOWER_O
 LOWER_X
 ID
 DATE
+TIME
+ZID
 NUM_ID
 TWO_SPACE_DASH
 FOUR_SPACE_DASH
 SYMBOL
 DASH
 DOT
 FSLASH
@@ -78,14 +82,16 @@
 T__4
 T__5
 NL
 LOWER_O
 LOWER_X
 ID
 DATE
+TIME
+ZID
 NUM_ID
 TWO_SPACE_DASH
 FOUR_SPACE_DASH
 SYMBOL
 DASH
 DOT
 FSLASH
@@ -102,20 +108,23 @@
 DQUOTE
 TILDE
 STAR
 LANGLE
 RANGLE
 UPPER_LETTER
 LOWER_LETTER
+ZID_CHAR
 NUM
+FIRST_D_NUM
+FIRST_M_NUM
 ALPHA
 ALPHANUM
 
 channel names:
 DEFAULT_TOKEN_CHANNEL
 HIDDEN
 
 mode names:
 DEFAULT_MODE
 
 atn:
-[4, 0, 33, 199, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 1, 0, 1, 0, 1, 1, 1, 1, 1, 2, 1, 2, 1, 2, 1, 3, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 3, 6, 103, 8, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 5, 9, 114, 8, 9, 10, 9, 12, 9, 117, 9, 9, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 11, 1, 11, 1, 11, 5, 11, 133, 8, 11, 10, 11, 12, 11, 136, 9, 11, 1, 12, 1, 12, 1, 12, 1, 12, 1, 13, 1, 13, 1, 13, 1, 13, 1, 13, 1, 13, 1, 14, 1, 14, 1, 15, 1, 15, 1, 16, 1, 16, 1, 17, 1, 17, 1, 18, 1, 18, 1, 19, 1, 19, 1, 20, 1, 20, 1, 21, 1, 21, 1, 22, 1, 22, 1, 23, 1, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 32, 1, 32, 1, 33, 1, 33, 1, 34, 1, 34, 1, 35, 1, 35, 1, 36, 1, 36, 3, 36, 194, 8, 36, 1, 37, 1, 37, 3, 37, 198, 8, 37, 0, 0, 38, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 27, 14, 29, 15, 31, 16, 33, 17, 35, 18, 37, 19, 39, 20, 41, 21, 43, 22, 45, 23, 47, 24, 49, 25, 51, 26, 53, 27, 55, 28, 57, 29, 59, 30, 61, 31, 63, 32, 65, 33, 67, 0, 69, 0, 71, 0, 73, 0, 75, 0, 1, 0, 1, 10, 0, 33, 33, 36, 36, 38, 38, 44, 44, 59, 59, 61, 61, 63, 63, 91, 94, 96, 96, 123, 125, 200, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 0, 27, 1, 0, 0, 0, 0, 29, 1, 0, 0, 0, 0, 31, 1, 0, 0, 0, 0, 33, 1, 0, 0, 0, 0, 35, 1, 0, 0, 0, 0, 37, 1, 0, 0, 0, 0, 39, 1, 0, 0, 0, 0, 41, 1, 0, 0, 0, 0, 43, 1, 0, 0, 0, 0, 45, 1, 0, 0, 0, 0, 47, 1, 0, 0, 0, 0, 49, 1, 0, 0, 0, 0, 51, 1, 0, 0, 0, 0, 53, 1, 0, 0, 0, 0, 55, 1, 0, 0, 0, 0, 57, 1, 0, 0, 0, 0, 59, 1, 0, 0, 0, 0, 61, 1, 0, 0, 0, 0, 63, 1, 0, 0, 0, 0, 65, 1, 0, 0, 0, 1, 77, 1, 0, 0, 0, 3, 79, 1, 0, 0, 0, 5, 81, 1, 0, 0, 0, 7, 84, 1, 0, 0, 0, 9, 87, 1, 0, 0, 0, 11, 95, 1, 0, 0, 0, 13, 102, 1, 0, 0, 0, 15, 106, 1, 0, 0, 0, 17, 108, 1, 0, 0, 0, 19, 110, 1, 0, 0, 0, 21, 118, 1, 0, 0, 0, 23, 129, 1, 0, 0, 0, 25, 137, 1, 0, 0, 0, 27, 141, 1, 0, 0, 0, 29, 147, 1, 0, 0, 0, 31, 149, 1, 0, 0, 0, 33, 151, 1, 0, 0, 0, 35, 153, 1, 0, 0, 0, 37, 155, 1, 0, 0, 0, 39, 157, 1, 0, 0, 0, 41, 159, 1, 0, 0, 0, 43, 161, 1, 0, 0, 0, 45, 163, 1, 0, 0, 0, 47, 165, 1, 0, 0, 0, 49, 167, 1, 0, 0, 0, 51, 169, 1, 0, 0, 0, 53, 171, 1, 0, 0, 0, 55, 173, 1, 0, 0, 0, 57, 175, 1, 0, 0, 0, 59, 177, 1, 0, 0, 0, 61, 179, 1, 0, 0, 0, 63, 181, 1, 0, 0, 0, 65, 183, 1, 0, 0, 0, 67, 185, 1, 0, 0, 0, 69, 187, 1, 0, 0, 0, 71, 189, 1, 0, 0, 0, 73, 193, 1, 0, 0, 0, 75, 197, 1, 0, 0, 0, 77, 78, 5, 91, 0, 0, 78, 2, 1, 0, 0, 0, 79, 80, 5, 93, 0, 0, 80, 4, 1, 0, 0, 0, 81, 82, 5, 91, 0, 0, 82, 83, 5, 91, 0, 0, 83, 6, 1, 0, 0, 0, 84, 85, 5, 93, 0, 0, 85, 86, 5, 93, 0, 0, 86, 8, 1, 0, 0, 0, 87, 88, 5, 61, 0, 0, 88, 89, 5, 61, 0, 0, 89, 90, 5, 61, 0, 0, 90, 91, 5, 61, 0, 0, 91, 92, 5, 61, 0, 0, 92, 93, 5, 61, 0, 0, 93, 94, 5, 61, 0, 0, 94, 10, 1, 0, 0, 0, 95, 96, 5, 42, 0, 0, 96, 97, 5, 42, 0, 0, 97, 98, 5, 42, 0, 0, 98, 99, 5, 42, 0, 0, 99, 100, 5, 42, 0, 0, 100, 12, 1, 0, 0, 0, 101, 103, 5, 13, 0, 0, 102, 101, 1, 0, 0, 0, 102, 103, 1, 0, 0, 0, 103, 104, 1, 0, 0, 0, 104, 105, 5, 10, 0, 0, 105, 14, 1, 0, 0, 0, 106, 107, 5, 111, 0, 0, 107, 16, 1, 0, 0, 0, 108, 109, 5, 120, 0, 0, 109, 18, 1, 0, 0, 0, 110, 115, 3, 73, 36, 0, 111, 114, 3, 75, 37, 0, 112, 114, 3, 37, 18, 0, 113, 111, 1, 0, 0, 0, 113, 112, 1, 0, 0, 0, 114, 117, 1, 0, 0, 0, 115, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 20, 1, 0, 0, 0, 117, 115, 1, 0, 0, 0, 118, 119, 5, 50, 0, 0, 119, 120, 3, 71, 35, 0, 120, 121, 3, 71, 35, 0, 121, 122, 3, 71, 35, 0, 122, 123, 3, 31, 15, 0, 123, 124, 2, 48, 50, 0, 124, 125, 3, 71, 35, 0, 125, 126, 3, 31, 15, 0, 126, 127, 2, 48, 51, 0, 127, 128, 3, 71, 35, 0, 128, 22, 1, 0, 0, 0, 129, 134, 3, 71, 35, 0, 130, 133, 3, 75, 37, 0, 131, 133, 3, 37, 18, 0, 132, 130, 1, 0, 0, 0, 132, 131, 1, 0, 0, 0, 133, 136, 1, 0, 0, 0, 134, 132, 1, 0, 0, 0, 134, 135, 1, 0, 0, 0, 135, 24, 1, 0, 0, 0, 136, 134, 1, 0, 0, 0, 137, 138, 5, 32, 0, 0, 138, 139, 5, 32, 0, 0, 139, 140, 5, 45, 0, 0, 140, 26, 1, 0, 0, 0, 141, 142, 5, 32, 0, 0, 142, 143, 5, 32, 0, 0, 143, 144, 5, 32, 0, 0, 144, 145, 5, 32, 0, 0, 145, 146, 5, 45, 0, 0, 146, 28, 1, 0, 0, 0, 147, 148, 7, 0, 0, 0, 148, 30, 1, 0, 0, 0, 149, 150, 5, 45, 0, 0, 150, 32, 1, 0, 0, 0, 151, 152, 5, 46, 0, 0, 152, 34, 1, 0, 0, 0, 153, 154, 5, 47, 0, 0, 154, 36, 1, 0, 0, 0, 155, 156, 5, 95, 0, 0, 156, 38, 1, 0, 0, 0, 157, 158, 5, 58, 0, 0, 158, 40, 1, 0, 0, 0, 159, 160, 5, 32, 0, 0, 160, 42, 1, 0, 0, 0, 161, 162, 5, 40, 0, 0, 162, 44, 1, 0, 0, 0, 163, 164, 5, 41, 0, 0, 164, 46, 1, 0, 0, 0, 165, 166, 5, 35, 0, 0, 166, 48, 1, 0, 0, 0, 167, 168, 5, 64, 0, 0, 168, 50, 1, 0, 0, 0, 169, 170, 5, 43, 0, 0, 170, 52, 1, 0, 0, 0, 171, 172, 5, 37, 0, 0, 172, 54, 1, 0, 0, 0, 173, 174, 5, 39, 0, 0, 174, 56, 1, 0, 0, 0, 175, 176, 5, 34, 0, 0, 176, 58, 1, 0, 0, 0, 177, 178, 5, 126, 0, 0, 178, 60, 1, 0, 0, 0, 179, 180, 5, 42, 0, 0, 180, 62, 1, 0, 0, 0, 181, 182, 5, 60, 0, 0, 182, 64, 1, 0, 0, 0, 183, 184, 5, 62, 0, 0, 184, 66, 1, 0, 0, 0, 185, 186, 2, 65, 90, 0, 186, 68, 1, 0, 0, 0, 187, 188, 2, 97, 122, 0, 188, 70, 1, 0, 0, 0, 189, 190, 2, 48, 57, 0, 190, 72, 1, 0, 0, 0, 191, 194, 3, 67, 33, 0, 192, 194, 3, 69, 34, 0, 193, 191, 1, 0, 0, 0, 193, 192, 1, 0, 0, 0, 194, 74, 1, 0, 0, 0, 195, 198, 3, 73, 36, 0, 196, 198, 3, 71, 35, 0, 197, 195, 1, 0, 0, 0, 197, 196, 1, 0, 0, 0, 198, 76, 1, 0, 0, 0, 8, 0, 102, 113, 115, 132, 134, 193, 197, 0]
+[4, 0, 35, 234, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 1, 0, 1, 0, 1, 1, 1, 1, 1, 2, 1, 2, 1, 2, 1, 3, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 3, 6, 113, 8, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 5, 9, 124, 8, 9, 10, 9, 12, 9, 127, 9, 9, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 11, 1, 11, 1, 11, 1, 11, 1, 11, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 3, 12, 155, 8, 12, 1, 13, 1, 13, 1, 13, 5, 13, 160, 8, 13, 10, 13, 12, 13, 163, 9, 13, 1, 14, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 1, 15, 1, 15, 1, 15, 1, 16, 1, 16, 1, 17, 1, 17, 1, 18, 1, 18, 1, 19, 1, 19, 1, 20, 1, 20, 1, 21, 1, 21, 1, 22, 1, 22, 1, 23, 1, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 32, 1, 32, 1, 33, 1, 33, 1, 34, 1, 34, 1, 35, 1, 35, 1, 36, 1, 36, 1, 37, 1, 37, 3, 37, 219, 8, 37, 1, 38, 1, 38, 1, 39, 1, 39, 1, 40, 1, 40, 1, 41, 1, 41, 3, 41, 229, 8, 41, 1, 42, 1, 42, 3, 42, 233, 8, 42, 0, 0, 43, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 27, 14, 29, 15, 31, 16, 33, 17, 35, 18, 37, 19, 39, 20, 41, 21, 43, 22, 45, 23, 47, 24, 49, 25, 51, 26, 53, 27, 55, 28, 57, 29, 59, 30, 61, 31, 63, 32, 65, 33, 67, 34, 69, 35, 71, 0, 73, 0, 75, 0, 77, 0, 79, 0, 81, 0, 83, 0, 85, 0, 1, 0, 2, 10, 0, 33, 33, 36, 36, 38, 38, 44, 44, 59, 59, 61, 61, 63, 63, 91, 94, 96, 96, 123, 125, 6, 0, 65, 72, 74, 78, 80, 90, 97, 105, 107, 107, 109, 122, 234, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 0, 27, 1, 0, 0, 0, 0, 29, 1, 0, 0, 0, 0, 31, 1, 0, 0, 0, 0, 33, 1, 0, 0, 0, 0, 35, 1, 0, 0, 0, 0, 37, 1, 0, 0, 0, 0, 39, 1, 0, 0, 0, 0, 41, 1, 0, 0, 0, 0, 43, 1, 0, 0, 0, 0, 45, 1, 0, 0, 0, 0, 47, 1, 0, 0, 0, 0, 49, 1, 0, 0, 0, 0, 51, 1, 0, 0, 0, 0, 53, 1, 0, 0, 0, 0, 55, 1, 0, 0, 0, 0, 57, 1, 0, 0, 0, 0, 59, 1, 0, 0, 0, 0, 61, 1, 0, 0, 0, 0, 63, 1, 0, 0, 0, 0, 65, 1, 0, 0, 0, 0, 67, 1, 0, 0, 0, 0, 69, 1, 0, 0, 0, 1, 87, 1, 0, 0, 0, 3, 89, 1, 0, 0, 0, 5, 91, 1, 0, 0, 0, 7, 94, 1, 0, 0, 0, 9, 97, 1, 0, 0, 0, 11, 105, 1, 0, 0, 0, 13, 112, 1, 0, 0, 0, 15, 116, 1, 0, 0, 0, 17, 118, 1, 0, 0, 0, 19, 120, 1, 0, 0, 0, 21, 128, 1, 0, 0, 0, 23, 139, 1, 0, 0, 0, 25, 144, 1, 0, 0, 0, 27, 156, 1, 0, 0, 0, 29, 164, 1, 0, 0, 0, 31, 168, 1, 0, 0, 0, 33, 174, 1, 0, 0, 0, 35, 176, 1, 0, 0, 0, 37, 178, 1, 0, 0, 0, 39, 180, 1, 0, 0, 0, 41, 182, 1, 0, 0, 0, 43, 184, 1, 0, 0, 0, 45, 186, 1, 0, 0, 0, 47, 188, 1, 0, 0, 0, 49, 190, 1, 0, 0, 0, 51, 192, 1, 0, 0, 0, 53, 194, 1, 0, 0, 0, 55, 196, 1, 0, 0, 0, 57, 198, 1, 0, 0, 0, 59, 200, 1, 0, 0, 0, 61, 202, 1, 0, 0, 0, 63, 204, 1, 0, 0, 0, 65, 206, 1, 0, 0, 0, 67, 208, 1, 0, 0, 0, 69, 210, 1, 0, 0, 0, 71, 212, 1, 0, 0, 0, 73, 214, 1, 0, 0, 0, 75, 218, 1, 0, 0, 0, 77, 220, 1, 0, 0, 0, 79, 222, 1, 0, 0, 0, 81, 224, 1, 0, 0, 0, 83, 228, 1, 0, 0, 0, 85, 232, 1, 0, 0, 0, 87, 88, 5, 91, 0, 0, 88, 2, 1, 0, 0, 0, 89, 90, 5, 93, 0, 0, 90, 4, 1, 0, 0, 0, 91, 92, 5, 91, 0, 0, 92, 93, 5, 91, 0, 0, 93, 6, 1, 0, 0, 0, 94, 95, 5, 93, 0, 0, 95, 96, 5, 93, 0, 0, 96, 8, 1, 0, 0, 0, 97, 98, 5, 61, 0, 0, 98, 99, 5, 61, 0, 0, 99, 100, 5, 61, 0, 0, 100, 101, 5, 61, 0, 0, 101, 102, 5, 61, 0, 0, 102, 103, 5, 61, 0, 0, 103, 104, 5, 61, 0, 0, 104, 10, 1, 0, 0, 0, 105, 106, 5, 42, 0, 0, 106, 107, 5, 42, 0, 0, 107, 108, 5, 42, 0, 0, 108, 109, 5, 42, 0, 0, 109, 110, 5, 42, 0, 0, 110, 12, 1, 0, 0, 0, 111, 113, 5, 13, 0, 0, 112, 111, 1, 0, 0, 0, 112, 113, 1, 0, 0, 0, 113, 114, 1, 0, 0, 0, 114, 115, 5, 10, 0, 0, 115, 14, 1, 0, 0, 0, 116, 117, 5, 111, 0, 0, 117, 16, 1, 0, 0, 0, 118, 119, 5, 120, 0, 0, 119, 18, 1, 0, 0, 0, 120, 125, 3, 83, 41, 0, 121, 124, 3, 85, 42, 0, 122, 124, 3, 41, 20, 0, 123, 121, 1, 0, 0, 0, 123, 122, 1, 0, 0, 0, 124, 127, 1, 0, 0, 0, 125, 123, 1, 0, 0, 0, 125, 126, 1, 0, 0, 0, 126, 20, 1, 0, 0, 0, 127, 125, 1, 0, 0, 0, 128, 129, 5, 50, 0, 0, 129, 130, 3, 77, 38, 0, 130, 131, 3, 77, 38, 0, 131, 132, 3, 77, 38, 0, 132, 133, 3, 35, 17, 0, 133, 134, 3, 81, 40, 0, 134, 135, 3, 77, 38, 0, 135, 136, 3, 35, 17, 0, 136, 137, 3, 79, 39, 0, 137, 138, 3, 77, 38, 0, 138, 22, 1, 0, 0, 0, 139, 140, 2, 48, 50, 0, 140, 141, 3, 77, 38, 0, 141, 142, 2, 48, 53, 0, 142, 143, 3, 77, 38, 0, 143, 24, 1, 0, 0, 0, 144, 145, 3, 77, 38, 0, 145, 146, 3, 77, 38, 0, 146, 147, 3, 81, 40, 0, 147, 148, 3, 77, 38, 0, 148, 149, 3, 79, 39, 0, 149, 150, 3, 77, 38, 0, 150, 151, 3, 51, 25, 0, 151, 152, 3, 75, 37, 0, 152, 154, 3, 75, 37, 0, 153, 155, 3, 75, 37, 0, 154, 153, 1, 0, 0, 0, 154, 155, 1, 0, 0, 0, 155, 26, 1, 0, 0, 0, 156, 161, 3, 77, 38, 0, 157, 160, 3, 85, 42, 0, 158, 160, 3, 41, 20, 0, 159, 157, 1, 0, 0, 0, 159, 158, 1, 0, 0, 0, 160, 163, 1, 0, 0, 0, 161, 159, 1, 0, 0, 0, 161, 162, 1, 0, 0, 0, 162, 28, 1, 0, 0, 0, 163, 161, 1, 0, 0, 0, 164, 165, 5, 32, 0, 0, 165, 166, 5, 32, 0, 0, 166, 167, 5, 45, 0, 0, 167, 30, 1, 0, 0, 0, 168, 169, 5, 32, 0, 0, 169, 170, 5, 32, 0, 0, 170, 171, 5, 32, 0, 0, 171, 172, 5, 32, 0, 0, 172, 173, 5, 45, 0, 0, 173, 32, 1, 0, 0, 0, 174, 175, 7, 0, 0, 0, 175, 34, 1, 0, 0, 0, 176, 177, 5, 45, 0, 0, 177, 36, 1, 0, 0, 0, 178, 179, 5, 46, 0, 0, 179, 38, 1, 0, 0, 0, 180, 181, 5, 47, 0, 0, 181, 40, 1, 0, 0, 0, 182, 183, 5, 95, 0, 0, 183, 42, 1, 0, 0, 0, 184, 185, 5, 58, 0, 0, 185, 44, 1, 0, 0, 0, 186, 187, 5, 32, 0, 0, 187, 46, 1, 0, 0, 0, 188, 189, 5, 40, 0, 0, 189, 48, 1, 0, 0, 0, 190, 191, 5, 41, 0, 0, 191, 50, 1, 0, 0, 0, 192, 193, 5, 35, 0, 0, 193, 52, 1, 0, 0, 0, 194, 195, 5, 64, 0, 0, 195, 54, 1, 0, 0, 0, 196, 197, 5, 43, 0, 0, 197, 56, 1, 0, 0, 0, 198, 199, 5, 37, 0, 0, 199, 58, 1, 0, 0, 0, 200, 201, 5, 39, 0, 0, 201, 60, 1, 0, 0, 0, 202, 203, 5, 34, 0, 0, 203, 62, 1, 0, 0, 0, 204, 205, 5, 126, 0, 0, 205, 64, 1, 0, 0, 0, 206, 207, 5, 42, 0, 0, 207, 66, 1, 0, 0, 0, 208, 209, 5, 60, 0, 0, 209, 68, 1, 0, 0, 0, 210, 211, 5, 62, 0, 0, 211, 70, 1, 0, 0, 0, 212, 213, 2, 65, 90, 0, 213, 72, 1, 0, 0, 0, 214, 215, 2, 97, 122, 0, 215, 74, 1, 0, 0, 0, 216, 219, 3, 77, 38, 0, 217, 219, 7, 1, 0, 0, 218, 216, 1, 0, 0, 0, 218, 217, 1, 0, 0, 0, 219, 76, 1, 0, 0, 0, 220, 221, 2, 48, 57, 0, 221, 78, 1, 0, 0, 0, 222, 223, 2, 48, 51, 0, 223, 80, 1, 0, 0, 0, 224, 225, 2, 48, 49, 0, 225, 82, 1, 0, 0, 0, 226, 229, 3, 71, 35, 0, 227, 229, 3, 73, 36, 0, 228, 226, 1, 0, 0, 0, 228, 227, 1, 0, 0, 0, 229, 84, 1, 0, 0, 0, 230, 233, 3, 83, 41, 0, 231, 233, 3, 77, 38, 0, 232, 230, 1, 0, 0, 0, 232, 231, 1, 0, 0, 0, 233, 86, 1, 0, 0, 0, 10, 0, 112, 123, 125, 154, 159, 161, 218, 228, 232, 0]
```

### Comparing `zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFileLexer.py` & `zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFileLexer.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,82 +6,95 @@
     from typing import TextIO
 else:
     from typing.io import TextIO
 
 
 def serializedATN():
     return [
-        4,0,33,199,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
+        4,0,35,234,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
         2,6,7,6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,
         13,7,13,2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,
         19,2,20,7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,
         26,7,26,2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,
-        32,2,33,7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,1,0,1,0,1,1,
-        1,1,1,2,1,2,1,2,1,3,1,3,1,3,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,5,
-        1,5,1,5,1,5,1,5,1,5,1,6,3,6,103,8,6,1,6,1,6,1,7,1,7,1,8,1,8,1,9,
-        1,9,1,9,5,9,114,8,9,10,9,12,9,117,9,9,1,10,1,10,1,10,1,10,1,10,1,
-        10,1,10,1,10,1,10,1,10,1,10,1,11,1,11,1,11,5,11,133,8,11,10,11,12,
-        11,136,9,11,1,12,1,12,1,12,1,12,1,13,1,13,1,13,1,13,1,13,1,13,1,
-        14,1,14,1,15,1,15,1,16,1,16,1,17,1,17,1,18,1,18,1,19,1,19,1,20,1,
-        20,1,21,1,21,1,22,1,22,1,23,1,23,1,24,1,24,1,25,1,25,1,26,1,26,1,
-        27,1,27,1,28,1,28,1,29,1,29,1,30,1,30,1,31,1,31,1,32,1,32,1,33,1,
-        33,1,34,1,34,1,35,1,35,1,36,1,36,3,36,194,8,36,1,37,1,37,3,37,198,
-        8,37,0,0,38,1,1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,10,21,11,
-        23,12,25,13,27,14,29,15,31,16,33,17,35,18,37,19,39,20,41,21,43,22,
-        45,23,47,24,49,25,51,26,53,27,55,28,57,29,59,30,61,31,63,32,65,33,
-        67,0,69,0,71,0,73,0,75,0,1,0,1,10,0,33,33,36,36,38,38,44,44,59,59,
-        61,61,63,63,91,94,96,96,123,125,200,0,1,1,0,0,0,0,3,1,0,0,0,0,5,
-        1,0,0,0,0,7,1,0,0,0,0,9,1,0,0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,
-        0,0,0,0,17,1,0,0,0,0,19,1,0,0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,
-        0,0,0,0,27,1,0,0,0,0,29,1,0,0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,
-        0,0,0,0,37,1,0,0,0,0,39,1,0,0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,
-        0,0,0,0,47,1,0,0,0,0,49,1,0,0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,
-        0,0,0,0,57,1,0,0,0,0,59,1,0,0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,
-        0,0,0,1,77,1,0,0,0,3,79,1,0,0,0,5,81,1,0,0,0,7,84,1,0,0,0,9,87,1,
-        0,0,0,11,95,1,0,0,0,13,102,1,0,0,0,15,106,1,0,0,0,17,108,1,0,0,0,
-        19,110,1,0,0,0,21,118,1,0,0,0,23,129,1,0,0,0,25,137,1,0,0,0,27,141,
-        1,0,0,0,29,147,1,0,0,0,31,149,1,0,0,0,33,151,1,0,0,0,35,153,1,0,
-        0,0,37,155,1,0,0,0,39,157,1,0,0,0,41,159,1,0,0,0,43,161,1,0,0,0,
-        45,163,1,0,0,0,47,165,1,0,0,0,49,167,1,0,0,0,51,169,1,0,0,0,53,171,
-        1,0,0,0,55,173,1,0,0,0,57,175,1,0,0,0,59,177,1,0,0,0,61,179,1,0,
-        0,0,63,181,1,0,0,0,65,183,1,0,0,0,67,185,1,0,0,0,69,187,1,0,0,0,
-        71,189,1,0,0,0,73,193,1,0,0,0,75,197,1,0,0,0,77,78,5,91,0,0,78,2,
-        1,0,0,0,79,80,5,93,0,0,80,4,1,0,0,0,81,82,5,91,0,0,82,83,5,91,0,
-        0,83,6,1,0,0,0,84,85,5,93,0,0,85,86,5,93,0,0,86,8,1,0,0,0,87,88,
-        5,61,0,0,88,89,5,61,0,0,89,90,5,61,0,0,90,91,5,61,0,0,91,92,5,61,
-        0,0,92,93,5,61,0,0,93,94,5,61,0,0,94,10,1,0,0,0,95,96,5,42,0,0,96,
-        97,5,42,0,0,97,98,5,42,0,0,98,99,5,42,0,0,99,100,5,42,0,0,100,12,
-        1,0,0,0,101,103,5,13,0,0,102,101,1,0,0,0,102,103,1,0,0,0,103,104,
-        1,0,0,0,104,105,5,10,0,0,105,14,1,0,0,0,106,107,5,111,0,0,107,16,
-        1,0,0,0,108,109,5,120,0,0,109,18,1,0,0,0,110,115,3,73,36,0,111,114,
-        3,75,37,0,112,114,3,37,18,0,113,111,1,0,0,0,113,112,1,0,0,0,114,
-        117,1,0,0,0,115,113,1,0,0,0,115,116,1,0,0,0,116,20,1,0,0,0,117,115,
-        1,0,0,0,118,119,5,50,0,0,119,120,3,71,35,0,120,121,3,71,35,0,121,
-        122,3,71,35,0,122,123,3,31,15,0,123,124,2,48,50,0,124,125,3,71,35,
-        0,125,126,3,31,15,0,126,127,2,48,51,0,127,128,3,71,35,0,128,22,1,
-        0,0,0,129,134,3,71,35,0,130,133,3,75,37,0,131,133,3,37,18,0,132,
-        130,1,0,0,0,132,131,1,0,0,0,133,136,1,0,0,0,134,132,1,0,0,0,134,
-        135,1,0,0,0,135,24,1,0,0,0,136,134,1,0,0,0,137,138,5,32,0,0,138,
-        139,5,32,0,0,139,140,5,45,0,0,140,26,1,0,0,0,141,142,5,32,0,0,142,
-        143,5,32,0,0,143,144,5,32,0,0,144,145,5,32,0,0,145,146,5,45,0,0,
-        146,28,1,0,0,0,147,148,7,0,0,0,148,30,1,0,0,0,149,150,5,45,0,0,150,
-        32,1,0,0,0,151,152,5,46,0,0,152,34,1,0,0,0,153,154,5,47,0,0,154,
-        36,1,0,0,0,155,156,5,95,0,0,156,38,1,0,0,0,157,158,5,58,0,0,158,
-        40,1,0,0,0,159,160,5,32,0,0,160,42,1,0,0,0,161,162,5,40,0,0,162,
-        44,1,0,0,0,163,164,5,41,0,0,164,46,1,0,0,0,165,166,5,35,0,0,166,
-        48,1,0,0,0,167,168,5,64,0,0,168,50,1,0,0,0,169,170,5,43,0,0,170,
-        52,1,0,0,0,171,172,5,37,0,0,172,54,1,0,0,0,173,174,5,39,0,0,174,
-        56,1,0,0,0,175,176,5,34,0,0,176,58,1,0,0,0,177,178,5,126,0,0,178,
-        60,1,0,0,0,179,180,5,42,0,0,180,62,1,0,0,0,181,182,5,60,0,0,182,
-        64,1,0,0,0,183,184,5,62,0,0,184,66,1,0,0,0,185,186,2,65,90,0,186,
-        68,1,0,0,0,187,188,2,97,122,0,188,70,1,0,0,0,189,190,2,48,57,0,190,
-        72,1,0,0,0,191,194,3,67,33,0,192,194,3,69,34,0,193,191,1,0,0,0,193,
-        192,1,0,0,0,194,74,1,0,0,0,195,198,3,73,36,0,196,198,3,71,35,0,197,
-        195,1,0,0,0,197,196,1,0,0,0,198,76,1,0,0,0,8,0,102,113,115,132,134,
-        193,197,0
+        32,2,33,7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,
+        39,7,39,2,40,7,40,2,41,7,41,2,42,7,42,1,0,1,0,1,1,1,1,1,2,1,2,1,
+        2,1,3,1,3,1,3,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,
+        5,1,5,1,6,3,6,113,8,6,1,6,1,6,1,7,1,7,1,8,1,8,1,9,1,9,1,9,5,9,124,
+        8,9,10,9,12,9,127,9,9,1,10,1,10,1,10,1,10,1,10,1,10,1,10,1,10,1,
+        10,1,10,1,10,1,11,1,11,1,11,1,11,1,11,1,12,1,12,1,12,1,12,1,12,1,
+        12,1,12,1,12,1,12,1,12,3,12,155,8,12,1,13,1,13,1,13,5,13,160,8,13,
+        10,13,12,13,163,9,13,1,14,1,14,1,14,1,14,1,15,1,15,1,15,1,15,1,15,
+        1,15,1,16,1,16,1,17,1,17,1,18,1,18,1,19,1,19,1,20,1,20,1,21,1,21,
+        1,22,1,22,1,23,1,23,1,24,1,24,1,25,1,25,1,26,1,26,1,27,1,27,1,28,
+        1,28,1,29,1,29,1,30,1,30,1,31,1,31,1,32,1,32,1,33,1,33,1,34,1,34,
+        1,35,1,35,1,36,1,36,1,37,1,37,3,37,219,8,37,1,38,1,38,1,39,1,39,
+        1,40,1,40,1,41,1,41,3,41,229,8,41,1,42,1,42,3,42,233,8,42,0,0,43,
+        1,1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,10,21,11,23,12,25,13,
+        27,14,29,15,31,16,33,17,35,18,37,19,39,20,41,21,43,22,45,23,47,24,
+        49,25,51,26,53,27,55,28,57,29,59,30,61,31,63,32,65,33,67,34,69,35,
+        71,0,73,0,75,0,77,0,79,0,81,0,83,0,85,0,1,0,2,10,0,33,33,36,36,38,
+        38,44,44,59,59,61,61,63,63,91,94,96,96,123,125,6,0,65,72,74,78,80,
+        90,97,105,107,107,109,122,234,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,
+        0,0,7,1,0,0,0,0,9,1,0,0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,
+        0,17,1,0,0,0,0,19,1,0,0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,
+        0,27,1,0,0,0,0,29,1,0,0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,
+        0,37,1,0,0,0,0,39,1,0,0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,
+        0,47,1,0,0,0,0,49,1,0,0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,
+        0,57,1,0,0,0,0,59,1,0,0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,
+        0,67,1,0,0,0,0,69,1,0,0,0,1,87,1,0,0,0,3,89,1,0,0,0,5,91,1,0,0,0,
+        7,94,1,0,0,0,9,97,1,0,0,0,11,105,1,0,0,0,13,112,1,0,0,0,15,116,1,
+        0,0,0,17,118,1,0,0,0,19,120,1,0,0,0,21,128,1,0,0,0,23,139,1,0,0,
+        0,25,144,1,0,0,0,27,156,1,0,0,0,29,164,1,0,0,0,31,168,1,0,0,0,33,
+        174,1,0,0,0,35,176,1,0,0,0,37,178,1,0,0,0,39,180,1,0,0,0,41,182,
+        1,0,0,0,43,184,1,0,0,0,45,186,1,0,0,0,47,188,1,0,0,0,49,190,1,0,
+        0,0,51,192,1,0,0,0,53,194,1,0,0,0,55,196,1,0,0,0,57,198,1,0,0,0,
+        59,200,1,0,0,0,61,202,1,0,0,0,63,204,1,0,0,0,65,206,1,0,0,0,67,208,
+        1,0,0,0,69,210,1,0,0,0,71,212,1,0,0,0,73,214,1,0,0,0,75,218,1,0,
+        0,0,77,220,1,0,0,0,79,222,1,0,0,0,81,224,1,0,0,0,83,228,1,0,0,0,
+        85,232,1,0,0,0,87,88,5,91,0,0,88,2,1,0,0,0,89,90,5,93,0,0,90,4,1,
+        0,0,0,91,92,5,91,0,0,92,93,5,91,0,0,93,6,1,0,0,0,94,95,5,93,0,0,
+        95,96,5,93,0,0,96,8,1,0,0,0,97,98,5,61,0,0,98,99,5,61,0,0,99,100,
+        5,61,0,0,100,101,5,61,0,0,101,102,5,61,0,0,102,103,5,61,0,0,103,
+        104,5,61,0,0,104,10,1,0,0,0,105,106,5,42,0,0,106,107,5,42,0,0,107,
+        108,5,42,0,0,108,109,5,42,0,0,109,110,5,42,0,0,110,12,1,0,0,0,111,
+        113,5,13,0,0,112,111,1,0,0,0,112,113,1,0,0,0,113,114,1,0,0,0,114,
+        115,5,10,0,0,115,14,1,0,0,0,116,117,5,111,0,0,117,16,1,0,0,0,118,
+        119,5,120,0,0,119,18,1,0,0,0,120,125,3,83,41,0,121,124,3,85,42,0,
+        122,124,3,41,20,0,123,121,1,0,0,0,123,122,1,0,0,0,124,127,1,0,0,
+        0,125,123,1,0,0,0,125,126,1,0,0,0,126,20,1,0,0,0,127,125,1,0,0,0,
+        128,129,5,50,0,0,129,130,3,77,38,0,130,131,3,77,38,0,131,132,3,77,
+        38,0,132,133,3,35,17,0,133,134,3,81,40,0,134,135,3,77,38,0,135,136,
+        3,35,17,0,136,137,3,79,39,0,137,138,3,77,38,0,138,22,1,0,0,0,139,
+        140,2,48,50,0,140,141,3,77,38,0,141,142,2,48,53,0,142,143,3,77,38,
+        0,143,24,1,0,0,0,144,145,3,77,38,0,145,146,3,77,38,0,146,147,3,81,
+        40,0,147,148,3,77,38,0,148,149,3,79,39,0,149,150,3,77,38,0,150,151,
+        3,51,25,0,151,152,3,75,37,0,152,154,3,75,37,0,153,155,3,75,37,0,
+        154,153,1,0,0,0,154,155,1,0,0,0,155,26,1,0,0,0,156,161,3,77,38,0,
+        157,160,3,85,42,0,158,160,3,41,20,0,159,157,1,0,0,0,159,158,1,0,
+        0,0,160,163,1,0,0,0,161,159,1,0,0,0,161,162,1,0,0,0,162,28,1,0,0,
+        0,163,161,1,0,0,0,164,165,5,32,0,0,165,166,5,32,0,0,166,167,5,45,
+        0,0,167,30,1,0,0,0,168,169,5,32,0,0,169,170,5,32,0,0,170,171,5,32,
+        0,0,171,172,5,32,0,0,172,173,5,45,0,0,173,32,1,0,0,0,174,175,7,0,
+        0,0,175,34,1,0,0,0,176,177,5,45,0,0,177,36,1,0,0,0,178,179,5,46,
+        0,0,179,38,1,0,0,0,180,181,5,47,0,0,181,40,1,0,0,0,182,183,5,95,
+        0,0,183,42,1,0,0,0,184,185,5,58,0,0,185,44,1,0,0,0,186,187,5,32,
+        0,0,187,46,1,0,0,0,188,189,5,40,0,0,189,48,1,0,0,0,190,191,5,41,
+        0,0,191,50,1,0,0,0,192,193,5,35,0,0,193,52,1,0,0,0,194,195,5,64,
+        0,0,195,54,1,0,0,0,196,197,5,43,0,0,197,56,1,0,0,0,198,199,5,37,
+        0,0,199,58,1,0,0,0,200,201,5,39,0,0,201,60,1,0,0,0,202,203,5,34,
+        0,0,203,62,1,0,0,0,204,205,5,126,0,0,205,64,1,0,0,0,206,207,5,42,
+        0,0,207,66,1,0,0,0,208,209,5,60,0,0,209,68,1,0,0,0,210,211,5,62,
+        0,0,211,70,1,0,0,0,212,213,2,65,90,0,213,72,1,0,0,0,214,215,2,97,
+        122,0,215,74,1,0,0,0,216,219,3,77,38,0,217,219,7,1,0,0,218,216,1,
+        0,0,0,218,217,1,0,0,0,219,76,1,0,0,0,220,221,2,48,57,0,221,78,1,
+        0,0,0,222,223,2,48,51,0,223,80,1,0,0,0,224,225,2,48,49,0,225,82,
+        1,0,0,0,226,229,3,71,35,0,227,229,3,73,36,0,228,226,1,0,0,0,228,
+        227,1,0,0,0,229,84,1,0,0,0,230,233,3,83,41,0,231,233,3,77,38,0,232,
+        230,1,0,0,0,232,231,1,0,0,0,233,86,1,0,0,0,10,0,112,123,125,154,
+        159,161,218,228,232,0
     ]
 
 class ZorgFileLexer(Lexer):
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
@@ -93,60 +106,64 @@
     T__4 = 5
     T__5 = 6
     NL = 7
     LOWER_O = 8
     LOWER_X = 9
     ID = 10
     DATE = 11
-    NUM_ID = 12
-    TWO_SPACE_DASH = 13
-    FOUR_SPACE_DASH = 14
-    SYMBOL = 15
-    DASH = 16
-    DOT = 17
-    FSLASH = 18
-    UNDERSCORE = 19
-    COLON = 20
-    SPACE = 21
-    LPAREN = 22
-    RPAREN = 23
-    HASH = 24
-    AT_SIGN = 25
-    PLUS = 26
-    PERCENT = 27
-    SQUOTE = 28
-    DQUOTE = 29
-    TILDE = 30
-    STAR = 31
-    LANGLE = 32
-    RANGLE = 33
+    TIME = 12
+    ZID = 13
+    NUM_ID = 14
+    TWO_SPACE_DASH = 15
+    FOUR_SPACE_DASH = 16
+    SYMBOL = 17
+    DASH = 18
+    DOT = 19
+    FSLASH = 20
+    UNDERSCORE = 21
+    COLON = 22
+    SPACE = 23
+    LPAREN = 24
+    RPAREN = 25
+    HASH = 26
+    AT_SIGN = 27
+    PLUS = 28
+    PERCENT = 29
+    SQUOTE = 30
+    DQUOTE = 31
+    TILDE = 32
+    STAR = 33
+    LANGLE = 34
+    RANGLE = 35
 
     channelNames = [ u"DEFAULT_TOKEN_CHANNEL", u"HIDDEN" ]
 
     modeNames = [ "DEFAULT_MODE" ]
 
     literalNames = [ "<INVALID>",
             "'['", "']'", "'[['", "']]'", "'======='", "'*****'", "'o'", 
             "'x'", "'  -'", "'    -'", "'-'", "'.'", "'/'", "'_'", "':'", 
             "' '", "'('", "')'", "'#'", "'@'", "'+'", "'%'", "'''", "'\"'", 
             "'~'", "'*'", "'<'", "'>'" ]
 
     symbolicNames = [ "<INVALID>",
-            "NL", "LOWER_O", "LOWER_X", "ID", "DATE", "NUM_ID", "TWO_SPACE_DASH", 
-            "FOUR_SPACE_DASH", "SYMBOL", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
-            "COLON", "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", 
-            "PERCENT", "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE" ]
+            "NL", "LOWER_O", "LOWER_X", "ID", "DATE", "TIME", "ZID", "NUM_ID", 
+            "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", "DOT", 
+            "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", "RPAREN", 
+            "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", "DQUOTE", "TILDE", 
+            "STAR", "LANGLE", "RANGLE" ]
 
     ruleNames = [ "T__0", "T__1", "T__2", "T__3", "T__4", "T__5", "NL", 
-                  "LOWER_O", "LOWER_X", "ID", "DATE", "NUM_ID", "TWO_SPACE_DASH", 
-                  "FOUR_SPACE_DASH", "SYMBOL", "DASH", "DOT", "FSLASH", 
-                  "UNDERSCORE", "COLON", "SPACE", "LPAREN", "RPAREN", "HASH", 
-                  "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", "DQUOTE", "TILDE", 
-                  "STAR", "LANGLE", "RANGLE", "UPPER_LETTER", "LOWER_LETTER", 
-                  "NUM", "ALPHA", "ALPHANUM" ]
+                  "LOWER_O", "LOWER_X", "ID", "DATE", "TIME", "ZID", "NUM_ID", 
+                  "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", 
+                  "DOT", "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", 
+                  "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", 
+                  "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE", "UPPER_LETTER", 
+                  "LOWER_LETTER", "ZID_CHAR", "NUM", "FIRST_D_NUM", "FIRST_M_NUM", 
+                  "ALPHA", "ALPHANUM" ]
 
     grammarFileName = "ZorgFile.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
```

### Comparing `zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFileListener.py` & `zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFileListener.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,29 +49,20 @@
         pass
 
     # Exit a parse tree produced by ZorgFileParser#item.
     def exitItem(self, ctx:ZorgFileParser.ItemContext):
         pass
 
 
-    # Enter a parse tree produced by ZorgFileParser#todo.
-    def enterTodo(self, ctx:ZorgFileParser.TodoContext):
-        pass
-
-    # Exit a parse tree produced by ZorgFileParser#todo.
-    def exitTodo(self, ctx:ZorgFileParser.TodoContext):
-        pass
-
-
-    # Enter a parse tree produced by ZorgFileParser#priority.
-    def enterPriority(self, ctx:ZorgFileParser.PriorityContext):
+    # Enter a parse tree produced by ZorgFileParser#footnote.
+    def enterFootnote(self, ctx:ZorgFileParser.FootnoteContext):
         pass
 
-    # Exit a parse tree produced by ZorgFileParser#priority.
-    def exitPriority(self, ctx:ZorgFileParser.PriorityContext):
+    # Exit a parse tree produced by ZorgFileParser#footnote.
+    def exitFootnote(self, ctx:ZorgFileParser.FootnoteContext):
         pass
 
 
     # Enter a parse tree produced by ZorgFileParser#note.
     def enterNote(self, ctx:ZorgFileParser.NoteContext):
         pass
 
@@ -85,20 +76,29 @@
         pass
 
     # Exit a parse tree produced by ZorgFileParser#base_note.
     def exitBase_note(self, ctx:ZorgFileParser.Base_noteContext):
         pass
 
 
-    # Enter a parse tree produced by ZorgFileParser#base_todo.
-    def enterBase_todo(self, ctx:ZorgFileParser.Base_todoContext):
+    # Enter a parse tree produced by ZorgFileParser#id_note_body.
+    def enterId_note_body(self, ctx:ZorgFileParser.Id_note_bodyContext):
         pass
 
-    # Exit a parse tree produced by ZorgFileParser#base_todo.
-    def exitBase_todo(self, ctx:ZorgFileParser.Base_todoContext):
+    # Exit a parse tree produced by ZorgFileParser#id_note_body.
+    def exitId_note_body(self, ctx:ZorgFileParser.Id_note_bodyContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgFileParser#note_body.
+    def enterNote_body(self, ctx:ZorgFileParser.Note_bodyContext):
+        pass
+
+    # Exit a parse tree produced by ZorgFileParser#note_body.
+    def exitNote_body(self, ctx:ZorgFileParser.Note_bodyContext):
         pass
 
 
     # Enter a parse tree produced by ZorgFileParser#subnote.
     def enterSubnote(self, ctx:ZorgFileParser.SubnoteContext):
         pass
 
@@ -112,29 +112,65 @@
         pass
 
     # Exit a parse tree produced by ZorgFileParser#subsubnote.
     def exitSubsubnote(self, ctx:ZorgFileParser.SubsubnoteContext):
         pass
 
 
-    # Enter a parse tree produced by ZorgFileParser#item_body.
-    def enterItem_body(self, ctx:ZorgFileParser.Item_bodyContext):
+    # Enter a parse tree produced by ZorgFileParser#todo.
+    def enterTodo(self, ctx:ZorgFileParser.TodoContext):
         pass
 
-    # Exit a parse tree produced by ZorgFileParser#item_body.
-    def exitItem_body(self, ctx:ZorgFileParser.Item_bodyContext):
+    # Exit a parse tree produced by ZorgFileParser#todo.
+    def exitTodo(self, ctx:ZorgFileParser.TodoContext):
         pass
 
 
-    # Enter a parse tree produced by ZorgFileParser#footnote.
-    def enterFootnote(self, ctx:ZorgFileParser.FootnoteContext):
+    # Enter a parse tree produced by ZorgFileParser#base_todo.
+    def enterBase_todo(self, ctx:ZorgFileParser.Base_todoContext):
         pass
 
-    # Exit a parse tree produced by ZorgFileParser#footnote.
-    def exitFootnote(self, ctx:ZorgFileParser.FootnoteContext):
+    # Exit a parse tree produced by ZorgFileParser#base_todo.
+    def exitBase_todo(self, ctx:ZorgFileParser.Base_todoContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgFileParser#todo_prefix.
+    def enterTodo_prefix(self, ctx:ZorgFileParser.Todo_prefixContext):
+        pass
+
+    # Exit a parse tree produced by ZorgFileParser#todo_prefix.
+    def exitTodo_prefix(self, ctx:ZorgFileParser.Todo_prefixContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgFileParser#x_or_tilde.
+    def enterX_or_tilde(self, ctx:ZorgFileParser.X_or_tildeContext):
+        pass
+
+    # Exit a parse tree produced by ZorgFileParser#x_or_tilde.
+    def exitX_or_tilde(self, ctx:ZorgFileParser.X_or_tildeContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgFileParser#priority.
+    def enterPriority(self, ctx:ZorgFileParser.PriorityContext):
+        pass
+
+    # Exit a parse tree produced by ZorgFileParser#priority.
+    def exitPriority(self, ctx:ZorgFileParser.PriorityContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgFileParser#zid.
+    def enterZid(self, ctx:ZorgFileParser.ZidContext):
+        pass
+
+    # Exit a parse tree produced by ZorgFileParser#zid.
+    def exitZid(self, ctx:ZorgFileParser.ZidContext):
         pass
 
 
     # Enter a parse tree produced by ZorgFileParser#space_atoms.
     def enterSpace_atoms(self, ctx:ZorgFileParser.Space_atomsContext):
         pass
 
@@ -193,14 +229,23 @@
         pass
 
     # Exit a parse tree produced by ZorgFileParser#date.
     def exitDate(self, ctx:ZorgFileParser.DateContext):
         pass
 
 
+    # Enter a parse tree produced by ZorgFileParser#time.
+    def enterTime(self, ctx:ZorgFileParser.TimeContext):
+        pass
+
+    # Exit a parse tree produced by ZorgFileParser#time.
+    def exitTime(self, ctx:ZorgFileParser.TimeContext):
+        pass
+
+
     # Enter a parse tree produced by ZorgFileParser#any_symbol.
     def enterAny_symbol(self, ctx:ZorgFileParser.Any_symbolContext):
         pass
 
     # Exit a parse tree produced by ZorgFileParser#any_symbol.
     def exitAny_symbol(self, ctx:ZorgFileParser.Any_symbolContext):
         pass
@@ -373,9 +418,18 @@
         pass
 
     # Exit a parse tree produced by ZorgFileParser#h4_header.
     def exitH4_header(self, ctx:ZorgFileParser.H4_headerContext):
         pass
 
 
+    # Enter a parse tree produced by ZorgFileParser#eol.
+    def enterEol(self, ctx:ZorgFileParser.EolContext):
+        pass
+
+    # Exit a parse tree produced by ZorgFileParser#eol.
+    def exitEol(self, ctx:ZorgFileParser.EolContext):
+        pass
+
+
 
 del ZorgFileParser
```

### Comparing `zettel-org-0.6.0/src/zorg/grammar/zorg_file/ZorgFileParser.py` & `zettel_org-0.6.1/src/zorg/grammar/zorg_file/ZorgFileParser.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,273 +6,305 @@
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
-        4,1,33,407,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        4,1,35,468,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
         6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,13,7,13,
         2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,19,2,20,
         7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,26,7,26,
         2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,32,2,33,
         7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,39,7,39,
-        2,40,7,40,1,0,1,0,4,0,85,8,0,11,0,12,0,86,1,0,5,0,90,8,0,10,0,12,
-        0,93,9,0,1,0,5,0,96,8,0,10,0,12,0,99,9,0,1,0,5,0,102,8,0,10,0,12,
-        0,105,9,0,3,0,107,8,0,1,0,1,0,1,1,4,1,112,8,1,11,1,12,1,113,1,2,
-        1,2,3,2,118,8,2,1,2,1,2,1,3,4,3,123,8,3,11,3,12,3,124,1,3,5,3,128,
-        8,3,10,3,12,3,131,9,3,1,4,1,4,1,4,1,4,3,4,137,8,4,1,5,1,5,5,5,141,
-        8,5,10,5,12,5,144,9,5,1,6,1,6,1,6,1,6,1,6,1,7,1,7,1,7,5,7,154,8,
-        7,10,7,12,7,157,9,7,1,8,1,8,1,8,1,9,1,9,1,9,3,9,165,8,9,1,9,1,9,
-        1,9,1,10,1,10,1,10,5,10,173,8,10,10,10,12,10,176,9,10,1,11,1,11,
-        1,11,1,12,1,12,1,12,4,12,184,8,12,11,12,12,12,185,1,12,5,12,189,
-        8,12,10,12,12,12,192,9,12,1,13,1,13,1,13,1,13,1,14,4,14,199,8,14,
-        11,14,12,14,200,1,15,1,15,1,15,3,15,206,8,15,1,15,1,15,5,15,210,
-        8,15,10,15,12,15,213,9,15,1,15,1,15,3,15,217,8,15,1,15,1,15,1,15,
-        5,15,222,8,15,10,15,12,15,225,9,15,3,15,227,8,15,1,15,3,15,230,8,
-        15,1,16,1,16,1,16,1,16,1,16,1,16,3,16,238,8,16,1,17,1,17,1,17,1,
-        17,1,17,1,18,1,18,4,18,247,8,18,11,18,12,18,248,1,18,1,18,5,18,253,
-        8,18,10,18,12,18,256,9,18,1,19,1,19,1,19,1,19,1,19,3,19,263,8,19,
-        1,20,1,20,1,21,1,21,1,21,1,21,1,21,3,21,272,8,21,1,22,1,22,1,23,
-        1,23,1,24,1,24,1,25,1,25,1,25,1,25,3,25,284,8,25,1,26,1,26,1,26,
-        1,27,1,27,1,27,1,28,1,28,1,28,1,29,1,29,1,29,1,30,1,30,1,30,1,30,
-        1,30,4,30,303,8,30,11,30,12,30,304,1,30,1,30,1,30,4,30,310,8,30,
-        11,30,12,30,311,1,30,1,30,3,30,316,8,30,1,31,1,31,1,31,1,31,1,32,
-        1,32,1,32,1,32,1,33,1,33,5,33,328,8,33,10,33,12,33,331,9,33,1,33,
-        3,33,334,8,33,1,33,5,33,337,8,33,10,33,12,33,340,9,33,1,34,1,34,
-        5,34,344,8,34,10,34,12,34,347,9,34,1,34,3,34,350,8,34,1,34,5,34,
-        353,8,34,10,34,12,34,356,9,34,1,35,1,35,5,35,360,8,35,10,35,12,35,
-        363,9,35,1,35,3,35,366,8,35,1,35,5,35,369,8,35,10,35,12,35,372,9,
-        35,1,36,1,36,5,36,376,8,36,10,36,12,36,379,9,36,1,37,1,37,1,37,1,
-        37,1,37,1,37,1,37,1,37,1,37,1,37,1,37,1,37,1,38,1,38,1,38,1,38,1,
-        39,1,39,1,39,1,39,1,40,1,40,1,40,1,40,1,40,1,40,1,40,0,0,41,0,2,
-        4,6,8,10,12,14,16,18,20,22,24,26,28,30,32,34,36,38,40,42,44,46,48,
-        50,52,54,56,58,60,62,64,66,68,70,72,74,76,78,80,0,4,3,0,8,9,30,30,
-        32,33,4,0,15,15,19,19,22,23,30,33,2,0,16,18,20,20,1,0,24,27,427,
-        0,82,1,0,0,0,2,111,1,0,0,0,4,115,1,0,0,0,6,122,1,0,0,0,8,136,1,0,
-        0,0,10,138,1,0,0,0,12,145,1,0,0,0,14,150,1,0,0,0,16,158,1,0,0,0,
-        18,161,1,0,0,0,20,169,1,0,0,0,22,177,1,0,0,0,24,180,1,0,0,0,26,193,
-        1,0,0,0,28,198,1,0,0,0,30,202,1,0,0,0,32,237,1,0,0,0,34,239,1,0,
-        0,0,36,244,1,0,0,0,38,262,1,0,0,0,40,264,1,0,0,0,42,271,1,0,0,0,
-        44,273,1,0,0,0,46,275,1,0,0,0,48,277,1,0,0,0,50,283,1,0,0,0,52,285,
-        1,0,0,0,54,288,1,0,0,0,56,291,1,0,0,0,58,294,1,0,0,0,60,315,1,0,
-        0,0,62,317,1,0,0,0,64,321,1,0,0,0,66,325,1,0,0,0,68,341,1,0,0,0,
-        70,357,1,0,0,0,72,373,1,0,0,0,74,380,1,0,0,0,76,392,1,0,0,0,78,396,
-        1,0,0,0,80,400,1,0,0,0,82,106,3,2,1,0,83,85,5,7,0,0,84,83,1,0,0,
-        0,85,86,1,0,0,0,86,84,1,0,0,0,86,87,1,0,0,0,87,91,1,0,0,0,88,90,
-        3,6,3,0,89,88,1,0,0,0,90,93,1,0,0,0,91,89,1,0,0,0,91,92,1,0,0,0,
-        92,97,1,0,0,0,93,91,1,0,0,0,94,96,3,68,34,0,95,94,1,0,0,0,96,99,
-        1,0,0,0,97,95,1,0,0,0,97,98,1,0,0,0,98,103,1,0,0,0,99,97,1,0,0,0,
-        100,102,3,66,33,0,101,100,1,0,0,0,102,105,1,0,0,0,103,101,1,0,0,
-        0,103,104,1,0,0,0,104,107,1,0,0,0,105,103,1,0,0,0,106,84,1,0,0,0,
-        106,107,1,0,0,0,107,108,1,0,0,0,108,109,5,0,0,1,109,1,1,0,0,0,110,
-        112,3,4,2,0,111,110,1,0,0,0,112,113,1,0,0,0,113,111,1,0,0,0,113,
-        114,1,0,0,0,114,3,1,0,0,0,115,117,5,24,0,0,116,118,3,28,14,0,117,
-        116,1,0,0,0,117,118,1,0,0,0,118,119,1,0,0,0,119,120,5,7,0,0,120,
-        5,1,0,0,0,121,123,3,8,4,0,122,121,1,0,0,0,123,124,1,0,0,0,124,122,
-        1,0,0,0,124,125,1,0,0,0,125,129,1,0,0,0,126,128,5,7,0,0,127,126,
-        1,0,0,0,128,131,1,0,0,0,129,127,1,0,0,0,129,130,1,0,0,0,130,7,1,
-        0,0,0,131,129,1,0,0,0,132,137,3,10,5,0,133,137,3,14,7,0,134,137,
-        3,26,13,0,135,137,3,4,2,0,136,132,1,0,0,0,136,133,1,0,0,0,136,134,
-        1,0,0,0,136,135,1,0,0,0,137,9,1,0,0,0,138,142,3,18,9,0,139,141,3,
-        20,10,0,140,139,1,0,0,0,141,144,1,0,0,0,142,140,1,0,0,0,142,143,
-        1,0,0,0,143,11,1,0,0,0,144,142,1,0,0,0,145,146,5,1,0,0,146,147,5,
-        24,0,0,147,148,5,10,0,0,148,149,5,2,0,0,149,13,1,0,0,0,150,151,5,
-        16,0,0,151,155,3,16,8,0,152,154,3,20,10,0,153,152,1,0,0,0,154,157,
-        1,0,0,0,155,153,1,0,0,0,155,156,1,0,0,0,156,15,1,0,0,0,157,155,1,
-        0,0,0,158,159,3,24,12,0,159,160,5,7,0,0,160,17,1,0,0,0,161,164,7,
-        0,0,0,162,163,5,21,0,0,163,165,3,12,6,0,164,162,1,0,0,0,164,165,
-        1,0,0,0,165,166,1,0,0,0,166,167,3,24,12,0,167,168,5,7,0,0,168,19,
-        1,0,0,0,169,170,5,13,0,0,170,174,3,16,8,0,171,173,3,22,11,0,172,
-        171,1,0,0,0,173,176,1,0,0,0,174,172,1,0,0,0,174,175,1,0,0,0,175,
-        21,1,0,0,0,176,174,1,0,0,0,177,178,5,14,0,0,178,179,3,16,8,0,179,
-        23,1,0,0,0,180,190,3,28,14,0,181,183,5,7,0,0,182,184,5,21,0,0,183,
-        182,1,0,0,0,184,185,1,0,0,0,185,183,1,0,0,0,185,186,1,0,0,0,186,
-        187,1,0,0,0,187,189,3,28,14,0,188,181,1,0,0,0,189,192,1,0,0,0,190,
-        188,1,0,0,0,190,191,1,0,0,0,191,25,1,0,0,0,192,190,1,0,0,0,193,194,
-        3,64,32,0,194,195,5,20,0,0,195,196,3,28,14,0,196,27,1,0,0,0,197,
-        199,3,30,15,0,198,197,1,0,0,0,199,200,1,0,0,0,200,198,1,0,0,0,200,
-        201,1,0,0,0,201,29,1,0,0,0,202,205,5,21,0,0,203,204,5,28,0,0,204,
-        206,3,44,22,0,205,203,1,0,0,0,205,206,1,0,0,0,206,211,1,0,0,0,207,
-        210,3,44,22,0,208,210,5,29,0,0,209,207,1,0,0,0,209,208,1,0,0,0,210,
-        213,1,0,0,0,211,209,1,0,0,0,211,212,1,0,0,0,212,216,1,0,0,0,213,
-        211,1,0,0,0,214,217,3,32,16,0,215,217,3,60,30,0,216,214,1,0,0,0,
-        216,215,1,0,0,0,216,217,1,0,0,0,217,226,1,0,0,0,218,223,3,42,21,
-        0,219,222,3,42,21,0,220,222,3,38,19,0,221,219,1,0,0,0,221,220,1,
-        0,0,0,222,225,1,0,0,0,223,221,1,0,0,0,223,224,1,0,0,0,224,227,1,
-        0,0,0,225,223,1,0,0,0,226,218,1,0,0,0,226,227,1,0,0,0,227,229,1,
-        0,0,0,228,230,3,64,32,0,229,228,1,0,0,0,229,230,1,0,0,0,230,31,1,
-        0,0,0,231,238,3,48,24,0,232,238,3,50,25,0,233,238,3,62,31,0,234,
-        238,3,34,17,0,235,238,3,36,18,0,236,238,3,64,32,0,237,231,1,0,0,
-        0,237,232,1,0,0,0,237,233,1,0,0,0,237,234,1,0,0,0,237,235,1,0,0,
-        0,237,236,1,0,0,0,238,33,1,0,0,0,239,240,5,10,0,0,240,241,5,20,0,
-        0,241,242,5,20,0,0,242,243,3,36,18,0,243,35,1,0,0,0,244,254,3,38,
-        19,0,245,247,3,46,23,0,246,245,1,0,0,0,247,248,1,0,0,0,248,246,1,
-        0,0,0,248,249,1,0,0,0,249,250,1,0,0,0,250,251,3,38,19,0,251,253,
-        1,0,0,0,252,246,1,0,0,0,253,256,1,0,0,0,254,252,1,0,0,0,254,255,
-        1,0,0,0,255,37,1,0,0,0,256,254,1,0,0,0,257,263,5,10,0,0,258,263,
-        5,12,0,0,259,263,3,40,20,0,260,263,5,8,0,0,261,263,5,9,0,0,262,257,
-        1,0,0,0,262,258,1,0,0,0,262,259,1,0,0,0,262,260,1,0,0,0,262,261,
-        1,0,0,0,263,39,1,0,0,0,264,265,5,11,0,0,265,41,1,0,0,0,266,272,5,
-        28,0,0,267,272,5,29,0,0,268,272,3,44,22,0,269,272,3,48,24,0,270,
-        272,3,46,23,0,271,266,1,0,0,0,271,267,1,0,0,0,271,268,1,0,0,0,271,
-        269,1,0,0,0,271,270,1,0,0,0,272,43,1,0,0,0,273,274,7,1,0,0,274,45,
-        1,0,0,0,275,276,7,2,0,0,276,47,1,0,0,0,277,278,7,3,0,0,278,49,1,
-        0,0,0,279,284,3,52,26,0,280,284,3,54,27,0,281,284,3,56,28,0,282,
-        284,3,58,29,0,283,279,1,0,0,0,283,280,1,0,0,0,283,281,1,0,0,0,283,
-        282,1,0,0,0,284,51,1,0,0,0,285,286,5,24,0,0,286,287,5,10,0,0,287,
-        53,1,0,0,0,288,289,5,25,0,0,289,290,5,10,0,0,290,55,1,0,0,0,291,
-        292,5,27,0,0,292,293,5,10,0,0,293,57,1,0,0,0,294,295,5,26,0,0,295,
-        296,5,10,0,0,296,59,1,0,0,0,297,302,5,28,0,0,298,303,3,32,16,0,299,
-        303,3,12,6,0,300,303,5,3,0,0,301,303,5,4,0,0,302,298,1,0,0,0,302,
-        299,1,0,0,0,302,300,1,0,0,0,302,301,1,0,0,0,303,304,1,0,0,0,304,
-        302,1,0,0,0,304,305,1,0,0,0,305,306,1,0,0,0,306,316,5,28,0,0,307,
-        309,5,29,0,0,308,310,3,32,16,0,309,308,1,0,0,0,310,311,1,0,0,0,311,
-        309,1,0,0,0,311,312,1,0,0,0,312,313,1,0,0,0,313,314,5,29,0,0,314,
-        316,1,0,0,0,315,297,1,0,0,0,315,307,1,0,0,0,316,61,1,0,0,0,317,318,
-        5,3,0,0,318,319,3,36,18,0,319,320,5,4,0,0,320,63,1,0,0,0,321,322,
-        5,1,0,0,322,323,3,36,18,0,323,324,5,2,0,0,324,65,1,0,0,0,325,329,
-        3,74,37,0,326,328,3,6,3,0,327,326,1,0,0,0,328,331,1,0,0,0,329,327,
-        1,0,0,0,329,330,1,0,0,0,330,338,1,0,0,0,331,329,1,0,0,0,332,334,
-        5,7,0,0,333,332,1,0,0,0,333,334,1,0,0,0,334,335,1,0,0,0,335,337,
-        3,68,34,0,336,333,1,0,0,0,337,340,1,0,0,0,338,336,1,0,0,0,338,339,
-        1,0,0,0,339,67,1,0,0,0,340,338,1,0,0,0,341,345,3,76,38,0,342,344,
-        3,6,3,0,343,342,1,0,0,0,344,347,1,0,0,0,345,343,1,0,0,0,345,346,
-        1,0,0,0,346,354,1,0,0,0,347,345,1,0,0,0,348,350,5,7,0,0,349,348,
-        1,0,0,0,349,350,1,0,0,0,350,351,1,0,0,0,351,353,3,70,35,0,352,349,
-        1,0,0,0,353,356,1,0,0,0,354,352,1,0,0,0,354,355,1,0,0,0,355,69,1,
-        0,0,0,356,354,1,0,0,0,357,361,3,78,39,0,358,360,3,6,3,0,359,358,
-        1,0,0,0,360,363,1,0,0,0,361,359,1,0,0,0,361,362,1,0,0,0,362,370,
-        1,0,0,0,363,361,1,0,0,0,364,366,5,7,0,0,365,364,1,0,0,0,365,366,
-        1,0,0,0,366,367,1,0,0,0,367,369,3,72,36,0,368,365,1,0,0,0,369,372,
-        1,0,0,0,370,368,1,0,0,0,370,371,1,0,0,0,371,71,1,0,0,0,372,370,1,
-        0,0,0,373,377,3,80,40,0,374,376,3,6,3,0,375,374,1,0,0,0,376,379,
-        1,0,0,0,377,375,1,0,0,0,377,378,1,0,0,0,378,73,1,0,0,0,379,377,1,
-        0,0,0,380,381,5,24,0,0,381,382,5,24,0,0,382,383,5,24,0,0,383,384,
-        5,24,0,0,384,385,5,24,0,0,385,386,5,24,0,0,386,387,5,24,0,0,387,
-        388,5,24,0,0,388,389,5,24,0,0,389,390,3,28,14,0,390,391,5,7,0,0,
-        391,75,1,0,0,0,392,393,5,5,0,0,393,394,3,28,14,0,394,395,5,7,0,0,
-        395,77,1,0,0,0,396,397,5,6,0,0,397,398,3,28,14,0,398,399,5,7,0,0,
-        399,79,1,0,0,0,400,401,5,16,0,0,401,402,5,16,0,0,402,403,5,16,0,
-        0,403,404,3,28,14,0,404,405,5,7,0,0,405,81,1,0,0,0,45,86,91,97,103,
-        106,113,117,124,129,136,142,155,164,174,185,190,200,205,209,211,
-        216,221,223,226,229,237,248,254,262,271,283,302,304,311,315,329,
-        333,338,345,349,354,361,365,370,377
+        2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,45,2,46,
+        7,46,1,0,1,0,4,0,97,8,0,11,0,12,0,98,1,0,5,0,102,8,0,10,0,12,0,105,
+        9,0,1,0,5,0,108,8,0,10,0,12,0,111,9,0,1,0,5,0,114,8,0,10,0,12,0,
+        117,9,0,3,0,119,8,0,1,0,1,0,1,1,4,1,124,8,1,11,1,12,1,125,1,2,1,
+        2,3,2,130,8,2,1,2,1,2,1,3,4,3,135,8,3,11,3,12,3,136,1,3,5,3,140,
+        8,3,10,3,12,3,143,9,3,1,4,1,4,1,4,1,4,3,4,149,8,4,1,5,1,5,1,5,1,
+        5,1,5,1,6,1,6,1,6,5,6,159,8,6,10,6,12,6,162,9,6,1,7,1,7,1,7,1,8,
+        1,8,3,8,169,8,8,1,8,1,8,1,9,1,9,1,9,4,9,176,8,9,11,9,12,9,177,1,
+        9,5,9,181,8,9,10,9,12,9,184,9,9,1,10,1,10,1,10,5,10,189,8,10,10,
+        10,12,10,192,9,10,1,11,1,11,1,11,1,12,1,12,5,12,199,8,12,10,12,12,
+        12,202,9,12,1,13,1,13,1,13,3,13,207,8,13,1,13,1,13,1,13,1,14,1,14,
+        1,14,1,14,3,14,216,8,14,1,15,1,15,1,15,3,15,221,8,15,1,16,1,16,1,
+        16,1,16,1,16,1,17,1,17,1,18,4,18,231,8,18,11,18,12,18,232,1,19,1,
+        19,1,19,3,19,238,8,19,1,19,1,19,5,19,242,8,19,10,19,12,19,245,9,
+        19,1,19,1,19,3,19,249,8,19,1,19,1,19,1,19,5,19,254,8,19,10,19,12,
+        19,257,9,19,3,19,259,8,19,1,19,3,19,262,8,19,1,20,1,20,1,20,1,20,
+        1,20,1,20,3,20,270,8,20,1,21,1,21,1,21,1,21,1,21,1,22,1,22,4,22,
+        279,8,22,11,22,12,22,280,1,22,1,22,5,22,285,8,22,10,22,12,22,288,
+        9,22,1,23,1,23,1,23,1,23,1,23,1,23,3,23,296,8,23,1,24,1,24,1,25,
+        1,25,1,26,1,26,1,26,1,26,1,26,3,26,307,8,26,1,27,1,27,1,28,1,28,
+        1,29,1,29,1,30,1,30,1,30,1,30,3,30,319,8,30,1,31,1,31,1,31,1,32,
+        1,32,1,32,1,33,1,33,1,33,1,34,1,34,1,34,1,35,1,35,1,35,1,35,1,35,
+        4,35,338,8,35,11,35,12,35,339,1,35,1,35,1,35,4,35,345,8,35,11,35,
+        12,35,346,1,35,1,35,3,35,351,8,35,1,36,1,36,1,36,1,36,1,37,1,37,
+        1,37,1,37,1,38,1,38,5,38,363,8,38,10,38,12,38,366,9,38,1,38,5,38,
+        369,8,38,10,38,12,38,372,9,38,1,38,3,38,375,8,38,1,38,5,38,378,8,
+        38,10,38,12,38,381,9,38,1,39,1,39,5,39,385,8,39,10,39,12,39,388,
+        9,39,1,39,5,39,391,8,39,10,39,12,39,394,9,39,1,39,3,39,397,8,39,
+        1,39,5,39,400,8,39,10,39,12,39,403,9,39,1,40,1,40,5,40,407,8,40,
+        10,40,12,40,410,9,40,1,40,5,40,413,8,40,10,40,12,40,416,9,40,1,40,
+        3,40,419,8,40,1,40,5,40,422,8,40,10,40,12,40,425,9,40,1,41,1,41,
+        5,41,429,8,41,10,41,12,41,432,9,41,1,41,5,41,435,8,41,10,41,12,41,
+        438,9,41,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,1,42,
+        1,42,1,43,1,43,1,43,1,43,1,44,1,44,1,44,1,44,1,45,1,45,1,45,1,45,
+        1,45,1,45,1,46,1,46,1,46,0,0,47,0,2,4,6,8,10,12,14,16,18,20,22,24,
+        26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,58,60,62,64,66,68,
+        70,72,74,76,78,80,82,84,86,88,90,92,0,5,2,0,9,9,32,32,4,0,17,17,
+        21,21,24,25,32,35,2,0,18,20,22,22,1,0,26,29,1,1,7,7,492,0,94,1,0,
+        0,0,2,123,1,0,0,0,4,127,1,0,0,0,6,134,1,0,0,0,8,148,1,0,0,0,10,150,
+        1,0,0,0,12,155,1,0,0,0,14,163,1,0,0,0,16,168,1,0,0,0,18,172,1,0,
+        0,0,20,185,1,0,0,0,22,193,1,0,0,0,24,196,1,0,0,0,26,203,1,0,0,0,
+        28,215,1,0,0,0,30,217,1,0,0,0,32,222,1,0,0,0,34,227,1,0,0,0,36,230,
+        1,0,0,0,38,234,1,0,0,0,40,269,1,0,0,0,42,271,1,0,0,0,44,276,1,0,
+        0,0,46,295,1,0,0,0,48,297,1,0,0,0,50,299,1,0,0,0,52,306,1,0,0,0,
+        54,308,1,0,0,0,56,310,1,0,0,0,58,312,1,0,0,0,60,318,1,0,0,0,62,320,
+        1,0,0,0,64,323,1,0,0,0,66,326,1,0,0,0,68,329,1,0,0,0,70,350,1,0,
+        0,0,72,352,1,0,0,0,74,356,1,0,0,0,76,360,1,0,0,0,78,382,1,0,0,0,
+        80,404,1,0,0,0,82,426,1,0,0,0,84,439,1,0,0,0,86,451,1,0,0,0,88,455,
+        1,0,0,0,90,459,1,0,0,0,92,465,1,0,0,0,94,118,3,2,1,0,95,97,5,7,0,
+        0,96,95,1,0,0,0,97,98,1,0,0,0,98,96,1,0,0,0,98,99,1,0,0,0,99,103,
+        1,0,0,0,100,102,3,6,3,0,101,100,1,0,0,0,102,105,1,0,0,0,103,101,
+        1,0,0,0,103,104,1,0,0,0,104,109,1,0,0,0,105,103,1,0,0,0,106,108,
+        3,78,39,0,107,106,1,0,0,0,108,111,1,0,0,0,109,107,1,0,0,0,109,110,
+        1,0,0,0,110,115,1,0,0,0,111,109,1,0,0,0,112,114,3,76,38,0,113,112,
+        1,0,0,0,114,117,1,0,0,0,115,113,1,0,0,0,115,116,1,0,0,0,116,119,
+        1,0,0,0,117,115,1,0,0,0,118,96,1,0,0,0,118,119,1,0,0,0,119,120,1,
+        0,0,0,120,121,5,0,0,1,121,1,1,0,0,0,122,124,3,4,2,0,123,122,1,0,
+        0,0,124,125,1,0,0,0,125,123,1,0,0,0,125,126,1,0,0,0,126,3,1,0,0,
+        0,127,129,5,26,0,0,128,130,3,36,18,0,129,128,1,0,0,0,129,130,1,0,
+        0,0,130,131,1,0,0,0,131,132,5,7,0,0,132,5,1,0,0,0,133,135,3,8,4,
+        0,134,133,1,0,0,0,135,136,1,0,0,0,136,134,1,0,0,0,136,137,1,0,0,
+        0,137,141,1,0,0,0,138,140,5,7,0,0,139,138,1,0,0,0,140,143,1,0,0,
+        0,141,139,1,0,0,0,141,142,1,0,0,0,142,7,1,0,0,0,143,141,1,0,0,0,
+        144,149,3,24,12,0,145,149,3,12,6,0,146,149,3,10,5,0,147,149,3,4,
+        2,0,148,144,1,0,0,0,148,145,1,0,0,0,148,146,1,0,0,0,148,147,1,0,
+        0,0,149,9,1,0,0,0,150,151,3,74,37,0,151,152,5,22,0,0,152,153,3,36,
+        18,0,153,154,5,7,0,0,154,11,1,0,0,0,155,156,5,18,0,0,156,160,3,14,
+        7,0,157,159,3,20,10,0,158,157,1,0,0,0,159,162,1,0,0,0,160,158,1,
+        0,0,0,160,161,1,0,0,0,161,13,1,0,0,0,162,160,1,0,0,0,163,164,3,16,
+        8,0,164,165,5,7,0,0,165,15,1,0,0,0,166,167,5,23,0,0,167,169,3,34,
+        17,0,168,166,1,0,0,0,168,169,1,0,0,0,169,170,1,0,0,0,170,171,3,18,
+        9,0,171,17,1,0,0,0,172,182,3,36,18,0,173,175,5,7,0,0,174,176,5,23,
+        0,0,175,174,1,0,0,0,176,177,1,0,0,0,177,175,1,0,0,0,177,178,1,0,
+        0,0,178,179,1,0,0,0,179,181,3,36,18,0,180,173,1,0,0,0,181,184,1,
+        0,0,0,182,180,1,0,0,0,182,183,1,0,0,0,183,19,1,0,0,0,184,182,1,0,
+        0,0,185,186,5,15,0,0,186,190,3,14,7,0,187,189,3,22,11,0,188,187,
+        1,0,0,0,189,192,1,0,0,0,190,188,1,0,0,0,190,191,1,0,0,0,191,21,1,
+        0,0,0,192,190,1,0,0,0,193,194,5,16,0,0,194,195,3,14,7,0,195,23,1,
+        0,0,0,196,200,3,26,13,0,197,199,3,20,10,0,198,197,1,0,0,0,199,202,
+        1,0,0,0,200,198,1,0,0,0,200,201,1,0,0,0,201,25,1,0,0,0,202,200,1,
+        0,0,0,203,206,3,28,14,0,204,205,5,23,0,0,205,207,3,32,16,0,206,204,
+        1,0,0,0,206,207,1,0,0,0,207,208,1,0,0,0,208,209,3,16,8,0,209,210,
+        5,7,0,0,210,27,1,0,0,0,211,216,5,8,0,0,212,216,3,30,15,0,213,216,
+        5,34,0,0,214,216,5,35,0,0,215,211,1,0,0,0,215,212,1,0,0,0,215,213,
+        1,0,0,0,215,214,1,0,0,0,216,29,1,0,0,0,217,220,7,0,0,0,218,219,5,
+        22,0,0,219,221,3,50,25,0,220,218,1,0,0,0,220,221,1,0,0,0,221,31,
+        1,0,0,0,222,223,5,1,0,0,223,224,5,26,0,0,224,225,5,10,0,0,225,226,
+        5,2,0,0,226,33,1,0,0,0,227,228,5,13,0,0,228,35,1,0,0,0,229,231,3,
+        38,19,0,230,229,1,0,0,0,231,232,1,0,0,0,232,230,1,0,0,0,232,233,
+        1,0,0,0,233,37,1,0,0,0,234,237,5,23,0,0,235,236,5,30,0,0,236,238,
+        3,54,27,0,237,235,1,0,0,0,237,238,1,0,0,0,238,243,1,0,0,0,239,242,
+        3,54,27,0,240,242,5,31,0,0,241,239,1,0,0,0,241,240,1,0,0,0,242,245,
+        1,0,0,0,243,241,1,0,0,0,243,244,1,0,0,0,244,248,1,0,0,0,245,243,
+        1,0,0,0,246,249,3,40,20,0,247,249,3,70,35,0,248,246,1,0,0,0,248,
+        247,1,0,0,0,248,249,1,0,0,0,249,258,1,0,0,0,250,255,3,52,26,0,251,
+        254,3,52,26,0,252,254,3,46,23,0,253,251,1,0,0,0,253,252,1,0,0,0,
+        254,257,1,0,0,0,255,253,1,0,0,0,255,256,1,0,0,0,256,259,1,0,0,0,
+        257,255,1,0,0,0,258,250,1,0,0,0,258,259,1,0,0,0,259,261,1,0,0,0,
+        260,262,3,74,37,0,261,260,1,0,0,0,261,262,1,0,0,0,262,39,1,0,0,0,
+        263,270,3,58,29,0,264,270,3,60,30,0,265,270,3,72,36,0,266,270,3,
+        42,21,0,267,270,3,44,22,0,268,270,3,74,37,0,269,263,1,0,0,0,269,
+        264,1,0,0,0,269,265,1,0,0,0,269,266,1,0,0,0,269,267,1,0,0,0,269,
+        268,1,0,0,0,270,41,1,0,0,0,271,272,5,10,0,0,272,273,5,22,0,0,273,
+        274,5,22,0,0,274,275,3,44,22,0,275,43,1,0,0,0,276,286,3,46,23,0,
+        277,279,3,56,28,0,278,277,1,0,0,0,279,280,1,0,0,0,280,278,1,0,0,
+        0,280,281,1,0,0,0,281,282,1,0,0,0,282,283,3,46,23,0,283,285,1,0,
+        0,0,284,278,1,0,0,0,285,288,1,0,0,0,286,284,1,0,0,0,286,287,1,0,
+        0,0,287,45,1,0,0,0,288,286,1,0,0,0,289,296,5,10,0,0,290,296,5,14,
+        0,0,291,296,3,48,24,0,292,296,3,50,25,0,293,296,5,8,0,0,294,296,
+        5,9,0,0,295,289,1,0,0,0,295,290,1,0,0,0,295,291,1,0,0,0,295,292,
+        1,0,0,0,295,293,1,0,0,0,295,294,1,0,0,0,296,47,1,0,0,0,297,298,5,
+        11,0,0,298,49,1,0,0,0,299,300,5,12,0,0,300,51,1,0,0,0,301,307,5,
+        30,0,0,302,307,5,31,0,0,303,307,3,54,27,0,304,307,3,58,29,0,305,
+        307,3,56,28,0,306,301,1,0,0,0,306,302,1,0,0,0,306,303,1,0,0,0,306,
+        304,1,0,0,0,306,305,1,0,0,0,307,53,1,0,0,0,308,309,7,1,0,0,309,55,
+        1,0,0,0,310,311,7,2,0,0,311,57,1,0,0,0,312,313,7,3,0,0,313,59,1,
+        0,0,0,314,319,3,62,31,0,315,319,3,64,32,0,316,319,3,66,33,0,317,
+        319,3,68,34,0,318,314,1,0,0,0,318,315,1,0,0,0,318,316,1,0,0,0,318,
+        317,1,0,0,0,319,61,1,0,0,0,320,321,5,26,0,0,321,322,5,10,0,0,322,
+        63,1,0,0,0,323,324,5,27,0,0,324,325,5,10,0,0,325,65,1,0,0,0,326,
+        327,5,29,0,0,327,328,5,10,0,0,328,67,1,0,0,0,329,330,5,28,0,0,330,
+        331,5,10,0,0,331,69,1,0,0,0,332,337,5,30,0,0,333,338,3,40,20,0,334,
+        338,3,32,16,0,335,338,5,3,0,0,336,338,5,4,0,0,337,333,1,0,0,0,337,
+        334,1,0,0,0,337,335,1,0,0,0,337,336,1,0,0,0,338,339,1,0,0,0,339,
+        337,1,0,0,0,339,340,1,0,0,0,340,341,1,0,0,0,341,351,5,30,0,0,342,
+        344,5,31,0,0,343,345,3,40,20,0,344,343,1,0,0,0,345,346,1,0,0,0,346,
+        344,1,0,0,0,346,347,1,0,0,0,347,348,1,0,0,0,348,349,5,31,0,0,349,
+        351,1,0,0,0,350,332,1,0,0,0,350,342,1,0,0,0,351,71,1,0,0,0,352,353,
+        5,3,0,0,353,354,3,44,22,0,354,355,5,4,0,0,355,73,1,0,0,0,356,357,
+        5,1,0,0,357,358,3,44,22,0,358,359,5,2,0,0,359,75,1,0,0,0,360,364,
+        3,84,42,0,361,363,5,7,0,0,362,361,1,0,0,0,363,366,1,0,0,0,364,362,
+        1,0,0,0,364,365,1,0,0,0,365,370,1,0,0,0,366,364,1,0,0,0,367,369,
+        3,6,3,0,368,367,1,0,0,0,369,372,1,0,0,0,370,368,1,0,0,0,370,371,
+        1,0,0,0,371,379,1,0,0,0,372,370,1,0,0,0,373,375,5,7,0,0,374,373,
+        1,0,0,0,374,375,1,0,0,0,375,376,1,0,0,0,376,378,3,78,39,0,377,374,
+        1,0,0,0,378,381,1,0,0,0,379,377,1,0,0,0,379,380,1,0,0,0,380,77,1,
+        0,0,0,381,379,1,0,0,0,382,386,3,86,43,0,383,385,5,7,0,0,384,383,
+        1,0,0,0,385,388,1,0,0,0,386,384,1,0,0,0,386,387,1,0,0,0,387,392,
+        1,0,0,0,388,386,1,0,0,0,389,391,3,6,3,0,390,389,1,0,0,0,391,394,
+        1,0,0,0,392,390,1,0,0,0,392,393,1,0,0,0,393,401,1,0,0,0,394,392,
+        1,0,0,0,395,397,5,7,0,0,396,395,1,0,0,0,396,397,1,0,0,0,397,398,
+        1,0,0,0,398,400,3,80,40,0,399,396,1,0,0,0,400,403,1,0,0,0,401,399,
+        1,0,0,0,401,402,1,0,0,0,402,79,1,0,0,0,403,401,1,0,0,0,404,408,3,
+        88,44,0,405,407,5,7,0,0,406,405,1,0,0,0,407,410,1,0,0,0,408,406,
+        1,0,0,0,408,409,1,0,0,0,409,414,1,0,0,0,410,408,1,0,0,0,411,413,
+        3,6,3,0,412,411,1,0,0,0,413,416,1,0,0,0,414,412,1,0,0,0,414,415,
+        1,0,0,0,415,423,1,0,0,0,416,414,1,0,0,0,417,419,5,7,0,0,418,417,
+        1,0,0,0,418,419,1,0,0,0,419,420,1,0,0,0,420,422,3,82,41,0,421,418,
+        1,0,0,0,422,425,1,0,0,0,423,421,1,0,0,0,423,424,1,0,0,0,424,81,1,
+        0,0,0,425,423,1,0,0,0,426,430,3,90,45,0,427,429,5,7,0,0,428,427,
+        1,0,0,0,429,432,1,0,0,0,430,428,1,0,0,0,430,431,1,0,0,0,431,436,
+        1,0,0,0,432,430,1,0,0,0,433,435,3,6,3,0,434,433,1,0,0,0,435,438,
+        1,0,0,0,436,434,1,0,0,0,436,437,1,0,0,0,437,83,1,0,0,0,438,436,1,
+        0,0,0,439,440,5,26,0,0,440,441,5,26,0,0,441,442,5,26,0,0,442,443,
+        5,26,0,0,443,444,5,26,0,0,444,445,5,26,0,0,445,446,5,26,0,0,446,
+        447,5,26,0,0,447,448,5,26,0,0,448,449,3,36,18,0,449,450,3,92,46,
+        0,450,85,1,0,0,0,451,452,5,5,0,0,452,453,3,36,18,0,453,454,3,92,
+        46,0,454,87,1,0,0,0,455,456,5,6,0,0,456,457,3,36,18,0,457,458,3,
+        92,46,0,458,89,1,0,0,0,459,460,5,18,0,0,460,461,5,18,0,0,461,462,
+        5,18,0,0,462,463,3,36,18,0,463,464,3,92,46,0,464,91,1,0,0,0,465,
+        466,7,4,0,0,466,93,1,0,0,0,52,98,103,109,115,118,125,129,136,141,
+        148,160,168,177,182,190,200,206,215,220,232,237,241,243,248,253,
+        255,258,261,269,280,286,295,306,318,337,339,346,350,364,370,374,
+        379,386,392,396,401,408,414,418,423,430,436
     ]
 
 class ZorgFileParser ( Parser ):
 
     grammarFileName = "ZorgFile.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
 
     sharedContextCache = PredictionContextCache()
 
     literalNames = [ "<INVALID>", "'['", "']'", "'[['", "']]'", "'======='", 
                      "'*****'", "<INVALID>", "'o'", "'x'", "<INVALID>", 
-                     "<INVALID>", "<INVALID>", "'  -'", "'    -'", "<INVALID>", 
-                     "'-'", "'.'", "'/'", "'_'", "':'", "' '", "'('", "')'", 
-                     "'#'", "'@'", "'+'", "'%'", "'''", "'\"'", "'~'", "'*'", 
-                     "'<'", "'>'" ]
+                     "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
+                     "'  -'", "'    -'", "<INVALID>", "'-'", "'.'", "'/'", 
+                     "'_'", "':'", "' '", "'('", "')'", "'#'", "'@'", "'+'", 
+                     "'%'", "'''", "'\"'", "'~'", "'*'", "'<'", "'>'" ]
 
     symbolicNames = [ "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "NL", "LOWER_O", 
-                      "LOWER_X", "ID", "DATE", "NUM_ID", "TWO_SPACE_DASH", 
-                      "FOUR_SPACE_DASH", "SYMBOL", "DASH", "DOT", "FSLASH", 
-                      "UNDERSCORE", "COLON", "SPACE", "LPAREN", "RPAREN", 
-                      "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", "DQUOTE", 
-                      "TILDE", "STAR", "LANGLE", "RANGLE" ]
+                      "LOWER_X", "ID", "DATE", "TIME", "ZID", "NUM_ID", 
+                      "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", 
+                      "DOT", "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", 
+                      "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", 
+                      "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE" ]
 
     RULE_prog = 0
     RULE_head = 1
     RULE_comment = 2
     RULE_block = 3
     RULE_item = 4
-    RULE_todo = 5
-    RULE_priority = 6
-    RULE_note = 7
-    RULE_base_note = 8
-    RULE_base_todo = 9
+    RULE_footnote = 5
+    RULE_note = 6
+    RULE_base_note = 7
+    RULE_id_note_body = 8
+    RULE_note_body = 9
     RULE_subnote = 10
     RULE_subsubnote = 11
-    RULE_item_body = 12
-    RULE_footnote = 13
-    RULE_space_atoms = 14
-    RULE_space_atom = 15
-    RULE_atom = 16
-    RULE_property = 17
-    RULE_id_group = 18
-    RULE_id = 19
-    RULE_date = 20
-    RULE_any_symbol = 21
-    RULE_non_tag_symbol = 22
-    RULE_id_symbol = 23
-    RULE_tag_symbol = 24
-    RULE_tag = 25
-    RULE_area = 26
-    RULE_context = 27
-    RULE_person = 28
-    RULE_project = 29
-    RULE_quoted = 30
-    RULE_link = 31
-    RULE_ref = 32
-    RULE_h1_section = 33
-    RULE_h2_section = 34
-    RULE_h3_section = 35
-    RULE_h4_section = 36
-    RULE_h1_header = 37
-    RULE_h2_header = 38
-    RULE_h3_header = 39
-    RULE_h4_header = 40
-
-    ruleNames =  [ "prog", "head", "comment", "block", "item", "todo", "priority", 
-                   "note", "base_note", "base_todo", "subnote", "subsubnote", 
-                   "item_body", "footnote", "space_atoms", "space_atom", 
-                   "atom", "property", "id_group", "id", "date", "any_symbol", 
+    RULE_todo = 12
+    RULE_base_todo = 13
+    RULE_todo_prefix = 14
+    RULE_x_or_tilde = 15
+    RULE_priority = 16
+    RULE_zid = 17
+    RULE_space_atoms = 18
+    RULE_space_atom = 19
+    RULE_atom = 20
+    RULE_property = 21
+    RULE_id_group = 22
+    RULE_id = 23
+    RULE_date = 24
+    RULE_time = 25
+    RULE_any_symbol = 26
+    RULE_non_tag_symbol = 27
+    RULE_id_symbol = 28
+    RULE_tag_symbol = 29
+    RULE_tag = 30
+    RULE_area = 31
+    RULE_context = 32
+    RULE_person = 33
+    RULE_project = 34
+    RULE_quoted = 35
+    RULE_link = 36
+    RULE_ref = 37
+    RULE_h1_section = 38
+    RULE_h2_section = 39
+    RULE_h3_section = 40
+    RULE_h4_section = 41
+    RULE_h1_header = 42
+    RULE_h2_header = 43
+    RULE_h3_header = 44
+    RULE_h4_header = 45
+    RULE_eol = 46
+
+    ruleNames =  [ "prog", "head", "comment", "block", "item", "footnote", 
+                   "note", "base_note", "id_note_body", "note_body", "subnote", 
+                   "subsubnote", "todo", "base_todo", "todo_prefix", "x_or_tilde", 
+                   "priority", "zid", "space_atoms", "space_atom", "atom", 
+                   "property", "id_group", "id", "date", "time", "any_symbol", 
                    "non_tag_symbol", "id_symbol", "tag_symbol", "tag", "area", 
                    "context", "person", "project", "quoted", "link", "ref", 
                    "h1_section", "h2_section", "h3_section", "h4_section", 
-                   "h1_header", "h2_header", "h3_header", "h4_header" ]
+                   "h1_header", "h2_header", "h3_header", "h4_header", "eol" ]
 
     EOF = Token.EOF
     T__0=1
     T__1=2
     T__2=3
     T__3=4
     T__4=5
     T__5=6
     NL=7
     LOWER_O=8
     LOWER_X=9
     ID=10
     DATE=11
-    NUM_ID=12
-    TWO_SPACE_DASH=13
-    FOUR_SPACE_DASH=14
-    SYMBOL=15
-    DASH=16
-    DOT=17
-    FSLASH=18
-    UNDERSCORE=19
-    COLON=20
-    SPACE=21
-    LPAREN=22
-    RPAREN=23
-    HASH=24
-    AT_SIGN=25
-    PLUS=26
-    PERCENT=27
-    SQUOTE=28
-    DQUOTE=29
-    TILDE=30
-    STAR=31
-    LANGLE=32
-    RANGLE=33
+    TIME=12
+    ZID=13
+    NUM_ID=14
+    TWO_SPACE_DASH=15
+    FOUR_SPACE_DASH=16
+    SYMBOL=17
+    DASH=18
+    DOT=19
+    FSLASH=20
+    UNDERSCORE=21
+    COLON=22
+    SPACE=23
+    LPAREN=24
+    RPAREN=25
+    HASH=26
+    AT_SIGN=27
+    PLUS=28
+    PERCENT=29
+    SQUOTE=30
+    DQUOTE=31
+    TILDE=32
+    STAR=33
+    LANGLE=34
+    RANGLE=35
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
@@ -337,66 +369,66 @@
     def prog(self):
 
         localctx = ZorgFileParser.ProgContext(self, self._ctx, self.state)
         self.enterRule(localctx, 0, self.RULE_prog)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 82
+            self.state = 94
             self.head()
-            self.state = 106
+            self.state = 118
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==7:
-                self.state = 84 
+                self.state = 96 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 83
+                    self.state = 95
                     self.match(ZorgFileParser.NL)
-                    self.state = 86 
+                    self.state = 98 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if not (_la==7):
                         break
 
-                self.state = 91
+                self.state = 103
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,1,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 88
+                        self.state = 100
                         self.block() 
-                    self.state = 93
+                    self.state = 105
                     self._errHandler.sync(self)
                     _alt = self._interp.adaptivePredict(self._input,1,self._ctx)
 
-                self.state = 97
+                self.state = 109
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while _la==5:
-                    self.state = 94
+                    self.state = 106
                     self.h2_section()
-                    self.state = 99
+                    self.state = 111
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 103
+                self.state = 115
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==24:
-                    self.state = 100
+                while _la==26:
+                    self.state = 112
                     self.h1_section()
-                    self.state = 105
+                    self.state = 117
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
 
 
-            self.state = 108
+            self.state = 120
             self.match(ZorgFileParser.EOF)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -434,24 +466,24 @@
     def head(self):
 
         localctx = ZorgFileParser.HeadContext(self, self._ctx, self.state)
         self.enterRule(localctx, 2, self.RULE_head)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 111 
+            self.state = 123 
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while True:
-                self.state = 110
+                self.state = 122
                 self.comment()
-                self.state = 113 
+                self.state = 125 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not (_la==24):
+                if not (_la==26):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -493,25 +525,25 @@
     def comment(self):
 
         localctx = ZorgFileParser.CommentContext(self, self._ctx, self.state)
         self.enterRule(localctx, 4, self.RULE_comment)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 115
+            self.state = 127
             self.match(ZorgFileParser.HASH)
-            self.state = 117
+            self.state = 129
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==21:
-                self.state = 116
+            if _la==23:
+                self.state = 128
                 self.space_atoms()
 
 
-            self.state = 119
+            self.state = 131
             self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -554,36 +586,36 @@
 
     def block(self):
 
         localctx = ZorgFileParser.BlockContext(self, self._ctx, self.state)
         self.enterRule(localctx, 6, self.RULE_block)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 122 
+            self.state = 134 
             self._errHandler.sync(self)
             _alt = 1
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt == 1:
-                    self.state = 121
+                    self.state = 133
                     self.item()
 
                 else:
                     raise NoViableAltException(self)
-                self.state = 124 
+                self.state = 136 
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,7,self._ctx)
 
-            self.state = 129
+            self.state = 141
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,8,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 126
+                    self.state = 138
                     self.match(ZorgFileParser.NL) 
-                self.state = 131
+                self.state = 143
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,8,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -630,150 +662,98 @@
 
 
     def item(self):
 
         localctx = ZorgFileParser.ItemContext(self, self._ctx, self.state)
         self.enterRule(localctx, 8, self.RULE_item)
         try:
-            self.state = 136
+            self.state = 148
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [8, 9, 30, 32, 33]:
+            if token in [8, 9, 32, 34, 35]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 132
+                self.state = 144
                 self.todo()
                 pass
-            elif token in [16]:
+            elif token in [18]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 133
+                self.state = 145
                 self.note()
                 pass
             elif token in [1]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 134
+                self.state = 146
                 self.footnote()
                 pass
-            elif token in [24]:
+            elif token in [26]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 135
+                self.state = 147
                 self.comment()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
-    class TodoContext(ParserRuleContext):
+    class FootnoteContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def base_todo(self):
-            return self.getTypedRuleContext(ZorgFileParser.Base_todoContext,0)
-
-
-        def subnote(self, i:int=None):
-            if i is None:
-                return self.getTypedRuleContexts(ZorgFileParser.SubnoteContext)
-            else:
-                return self.getTypedRuleContext(ZorgFileParser.SubnoteContext,i)
-
-
-        def getRuleIndex(self):
-            return ZorgFileParser.RULE_todo
-
-        def enterRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "enterTodo" ):
-                listener.enterTodo(self)
-
-        def exitRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "exitTodo" ):
-                listener.exitTodo(self)
-
-
-
-
-    def todo(self):
-
-        localctx = ZorgFileParser.TodoContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 10, self.RULE_todo)
-        self._la = 0 # Token type
-        try:
-            self.enterOuterAlt(localctx, 1)
-            self.state = 138
-            self.base_todo()
-            self.state = 142
-            self._errHandler.sync(self)
-            _la = self._input.LA(1)
-            while _la==13:
-                self.state = 139
-                self.subnote()
-                self.state = 144
-                self._errHandler.sync(self)
-                _la = self._input.LA(1)
+        def ref(self):
+            return self.getTypedRuleContext(ZorgFileParser.RefContext,0)
 
-        except RecognitionException as re:
-            localctx.exception = re
-            self._errHandler.reportError(self, re)
-            self._errHandler.recover(self, re)
-        finally:
-            self.exitRule()
-        return localctx
 
+        def COLON(self):
+            return self.getToken(ZorgFileParser.COLON, 0)
 
-    class PriorityContext(ParserRuleContext):
-        __slots__ = 'parser'
+        def space_atoms(self):
+            return self.getTypedRuleContext(ZorgFileParser.Space_atomsContext,0)
 
-        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
-            super().__init__(parent, invokingState)
-            self.parser = parser
 
-        def HASH(self):
-            return self.getToken(ZorgFileParser.HASH, 0)
-
-        def ID(self):
-            return self.getToken(ZorgFileParser.ID, 0)
+        def NL(self):
+            return self.getToken(ZorgFileParser.NL, 0)
 
         def getRuleIndex(self):
-            return ZorgFileParser.RULE_priority
+            return ZorgFileParser.RULE_footnote
 
         def enterRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "enterPriority" ):
-                listener.enterPriority(self)
+            if hasattr( listener, "enterFootnote" ):
+                listener.enterFootnote(self)
 
         def exitRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "exitPriority" ):
-                listener.exitPriority(self)
+            if hasattr( listener, "exitFootnote" ):
+                listener.exitFootnote(self)
 
 
 
 
-    def priority(self):
+    def footnote(self):
 
-        localctx = ZorgFileParser.PriorityContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 12, self.RULE_priority)
+        localctx = ZorgFileParser.FootnoteContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 10, self.RULE_footnote)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 145
-            self.match(ZorgFileParser.T__0)
-            self.state = 146
-            self.match(ZorgFileParser.HASH)
-            self.state = 147
-            self.match(ZorgFileParser.ID)
-            self.state = 148
-            self.match(ZorgFileParser.T__1)
+            self.state = 150
+            self.ref()
+            self.state = 151
+            self.match(ZorgFileParser.COLON)
+            self.state = 152
+            self.space_atoms()
+            self.state = 153
+            self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -813,29 +793,29 @@
 
 
 
 
     def note(self):
 
         localctx = ZorgFileParser.NoteContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 14, self.RULE_note)
+        self.enterRule(localctx, 12, self.RULE_note)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 150
+            self.state = 155
             self.match(ZorgFileParser.DASH)
-            self.state = 151
+            self.state = 156
             self.base_note()
-            self.state = 155
+            self.state = 160
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==13:
-                self.state = 152
-                self.subnote()
+            while _la==15:
                 self.state = 157
+                self.subnote()
+                self.state = 162
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -847,16 +827,16 @@
     class Base_noteContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def item_body(self):
-            return self.getTypedRuleContext(ZorgFileParser.Item_bodyContext,0)
+        def id_note_body(self):
+            return self.getTypedRuleContext(ZorgFileParser.Id_note_bodyContext,0)
 
 
         def NL(self):
             return self.getToken(ZorgFileParser.NL, 0)
 
         def getRuleIndex(self):
             return ZorgFileParser.RULE_base_note
@@ -871,108 +851,164 @@
 
 
 
 
     def base_note(self):
 
         localctx = ZorgFileParser.Base_noteContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 16, self.RULE_base_note)
+        self.enterRule(localctx, 14, self.RULE_base_note)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 158
-            self.item_body()
-            self.state = 159
+            self.state = 163
+            self.id_note_body()
+            self.state = 164
             self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
-    class Base_todoContext(ParserRuleContext):
+    class Id_note_bodyContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def item_body(self):
-            return self.getTypedRuleContext(ZorgFileParser.Item_bodyContext,0)
+        def note_body(self):
+            return self.getTypedRuleContext(ZorgFileParser.Note_bodyContext,0)
 
 
-        def NL(self):
-            return self.getToken(ZorgFileParser.NL, 0)
+        def SPACE(self):
+            return self.getToken(ZorgFileParser.SPACE, 0)
 
-        def LOWER_O(self):
-            return self.getToken(ZorgFileParser.LOWER_O, 0)
+        def zid(self):
+            return self.getTypedRuleContext(ZorgFileParser.ZidContext,0)
 
-        def LOWER_X(self):
-            return self.getToken(ZorgFileParser.LOWER_X, 0)
 
-        def TILDE(self):
-            return self.getToken(ZorgFileParser.TILDE, 0)
+        def getRuleIndex(self):
+            return ZorgFileParser.RULE_id_note_body
 
-        def LANGLE(self):
-            return self.getToken(ZorgFileParser.LANGLE, 0)
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterId_note_body" ):
+                listener.enterId_note_body(self)
 
-        def RANGLE(self):
-            return self.getToken(ZorgFileParser.RANGLE, 0)
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitId_note_body" ):
+                listener.exitId_note_body(self)
 
-        def SPACE(self):
-            return self.getToken(ZorgFileParser.SPACE, 0)
 
-        def priority(self):
-            return self.getTypedRuleContext(ZorgFileParser.PriorityContext,0)
 
 
+    def id_note_body(self):
+
+        localctx = ZorgFileParser.Id_note_bodyContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 16, self.RULE_id_note_body)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 168
+            self._errHandler.sync(self)
+            la_ = self._interp.adaptivePredict(self._input,11,self._ctx)
+            if la_ == 1:
+                self.state = 166
+                self.match(ZorgFileParser.SPACE)
+                self.state = 167
+                self.zid()
+
+
+            self.state = 170
+            self.note_body()
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Note_bodyContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def space_atoms(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(ZorgFileParser.Space_atomsContext)
+            else:
+                return self.getTypedRuleContext(ZorgFileParser.Space_atomsContext,i)
+
+
+        def NL(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgFileParser.NL)
+            else:
+                return self.getToken(ZorgFileParser.NL, i)
+
+        def SPACE(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgFileParser.SPACE)
+            else:
+                return self.getToken(ZorgFileParser.SPACE, i)
+
         def getRuleIndex(self):
-            return ZorgFileParser.RULE_base_todo
+            return ZorgFileParser.RULE_note_body
 
         def enterRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "enterBase_todo" ):
-                listener.enterBase_todo(self)
+            if hasattr( listener, "enterNote_body" ):
+                listener.enterNote_body(self)
 
         def exitRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "exitBase_todo" ):
-                listener.exitBase_todo(self)
+            if hasattr( listener, "exitNote_body" ):
+                listener.exitNote_body(self)
 
 
 
 
-    def base_todo(self):
+    def note_body(self):
 
-        localctx = ZorgFileParser.Base_todoContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 18, self.RULE_base_todo)
-        self._la = 0 # Token type
+        localctx = ZorgFileParser.Note_bodyContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 18, self.RULE_note_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 161
-            _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 13958644480) != 0)):
-                self._errHandler.recoverInline(self)
-            else:
-                self._errHandler.reportMatch(self)
-                self.consume()
-            self.state = 164
+            self.state = 172
+            self.space_atoms()
+            self.state = 182
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,12,self._ctx)
-            if la_ == 1:
-                self.state = 162
-                self.match(ZorgFileParser.SPACE)
-                self.state = 163
-                self.priority()
+            _alt = self._interp.adaptivePredict(self._input,13,self._ctx)
+            while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
+                if _alt==1:
+                    self.state = 173
+                    self.match(ZorgFileParser.NL)
+                    self.state = 175 
+                    self._errHandler.sync(self)
+                    _alt = 1
+                    while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
+                        if _alt == 1:
+                            self.state = 174
+                            self.match(ZorgFileParser.SPACE)
 
+                        else:
+                            raise NoViableAltException(self)
+                        self.state = 177 
+                        self._errHandler.sync(self)
+                        _alt = self._interp.adaptivePredict(self._input,12,self._ctx)
+
+                    self.state = 179
+                    self.space_atoms() 
+                self.state = 184
+                self._errHandler.sync(self)
+                _alt = self._interp.adaptivePredict(self._input,13,self._ctx)
 
-            self.state = 166
-            self.item_body()
-            self.state = 167
-            self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -1016,25 +1052,25 @@
     def subnote(self):
 
         localctx = ZorgFileParser.SubnoteContext(self, self._ctx, self.state)
         self.enterRule(localctx, 20, self.RULE_subnote)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 169
+            self.state = 185
             self.match(ZorgFileParser.TWO_SPACE_DASH)
-            self.state = 170
+            self.state = 186
             self.base_note()
-            self.state = 174
+            self.state = 190
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==14:
-                self.state = 171
+            while _la==16:
+                self.state = 187
                 self.subsubnote()
-                self.state = 176
+                self.state = 192
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1073,155 +1109,377 @@
 
     def subsubnote(self):
 
         localctx = ZorgFileParser.SubsubnoteContext(self, self._ctx, self.state)
         self.enterRule(localctx, 22, self.RULE_subsubnote)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 177
+            self.state = 193
             self.match(ZorgFileParser.FOUR_SPACE_DASH)
-            self.state = 178
+            self.state = 194
             self.base_note()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
-    class Item_bodyContext(ParserRuleContext):
+    class TodoContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def space_atoms(self, i:int=None):
-            if i is None:
-                return self.getTypedRuleContexts(ZorgFileParser.Space_atomsContext)
-            else:
-                return self.getTypedRuleContext(ZorgFileParser.Space_atomsContext,i)
+        def base_todo(self):
+            return self.getTypedRuleContext(ZorgFileParser.Base_todoContext,0)
 
 
-        def NL(self, i:int=None):
+        def subnote(self, i:int=None):
             if i is None:
-                return self.getTokens(ZorgFileParser.NL)
+                return self.getTypedRuleContexts(ZorgFileParser.SubnoteContext)
             else:
-                return self.getToken(ZorgFileParser.NL, i)
+                return self.getTypedRuleContext(ZorgFileParser.SubnoteContext,i)
 
-        def SPACE(self, i:int=None):
-            if i is None:
-                return self.getTokens(ZorgFileParser.SPACE)
-            else:
-                return self.getToken(ZorgFileParser.SPACE, i)
 
         def getRuleIndex(self):
-            return ZorgFileParser.RULE_item_body
+            return ZorgFileParser.RULE_todo
 
         def enterRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "enterItem_body" ):
-                listener.enterItem_body(self)
+            if hasattr( listener, "enterTodo" ):
+                listener.enterTodo(self)
 
         def exitRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "exitItem_body" ):
-                listener.exitItem_body(self)
+            if hasattr( listener, "exitTodo" ):
+                listener.exitTodo(self)
 
 
 
 
-    def item_body(self):
+    def todo(self):
 
-        localctx = ZorgFileParser.Item_bodyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 24, self.RULE_item_body)
+        localctx = ZorgFileParser.TodoContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 24, self.RULE_todo)
+        self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 180
-            self.space_atoms()
-            self.state = 190
+            self.state = 196
+            self.base_todo()
+            self.state = 200
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,15,self._ctx)
-            while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
-                if _alt==1:
-                    self.state = 181
-                    self.match(ZorgFileParser.NL)
-                    self.state = 183 
-                    self._errHandler.sync(self)
-                    _alt = 1
-                    while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
-                        if _alt == 1:
-                            self.state = 182
-                            self.match(ZorgFileParser.SPACE)
+            _la = self._input.LA(1)
+            while _la==15:
+                self.state = 197
+                self.subnote()
+                self.state = 202
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
 
-                        else:
-                            raise NoViableAltException(self)
-                        self.state = 185 
-                        self._errHandler.sync(self)
-                        _alt = self._interp.adaptivePredict(self._input,14,self._ctx)
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
 
-                    self.state = 187
-                    self.space_atoms() 
-                self.state = 192
-                self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,15,self._ctx)
 
+    class Base_todoContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def todo_prefix(self):
+            return self.getTypedRuleContext(ZorgFileParser.Todo_prefixContext,0)
+
+
+        def id_note_body(self):
+            return self.getTypedRuleContext(ZorgFileParser.Id_note_bodyContext,0)
+
+
+        def NL(self):
+            return self.getToken(ZorgFileParser.NL, 0)
+
+        def SPACE(self):
+            return self.getToken(ZorgFileParser.SPACE, 0)
+
+        def priority(self):
+            return self.getTypedRuleContext(ZorgFileParser.PriorityContext,0)
+
+
+        def getRuleIndex(self):
+            return ZorgFileParser.RULE_base_todo
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterBase_todo" ):
+                listener.enterBase_todo(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitBase_todo" ):
+                listener.exitBase_todo(self)
+
+
+
+
+    def base_todo(self):
+
+        localctx = ZorgFileParser.Base_todoContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 26, self.RULE_base_todo)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 203
+            self.todo_prefix()
+            self.state = 206
+            self._errHandler.sync(self)
+            la_ = self._interp.adaptivePredict(self._input,16,self._ctx)
+            if la_ == 1:
+                self.state = 204
+                self.match(ZorgFileParser.SPACE)
+                self.state = 205
+                self.priority()
+
+
+            self.state = 208
+            self.id_note_body()
+            self.state = 209
+            self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
-    class FootnoteContext(ParserRuleContext):
+    class Todo_prefixContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def ref(self):
-            return self.getTypedRuleContext(ZorgFileParser.RefContext,0)
+        def LOWER_O(self):
+            return self.getToken(ZorgFileParser.LOWER_O, 0)
+
+        def x_or_tilde(self):
+            return self.getTypedRuleContext(ZorgFileParser.X_or_tildeContext,0)
+
+
+        def LANGLE(self):
+            return self.getToken(ZorgFileParser.LANGLE, 0)
+
+        def RANGLE(self):
+            return self.getToken(ZorgFileParser.RANGLE, 0)
 
+        def getRuleIndex(self):
+            return ZorgFileParser.RULE_todo_prefix
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterTodo_prefix" ):
+                listener.enterTodo_prefix(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitTodo_prefix" ):
+                listener.exitTodo_prefix(self)
+
+
+
+
+    def todo_prefix(self):
+
+        localctx = ZorgFileParser.Todo_prefixContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 28, self.RULE_todo_prefix)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 215
+            self._errHandler.sync(self)
+            token = self._input.LA(1)
+            if token in [8]:
+                self.state = 211
+                self.match(ZorgFileParser.LOWER_O)
+                pass
+            elif token in [9, 32]:
+                self.state = 212
+                self.x_or_tilde()
+                pass
+            elif token in [34]:
+                self.state = 213
+                self.match(ZorgFileParser.LANGLE)
+                pass
+            elif token in [35]:
+                self.state = 214
+                self.match(ZorgFileParser.RANGLE)
+                pass
+            else:
+                raise NoViableAltException(self)
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class X_or_tildeContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def LOWER_X(self):
+            return self.getToken(ZorgFileParser.LOWER_X, 0)
+
+        def TILDE(self):
+            return self.getToken(ZorgFileParser.TILDE, 0)
 
         def COLON(self):
             return self.getToken(ZorgFileParser.COLON, 0)
 
-        def space_atoms(self):
-            return self.getTypedRuleContext(ZorgFileParser.Space_atomsContext,0)
+        def time(self):
+            return self.getTypedRuleContext(ZorgFileParser.TimeContext,0)
 
 
         def getRuleIndex(self):
-            return ZorgFileParser.RULE_footnote
+            return ZorgFileParser.RULE_x_or_tilde
 
         def enterRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "enterFootnote" ):
-                listener.enterFootnote(self)
+            if hasattr( listener, "enterX_or_tilde" ):
+                listener.enterX_or_tilde(self)
 
         def exitRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "exitFootnote" ):
-                listener.exitFootnote(self)
+            if hasattr( listener, "exitX_or_tilde" ):
+                listener.exitX_or_tilde(self)
 
 
 
 
-    def footnote(self):
+    def x_or_tilde(self):
 
-        localctx = ZorgFileParser.FootnoteContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 26, self.RULE_footnote)
+        localctx = ZorgFileParser.X_or_tildeContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 30, self.RULE_x_or_tilde)
+        self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 193
-            self.ref()
-            self.state = 194
-            self.match(ZorgFileParser.COLON)
-            self.state = 195
-            self.space_atoms()
+            self.state = 217
+            _la = self._input.LA(1)
+            if not(_la==9 or _la==32):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
+            self.state = 220
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==22:
+                self.state = 218
+                self.match(ZorgFileParser.COLON)
+                self.state = 219
+                self.time()
+
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class PriorityContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def HASH(self):
+            return self.getToken(ZorgFileParser.HASH, 0)
+
+        def ID(self):
+            return self.getToken(ZorgFileParser.ID, 0)
+
+        def getRuleIndex(self):
+            return ZorgFileParser.RULE_priority
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterPriority" ):
+                listener.enterPriority(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitPriority" ):
+                listener.exitPriority(self)
+
+
+
+
+    def priority(self):
+
+        localctx = ZorgFileParser.PriorityContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 32, self.RULE_priority)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 222
+            self.match(ZorgFileParser.T__0)
+            self.state = 223
+            self.match(ZorgFileParser.HASH)
+            self.state = 224
+            self.match(ZorgFileParser.ID)
+            self.state = 225
+            self.match(ZorgFileParser.T__1)
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class ZidContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def ZID(self):
+            return self.getToken(ZorgFileParser.ZID, 0)
+
+        def getRuleIndex(self):
+            return ZorgFileParser.RULE_zid
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterZid" ):
+                listener.enterZid(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitZid" ):
+                listener.exitZid(self)
+
+
+
+
+    def zid(self):
+
+        localctx = ZorgFileParser.ZidContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 34, self.RULE_zid)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 227
+            self.match(ZorgFileParser.ZID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -1254,28 +1512,28 @@
 
 
 
 
     def space_atoms(self):
 
         localctx = ZorgFileParser.Space_atomsContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 28, self.RULE_space_atoms)
+        self.enterRule(localctx, 36, self.RULE_space_atoms)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 198 
+            self.state = 230 
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while True:
-                self.state = 197
+                self.state = 229
                 self.space_atom()
-                self.state = 200 
+                self.state = 232 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not (_la==21):
+                if not (_la==23):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -1348,100 +1606,100 @@
 
 
 
 
     def space_atom(self):
 
         localctx = ZorgFileParser.Space_atomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 30, self.RULE_space_atom)
+        self.enterRule(localctx, 38, self.RULE_space_atom)
+        self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 202
+            self.state = 234
             self.match(ZorgFileParser.SPACE)
-            self.state = 205
+            self.state = 237
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,17,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,20,self._ctx)
             if la_ == 1:
-                self.state = 203
+                self.state = 235
                 self.match(ZorgFileParser.SQUOTE)
-                self.state = 204
+                self.state = 236
                 self.non_tag_symbol()
 
 
-            self.state = 211
+            self.state = 243
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,19,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,22,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 209
+                    self.state = 241
                     self._errHandler.sync(self)
                     token = self._input.LA(1)
-                    if token in [15, 19, 22, 23, 30, 31, 32, 33]:
-                        self.state = 207
+                    if token in [17, 21, 24, 25, 32, 33, 34, 35]:
+                        self.state = 239
                         self.non_tag_symbol()
                         pass
-                    elif token in [29]:
-                        self.state = 208
+                    elif token in [31]:
+                        self.state = 240
                         self.match(ZorgFileParser.DQUOTE)
                         pass
                     else:
                         raise NoViableAltException(self)
              
-                self.state = 213
+                self.state = 245
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,19,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,22,self._ctx)
 
-            self.state = 216
+            self.state = 248
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,20,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,23,self._ctx)
             if la_ == 1:
-                self.state = 214
+                self.state = 246
                 self.atom()
 
             elif la_ == 2:
-                self.state = 215
+                self.state = 247
                 self.quoted()
 
 
-            self.state = 226
+            self.state = 258
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,23,self._ctx)
-            if la_ == 1:
-                self.state = 218
+            _la = self._input.LA(1)
+            if (((_la) & ~0x3f) == 0 and ((1 << _la) & 68710957056) != 0):
+                self.state = 250
                 self.any_symbol()
-                self.state = 223
+                self.state = 255
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,22,self._ctx)
-                while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
-                    if _alt==1:
-                        self.state = 221
-                        self._errHandler.sync(self)
-                        token = self._input.LA(1)
-                        if token in [15, 16, 17, 18, 19, 20, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33]:
-                            self.state = 219
-                            self.any_symbol()
-                            pass
-                        elif token in [8, 9, 10, 11, 12]:
-                            self.state = 220
-                            self.id_()
-                            pass
-                        else:
-                            raise NoViableAltException(self)
-                 
-                    self.state = 225
+                _la = self._input.LA(1)
+                while (((_la) & ~0x3f) == 0 and ((1 << _la) & 68710981376) != 0):
+                    self.state = 253
+                    self._errHandler.sync(self)
+                    token = self._input.LA(1)
+                    if token in [17, 18, 19, 20, 21, 22, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35]:
+                        self.state = 251
+                        self.any_symbol()
+                        pass
+                    elif token in [8, 9, 10, 11, 12, 14]:
+                        self.state = 252
+                        self.id_()
+                        pass
+                    else:
+                        raise NoViableAltException(self)
+
+                    self.state = 257
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,22,self._ctx)
+                    _la = self._input.LA(1)
 
 
 
-            self.state = 229
+            self.state = 261
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,24,self._ctx)
-            if la_ == 1:
-                self.state = 228
+            _la = self._input.LA(1)
+            if _la==1:
+                self.state = 260
                 self.ref()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1494,52 +1752,52 @@
 
 
 
 
     def atom(self):
 
         localctx = ZorgFileParser.AtomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 32, self.RULE_atom)
+        self.enterRule(localctx, 40, self.RULE_atom)
         try:
-            self.state = 237
+            self.state = 269
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,25,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,28,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 231
+                self.state = 263
                 self.tag_symbol()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 232
+                self.state = 264
                 self.tag()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 233
+                self.state = 265
                 self.link()
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 234
+                self.state = 266
                 self.property_()
                 pass
 
             elif la_ == 5:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 235
+                self.state = 267
                 self.id_group()
                 pass
 
             elif la_ == 6:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 236
+                self.state = 268
                 self.ref()
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -1582,24 +1840,24 @@
 
 
 
 
     def property_(self):
 
         localctx = ZorgFileParser.PropertyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 34, self.RULE_property)
+        self.enterRule(localctx, 42, self.RULE_property)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 239
+            self.state = 271
             self.match(ZorgFileParser.ID)
-            self.state = 240
+            self.state = 272
             self.match(ZorgFileParser.COLON)
-            self.state = 241
+            self.state = 273
             self.match(ZorgFileParser.COLON)
-            self.state = 242
+            self.state = 274
             self.id_group()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1640,42 +1898,42 @@
 
 
 
 
     def id_group(self):
 
         localctx = ZorgFileParser.Id_groupContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 36, self.RULE_id_group)
+        self.enterRule(localctx, 44, self.RULE_id_group)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 244
+            self.state = 276
             self.id_()
-            self.state = 254
+            self.state = 286
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,27,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,30,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 246 
+                    self.state = 278 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     while True:
-                        self.state = 245
+                        self.state = 277
                         self.id_symbol()
-                        self.state = 248 
+                        self.state = 280 
                         self._errHandler.sync(self)
                         _la = self._input.LA(1)
-                        if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1507328) != 0)):
+                        if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 6029312) != 0)):
                             break
 
-                    self.state = 250
+                    self.state = 282
                     self.id_() 
-                self.state = 256
+                self.state = 288
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,27,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,30,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1695,14 +1953,18 @@
         def NUM_ID(self):
             return self.getToken(ZorgFileParser.NUM_ID, 0)
 
         def date(self):
             return self.getTypedRuleContext(ZorgFileParser.DateContext,0)
 
 
+        def time(self):
+            return self.getTypedRuleContext(ZorgFileParser.TimeContext,0)
+
+
         def LOWER_O(self):
             return self.getToken(ZorgFileParser.LOWER_O, 0)
 
         def LOWER_X(self):
             return self.getToken(ZorgFileParser.LOWER_X, 0)
 
         def getRuleIndex(self):
@@ -1718,42 +1980,47 @@
 
 
 
 
     def id_(self):
 
         localctx = ZorgFileParser.IdContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 38, self.RULE_id)
+        self.enterRule(localctx, 46, self.RULE_id)
         try:
-            self.state = 262
+            self.state = 295
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [10]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 257
+                self.state = 289
                 self.match(ZorgFileParser.ID)
                 pass
-            elif token in [12]:
+            elif token in [14]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 258
+                self.state = 290
                 self.match(ZorgFileParser.NUM_ID)
                 pass
             elif token in [11]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 259
+                self.state = 291
                 self.date()
                 pass
-            elif token in [8]:
+            elif token in [12]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 260
+                self.state = 292
+                self.time()
+                pass
+            elif token in [8]:
+                self.enterOuterAlt(localctx, 5)
+                self.state = 293
                 self.match(ZorgFileParser.LOWER_O)
                 pass
             elif token in [9]:
-                self.enterOuterAlt(localctx, 5)
-                self.state = 261
+                self.enterOuterAlt(localctx, 6)
+                self.state = 294
                 self.match(ZorgFileParser.LOWER_X)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -1787,28 +2054,69 @@
 
 
 
 
     def date(self):
 
         localctx = ZorgFileParser.DateContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 40, self.RULE_date)
+        self.enterRule(localctx, 48, self.RULE_date)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 264
+            self.state = 297
             self.match(ZorgFileParser.DATE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
+    class TimeContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def TIME(self):
+            return self.getToken(ZorgFileParser.TIME, 0)
+
+        def getRuleIndex(self):
+            return ZorgFileParser.RULE_time
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterTime" ):
+                listener.enterTime(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitTime" ):
+                listener.exitTime(self)
+
+
+
+
+    def time(self):
+
+        localctx = ZorgFileParser.TimeContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 50, self.RULE_time)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 299
+            self.match(ZorgFileParser.TIME)
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
     class Any_symbolContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
@@ -1843,42 +2151,42 @@
 
 
 
 
     def any_symbol(self):
 
         localctx = ZorgFileParser.Any_symbolContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 42, self.RULE_any_symbol)
+        self.enterRule(localctx, 52, self.RULE_any_symbol)
         try:
-            self.state = 271
+            self.state = 306
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [28]:
+            if token in [30]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 266
+                self.state = 301
                 self.match(ZorgFileParser.SQUOTE)
                 pass
-            elif token in [29]:
+            elif token in [31]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 267
+                self.state = 302
                 self.match(ZorgFileParser.DQUOTE)
                 pass
-            elif token in [15, 19, 22, 23, 30, 31, 32, 33]:
+            elif token in [17, 21, 24, 25, 32, 33, 34, 35]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 268
+                self.state = 303
                 self.non_tag_symbol()
                 pass
-            elif token in [24, 25, 26, 27]:
+            elif token in [26, 27, 28, 29]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 269
+                self.state = 304
                 self.tag_symbol()
                 pass
-            elif token in [16, 17, 18, 20]:
+            elif token in [18, 19, 20, 22]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 270
+                self.state = 305
                 self.id_symbol()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -1933,21 +2241,21 @@
 
 
 
 
     def non_tag_symbol(self):
 
         localctx = ZorgFileParser.Non_tag_symbolContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 44, self.RULE_non_tag_symbol)
+        self.enterRule(localctx, 54, self.RULE_non_tag_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 273
+            self.state = 308
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 16119267328) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 64477069312) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -1989,21 +2297,21 @@
 
 
 
 
     def id_symbol(self):
 
         localctx = ZorgFileParser.Id_symbolContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 46, self.RULE_id_symbol)
+        self.enterRule(localctx, 56, self.RULE_id_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 275
+            self.state = 310
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1507328) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 6029312) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -2045,21 +2353,21 @@
 
 
 
 
     def tag_symbol(self):
 
         localctx = ZorgFileParser.Tag_symbolContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 48, self.RULE_tag_symbol)
+        self.enterRule(localctx, 58, self.RULE_tag_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 277
+            self.state = 312
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 251658240) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006632960) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -2105,37 +2413,37 @@
 
 
 
 
     def tag(self):
 
         localctx = ZorgFileParser.TagContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 50, self.RULE_tag)
+        self.enterRule(localctx, 60, self.RULE_tag)
         try:
-            self.state = 283
+            self.state = 318
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [24]:
+            if token in [26]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 279
+                self.state = 314
                 self.area()
                 pass
-            elif token in [25]:
+            elif token in [27]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 280
+                self.state = 315
                 self.context()
                 pass
-            elif token in [27]:
+            elif token in [29]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 281
+                self.state = 316
                 self.person()
                 pass
-            elif token in [26]:
+            elif token in [28]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 282
+                self.state = 317
                 self.project()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2172,20 +2480,20 @@
 
 
 
 
     def area(self):
 
         localctx = ZorgFileParser.AreaContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 52, self.RULE_area)
+        self.enterRule(localctx, 62, self.RULE_area)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 285
+            self.state = 320
             self.match(ZorgFileParser.HASH)
-            self.state = 286
+            self.state = 321
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2218,20 +2526,20 @@
 
 
 
 
     def context(self):
 
         localctx = ZorgFileParser.ContextContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 54, self.RULE_context)
+        self.enterRule(localctx, 64, self.RULE_context)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 288
+            self.state = 323
             self.match(ZorgFileParser.AT_SIGN)
-            self.state = 289
+            self.state = 324
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2264,20 +2572,20 @@
 
 
 
 
     def person(self):
 
         localctx = ZorgFileParser.PersonContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 56, self.RULE_person)
+        self.enterRule(localctx, 66, self.RULE_person)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 291
+            self.state = 326
             self.match(ZorgFileParser.PERCENT)
-            self.state = 292
+            self.state = 327
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2310,20 +2618,20 @@
 
 
 
 
     def project(self):
 
         localctx = ZorgFileParser.ProjectContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 58, self.RULE_project)
+        self.enterRule(localctx, 68, self.RULE_project)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 294
+            self.state = 329
             self.match(ZorgFileParser.PLUS)
-            self.state = 295
+            self.state = 330
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2376,77 +2684,77 @@
 
 
 
 
     def quoted(self):
 
         localctx = ZorgFileParser.QuotedContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 60, self.RULE_quoted)
+        self.enterRule(localctx, 70, self.RULE_quoted)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 315
+            self.state = 350
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [28]:
-                self.state = 297
+            if token in [30]:
+                self.state = 332
                 self.match(ZorgFileParser.SQUOTE)
-                self.state = 302 
+                self.state = 337 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 302
+                    self.state = 337
                     self._errHandler.sync(self)
-                    la_ = self._interp.adaptivePredict(self._input,31,self._ctx)
+                    la_ = self._interp.adaptivePredict(self._input,34,self._ctx)
                     if la_ == 1:
-                        self.state = 298
+                        self.state = 333
                         self.atom()
                         pass
 
                     elif la_ == 2:
-                        self.state = 299
+                        self.state = 334
                         self.priority()
                         pass
 
                     elif la_ == 3:
-                        self.state = 300
+                        self.state = 335
                         self.match(ZorgFileParser.T__2)
                         pass
 
                     elif la_ == 4:
-                        self.state = 301
+                        self.state = 336
                         self.match(ZorgFileParser.T__3)
                         pass
 
 
-                    self.state = 304 
+                    self.state = 339 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 251666202) != 0)):
+                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006657306) != 0)):
                         break
 
-                self.state = 306
+                self.state = 341
                 self.match(ZorgFileParser.SQUOTE)
                 pass
-            elif token in [29]:
-                self.state = 307
+            elif token in [31]:
+                self.state = 342
                 self.match(ZorgFileParser.DQUOTE)
-                self.state = 309 
+                self.state = 344 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 308
+                    self.state = 343
                     self.atom()
-                    self.state = 311 
+                    self.state = 346 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 251666186) != 0)):
+                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006657290) != 0)):
                         break
 
-                self.state = 313
+                self.state = 348
                 self.match(ZorgFileParser.DQUOTE)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2481,22 +2789,22 @@
 
 
 
 
     def link(self):
 
         localctx = ZorgFileParser.LinkContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 62, self.RULE_link)
+        self.enterRule(localctx, 72, self.RULE_link)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 317
+            self.state = 352
             self.match(ZorgFileParser.T__2)
-            self.state = 318
+            self.state = 353
             self.id_group()
-            self.state = 319
+            self.state = 354
             self.match(ZorgFileParser.T__3)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2527,22 +2835,22 @@
 
 
 
 
     def ref(self):
 
         localctx = ZorgFileParser.RefContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 64, self.RULE_ref)
+        self.enterRule(localctx, 74, self.RULE_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 321
+            self.state = 356
             self.match(ZorgFileParser.T__0)
-            self.state = 322
+            self.state = 357
             self.id_group()
-            self.state = 323
+            self.state = 358
             self.match(ZorgFileParser.T__1)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2556,34 +2864,34 @@
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def h1_header(self):
             return self.getTypedRuleContext(ZorgFileParser.H1_headerContext,0)
 
 
+        def NL(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgFileParser.NL)
+            else:
+                return self.getToken(ZorgFileParser.NL, i)
+
         def block(self, i:int=None):
             if i is None:
                 return self.getTypedRuleContexts(ZorgFileParser.BlockContext)
             else:
                 return self.getTypedRuleContext(ZorgFileParser.BlockContext,i)
 
 
         def h2_section(self, i:int=None):
             if i is None:
                 return self.getTypedRuleContexts(ZorgFileParser.H2_sectionContext)
             else:
                 return self.getTypedRuleContext(ZorgFileParser.H2_sectionContext,i)
 
 
-        def NL(self, i:int=None):
-            if i is None:
-                return self.getTokens(ZorgFileParser.NL)
-            else:
-                return self.getToken(ZorgFileParser.NL, i)
-
         def getRuleIndex(self):
             return ZorgFileParser.RULE_h1_section
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterH1_section" ):
                 listener.enterH1_section(self)
 
@@ -2593,46 +2901,57 @@
 
 
 
 
     def h1_section(self):
 
         localctx = ZorgFileParser.H1_sectionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 66, self.RULE_h1_section)
+        self.enterRule(localctx, 76, self.RULE_h1_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 325
+            self.state = 360
             self.h1_header()
-            self.state = 329
+            self.state = 364
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,35,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
+            while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
+                if _alt==1:
+                    self.state = 361
+                    self.match(ZorgFileParser.NL) 
+                self.state = 366
+                self._errHandler.sync(self)
+                _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
+
+            self.state = 370
+            self._errHandler.sync(self)
+            _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 326
+                    self.state = 367
                     self.block() 
-                self.state = 331
+                self.state = 372
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,35,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
 
-            self.state = 338
+            self.state = 379
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==5 or _la==7:
-                self.state = 333
+                self.state = 374
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la==7:
-                    self.state = 332
+                    self.state = 373
                     self.match(ZorgFileParser.NL)
 
 
-                self.state = 335
+                self.state = 376
                 self.h2_section()
-                self.state = 340
+                self.state = 381
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -2648,34 +2967,34 @@
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def h2_header(self):
             return self.getTypedRuleContext(ZorgFileParser.H2_headerContext,0)
 
 
+        def NL(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgFileParser.NL)
+            else:
+                return self.getToken(ZorgFileParser.NL, i)
+
         def block(self, i:int=None):
             if i is None:
                 return self.getTypedRuleContexts(ZorgFileParser.BlockContext)
             else:
                 return self.getTypedRuleContext(ZorgFileParser.BlockContext,i)
 
 
         def h3_section(self, i:int=None):
             if i is None:
                 return self.getTypedRuleContexts(ZorgFileParser.H3_sectionContext)
             else:
                 return self.getTypedRuleContext(ZorgFileParser.H3_sectionContext,i)
 
 
-        def NL(self, i:int=None):
-            if i is None:
-                return self.getTokens(ZorgFileParser.NL)
-            else:
-                return self.getToken(ZorgFileParser.NL, i)
-
         def getRuleIndex(self):
             return ZorgFileParser.RULE_h2_section
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterH2_section" ):
                 listener.enterH2_section(self)
 
@@ -2685,49 +3004,60 @@
 
 
 
 
     def h2_section(self):
 
         localctx = ZorgFileParser.H2_sectionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 68, self.RULE_h2_section)
+        self.enterRule(localctx, 78, self.RULE_h2_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 341
+            self.state = 382
             self.h2_header()
-            self.state = 345
+            self.state = 386
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
+            while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
+                if _alt==1:
+                    self.state = 383
+                    self.match(ZorgFileParser.NL) 
+                self.state = 388
+                self._errHandler.sync(self)
+                _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
+
+            self.state = 392
+            self._errHandler.sync(self)
+            _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 342
+                    self.state = 389
                     self.block() 
-                self.state = 347
+                self.state = 394
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
 
-            self.state = 354
+            self.state = 401
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,40,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 349
+                    self.state = 396
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 348
+                        self.state = 395
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 351
+                    self.state = 398
                     self.h3_section() 
-                self.state = 356
+                self.state = 403
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,40,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2741,34 +3071,34 @@
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def h3_header(self):
             return self.getTypedRuleContext(ZorgFileParser.H3_headerContext,0)
 
 
+        def NL(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgFileParser.NL)
+            else:
+                return self.getToken(ZorgFileParser.NL, i)
+
         def block(self, i:int=None):
             if i is None:
                 return self.getTypedRuleContexts(ZorgFileParser.BlockContext)
             else:
                 return self.getTypedRuleContext(ZorgFileParser.BlockContext,i)
 
 
         def h4_section(self, i:int=None):
             if i is None:
                 return self.getTypedRuleContexts(ZorgFileParser.H4_sectionContext)
             else:
                 return self.getTypedRuleContext(ZorgFileParser.H4_sectionContext,i)
 
 
-        def NL(self, i:int=None):
-            if i is None:
-                return self.getTokens(ZorgFileParser.NL)
-            else:
-                return self.getToken(ZorgFileParser.NL, i)
-
         def getRuleIndex(self):
             return ZorgFileParser.RULE_h3_section
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterH3_section" ):
                 listener.enterH3_section(self)
 
@@ -2778,49 +3108,60 @@
 
 
 
 
     def h3_section(self):
 
         localctx = ZorgFileParser.H3_sectionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 70, self.RULE_h3_section)
+        self.enterRule(localctx, 80, self.RULE_h3_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 357
+            self.state = 404
             self.h3_header()
-            self.state = 361
+            self.state = 408
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,41,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 358
+                    self.state = 405
+                    self.match(ZorgFileParser.NL) 
+                self.state = 410
+                self._errHandler.sync(self)
+                _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
+
+            self.state = 414
+            self._errHandler.sync(self)
+            _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
+            while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
+                if _alt==1:
+                    self.state = 411
                     self.block() 
-                self.state = 363
+                self.state = 416
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,41,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
 
-            self.state = 370
+            self.state = 423
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 365
+                    self.state = 418
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 364
+                        self.state = 417
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 367
+                    self.state = 420
                     self.h4_section() 
-                self.state = 372
+                self.state = 425
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2834,14 +3175,20 @@
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def h4_header(self):
             return self.getTypedRuleContext(ZorgFileParser.H4_headerContext,0)
 
 
+        def NL(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgFileParser.NL)
+            else:
+                return self.getToken(ZorgFileParser.NL, i)
+
         def block(self, i:int=None):
             if i is None:
                 return self.getTypedRuleContexts(ZorgFileParser.BlockContext)
             else:
                 return self.getTypedRuleContext(ZorgFileParser.BlockContext,i)
 
 
@@ -2858,29 +3205,40 @@
 
 
 
 
     def h4_section(self):
 
         localctx = ZorgFileParser.H4_sectionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 72, self.RULE_h4_section)
+        self.enterRule(localctx, 82, self.RULE_h4_section)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 373
+            self.state = 426
             self.h4_header()
-            self.state = 377
+            self.state = 430
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,44,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 374
+                    self.state = 427
+                    self.match(ZorgFileParser.NL) 
+                self.state = 432
+                self._errHandler.sync(self)
+                _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
+
+            self.state = 436
+            self._errHandler.sync(self)
+            _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
+            while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
+                if _alt==1:
+                    self.state = 433
                     self.block() 
-                self.state = 379
+                self.state = 438
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,44,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2900,16 +3258,17 @@
             else:
                 return self.getToken(ZorgFileParser.HASH, i)
 
         def space_atoms(self):
             return self.getTypedRuleContext(ZorgFileParser.Space_atomsContext,0)
 
 
-        def NL(self):
-            return self.getToken(ZorgFileParser.NL, 0)
+        def eol(self):
+            return self.getTypedRuleContext(ZorgFileParser.EolContext,0)
+
 
         def getRuleIndex(self):
             return ZorgFileParser.RULE_h1_header
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterH1_header" ):
                 listener.enterH1_header(self)
@@ -2920,39 +3279,39 @@
 
 
 
 
     def h1_header(self):
 
         localctx = ZorgFileParser.H1_headerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 74, self.RULE_h1_header)
+        self.enterRule(localctx, 84, self.RULE_h1_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 380
+            self.state = 439
             self.match(ZorgFileParser.HASH)
-            self.state = 381
+            self.state = 440
             self.match(ZorgFileParser.HASH)
-            self.state = 382
+            self.state = 441
             self.match(ZorgFileParser.HASH)
-            self.state = 383
+            self.state = 442
             self.match(ZorgFileParser.HASH)
-            self.state = 384
+            self.state = 443
             self.match(ZorgFileParser.HASH)
-            self.state = 385
+            self.state = 444
             self.match(ZorgFileParser.HASH)
-            self.state = 386
+            self.state = 445
             self.match(ZorgFileParser.HASH)
-            self.state = 387
+            self.state = 446
             self.match(ZorgFileParser.HASH)
-            self.state = 388
+            self.state = 447
             self.match(ZorgFileParser.HASH)
-            self.state = 389
+            self.state = 448
             self.space_atoms()
-            self.state = 390
-            self.match(ZorgFileParser.NL)
+            self.state = 449
+            self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -2965,16 +3324,17 @@
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def space_atoms(self):
             return self.getTypedRuleContext(ZorgFileParser.Space_atomsContext,0)
 
 
-        def NL(self):
-            return self.getToken(ZorgFileParser.NL, 0)
+        def eol(self):
+            return self.getTypedRuleContext(ZorgFileParser.EolContext,0)
+
 
         def getRuleIndex(self):
             return ZorgFileParser.RULE_h2_header
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterH2_header" ):
                 listener.enterH2_header(self)
@@ -2985,23 +3345,23 @@
 
 
 
 
     def h2_header(self):
 
         localctx = ZorgFileParser.H2_headerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 76, self.RULE_h2_header)
+        self.enterRule(localctx, 86, self.RULE_h2_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 392
+            self.state = 451
             self.match(ZorgFileParser.T__4)
-            self.state = 393
+            self.state = 452
             self.space_atoms()
-            self.state = 394
-            self.match(ZorgFileParser.NL)
+            self.state = 453
+            self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -3014,16 +3374,17 @@
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def space_atoms(self):
             return self.getTypedRuleContext(ZorgFileParser.Space_atomsContext,0)
 
 
-        def NL(self):
-            return self.getToken(ZorgFileParser.NL, 0)
+        def eol(self):
+            return self.getTypedRuleContext(ZorgFileParser.EolContext,0)
+
 
         def getRuleIndex(self):
             return ZorgFileParser.RULE_h3_header
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterH3_header" ):
                 listener.enterH3_header(self)
@@ -3034,23 +3395,23 @@
 
 
 
 
     def h3_header(self):
 
         localctx = ZorgFileParser.H3_headerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 78, self.RULE_h3_header)
+        self.enterRule(localctx, 88, self.RULE_h3_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 396
+            self.state = 455
             self.match(ZorgFileParser.T__5)
-            self.state = 397
+            self.state = 456
             self.space_atoms()
-            self.state = 398
-            self.match(ZorgFileParser.NL)
+            self.state = 457
+            self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -3069,16 +3430,17 @@
             else:
                 return self.getToken(ZorgFileParser.DASH, i)
 
         def space_atoms(self):
             return self.getTypedRuleContext(ZorgFileParser.Space_atomsContext,0)
 
 
-        def NL(self):
-            return self.getToken(ZorgFileParser.NL, 0)
+        def eol(self):
+            return self.getTypedRuleContext(ZorgFileParser.EolContext,0)
+
 
         def getRuleIndex(self):
             return ZorgFileParser.RULE_h4_header
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterH4_header" ):
                 listener.enterH4_header(self)
@@ -3089,27 +3451,77 @@
 
 
 
 
     def h4_header(self):
 
         localctx = ZorgFileParser.H4_headerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 80, self.RULE_h4_header)
+        self.enterRule(localctx, 90, self.RULE_h4_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 400
+            self.state = 459
             self.match(ZorgFileParser.DASH)
-            self.state = 401
+            self.state = 460
             self.match(ZorgFileParser.DASH)
-            self.state = 402
+            self.state = 461
             self.match(ZorgFileParser.DASH)
-            self.state = 403
+            self.state = 462
             self.space_atoms()
-            self.state = 404
-            self.match(ZorgFileParser.NL)
+            self.state = 463
+            self.eol()
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class EolContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def NL(self):
+            return self.getToken(ZorgFileParser.NL, 0)
+
+        def EOF(self):
+            return self.getToken(ZorgFileParser.EOF, 0)
+
+        def getRuleIndex(self):
+            return ZorgFileParser.RULE_eol
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterEol" ):
+                listener.enterEol(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitEol" ):
+                listener.exitEol(self)
+
+
+
+
+    def eol(self):
+
+        localctx = ZorgFileParser.EolContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 92, self.RULE_eol)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 465
+            _la = self._input.LA(1)
+            if not(_la==-1 or _la==7):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
```

### Comparing `zettel-org-0.6.0/src/zorg/runners/__init__.py` & `zettel_org-0.6.1/src/zorg/app/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/src/zorg/runners/_run_action.py` & `zettel_org-0.6.1/src/zorg/app/runners/_run_action.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Contains runners for the 'zorg action' command."""
 
 from pathlib import Path
 
-from ..common import prepend_zdir
+from ...service.common import prepend_zdir
+from ...service.templates import init_from_template
 from ..config import OpenActionConfig
-from ..templates import init_from_template
 from ._runners import runner
 
 
 @runner
 def run_action_open(cfg: OpenActionConfig) -> int:
     """Runner for the 'action open' command."""
     zo_path = prepend_zdir(cfg.zettel_dir, [cfg.zo_path])[0]
```

### Comparing `zettel-org-0.6.0/src/zorg/runners/_run_template.py` & `zettel_org-0.6.1/src/zorg/app/runners/_run_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Contains runners for the 'zorg template' command."""
 
+from ...service.templates import ZorgTemplateManager, init_from_template
 from ..config import TemplateInitConfig, TemplateRenderConfig
-from ..templates import ZorgTemplateManager, init_from_template
 from ._runners import runner
 
 
 @runner
 def run_template_init(cfg: TemplateInitConfig) -> int:
     """Runner for the 'template init' command."""
     init_from_template(
```

### Comparing `zettel-org-0.6.0/src/zorg/sql_models.py` & `zettel_org-0.6.1/src/zorg/storage/sql/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # WARNING: Don't bother importing __future__.annotations in this module!
 import datetime as dt
 from typing import List, Optional
 
 from sqlmodel import Field, Relationship, SQLModel, String
 from sqlmodel.sql.expression import Select, SelectOfScalar
 
+from ...domain.types import TodoStatus
+
 
 # HACK: see https://github.com/tiangolo/sqlmodel/issues/189
 Select.inherit_cache = True
 SelectOfScalar.inherit_cache = True
 
 
 ###############################################################################
@@ -22,15 +24,15 @@
     id: Optional[int] = Field(default=None, primary_key=True)
 
 
 class NoteLink(SQLModel):
     """Abstract model for association/link models."""
 
     note_id: Optional[int] = Field(
-        default=None, foreign_key="note.id", primary_key=True
+        default=None, foreign_key="zorgnote.id", primary_key=True
     )
 
 
 class Tag(Base):
     """Abstract model class for todo.txt tags."""
 
     name: str = Field(sa_type=String)
@@ -67,41 +69,69 @@
     """Association model for notes-to-areas relationships."""
 
     person_id: Optional[int] = Field(
         default=None, foreign_key="person.id", primary_key=True
     )
 
 
+class ZorgFileLink(NoteLink, table=True):
+    """Association model for notes to zorg files."""
+
+    zorg_file_id: Optional[int] = Field(
+        default=None, foreign_key="zorgfile.id", primary_key=True
+    )
+
+
 class PropertyLink(NoteLink, table=True):
-    """Association model for notes-to-metatags relationships."""
+    """Association model for note-to-property relationships."""
 
-    metatag_id: Optional[int] = Field(
-        default=None, foreign_key="prop.id", primary_key=True
+    prop_id: Optional[int] = Field(
+        default=None, foreign_key="property.id", primary_key=True
     )
 
-    note: "Note" = Relationship(back_populates="property_links")
+    note: "ZorgNote" = Relationship(back_populates="property_links")
     prop: "Property" = Relationship(back_populates="links")
 
     value: str
 
 
 ###############################################################################
+# model used to track zorg (*.zo) files
+###############################################################################
+class ZorgFile(Base, table=True):
+    """Model class for zorg (*.zo) files."""
+
+    path: str
+    has_errors: bool = False
+    notes: List["ZorgNote"] = Relationship(
+        back_populates="zorg_file", link_model=ZorgFileLink
+    )
+
+
+###############################################################################
 # model used to store notes
 ###############################################################################
-class Note(Base, table=True):
+class ZorgNote(Base, table=True):
     """Model class for zorg notes."""
 
     # table columns
-    create_date: dt.date
-    desc: str
-    done: bool
-    done_date: Optional[dt.date]
-    priority: str
+    body: str
+
+    # TODO(bugyi): Make zid required to persist to DB.
+    # TODO(bugyi): Make zid unique.
+    zid: Optional[str] = Field(default=None)
+
+    create_date: dt.date = Field(default_factory=dt.date.today)
+    todo_priority: Optional[str] = None
+    todo_status: Optional[TodoStatus] = None
 
     # relationships
+    zorg_file: ZorgFile = Relationship(
+        back_populates="notes", link_model=ZorgFileLink
+    )
     contexts: List["Context"] = Relationship(
         back_populates="notes", link_model=ContextLink
     )
     areas: List["Area"] = Relationship(
         back_populates="notes", link_model=AreaLink
     )
     people: List["Person"] = Relationship(
@@ -115,39 +145,39 @@
 
 ###############################################################################
 # tag models
 ###############################################################################
 class Project(Tag, table=True):
     """Model class for todo.txt project tags (e.g. +zorg)."""
 
-    notes: List[Note] = Relationship(
+    notes: List[ZorgNote] = Relationship(
         back_populates="projects", link_model=ProjectLink
     )
 
 
 class Context(Tag, table=True):
     """Model class for todo.txt context tags (e.g. @home)."""
 
-    notes: List[Note] = Relationship(
+    notes: List[ZorgNote] = Relationship(
         back_populates="contexts", link_model=ContextLink
     )
 
 
 class Area(Tag, table=True):
     """Model class for todo.txt area tags (e.g. #gtd)."""
 
-    notes: List[Note] = Relationship(
+    notes: List[ZorgNote] = Relationship(
         back_populates="areas", link_model=AreaLink
     )
 
 
 class Person(Tag, table=True):
     """Model class for todo.txt person tags (e.g. %john)."""
 
-    notes: List[Note] = Relationship(
+    notes: List[ZorgNote] = Relationship(
         back_populates="people", link_model=PersonLink
     )
 
 
 class Property(Tag, table=True):
     """Model class for metadata tags (e.g. due:2022-06-01)."""
```

### Comparing `zettel-org-0.6.0/src/zorg/templates.py` & `zettel_org-0.6.1/src/zorg/service/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, Mapping
 
 import jinja2
 from logrus import Logger
 from typist import PathLike
 
 from . import common
-from .types import TemplatePatternMapType, VarMapType
+from ..domain.types import TemplatePatternMapType, VarMapType
 
 
 logger = Logger(__name__)
 
 
 def init_from_template(
     zettel_dir: PathLike,
```

### Comparing `zettel-org-0.6.0/src/zorg/types.py` & `zettel_org-0.6.1/src/zorg/domain/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 """Custom types used by zorg."""
 
+import abc
 import enum
 from pathlib import Path
-from typing import Any, Literal, Mapping, Pattern, Protocol, Sequence
+from typing import (
+    Any,
+    Generic,
+    Literal,
+    Mapping,
+    Pattern,
+    Protocol,
+    Sequence,
+    TypeVar,
+)
 
 from sqlalchemy.future import Engine
 
 
+E = TypeVar("E")
+T = TypeVar("T")
+
+
 FileGroupMapType = Mapping[str, Sequence[str]]
 TodoPriorityType = Literal[
     "A",
     "B",
     "C",
     "D",
     "E",
@@ -34,22 +48,25 @@
     "W",
     "X",
     "Y",
     "Z",
 ]
 TemplatePatternMapType = Mapping[Pattern, Path]
 VarMapType = Mapping[str, Any]
+TodoStatusPrefixChar = Literal["o", "x", "~", "<", ">"]
 
 
 class TodoStatus(enum.Enum):
-    """Status of a Zorg todo."""
+    """Zorg todo status."""
 
-    OPEN = enum.auto()
-    CLOSED = enum.auto()
-    CANCELED = enum.auto()
+    OPEN = enum.auto()  # o
+    CLOSED = enum.auto()  # x
+    CANCELED = enum.auto()  # ~
+    BLOCKED = enum.auto()  # <
+    PARENT = enum.auto()  # >
 
 
 class CreateEngineType(Protocol):
     """The type of a `db.create_engine()` callable."""
 
     def __call__(self, url: str, /, **kwargs: Any) -> Engine:
         """The function's call signature."""
@@ -58,15 +75,15 @@
 class DescOperator(enum.Enum):
     """Used to determine the type of description constraint specified."""
 
     CONTAINS = enum.auto()
     NOT_CONTAINS = enum.auto()
 
 
-class MetatagOperator(enum.Enum):
+class PropertyOperator(enum.Enum):
     """Used to determine what kind of metatag constraint has been specified."""
 
     # exists / not exists
     EXISTS = enum.auto()
     NOT_EXISTS = enum.auto()
 
     # comparison operators
@@ -74,13 +91,25 @@
     NE = enum.auto()
     LT = enum.auto()
     LE = enum.auto()
     GT = enum.auto()
     GE = enum.auto()
 
 
-class MetatagValueType(enum.Enum):
-    """Specifies the data type of a MetatagFilter's value."""
+class PropertyValueType(enum.Enum):
+    """Specifies the data type of a PropertyFilter's value."""
 
     DATE = enum.auto()
     INTEGER = enum.auto()
     STRING = enum.auto()
+
+
+class EntityConverter(Generic[E, T], abc.ABC):
+    """Abstract interface for domain entity converters."""
+
+    @abc.abstractmethod
+    def to_entity(self, _: T) -> E:
+        """Converts some non-domain object into a domain entity."""
+
+    @abc.abstractmethod
+    def from_entity(self, entity: E) -> T:
+        """Converts some domain entity into something else."""
```

### Comparing `zettel-org-0.6.0/targets.mk` & `zettel_org-0.6.1/targets.mk`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/tests/__snapshots__/test_run_compile.ambr` & `zettel_org-0.6.1/tests/__snapshots__/test_run_compile.ambr`

 * *Files 12% similar despite different names*

```diff
@@ -1,1854 +1,1942 @@
 # serializer version: 1
 # name: test_compile[YAMLConfigFile-20240323]
   '''
   {'notes': [{'areas': ['gtd'],
-              'body': ' #gtd pomodoro',
+              'body': '#gtd pomodoro',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 1,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}},
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': ['own'],
-              'body': ' #own Buy rubber duck',
+              'body': '#own Buy rubber duck',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 2,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '2'}},
+              'properties': {'p': '2'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg Parametrize test_run_compile()',
+              'body': '+zorg Parametrize test_run_compile()',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 3,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '2'}},
+              'properties': {'p': '2'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg Move models.py and file_groups.py',
+              'body': '+zorg Move models.py and file_groups.py',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 4,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '3'}},
+              'properties': {'p': '3'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg Add links to grammar',
+              'body': '+zorg Add links to grammar',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 5,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '3'}},
+              'properties': {'p': '3'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg Fix grammar so it works with this file',
+              'body': '+zorg Fix grammar so it works with this file',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 6,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '4'}},
+              'properties': {'p': '4'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg Add this file to test data',
+              'body': '+zorg Add this file to test data',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 7,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '5'}},
+              'properties': {'p': '5'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg Filter out all numeric tag names',
+              'body': '+zorg Filter out all numeric tag names',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 8,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '5'}},
+              'properties': {'p': '5'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg Test against all examples/ files',
+              'body': '+zorg Test against all examples/ files',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 9,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '6'}},
+              'properties': {'p': '6'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': " +zorg wip: Replace 'john@' with '%john'",
+              'body': "+zorg wip: Replace 'john@' with '%john'",
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 10,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '6'}},
+              'properties': {'p': '6'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +laundry dry whites',
+              'body': '+laundry dry whites',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 11,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['laundry'],
-              'properties': {'p': '7'}},
+              'properties': {'p': '7'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg wip: migrate people',
+              'body': '+zorg wip: migrate people',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 12,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '7'}},
+              'properties': {'p': '7'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': " +zorg Finished 'john@' to '%john' migration",
+              'body': "+zorg Finished 'john@' to '%john' migration",
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 13,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '8'}},
+              'properties': {'p': '8'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg Updated grammar to handle quotes',
+              'body': '+zorg Updated grammar to handle quotes',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 14,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '9'}},
+              'properties': {'p': '9'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +laundry wip: fold darks',
+              'body': '+laundry wip: fold darks',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 15,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['laundry'],
-              'properties': {'p': '10'}},
+              'properties': {'p': '10'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +laundry fold darks',
+              'body': '+laundry fold darks',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 16,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['laundry'],
-              'properties': {'p': '11'}},
+              'properties': {'p': '11'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +laundry wash delicates',
+              'body': '+laundry wash delicates',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 17,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['laundry'],
-              'properties': {'p': '12'}},
+              'properties': {'p': '12'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' +zorg [[xmind/zorg_e2e_query_arch.xmind]]',
+              'body': '+zorg [[xmind/zorg_e2e_query_arch.xmind]]',
               'child_note_ids': [],
               'contexts': ['pomodoro'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 18,
+              'create_date': FakeDatetime(2024, 3, 23, 0, 0),
               'links': ['xmind/zorg_e2e_query_arch.xmind'],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['zorg'],
-              'properties': {'p': '14'}}],
-   'todos': []}
+              'properties': {'p': '14'},
+              'todo_payload': None,
+              'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-basic]
   '''
   {'notes': [{'areas': [],
-              'body': ' First note in first block',
+              'body': 'First note in first block',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 1,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Second note in first block',
+              'body': 'Second note in first block',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 2,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}}],
-   'todos': [{'areas': [],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
+             {'areas': [],
               'body': ' bazbuz is ok too...',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'done_date': None,
-              'ident': 3,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>}]}
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-links]
   '''
   {'notes': [{'areas': [],
-              'body': ' Some note with a [[bar.sh]] link to a bash script.',
+              'body': 'Some note with a [[bar.sh]] link to a bash script.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 1,
               'links': ['bar.sh'],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Some note with a link in parens (see [[baz]]).',
+              'body': 'Some note with a link in parens (see [[baz]]).',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 2,
               'links': ['baz'],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Some note with a link in parens and a block-level link '
+              'body': 'Some note with a link in parens and a block-level link '
                       '([[buz::fuzz]]).',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 3,
               'links': ['buz::fuzz'],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}}],
-   'todos': []}
+              'properties': {},
+              'todo_payload': None,
+              'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-multiblocks]
   '''
   {'notes': [{'areas': [],
-              'body': ' A note about life...',
+              'body': ' Some todo',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 3,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None},
              {'areas': [],
-              'body': ' With a note',
+              'body': ' Another related todo',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 5,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None},
              {'areas': [],
-              'body': ' Some note in section 0',
+              'body': 'A note about life...',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 6,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Note A1',
+              'body': ' Some other todo',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 7,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None},
              {'areas': [],
-              'body': ' Note A2',
+              'body': 'With a note',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 8,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Note B',
+              'body': 'Some note in section 0',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 9,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Note C',
+              'body': 'Note A1',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 10,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Note D',
+              'body': 'Note A2',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 11,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Note E',
+              'body': 'Note B',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 12,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}}],
-   'todos': [{'areas': [],
-              'body': ' Some todo',
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
+             {'areas': [],
+              'body': 'Note C',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'done_date': None,
-              'ident': 1,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Another related todo',
+              'body': 'Note D',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'done_date': None,
-              'ident': 2,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Some other todo',
+              'body': 'Note E',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'done_date': None,
-              'ident': 4,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>}]}
+              'todo_payload': None,
+              'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-priority]
   '''
-  {'notes': [],
-   'todos': [{'areas': [],
+  {'notes': [{'areas': [],
               'body': ' 2024-03-13 High Priority TODO',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDatetime(2024, 3, 13, 0, 0),
-              'done_date': None,
-              'ident': 1,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'A',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'A', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None},
              {'areas': [],
               'body': ' 2024-03-13 Medium Priority TODO',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDatetime(2024, 3, 13, 0, 0),
-              'done_date': None,
-              'ident': 2,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'B',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'B', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None},
              {'areas': [],
               'body': ' 2024-03-13 Low Priority TODO',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDatetime(2024, 3, 13, 0, 0),
-              'done_date': None,
-              'ident': 3,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>}]}
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-property]
   '''
   {'notes': [{'areas': [],
-              'body': ' 2024-03-30 This note contains a key::value pair.',
+              'body': '2024-03-30 This note contains a key::value pair.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDatetime(2024, 3, 30, 0, 0),
-              'ident': 1,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'key': 'value', 'p': '1'}}],
-   'todos': [{'areas': [],
+              'properties': {'key': 'value', 'p': '1'},
+              'todo_payload': None,
+              'zid': None},
+             {'areas': [],
               'body': ' This todo is @due today! | due::2024-03-13',
               'child_note_ids': [],
               'contexts': ['due'],
               'create_date': FakeDate(2000, 1, 3),
-              'done_date': None,
-              'ident': 2,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
               'properties': {'due': '2024-03-13', 'p': '1'},
-              'status': <TodoStatus.OPEN: 1>}]}
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-scrambled_prj_notes]
   '''
   {'notes': [{'areas': [],
-              'body': ' Sqtdicu Gfwebkj: fdxd://rd/czge-nxgz-vmuncaf',
+              'body': 'Sqtdicu Gfwebkj: fdxd://rd/czge-nxgz-vmuncaf',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 1,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['arms'],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Reqzlu Zkba Inzlqq Zusqxur: '
+              'body': 'Reqzlu Zkba Inzlqq Zusqxur: '
                       'pclx://hn/oqdu-syxf-oxzpzp-hxdszea',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 2,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['arms'],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Tzus %clyzajrm: +cmeq ylevgv frxb gevcfp xa 26cb',
+              'body': 'Tzus %clyzajrm: +cmeq ylevgv frxb gevcfp xa 26cb',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 3,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': ['clyzajrm'],
               'prev_note_id': None,
-              'projects': ['arms/cmeq'],
-              'properties': {}},
+              'projects': ['arms', 'cmeq'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Eongcgfy tho pscz giwq arjebc@?',
+              'body': 'Eongcgfy tho pscz giwq arjebc@?',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 4,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Crxekimyx kq fjboaq:',
+              'body': 'Crxekimyx kq fjboaq:',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 5,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Lcnoajccb Injdqwlf',
+              'body': 'Lcnoajccb Injdqwlf',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 6,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 5,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Lrry-Jhfv Nfsw',
+              'body': 'Lrry-Jhfv Nfsw',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 7,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 5,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Ga Ewwnanwqgoq',
+              'body': 'Ga Ewwnanwqgoq',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 8,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 5,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Gaonrjmk: Cbnuev, Xvdgisy, Aeyfbb?',
+              'body': 'Gaonrjmk: Cbnuev, Xvdgisy, Aeyfbb?',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 9,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 5,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Vont ywgotqe vndsv (lfqbnlfar, kwmnafb, '
+              'body': 'Vont ywgotqe vndsv (lfqbnlfar, kwmnafb, '
                       'Yneicgqi/Mxvvkclvzk)',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 10,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 5,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Eyfptapyh ijmfacppn (lqrui ?jr=HF)',
+              'body': 'Eyfptapyh ijmfacppn (lqrui ?jr=HF)',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 11,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 5,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Gziien fxfmhul',
+              'body': 'Gziien fxfmhul',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 12,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 5,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Ajfn dz Rhyt (ty 6499 cw 6075)',
+              'body': 'Ajfn dz Rhyt (ty 6499 cw 6075)',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 13,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 5,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/saxy'],
-              'properties': {}},
+              'projects': ['arms', 'saxy'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' setw://fq/zfv-haow-micxv',
+              'body': 'setw://fq/zfv-haow-micxv',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 14,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/judo/vfntwi'],
-              'properties': {}},
+              'projects': ['arms', 'judo', 'vfntwi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' sorj',
+              'body': 'sorj',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 15,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/judo/vfntwi'],
-              'properties': {}},
+              'projects': ['arms', 'judo', 'vfntwi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' '
-                      'bhkh://xzywfi3/relyocplej/dpw/qk/otehzx/qpsiyunh/rgthilw_sldeu/fonvlqflxv/rjluzb/tbf/hrtkdrq_mnurg_eltj_szkb.raja',
+              'body': 'bhkh://xzywfi3/relyocplej/dpw/qk/otehzx/qpsiyunh/rgthilw_sldeu/fonvlqflxv/rjluzb/tbf/hrtkdrq_mnurg_eltj_szkb.raja',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 16,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 15,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/judo/vfntwi'],
-              'properties': {}},
+              'projects': ['arms', 'judo', 'vfntwi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' '
-                      'knlo://evfkaz3/kmxgifnodz/wav/nz/idlwsr/oslzcscp/raarqgi_bjfdp/xftsdpbcka/itulza/prk/pkgxzoc_zgntm_txeg_npbvju.jldf',
+              'body': 'knlo://evfkaz3/kmxgifnodz/wav/nz/idlwsr/oslzcscp/raarqgi_bjfdp/xftsdpbcka/itulza/prk/pkgxzoc_zgntm_txeg_npbvju.jldf',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 17,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 15,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/judo/vfntwi'],
-              'properties': {}},
+              'projects': ['arms', 'judo', 'vfntwi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' ykseciqhy IG: bp/531522711',
+              'body': 'ykseciqhy IG: bp/531522711',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 18,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/judo/vennc'],
-              'properties': {}},
+              'projects': ['arms', 'judo', 'vennc'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Nyhha trra://hk/wyp-slg-lbyuqz pris oiqf nywj kg smoy '
+              'body': 'Nyhha trra://hk/wyp-slg-lbyuqz pris oiqf nywj kg smoy '
                       'nwdraivpht() cu jzusgcwm zwyirs?',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 19,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/bmlakcr'],
-              'properties': {}},
+              'projects': ['arms', 'bmlakcr'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Wouvp rx cmmi jk zes r kv/u1abtunoeaorevyolmef: "Njwb '
+              'body': 'Wouvp rx cmmi jk zes r kv/u1abtunoeaorevyolmef: "Njwb '
                       'opjiv wlyvyfrb; tqcwkrs qlawalk: 200F."',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 20,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/bmlakcr/lozmhqjd'],
-              'properties': {}},
+              'projects': ['arms', 'bmlakcr', 'lozmhqjd'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' e2.0 xrestv rlqt cszmjhp: 1) Cnelcge 2) uttnzeu tncj 3) '
+              'body': 'e2.0 xrestv rlqt cszmjhp: 1) Cnelcge 2) uttnzeu tncj 3) '
                       'Rasemja zzvilcys',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 21,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/bmlakcr/wjybwa'],
-              'properties': {}},
+              'projects': ['arms', 'bmlakcr', 'wjybwa'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Qtvhtfc ywtyvbppqu (qs odvqdfjk nydxt):',
+              'body': 'Qtvhtfc ywtyvbppqu (qs odvqdfjk nydxt):',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 22,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/bmlakcr/wjybwa'],
-              'properties': {}},
+              'projects': ['arms', 'bmlakcr', 'wjybwa'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' XC: Wvlotmog | Akjrgluk cck dpvcvia',
+              'body': 'XC: Wvlotmog | Akjrgluk cck dpvcvia',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 23,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 22,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/bmlakcr/wjybwa'],
-              'properties': {}},
+              'projects': ['arms', 'bmlakcr', 'wjybwa'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Oers Higwy   | NYS / Cyuxu fyod mrfwalatc',
+              'body': 'Oers Higwy   | NYS / Cyuxu fyod mrfwalatc',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 24,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 22,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/bmlakcr/wjybwa'],
-              'properties': {}},
+              'projects': ['arms', 'bmlakcr', 'wjybwa'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Lveg         | Kfvunvqioefmgo Rlqu',
+              'body': 'Lveg         | Kfvunvqioefmgo Rlqu',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 25,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 22,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/bmlakcr/wjybwa'],
-              'properties': {}},
+              'projects': ['arms', 'bmlakcr', 'wjybwa'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' HU: Yoxlnl   | Kyahuurpzq mt VV (v.u. boh coveshbg rsp '
+              'body': 'HU: Yoxlnl   | Kyahuurpzq mt VV (v.u. boh coveshbg rsp '
                       'hbyhmm-pav)',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 26,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 22,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/bmlakcr/wjybwa'],
-              'properties': {}},
+              'projects': ['arms', 'bmlakcr', 'wjybwa'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' TbuburbQuf zilo '
+              'body': 'TbuburbQuf zilo '
                       'hpfu://wz/ytg:hep_epzc_ek_jehnmz?h=omm:cpdu :\n'
-                      '    (2576796, 2584174, 2585902, 2611556, 2612222) ',
+                      '    (2576796, 2584174, 2585902, 2611556, 2612222)',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 27,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/jws_pkaft'],
-              'properties': {}},
+              'projects': ['arms', 'jws_pkaft'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Kmue izlgeghae jivs kkhoh:\n'
+              'body': 'Kmue izlgeghae jivs kkhoh:\n'
                       '    (23068288959, 23070555923, 23071198233, 23081557400, '
                       '23082128453)',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 28,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/jws_pkaft'],
-              'properties': {}},
+              'projects': ['arms', 'jws_pkaft'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' KU onbf',
+              'body': 'KU onbf',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 29,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Adah wv wsr: Pwyv qrykrmat',
+              'body': 'Adah wv wsr: Pwyv qrykrmat',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 30,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 29,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Fjdu lk aozqwmt rdtv (ingu yhlzh kha zro zstolomj?): '
+              'body': 'Fjdu lk aozqwmt rdtv (ingu yhlzh kha zro zstolomj?): '
                       'Vujflym',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 31,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 29,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Cyuyngz rpzj (<tzcx_zm> nat <iqge_xqu>): Opalekb / Ubq '
+              'body': 'Cyuyngz rpzj (<tzcx_zm> nat <iqge_xqu>): Opalekb / Ubq '
                       'hefcgpa',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 32,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 29,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Snke udr djwhji ku iysauiroj (<wtflgi_jw_aykjvl>):',
+              'body': 'Snke udr djwhji ku iysauiroj (<wtflgi_jw_aykjvl>):',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 33,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 29,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Puny mng lomkrpd',
+              'body': 'Puny mng lomkrpd',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 34,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 33,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Eipahnv',
+              'body': 'Eipahnv',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 35,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 33,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' <olxh_cqe>',
+              'body': '<olxh_cqe>',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 36,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 33,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Fe dxiovcyxz kuirhi: Kjwjjl hxd: '
+              'body': 'Fe dxiovcyxz kuirhi: Kjwjjl hxd: '
                       '<lllwcz_bp_mjklvt>\\wZkzuguo/yckqyt: <awqxbdj>',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 37,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 33,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Nid bzvqqd gktb uhwgmwk jfiwf atukar oq znzg-htqz bpba?: '
+              'body': 'Nid bzvqqd gktb uhwgmwk jfiwf atukar oq znzg-htqz bpba?: '
                       '(<izljyv_dk_ebsiqu>)',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 38,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 33,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Poxi hdtlblgq:',
+              'body': 'Poxi hdtlblgq:',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 39,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 33,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Uripbc uui qr njuytfkxf',
+              'body': 'Uripbc uui qr njuytfkxf',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 40,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 39,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Dvfbqlk/ignpsr lb imwgiazpd',
+              'body': 'Dvfbqlk/ignpsr lb imwgiazpd',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 41,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 39,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Rb rnfqqbizlps',
+              'body': 'Rb rnfqqbizlps',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 42,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 39,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Wuxpotyb:',
+              'body': 'Wuxpotyb:',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 43,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Me fkf zddkb?',
+              'body': 'Me fkf zddkb?',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 44,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 43,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' An fsqw hdegvhwy?',
+              'body': 'An fsqw hdegvhwy?',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 45,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 43,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Tyrgbh iwj fcq jjuea qpltzla rkyq br at DS tfvwjwf?',
+              'body': 'Tyrgbh iwj fcq jjuea qpltzla rkyq br at DS tfvwjwf?',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 46,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/owwnfb/qbsum'],
-              'properties': {}},
+              'projects': ['arms', 'owwnfb', 'qbsum'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Rmy [[eswz_xqow::empiz_ljyiwjbmi_szstj]]',
+              'body': 'Rmy [[eswz_xqow::empiz_ljyiwjbmi_szstj]]',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 47,
               'links': ['eswz_xqow::empiz_ljyiwjbmi_szstj'],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/rgw_sxtvx'],
-              'properties': {}},
+              'projects': ['arms', 'rgw_sxtvx'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' '
-                      'nejo/vpe/gjggaa/fwi/kgrtqhtdy/ynbwnm/qekadk/cvhc/MqgomkswAgbkGhthPoqfvqt.ednt',
+              'body': 'nejo/vpe/gjggaa/fwi/kgrtqhtdy/ynbwnm/qekadk/cvhc/MqgomkswAgbkGhthPoqfvqt.ednt',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 48,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/rgw_sxtvx/zv_jzdd_djqa'],
-              'properties': {}},
+              'projects': ['arms', 'rgw_sxtvx', 'zv_jzdd_djqa'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' '
-                      'qiuz/adb/lhwggp/kqt/ldmqosmbs/qtjvrxutayfiyh/oocyfjbnuih/jmov/faaat/XibsjbhuFsbuRrawDgfksjcXwjudTvvzbxa.vvep',
+              'body': 'qiuz/adb/lhwggp/kqt/ldmqosmbs/qtjvrxutayfiyh/oocyfjbnuih/jmov/faaat/XibsjbhuFsbuRrawDgfksjcXwjudTvvzbxa.vvep',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 49,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/rgw_sxtvx/zv_jzdd_djqa'],
-              'properties': {}},
+              'projects': ['arms', 'rgw_sxtvx', 'zv_jzdd_djqa'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Ajbss udcor xf tylgpk:',
+              'body': 'Ajbss udcor xf tylgpk:',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 50,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/ipyt/bqf/cpv_mociy'],
-              'properties': {}},
+              'projects': ['arms', 'bqf', 'cpv_mociy', 'ipyt'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' ibmxadcdz.iwmdvsxeg_uxzvuntgl',
+              'body': 'ibmxadcdz.iwmdvsxeg_uxzvuntgl',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 51,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 50,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/ipyt/bqf/cpv_mociy'],
-              'properties': {}},
+              'projects': ['arms', 'bqf', 'cpv_mociy', 'ipyt'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' oiuglzpuv.xwhjvfwrs_imjxfgwoo.fvyclrkt_vqycmgeuj_ihblc',
+              'body': 'oiuglzpuv.xwhjvfwrs_imjxfgwoo.fvyclrkt_vqycmgeuj_ihblc',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 52,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 50,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/ipyt/bqf/cpv_mociy'],
-              'properties': {}},
+              'projects': ['arms', 'bqf', 'cpv_mociy', 'ipyt'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' '
-                      'ycdcddvhw.shmlpcnju_chsokpadf.bcpgad_hoargfl_fhzshiqoe_qrsrxtdsq',
+              'body': 'ycdcddvhw.shmlpcnju_chsokpadf.bcpgad_hoargfl_fhzshiqoe_qrsrxtdsq',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 53,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 50,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/ipyt/bqf/cpv_mociy'],
-              'properties': {}},
+              'projects': ['arms', 'bqf', 'cpv_mociy', 'ipyt'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' bpeijqkwt.ysazfxpem_tnpnkohdy.nppowgku_kqhexqeih_njhno',
+              'body': 'bpeijqkwt.ysazfxpem_tnpnkohdy.nppowgku_kqhexqeih_njhno',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 54,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 50,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/ipyt/bqf/cpv_mociy'],
-              'properties': {}},
+              'projects': ['arms', 'bqf', 'cpv_mociy', 'ipyt'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' uceq://ap/591285707',
+              'body': 'uceq://ap/591285707',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 55,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/ipyt/bqf/uahi'],
-              'properties': {}},
+              'projects': ['arms', 'bqf', 'ipyt', 'uahi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Git [[desd_cd_kdzb.yhdxx]] hgq lkl[1] @dzwk',
+              'body': 'Git [[desd_cd_kdzb.yhdxx]] hgq lkl[1] @dzwk',
               'child_note_ids': [],
               'contexts': ['dzwk'],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 56,
               'links': ['desd_cd_kdzb.yhdxx'],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/vd_clxi/xoao'],
-              'properties': {}},
+              'projects': ['arms', 'vd_clxi', 'xoao'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Mcjr bdukfjxm 14521206',
+              'body': 'Mcjr bdukfjxm 14521206',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 57,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/vd_clxi/okwz'],
-              'properties': {}},
+              'projects': ['arms', 'okwz', 'vd_clxi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Spuekgphn 14521428',
+              'body': 'Spuekgphn 14521428',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 58,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/vd_clxi/okwz'],
-              'properties': {}},
+              'projects': ['arms', 'okwz', 'vd_clxi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Necywz met td fuvbdooge 14524967',
+              'body': 'Necywz met td fuvbdooge 14524967',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 59,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/vd_clxi/okwz'],
-              'properties': {}},
+              'projects': ['arms', 'okwz', 'vd_clxi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Fbtqtkb, fywupn qr mzrgsvqve 14521641',
+              'body': 'Fbtqtkb, fywupn qr mzrgsvqve 14521641',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 60,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/vd_clxi/okwz'],
-              'properties': {}},
+              'projects': ['arms', 'okwz', 'vd_clxi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Uc lsmpfxhtkyh 14522952',
+              'body': 'Uc lsmpfxhtkyh 14522952',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 61,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/vd_clxi/okwz'],
-              'properties': {}},
+              'projects': ['arms', 'okwz', 'vd_clxi'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Ikr lr 20 pggmb',
+              'body': 'Ikr lr 20 pggmb',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 62,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/fgifr'],
-              'properties': {}},
+              'projects': ['arms', 'fgifr'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Ttx-yecb mxovcuwbc',
+              'body': 'Ttx-yecb mxovcuwbc',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 63,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/fgifr'],
-              'properties': {}},
+              'projects': ['arms', 'fgifr'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Rzq-itde mpfj',
+              'body': 'Rzq-itde mpfj',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 64,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/fgifr'],
-              'properties': {}},
+              'projects': ['arms', 'fgifr'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Zee-lpfg uqogce bk khxsvgrkq bbgvmf',
+              'body': 'Zee-lpfg uqogce bk khxsvgrkq bbgvmf',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 65,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['arms/fgifr'],
-              'properties': {}}],
-   'todos': []}
+              'projects': ['arms', 'fgifr'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-subnotes]
   '''
   {'notes': [{'areas': [],
-              'body': ' foobar',
+              'body': 'foobar',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 1,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}},
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Todo subnote A',
+              'body': ' This todo is due::2024-03-30 and has some subnotes',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 3,
               'links': [],
               'next_note_id': None,
-              'parent_note_id': 2,
+              'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}},
+              'properties': {'due': '2024-03-30', 'p': '1'},
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None},
              {'areas': [],
-              'body': ' Todo subnote B',
+              'body': 'Todo subnote A',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 4,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 2,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}},
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Todo subsubnote C',
+              'body': 'Todo subnote B',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 5,
               'links': [],
               'next_note_id': None,
-              'parent_note_id': 4,
+              'parent_note_id': 2,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}},
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' This note has many subnotes.',
+              'body': 'Todo subsubnote C',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 6,
               'links': [],
               'next_note_id': None,
-              'parent_note_id': None,
+              'parent_note_id': 4,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}},
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' 2024-03-30 This note contains a key::value pair.',
+              'body': 'This note has many subnotes.',
               'child_note_ids': [],
               'contexts': [],
-              'create_date': FakeDatetime(2024, 3, 30, 0, 0),
-              'ident': 7,
+              'create_date': FakeDate(2000, 1, 3),
               'links': [],
               'next_note_id': None,
-              'parent_note_id': 6,
+              'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'key': 'value', 'p': '1'}},
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' bazbuz',
+              'body': '2024-03-30 This note contains a key::value pair.',
               'child_note_ids': [],
               'contexts': [],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 8,
+              'create_date': FakeDatetime(2024, 3, 30, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': 6,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}},
+              'properties': {'key': 'value', 'p': '1'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' pig',
+              'body': 'bazbuz',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 9,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 6,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}},
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' is fat',
+              'body': 'pig',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 10,
               'links': [],
               'next_note_id': None,
-              'parent_note_id': 9,
+              'parent_note_id': 6,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}},
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' is stinky',
+              'body': 'is fat',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 11,
               'links': [],
               'next_note_id': None,
               'parent_note_id': 9,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {'p': '1'}}],
-   'todos': [{'areas': [],
-              'body': ' This todo is due::2024-03-30 and has some subnotes',
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None},
+             {'areas': [],
+              'body': 'is stinky',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'done_date': None,
-              'ident': 2,
               'links': [],
               'next_note_id': None,
-              'parent_note_id': None,
+              'parent_note_id': 9,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
-              'properties': {'due': '2024-03-30', 'p': '1'},
-              'status': <TodoStatus.OPEN: 1>}]}
+              'properties': {'p': '1'},
+              'todo_payload': None,
+              'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-subsections]
   '''
   {'notes': [{'areas': [],
-              'body': ' Note about A1',
+              'body': 'Note about A1',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 1,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Note about something',
+              'body': 'Note about something',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 2,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' Another note',
+              'body': 'Another note',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 3,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' A note on the second section.',
+              'body': ' A todo for something',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 5,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None},
              {'areas': [],
-              'body': ' A sub-note.',
+              'body': 'A note on the second section.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 6,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' And another note.',
+              'body': 'A sub-note.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 7,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' This is inside of h4_section!',
+              'body': 'And another note.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 9,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' A note on the third section.',
+              'body': ' Some foobar todo.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 10,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None},
              {'areas': [],
-              'body': ' A sub-note.',
+              'body': 'This is inside of h4_section!',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 11,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' And another note.',
+              'body': 'A note on the third section.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 12,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
-              'body': ' This is the final section!',
+              'body': 'A sub-note.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 14,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
-              'properties': {}}],
-   'todos': [{'areas': [],
-              'body': ' A todo for something',
+              'properties': {},
+              'todo_payload': None,
+              'zid': None},
+             {'areas': [],
+              'body': 'And another note.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'done_date': None,
-              'ident': 4,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': None,
+              'zid': None},
              {'areas': [],
               'body': ' Some foobar todo.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'done_date': None,
-              'ident': 8,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'zid': None},
              {'areas': [],
-              'body': ' Some foobar todo.',
+              'body': 'This is the final section!',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'done_date': None,
-              'ident': 13,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'priority': 'C',
               'projects': [],
               'properties': {},
-              'status': <TodoStatus.OPEN: 1>}]}
+              'todo_payload': None,
+              'zid': None}]}
   
   '''
 # ---
-# name: test_compile[YAMLConfigFile-tags]
+# name: test_compile[YAMLConfigFile-tags_and_ids]
   '''
   {'notes': [{'areas': ['tags'],
-              'body': ' Some note',
+              'body': '240408#0X Some note',
               'child_note_ids': [],
               'contexts': ['fat_pig'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 1,
+              'create_date': FakeDatetime(2024, 4, 8, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': ['foobar'],
-              'properties': {}},
+              'properties': {},
+              'todo_payload': None,
+              'zid': '240408#0X'},
              {'areas': ['tags', 'thoughts'],
-              'body': ' When I talk to %pig I always want to @puke.',
+              'body': '301231#X0 When I talk to %pig I always want to @puke.',
               'child_note_ids': [],
               'contexts': ['fat_pig', 'puke'],
-              'create_date': FakeDate(2000, 1, 3),
-              'ident': 2,
+              'create_date': FakeDatetime(2030, 12, 31, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': ['pig'],
               'prev_note_id': None,
-              'projects': ['foobar/bazbuz'],
-              'properties': {}},
+              'projects': ['bazbuz', 'foobar'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': '301231#X0'},
              {'areas': ['tags'],
-              'body': ' Da nah nah nuh...',
+              'body': '240408#NO Da nah nah nuh...',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
-              'ident': 3,
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
-              'projects': ['bad/to_the_bone'],
-              'properties': {}}],
-   'todos': []}
+              'projects': ['bad', 'to_the_bone'],
+              'properties': {},
+              'todo_payload': None,
+              'zid': None}]}
   
   '''
 # ---
```

### Comparing `zettel-org-0.6.0/tests/__snapshots__/test_run_edit.ambr` & `zettel_org-0.6.1/tests/__snapshots__/test_run_edit.ambr`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   # 2000-01-03.Mon
   #
   # ^ = [[2000/20000103]]
   # < = [[2000/20000102_day]]
   # > = [[2000/20000104_day]]
   # @ = [[day_log.zot]]
   
-  o #gtd pomodoro
+  o 000103#1t #gtd pomodoro
     * Google Calendar (bbugyi@google + bryanbugyi34@gmail)
     * Process yesterday's bujo log (e.g. close events, add missing pomodoros, rollover goals)
     * Copy any important gchat convos from yesterday into chat/*.txt
     * Check today's tickler file: [[tick_03]]
     * Fill out yesterday's habit tracker: [[2000/20000102_habit]]
     * go/g3co
     * Review Google Keep Inbox
```

### Comparing `zettel-org-0.6.0/tests/__snapshots__/test_run_template.ambr` & `zettel_org-0.6.1/tests/__snapshots__/test_run_template.ambr`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/tests/common.py` & `zettel_org-0.6.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/tests/data/day_log.zot` & `zettel_org-0.6.1/tests/data/day_log.zot`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/tests/data/done_log.zot` & `zettel_org-0.6.1/tests/data/done_log.zot`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/tests/data/habit_log.zot` & `zettel_org-0.6.1/tests/data/habit_log.zot`

 * *Files identical despite different names*

### Comparing `zettel-org-0.6.0/tests/test_config.py` & `zettel_org-0.6.1/tests/test_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 from typing import Any, Sequence, cast
 
 from clack import clack_envvars_set
 from clack.types import ClackConfig
 
-from zorg.config import EditConfig, TemplateRenderConfig, clack_parser
+from zorg.app.config import EditConfig, TemplateRenderConfig, clack_parser
 
 
 def test_defaultToEdit_whenNoCommandIsGiven() -> None:
     """Default to 'edit' when no subcommand is explicitly specified.
 
     When no subcommand is provided, default to using the 'edit' command with
     the default file group (i.e. @default).
```

### Comparing `zettel-org-0.6.0/tests/test_file_groups.py` & `zettel_org-0.6.1/tests/test_file_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests that flex file group logic."""
 
 from pathlib import Path
 
-from zorg.file_groups import expand_file_group_paths
+from zorg.service.file_groups import expand_file_group_paths
 
 from . import common as c
 
 
 def test_expand_file_group_paths() -> None:
     """Tests that file group path expansion is WAI."""
     paths = expand_file_group_paths(
```

### Comparing `zettel-org-0.6.0/tests/test_run_action_open.py` & `zettel_org-0.6.1/tests/test_run_action_open.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,25 +16,20 @@
 @params(
     "lineno,expected",
     [(3, "foo.zo"), (5, "bar.sh"), (6, "baz.zo"), (7, "buz.zo")],
 )
 def test_action_open(
     main: c.MainType,
     capsys: CaptureFixture,
-    tmp_path: Path,
+    zettel_dir: Path,
     lineno: int,
     expected: str,
 ) -> None:
     """Test that the OPEN_LINK action is WAI."""
-    zettel_dir = tmp_path / "org"
-    zettel_dir.mkdir(parents=True, exist_ok=True)
-    path_to_links = Path(__file__).parent / Path("data/links.zo")
     zpath_to_links = zettel_dir / "links.zo"
-    zpath_to_links.write_bytes(path_to_links.read_bytes())
-
     exit_code = main(
         "--dir",
         str(zettel_dir),
         "action",
         "open",
         str(zpath_to_links),
         str(lineno),
```

### Comparing `zettel-org-0.6.0/tests/test_run_compile.py` & `zettel_org-0.6.1/tests/test_run_compile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 """Tests for the zorg project's 'compile' CLI command."""
 
 from __future__ import annotations
 
-import itertools as it
 from pathlib import Path
-from typing import Iterator
 
 from _pytest.capture import CaptureFixture
 from pytest import mark, param
 from syrupy.assertion import SnapshotAssertion as Snapshot
 
 from . import common as c
 
 
 params = mark.parametrize
 
 
 def _get_all_zo_paths() -> list[Path]:
-    tests_dir = Path(__file__).parent
-    data_dir = tests_dir / "data"
-    examples_dir = tests_dir.parent / "examples"
-    return sorted(
-        path
-        for path in it.chain(
-            _get_zo_path_iter(data_dir), _get_zo_path_iter(examples_dir)
-        )
-    )
-
-
-def _get_zo_path_iter(src_dir: Path) -> Iterator[Path]:
-    yield from src_dir.rglob("*.zo")
+    root_dir = Path(__file__).parent.parent
+    return sorted(root_dir.rglob("*.zo"))
 
 
 @params(
     "zo_path",
     [param(zo_path, id=zo_path.stem) for zo_path in _get_all_zo_paths()],
 )
 def test_compile(
```

### Comparing `zettel-org-0.6.0/tests/test_run_edit.py` & `zettel_org-0.6.1/tests/test_run_edit.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,38 +8,24 @@
 
 from syrupy.assertion import SnapshotAssertion as Snapshot
 
 from . import common as c
 
 
 def test_edit_day_logs(
-    main: c.MainType, vim_proc_mock: Mock, tmp_path: Path, snapshot: Snapshot
+    main: c.MainType, vim_proc_mock: Mock, zettel_dir: Path, snapshot: Snapshot
 ) -> None:
     """Test that we properly generate test day, habit, and done logs."""
-    zettel_dir = tmp_path / "org"
-    kwargs: dict[str, Any] = {
-        "vim_commands": ["echo hi", "source {zdir}/vimrc"]
-    }
-    for key, template_stem in [
-        ("day_log_template", "day_log"),
-        ("habit_log_template", "habit_log"),
-        ("done_log_template", "done_log"),
-    ]:
-        template_path: Path = zettel_dir / f"{template_stem}.zot"
-        template_path.parent.mkdir(parents=True, exist_ok=True)
-        test_data_template_path = Path(__file__).parent / Path(
-            f"data/{template_stem}.zot"
-        )
-        template_path.write_bytes(test_data_template_path.read_bytes())
-        kwargs[key] = template_path.name
-
     day_log = f"{c.YYYY}/{c.YYYY}{c.MM}{c.DD}.zo"
     habit_log = f"{c.YYYY}/{c.YYYY}{c.MM}{c.YEST_DD}_habit.zo"
     done_log = f"{c.YYYY}/{c.YYYY}{c.MM}{c.DD}_done.zo"
     re_date_group = "(?P<date>[0-9]{4}[01][0-9][0-3][0-9])"
+    kwargs: dict[str, Any] = {
+        "vim_commands": ["echo hi", "source {zdir}/vimrc"]
+    }
     exit_code = main(
         "--dir",
         str(zettel_dir),
         "edit",
         day_log,
         habit_log,
         done_log,
```

