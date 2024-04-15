# Comparing `tmp/tendril-auth-0.4.0.tar.gz` & `tmp/tendril_auth-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-auth-0.4.0.tar", last modified: Wed Apr 10 18:32:21 2024, max compression
+gzip compressed data, was "tendril_auth-0.4.1.tar", last modified: Mon Apr 15 06:50:05 2024, max compression
```

## Comparing `tendril-auth-0.4.0.tar` & `tendril_auth-0.4.1.tar`

### file list

```diff
@@ -1,73 +1,78 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.482400 tendril-auth-0.4.0/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-auth-0.4.0/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3253 2023-03-15 16:03:53.000000 tendril-auth-0.4.0/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.478401 tendril-auth-0.4.0/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.4.0/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.486400 tendril-auth-0.4.0/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.4.0/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1198 2024-04-08 19:39:52.000000 tendril-auth-0.4.0/src/tendril/apiserver/routers/authn.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authn/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-16 14:15:27.000000 tendril-auth-0.4.0/src/tendril/authn/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6159 2024-04-09 12:57:03.000000 tendril-auth-0.4.0/src/tendril/authn/auth0.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1836 2023-04-21 09:10:22.000000 tendril-auth-0.4.0/src/tendril/authn/client.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authn/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.4.0/src/tendril/authn/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril-auth-0.4.0/src/tendril/authn/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril-auth-0.4.0/src/tendril/authn/db/mixins.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril-auth-0.4.0/src/tendril/authn/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1393 2023-04-21 12:28:51.000000 tendril-auth-0.4.0/src/tendril/authn/pydantic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2945 2024-04-09 12:57:04.000000 tendril-auth-0.4.0/src/tendril/authn/users.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril-auth-0.4.0/src/tendril/authz/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1926 2023-09-12 04:42:42.000000 tendril-auth-0.4.0/src/tendril/authz/auth0.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril-auth-0.4.0/src/tendril/authz/connector.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authz/domains/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      245 2024-04-08 19:48:32.000000 tendril-auth-0.4.0/src/tendril/authz/domains/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      435 2024-04-09 13:07:58.000000 tendril-auth-0.4.0/src/tendril/authz/domains/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1030 2024-04-10 18:31:18.000000 tendril-auth-0.4.0/src/tendril/authz/domains/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1094 2024-04-08 20:14:41.000000 tendril-auth-0.4.0/src/tendril/authz/domains/scopes.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril-auth-0.4.0/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril-auth-0.4.0/src/tendril/authz/scopes/common.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1357 2023-02-28 00:59:55.000000 tendril-auth-0.4.0/src/tendril/authz/scopes/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.490400 tendril-auth-0.4.0/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-auth-0.4.0/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2708 2023-03-28 18:07:23.000000 tendril-auth-0.4.0/src/tendril/config/auth.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/src/tendril_auth.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1415 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-10 18:32:21.000000 tendril-auth-0.4.0/src/tendril_auth.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 18:32:21.494400 tendril-auth-0.4.0/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril-auth-0.4.0/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.991567 tendril_auth-0.4.1/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5384 2024-04-15 06:50:05.987568 tendril_auth-0.4.1/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.971567 tendril_auth-0.4.1/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_auth-0.4.1/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-15 06:50:05.991567 tendril_auth-0.4.1/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3286 2024-04-15 02:28:03.000000 tendril_auth-0.4.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.971567 tendril_auth-0.4.1/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril_auth-0.4.1/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.975567 tendril_auth-0.4.1/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril_auth-0.4.1/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1198 2024-04-08 19:39:52.000000 tendril_auth-0.4.1/src/tendril/apiserver/routers/authn.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2024-04-15 05:40:52.000000 tendril_auth-0.4.1/src/tendril/apiserver/routers/jwt.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.979567 tendril_auth-0.4.1/src/tendril/authn/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-16 14:15:27.000000 tendril_auth-0.4.1/src/tendril/authn/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6159 2024-04-09 12:57:03.000000 tendril_auth-0.4.1/src/tendril/authn/auth0.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1836 2023-04-21 09:10:22.000000 tendril_auth-0.4.1/src/tendril/authn/client.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.979567 tendril_auth-0.4.1/src/tendril/authn/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril_auth-0.4.1/src/tendril/authn/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril_auth-0.4.1/src/tendril/authn/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril_auth-0.4.1/src/tendril/authn/db/mixins.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril_auth-0.4.1/src/tendril/authn/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1393 2023-04-21 12:28:51.000000 tendril_auth-0.4.1/src/tendril/authn/pydantic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2945 2024-04-09 12:57:04.000000 tendril_auth-0.4.1/src/tendril/authn/users.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.979567 tendril_auth-0.4.1/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril_auth-0.4.1/src/tendril/authz/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1926 2023-09-12 04:42:42.000000 tendril_auth-0.4.1/src/tendril/authz/auth0.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril_auth-0.4.1/src/tendril/authz/connector.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril/authz/domains/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      245 2024-04-08 19:48:32.000000 tendril_auth-0.4.1/src/tendril/authz/domains/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      456 2024-04-15 05:12:04.000000 tendril_auth-0.4.1/src/tendril/authz/domains/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1218 2024-04-15 05:45:55.000000 tendril_auth-0.4.1/src/tendril/authz/domains/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1094 2024-04-08 20:14:41.000000 tendril_auth-0.4.1/src/tendril/authz/domains/scopes.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril_auth-0.4.1/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril_auth-0.4.1/src/tendril/authz/scopes/common.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1431 2024-04-10 20:39:39.000000 tendril_auth-0.4.1/src/tendril/authz/scopes/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril_auth-0.4.1/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3766 2024-04-15 05:50:52.000000 tendril_auth-0.4.1/src/tendril/config/auth.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril/jwt/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-15 04:11:08.000000 tendril_auth-0.4.1/src/tendril/jwt/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      567 2024-04-15 05:56:45.000000 tendril_auth-0.4.1/src/tendril/jwt/secrets.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1093 2024-04-15 05:56:45.000000 tendril_auth-0.4.1/src/tendril/jwt/signer.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/src/tendril_auth.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5384 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1533 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      604 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-15 06:50:05.000000 tendril_auth-0.4.1/src/tendril_auth.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-15 06:50:05.983567 tendril_auth-0.4.1/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril_auth-0.4.1/tox.ini
```

### Comparing `tendril-auth-0.4.0/.gitignore` & `tendril_auth-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/.readthedocs.yml` & `tendril_auth-0.4.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/.travis.yml` & `tendril_auth-0.4.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/LICENSE` & `tendril_auth-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/README.rst` & `tendril_auth-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/docs/Makefile` & `tendril_auth-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/docs/_static/custom.css` & `tendril_auth-0.4.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/docs/_static/favicon.ico` & `tendril_auth-0.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/docs/_static/logo.png` & `tendril_auth-0.4.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/docs/_static/logo_packed.png` & `tendril_auth-0.4.1/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/docs/_templates/about.html` & `tendril_auth-0.4.1/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/docs/conf.py` & `tendril_auth-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/docs/index.rst` & `tendril_auth-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/docs/installation.rst` & `tendril_auth-0.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/setup.py` & `tendril_auth-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 core_dependencies = [
     'fastapi',
     'fastapi_auth0',
     'tendril-config',
     'tendril-caching',
     'tendril-utils-db',
     'auth0-python>=4.0',
+    'pyjwt',
+    'cryptography',
 ]
 
 install_requires = core_dependencies + ['wheel']
 
 setup_requires = ['setuptools_scm']
 
 doc_requires = setup_requires + ['sphinx', 'sphinx-argparse', 'alabaster']
```

### Comparing `tendril-auth-0.4.0/src/tendril/apiserver/routers/authn.py` & `tendril_auth-0.4.1/src/tendril/apiserver/routers/authn.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authn/auth0.py` & `tendril_auth-0.4.1/src/tendril/authn/auth0.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authn/client.py` & `tendril_auth-0.4.1/src/tendril/authn/client.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authn/db/controller.py` & `tendril_auth-0.4.1/src/tendril/authn/db/controller.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authn/db/model.py` & `tendril_auth-0.4.1/src/tendril/authn/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authn/pydantic.py` & `tendril_auth-0.4.1/src/tendril/authn/pydantic.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authn/users.py` & `tendril_auth-0.4.1/src/tendril/authn/users.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authz/auth0.py` & `tendril_auth-0.4.1/src/tendril/authz/auth0.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authz/connector.py` & `tendril_auth-0.4.1/src/tendril/authz/connector.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authz/domains/manager.py` & `tendril_auth-0.4.1/src/tendril/authz/domains/manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 
 import importlib
 
+from tendril.jwt.signer import register_domain
 from tendril.utils.versions import get_namespace_package_names
 from tendril.utils import log
 logger = log.get_logger(__name__)
 
 
 class AuthzDomainsManager(object):
     def __init__(self, prefix):
@@ -19,14 +20,17 @@
         modules = list(get_namespace_package_names(self._prefix))
         for m_name in modules:
             if m_name == __name__:
                 continue
             m = importlib.import_module(m_name)
             logger.info("Loading authz domains from {0}".format(m_name))
             self._domains.update(m.domains)
+            for domain, obj in m.domains.items():
+                if obj.jwt_spec:
+                    register_domain(domain, obj.jwt_spec)
 
     def finalize(self):
         self.finalized = True
 
     async def upsert(self, user, first_login):
         for domain in self._domains.values():
             await domain.upsert(user, first_login)
```

### Comparing `tendril-auth-0.4.0/src/tendril/authz/domains/scopes.py` & `tendril_auth-0.4.1/src/tendril/authz/domains/scopes.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/authz/scopes/manager.py` & `tendril_auth-0.4.1/src/tendril/authz/scopes/manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             self._scopes.update(m.scopes)
             if hasattr(m, 'default_scopes'):
                 self._default_scopes.extend(m.default_scopes)
 
     def finalize(self):
         self.finalized = True
         if AUTH0_PATCH_SCOPES_ON_STARTUP:
+            # TODO This causes a circular import which needs to be fixed.
             self._create_scopes()
 
     @property
     def scopes(self):
         return self._scopes
 
     @property
```

### Comparing `tendril-auth-0.4.0/src/tendril/config/__init__.py` & `tendril_auth-0.4.1/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/src/tendril/config/auth.py` & `tendril_auth-0.4.1/src/tendril/config/auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -79,19 +79,53 @@
         'None',
         'Auth0 Connection to use to store Mechanized Users'
     ),
     ConfigOption(
         'AUTH0_MECHANIZED_USER_DOMAIN',
         '"tendril.link"',
         "Domain to use for mechanized user email addresses."
+    ),
+    ConfigOption(
+        'AUTH_JWKS_PATH',
+        'os.path.join(INSTANCE_ROOT, "jwt", "jwks.json")',
+        "Path to the jwks.json file to serve."
+    ),
+    ConfigOption(
+        'AUTH_JWT_PRIVATE_KEY',
+        'os.path.join(INSTANCE_ROOT, "jwt", "privateKey.pem")',
+        "Path to the private key to use to sign JWTs."
+    ),
+    ConfigOption(
+        'AUTH_JWT_PUBLIC_KEY',
+        'os.path.join(INSTANCE_ROOT, "jwt", "publicKey.pem")',
+        "Path to the public key to use to verify JWTs."
+    ),
+    ConfigOption(
+        'AUTH_JWT_ISSUER',
+        '"tendril.link"',
+        "Issuer to specify in the issued JWT claims."
+    ),
+    ConfigOption(
+        'AUTH_JWT_TTL',
+        '0',
+        "TTL in seconds before the issued JWT can be used."
+    ),
+    ConfigOption(
+        'AUTH_JWT_VALIDITY',
+        '3600',
+        "Duration in seconds before the issued JWT is expired."
+    ),
+    ConfigOption(
+        'AUTH_JWT_ALGORITHMS',
+        '["RS256"]',
+        "Algorithm to use to sign or verify JWTs. The first element used for encode."
     )
 ]
 
 
 def load(manager):
     logger.debug("Loading {0}".format(__name__))
     manager.load_elements(config_elements_auth,
                           doc="Authentication Configuration")
     if manager.AUTH_PROVIDER == "auth0":
         manager.load_elements(config_elements_auth0,
                               doc="Auth0 Configuration")
-
```

### Comparing `tendril-auth-0.4.0/src/tendril_auth.egg-info/SOURCES.txt` & `tendril_auth-0.4.1/src/tendril_auth.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 docs/api/index.rst
 docs/usage/standalone.rst
 docs/usage/tendril.rst
 src/tendril/__init__.py
 src/tendril/apiserver/__init__.py
 src/tendril/apiserver/routers/__init__.py
 src/tendril/apiserver/routers/authn.py
+src/tendril/apiserver/routers/jwt.py
 src/tendril/authn/__init__.py
 src/tendril/authn/auth0.py
 src/tendril/authn/client.py
 src/tendril/authn/pydantic.py
 src/tendril/authn/users.py
 src/tendril/authn/db/__init__.py
 src/tendril/authn/db/controller.py
@@ -41,14 +42,17 @@
 src/tendril/authz/domains/manager.py
 src/tendril/authz/domains/scopes.py
 src/tendril/authz/scopes/__init__.py
 src/tendril/authz/scopes/common.py
 src/tendril/authz/scopes/manager.py
 src/tendril/config/__init__.py
 src/tendril/config/auth.py
+src/tendril/jwt/__init__.py
+src/tendril/jwt/secrets.py
+src/tendril/jwt/signer.py
 src/tendril_auth.egg-info/PKG-INFO
 src/tendril_auth.egg-info/SOURCES.txt
 src/tendril_auth.egg-info/dependency_links.txt
 src/tendril_auth.egg-info/requires.txt
 src/tendril_auth.egg-info/top_level.txt
 tests/__init__.py
 tests/coveralls.py
```

### Comparing `tendril-auth-0.4.0/src/tendril_auth.egg-info/requires.txt` & `tendril_auth-0.4.1/src/tendril_auth.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 fastapi
 fastapi_auth0
 tendril-config
 tendril-caching
 tendril-utils-db
 auth0-python>=4.0
+pyjwt
+cryptography
 wheel
 
 [build]
 setuptools_scm
 sphinx
 sphinx-argparse
 alabaster
```

### Comparing `tendril-auth-0.4.0/tests/coveralls.py` & `tendril_auth-0.4.1/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.4.0/tox.ini` & `tendril_auth-0.4.1/tox.ini`

 * *Files identical despite different names*

