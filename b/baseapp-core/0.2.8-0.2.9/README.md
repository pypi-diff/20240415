# Comparing `tmp/baseapp-core-0.2.8.tar.gz` & `tmp/baseapp-core-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp-core-0.2.8.tar", last modified: Wed Jan 31 13:53:56 2024, max compression
+gzip compressed data, was "baseapp-core-0.2.9.tar", last modified: Thu Feb 29 14:18:55 2024, max compression
```

## Comparing `baseapp-core-0.2.8.tar` & `baseapp-core-0.2.9.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.302519 baseapp-core-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-31 13:53:56.302519 baseapp-core-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.294519 baseapp-core-0.2.8/baseapp_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/debug_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/deep_links.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.298519 baseapp-core-0.2.8/baseapp_core/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/consumers.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/object_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/relay.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/serializer_mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.298519 baseapp-core-0.2.8/baseapp_core/graphql/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/graphql/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.298519 baseapp-core-0.2.8/baseapp_core/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/rest_framework/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/rest_framework/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/rest_framework/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/rest_framework/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/rest_framework/routers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.298519 baseapp-core-0.2.8/baseapp_core/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/settings/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.290519 baseapp-core-0.2.8/baseapp_core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.298519 baseapp-core-0.2.8/baseapp_core/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/templates/admin/base_site.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.298519 baseapp-core-0.2.8/baseapp_core/templates/emails/
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/templates/emails/base.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/templates/emails/base.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.302519 baseapp-core-0.2.8/baseapp_core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tests/test_celery_beat_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tests/test_migration_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/baseapp_core/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.294519 baseapp-core-0.2.8/baseapp_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-31 13:53:55.000000 baseapp-core-0.2.8/baseapp_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-01-31 13:53:56.000000 baseapp-core-0.2.8/baseapp_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 13:53:55.000000 baseapp-core-0.2.8/baseapp_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-31 13:53:55.000000 baseapp-core-0.2.8/baseapp_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-31 13:53:55.000000 baseapp-core-0.2.8/baseapp_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-31 13:53:56.302519 baseapp-core-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:56.302519 baseapp-core-0.2.8/testproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-31 13:53:54.000000 baseapp-core-0.2.8/testproject/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.670857 baseapp-core-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-29 14:18:55.670857 baseapp-core-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.662856 baseapp-core-0.2.9/baseapp_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/debug_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/deep_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.666857 baseapp-core-0.2.9/baseapp_core/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/consumers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/object_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/serializer_mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.666857 baseapp-core-0.2.9/baseapp_core/graphql/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/graphql/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.666857 baseapp-core-0.2.9/baseapp_core/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/rest_framework/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/rest_framework/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/rest_framework/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/rest_framework/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/rest_framework/routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.666857 baseapp-core-0.2.9/baseapp_core/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/settings/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.658856 baseapp-core-0.2.9/baseapp_core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.666857 baseapp-core-0.2.9/baseapp_core/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/templates/admin/base_site.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.666857 baseapp-core-0.2.9/baseapp_core/templates/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/templates/emails/base.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/templates/emails/base.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.670857 baseapp-core-0.2.9/baseapp_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tests/test_celery_beat_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tests/test_migration_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/baseapp_core/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.662856 baseapp-core-0.2.9/baseapp_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-29 14:18:55.000000 baseapp-core-0.2.9/baseapp_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-29 14:18:55.000000 baseapp-core-0.2.9/baseapp_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 14:18:55.000000 baseapp-core-0.2.9/baseapp_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-29 14:18:55.000000 baseapp-core-0.2.9/baseapp_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-29 14:18:55.000000 baseapp-core-0.2.9/baseapp_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-29 14:18:55.670857 baseapp-core-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:55.670857 baseapp-core-0.2.9/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-29 14:18:54.000000 baseapp-core-0.2.9/testproject/settings.py
```

### Comparing `baseapp-core-0.2.8/baseapp_core/channels.py` & `baseapp-core-0.2.9/baseapp_core/channels.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/deep_links.py` & `baseapp-core-0.2.9/baseapp_core/deep_links.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/__init__.py` & `baseapp-core-0.2.9/baseapp_core/graphql/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from .connections import CountedConnection  # noqa
 from .decorators import login_required, user_passes_test  # noqa
 from .errors import Errors, ErrorType  # noqa
 from .fields import File, ThumbnailField  # noqa
-from .middlewares import LogExceptionMiddleware, TokenAuthentication  # noqa
+from .middlewares import (  # noqa
+    JWTAuthentication,
+    LogExceptionMiddleware,
+    TokenAuthentication,
+)
 from .models import RelayModel  # noqa
-from .mutations import RelayMutation  # noqa
+from .mutations import DeleteNode, RelayMutation  # noqa
 from .object_types import DjangoObjectType  # noqa
 from .relay import Node  # noqa
 from .serializer_mutation import SerializerMutation  # noqa
+from .translation import LanguagesEnum  # noqa
 from .utils import get_obj_from_relay_id, get_obj_relay_id, get_pk_from_relay_id  # noqa
 from .views import GraphQLView  # noqa
```

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/consumers.py` & `baseapp-core-0.2.9/baseapp_core/graphql/consumers.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/decorators.py` & `baseapp-core-0.2.9/baseapp_core/graphql/decorators.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/fields.py` & `baseapp-core-0.2.9/baseapp_core/graphql/fields.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/middlewares.py` & `baseapp-core-0.2.9/baseapp_core/graphql/middlewares.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import logging
 
 from rest_framework.authentication import TokenAuthentication as RestTokenAuthentication
+from rest_framework_simplejwt.authentication import (
+    JWTAuthentication as RestJWTAuthentication,
+)
 
 
 class LogExceptionMiddleware(object):
     def on_error(self, error):
         # need to raise error again to get access to traceback
         try:
             raise error
@@ -23,11 +26,25 @@
     authenticated = False
 
     def resolve(self, next, root, info, **kwargs):
         if not self.authenticated:
             auth = self.authenticate(info.context)
             if auth:
                 user = auth[0]
+                if user and user.is_authenticated:
+                    info.context.user = user
+            self.authenticated = True
+        return next(root, info, **kwargs)
+
+
+class JWTAuthentication(RestJWTAuthentication):
+    authenticated = False
+
+    def resolve(self, next, root, info, **kwargs):
+        if not self.authenticated:
+            auth = self.authenticate(info.context)
+            if auth:
+                user = auth[0]
                 if user and user.is_authenticated:
                     info.context.user = user
             self.authenticated = True
         return next(root, info, **kwargs)
```

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/object_types.py` & `baseapp-core-0.2.9/baseapp_core/graphql/object_types.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/relay.py` & `baseapp-core-0.2.9/baseapp_core/graphql/relay.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/serializer_mutation.py` & `baseapp-core-0.2.9/baseapp_core/graphql/serializer_mutation.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/testing/fixtures.py` & `baseapp-core-0.2.9/baseapp_core/graphql/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/utils.py` & `baseapp-core-0.2.9/baseapp_core/graphql/utils.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/graphql/views.py` & `baseapp-core-0.2.9/baseapp_core/graphql/views.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/logging.py` & `baseapp-core-0.2.9/baseapp_core/logging.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/middleware.py` & `baseapp-core-0.2.9/baseapp_core/middleware.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/models.py` & `baseapp-core-0.2.9/baseapp_core/models.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/rest_framework/decorators.py` & `baseapp-core-0.2.9/baseapp_core/rest_framework/decorators.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/rest_framework/fields.py` & `baseapp-core-0.2.9/baseapp_core/rest_framework/fields.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/rest_framework/mixins.py` & `baseapp-core-0.2.9/baseapp_core/rest_framework/mixins.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/rest_framework/routers.py` & `baseapp-core-0.2.9/baseapp_core/rest_framework/routers.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/rest_framework/serializers.py` & `baseapp-core-0.2.9/baseapp_core/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/sentry.py` & `baseapp-core-0.2.9/baseapp_core/sentry.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/settings/env.py` & `baseapp-core-0.2.9/baseapp_core/settings/env.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/templates/admin/base_site.html` & `baseapp-core-0.2.9/baseapp_core/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/templates/emails/base.html.j2` & `baseapp-core-0.2.9/baseapp_core/templates/emails/base.html.j2`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/tests/fixtures.py` & `baseapp-core-0.2.9/baseapp_core/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/tests/helpers.py` & `baseapp-core-0.2.9/baseapp_core/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/tests/mixins.py` & `baseapp-core-0.2.9/baseapp_core/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/tests/settings.py` & `baseapp-core-0.2.9/baseapp_core/tests/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,20 +47,22 @@
     "rest_framework",
     "rest_framework.authtoken",
     "djmail",
     "baseapp_core",
     "easy_thumbnails",
     "constance",
     "constance.backends.database",
+    "pgtrigger",
     "pghistory",
 ]
 
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.locale.LocaleMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
 ]
 
@@ -164,15 +166,15 @@
 DJMAIL_REAL_BACKEND = "django.core.mail.backends.console.EmailBackend"
 
 # Channels
 CHANNEL_LAYERS = {"default": {"BACKEND": "channels.layers.InMemoryChannelLayer"}}
 
 # GraphQL
 GRAPHENE = {
-    "SCHEMA": "testproject.graphql.schema.schema",
+    "SCHEMA": "testproject.graphql.schema",
     "MIDDLEWARE": (
         "baseapp_core.graphql.LogExceptionMiddleware",
         "baseapp_core.graphql.TokenAuthentication",
     ),
     "SCHEMA_OUTPUT": "schema.graphql",
 }
```

### Comparing `baseapp-core-0.2.8/baseapp_core/tests/test_celery_beat_health_check.py` & `baseapp-core-0.2.9/baseapp_core/tests/test_celery_beat_health_check.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/tests/test_migration_health_check.py` & `baseapp-core-0.2.9/baseapp_core/tests/test_migration_health_check.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/tokens.py` & `baseapp-core-0.2.9/baseapp_core/tokens.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core/utils.py` & `baseapp-core-0.2.9/baseapp_core/utils.py`

 * *Files identical despite different names*

### Comparing `baseapp-core-0.2.8/baseapp_core.egg-info/SOURCES.txt` & `baseapp-core-0.2.9/baseapp_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 baseapp_core/graphql/fields.py
 baseapp_core/graphql/middlewares.py
 baseapp_core/graphql/models.py
 baseapp_core/graphql/mutations.py
 baseapp_core/graphql/object_types.py
 baseapp_core/graphql/relay.py
 baseapp_core/graphql/serializer_mutation.py
+baseapp_core/graphql/translation.py
 baseapp_core/graphql/utils.py
 baseapp_core/graphql/views.py
 baseapp_core/graphql/testing/__init__.py
 baseapp_core/graphql/testing/fixtures.py
 baseapp_core/rest_framework/__init__.py
 baseapp_core/rest_framework/decorators.py
 baseapp_core/rest_framework/fields.py
```

### Comparing `baseapp-core-0.2.8/setup.cfg` & `baseapp-core-0.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = baseapp-core
-version = 0.2.8
+version = 0.2.9
 description = BaseApp Core
 long_description = file: README.md
 url = https://github.com/silverlogic/baseapp-backend
 author = The SilverLogic
 author_email = dev@tsl.io
 license = BSD-3-Clause  # Example license
```

