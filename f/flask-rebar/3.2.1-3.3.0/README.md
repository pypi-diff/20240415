# Comparing `tmp/flask-rebar-3.2.1.tar.gz` & `tmp/flask_rebar-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-rebar-3.2.1.tar", last modified: Wed Mar 27 18:13:45 2024, max compression
+gzip compressed data, was "flask_rebar-3.3.0.tar", last modified: Mon Apr 15 21:25:49 2024, max compression
```

## Comparing `flask-rebar-3.2.1.tar` & `flask_rebar-3.3.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.228082 flask-rebar-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-03-27 18:13:45.228082 flask-rebar-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.200081 flask-rebar-3.2.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.200081 flask-rebar-3.2.1/examples/todo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/generate_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.204081 flask-rebar-3.2.1/examples/todo/todo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/todo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/todo/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/todo/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/todo/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.204081 flask-rebar-3.2.1/examples/todo/todo/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/todo/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/todo/handlers/todo_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/todo/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/examples/todo/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.204081 flask-rebar-3.2.1/flask_rebar/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.204081 flask-rebar-3.2.1/flask_rebar/authenticators/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/authenticators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/authenticators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/authenticators/header_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    34831 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/rebar.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/request_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.208082 flask-rebar-3.2.1/flask_rebar/swagger_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/authenticator_to_swagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/marshmallow_to_swagger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.208082 flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_generator/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_generator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_generator_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_generator_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_words.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.208082 flask-rebar-3.2.1/flask_rebar/swagger_ui/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.224082 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/oauth2-redirect.html
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-initializer.js
--rw-r--r--   0 runner    (1001) docker     (127)  1442694 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)  2079773 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   504647 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-es-bundle-core.js
--rw-r--r--   0 runner    (1001) docker     (127)  1651449 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-es-bundle-core.js.map
--rw-r--r--   0 runner    (1001) docker     (127)  1442484 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-es-bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)  2070565 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-es-bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   246440 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (127)   398288 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   150947 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (127)   260489 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   389867 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui.js
--rw-r--r--   0 runner    (1001) docker     (127)   423707 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.224082 flask-rebar-3.2.1/flask_rebar/swagger_ui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/swagger_ui/templates/index.html.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.224082 flask-rebar-3.2.1/flask_rebar/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71601 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/testing/swagger_jsonschema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.228082 flask-rebar-3.2.1/flask_rebar/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/utils/marshmallow_objects_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/utils/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/flask_rebar/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.228082 flask-rebar-3.2.1/flask_rebar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-03-27 18:13:45.000000 flask-rebar-3.2.1/flask_rebar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-03-27 18:13:45.000000 flask-rebar-3.2.1/flask_rebar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 18:13:45.000000 flask-rebar-3.2.1/flask_rebar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-27 18:13:45.000000 flask-rebar-3.2.1/flask_rebar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 18:13:45.000000 flask-rebar-3.2.1/flask_rebar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-27 18:13:45.232082 flask-rebar-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:13:45.228082 flask-rebar-3.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/tests/test_deprecation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    29561 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/tests/test_rebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/tests/test_request_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-03-27 18:13:41.000000 flask-rebar-3.2.1/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.716881 flask_rebar-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-15 21:25:49.716881 flask_rebar-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.688881 flask_rebar-3.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.692881 flask_rebar-3.3.0/examples/todo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/generate_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.692881 flask_rebar-3.3.0/examples/todo/todo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/todo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/todo/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/todo/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/todo/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.692881 flask_rebar-3.3.0/examples/todo/todo/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/todo/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/todo/handlers/todo_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/todo/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/examples/todo/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.692881 flask_rebar-3.3.0/flask_rebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.696881 flask_rebar-3.3.0/flask_rebar/authenticators/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/authenticators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/authenticators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/authenticators/header_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    34856 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/rebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/request_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.696881 flask_rebar-3.3.0/flask_rebar/swagger_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/authenticator_to_swagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/marshmallow_to_swagger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.696881 flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_generator_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_generator_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_words.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.696881 flask_rebar-3.3.0/flask_rebar/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.712881 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-initializer.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1442694 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2079773 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   504647 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1651449 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-es-bundle-core.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)  1442484 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-es-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2070565 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-es-bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   246440 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (127)   398288 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   150947 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (127)   260489 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   389867 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)   423707 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.712881 flask_rebar-3.3.0/flask_rebar/swagger_ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/swagger_ui/templates/index.html.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.712881 flask_rebar-3.3.0/flask_rebar/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71601 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/testing/swagger_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.716881 flask_rebar-3.3.0/flask_rebar/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/utils/marshmallow_objects_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/utils/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/flask_rebar/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.716881 flask_rebar-3.3.0/flask_rebar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-15 21:25:49.000000 flask_rebar-3.3.0/flask_rebar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-15 21:25:49.000000 flask_rebar-3.3.0/flask_rebar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:25:49.000000 flask_rebar-3.3.0/flask_rebar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 21:25:49.000000 flask_rebar-3.3.0/flask_rebar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 21:25:49.000000 flask_rebar-3.3.0/flask_rebar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 21:25:49.720881 flask_rebar-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:25:49.716881 flask_rebar-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/tests/test_deprecation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30079 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/tests/test_rebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/tests/test_request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-15 21:25:46.000000 flask_rebar-3.3.0/tests/test_validation.py
```

### Comparing `flask-rebar-3.2.1/LICENSE` & `flask_rebar-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/PKG-INFO` & `flask_rebar-3.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rebar
-Version: 3.2.1
+Version: 3.3.0
 Summary: Flask-Rebar combines flask, marshmallow, and swagger for robust REST services.
 Home-page: https://github.com/plangrid/flask-rebar
 Author: Barak Alon
 Author-email: barak.s.alon@gmail.com
 License: MIT
 Keywords: flask,rest,marshmallow,openapi,swagger
 Classifier: Environment :: Web Environment
@@ -40,16 +40,19 @@
 Requires-Dist: pre-commit>=1.14.4; extra == "dev"
 Requires-Dist: pytest~=7.4; extra == "dev"
 Requires-Dist: pytest-order~=1.0; extra == "dev"
 Requires-Dist: Sphinx<7.0.0,>=6.0.0; extra == "dev"
 Requires-Dist: sphinx_rtd_theme==1.2.2; extra == "dev"
 Requires-Dist: types-jsonschema==4.17.0.10; extra == "dev"
 Requires-Dist: types-setuptools==68.0.0.3; extra == "dev"
+Requires-Dist: flask[async]<4,>=2; extra == "dev"
 Provides-Extra: enum
 Requires-Dist: marshmallow-enum~=1.5; extra == "enum"
+Provides-Extra: async
+Requires-Dist: flask[async]<4,>=2; extra == "async"
 
 Flask-Rebar
 ===========
 
 .. image:: https://readthedocs.org/projects/flask-rebar/badge/?version=latest
    :target: http://flask-rebar.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
```

### Comparing `flask-rebar-3.2.1/README.rst` & `flask_rebar-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/examples/todo/generate_output.py` & `flask_rebar-3.3.0/examples/todo/generate_output.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/examples/todo/todo/app.py` & `flask_rebar-3.3.0/examples/todo/todo/app.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/examples/todo/todo/converters.py` & `flask_rebar-3.3.0/examples/todo/todo/converters.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/examples/todo/todo/handlers/todo_handlers.py` & `flask_rebar-3.3.0/examples/todo/todo/handlers/todo_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import Enum
+import asyncio
 
 from todo.database import todo_id_sequence, todo_database
 from todo.app import rebar
 from todo.app import registry
 from todo.schemas import (
     CreateTodoSchema,
     GetTodoListSchema,
```

### Comparing `flask-rebar-3.2.1/examples/todo/todo/schemas.py` & `flask_rebar-3.3.0/examples/todo/todo/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/__init__.py` & `flask_rebar-3.3.0/flask_rebar/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/authenticators/base.py` & `flask_rebar-3.3.0/flask_rebar/authenticators/base.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/authenticators/header_api_key.py` & `flask_rebar-3.3.0/flask_rebar/authenticators/header_api_key.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/compat.py` & `flask_rebar-3.3.0/flask_rebar/compat.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/errors.py` & `flask_rebar-3.3.0/flask_rebar/errors.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/messages.py` & `flask_rebar-3.3.0/flask_rebar/messages.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/rebar.py` & `flask_rebar-3.3.0/flask_rebar/rebar.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
         if request_body_schema:
             g.validated_body = get_json_body_params_or_400(schema=request_body_schema)
 
         if headers_schema:
             g.validated_headers = get_header_params_or_400(schema=headers_schema)
 
-        rv: Any = f(*args, **kwargs)
+        rv: Any = current_app.ensure_sync(f)(*args, **kwargs)
 
         if not response_body_schema:
             return rv
 
         if isinstance(rv, current_app.response_class):
             schema = response_body_schema[rv.status_code]
             # The schema may be set to None to bypass marshaling (e.g. for 204 responses).
```

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_generation/__init__.py` & `flask_rebar-3.3.0/flask_rebar/swagger_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_generation/authenticator_to_swagger.py` & `flask_rebar-3.3.0/flask_rebar/swagger_generation/authenticator_to_swagger.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_generation/generator_utils.py` & `flask_rebar-3.3.0/flask_rebar/swagger_generation/generator_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_generation/marshmallow_to_swagger.py` & `flask_rebar-3.3.0/flask_rebar/swagger_generation/marshmallow_to_swagger.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_generator_base.py` & `flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_generator_base.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_generator_v2.py` & `flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_generator_v2.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_generator_v3.py` & `flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_generator_v3.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_objects.py` & `flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_objects.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_generation/swagger_words.py` & `flask_rebar-3.3.0/flask_rebar/swagger_generation/swagger_words.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/blueprint.py` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/favicon-16x16.png` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/favicon-32x32.png` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/index.html` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/index.html`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/oauth2-redirect.html` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-initializer.js` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-bundle.js` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-es-bundle-core.js` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-es-bundle-core.js.map` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-es-bundle-core.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-es-bundle.js` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-es-bundle.js.map` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-es-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui.css` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui.css.map` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui.js` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/static/swagger-ui.js.map` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/static/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/swagger_ui/templates/index.html.jinja2` & `flask_rebar-3.3.0/flask_rebar/swagger_ui/templates/index.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/testing/__init__.py` & `flask_rebar-3.3.0/flask_rebar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/testing/swagger_jsonschema.py` & `flask_rebar-3.3.0/flask_rebar/testing/swagger_jsonschema.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/utils/deprecation.py` & `flask_rebar-3.3.0/flask_rebar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/utils/marshmallow_objects_helpers.py` & `flask_rebar-3.3.0/flask_rebar/utils/marshmallow_objects_helpers.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/utils/request_utils.py` & `flask_rebar-3.3.0/flask_rebar/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar/validation.py` & `flask_rebar-3.3.0/flask_rebar/validation.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/flask_rebar.egg-info/PKG-INFO` & `flask_rebar-3.3.0/flask_rebar.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rebar
-Version: 3.2.1
+Version: 3.3.0
 Summary: Flask-Rebar combines flask, marshmallow, and swagger for robust REST services.
 Home-page: https://github.com/plangrid/flask-rebar
 Author: Barak Alon
 Author-email: barak.s.alon@gmail.com
 License: MIT
 Keywords: flask,rest,marshmallow,openapi,swagger
 Classifier: Environment :: Web Environment
@@ -40,16 +40,19 @@
 Requires-Dist: pre-commit>=1.14.4; extra == "dev"
 Requires-Dist: pytest~=7.4; extra == "dev"
 Requires-Dist: pytest-order~=1.0; extra == "dev"
 Requires-Dist: Sphinx<7.0.0,>=6.0.0; extra == "dev"
 Requires-Dist: sphinx_rtd_theme==1.2.2; extra == "dev"
 Requires-Dist: types-jsonschema==4.17.0.10; extra == "dev"
 Requires-Dist: types-setuptools==68.0.0.3; extra == "dev"
+Requires-Dist: flask[async]<4,>=2; extra == "dev"
 Provides-Extra: enum
 Requires-Dist: marshmallow-enum~=1.5; extra == "enum"
+Provides-Extra: async
+Requires-Dist: flask[async]<4,>=2; extra == "async"
 
 Flask-Rebar
 ===========
 
 .. image:: https://readthedocs.org/projects/flask-rebar/badge/?version=latest
    :target: http://flask-rebar.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
```

### Comparing `flask-rebar-3.2.1/flask_rebar.egg-info/SOURCES.txt` & `flask_rebar-3.3.0/flask_rebar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/pyproject.toml` & `flask_rebar-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/setup.py` & `flask_rebar-3.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,42 @@
     "pre-commit>=1.14.4",
     "pytest~=7.4",
     "pytest-order~=1.0",
     "Sphinx>=6.0.0,<7.0.0",
     "sphinx_rtd_theme==1.2.2",
     "types-jsonschema==4.17.0.10",
     "types-setuptools==68.0.0.3",
+    "flask[async]>=2,<4",
 ]
 
 install_requires = [
     "Flask>=1.0,<4",
     "marshmallow>=3.0,<4",
     "typing-extensions>=4.8,<5;python_version<'3.10'",
     "Werkzeug>=2.2,<4",
 ]
 
 if __name__ == "__main__":
     setup(
         name="flask-rebar",
-        version="3.2.1",
+        version="3.3.0",
         author="Barak Alon",
         author_email="barak.s.alon@gmail.com",
         description="Flask-Rebar combines flask, marshmallow, and swagger for robust REST services.",
         long_description=open("README.rst").read(),
         keywords=["flask", "rest", "marshmallow", "openapi", "swagger"],
         license="MIT",
         packages=find_packages(exclude=("test*", "examples")),
         package_data={"flask_rebar": ["py.typed"]},
         include_package_data=True,
-        extras_require={"dev": development, "enum": ["marshmallow-enum~=1.5"]},
+        extras_require={
+            "dev": development,
+            "enum": ["marshmallow-enum~=1.5"],
+            "async": ["flask[async]>=2,<4"],
+        },
         install_requires=install_requires,
         url="https://github.com/plangrid/flask-rebar",
         classifiers=[
             "Environment :: Web Environment",
             "Framework :: Flask",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: MIT License",
```

### Comparing `flask-rebar-3.2.1/tests/test_deprecation_utils.py` & `flask_rebar-3.3.0/tests/test_deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/tests/test_errors.py` & `flask_rebar-3.3.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/tests/test_rebar.py` & `flask_rebar-3.3.0/tests/test_rebar.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     ~~~~~~~~~~
 
     Tests for the basic usage of Flask-Rebar.
 
     :copyright: Copyright 2018 PlanGrid, Inc., see AUTHORS.
     :license: MIT, see LICENSE for details.
 """
+import asyncio
 import json
 import unittest
 
 import marshmallow as m
 import marshmallow_objects as mo
 from flask import Flask, make_response
 
@@ -860,7 +861,24 @@
         # ensure Swagger generation doesn't break (Issue #115)
         from flask_rebar import SwaggerV2Generator, SwaggerV3Generator
 
         swagger = SwaggerV2Generator().generate(registry)
         self.assertIsNotNone(swagger)  # really only care that it didn't barf
         swagger = SwaggerV3Generator().generate(registry)
         self.assertIsNotNone(swagger)
+
+    def test_async_handler(self):
+        rebar = Rebar()
+        registry = rebar.create_handler_registry()
+
+        @registry.handles(
+            rule="/async",
+            method="GET",
+            response_body_schema=DefaultResponseSchema(),
+        )
+        async def get_response():
+            await asyncio.sleep(0)
+            return DEFAULT_RESPONSE
+
+        app = create_rebar_app(rebar)
+        resp = app.test_client().get(path="/async")
+        self.assertEqual(resp.status_code, 200)
```

### Comparing `flask-rebar-3.2.1/tests/test_request_utils.py` & `flask_rebar-3.3.0/tests/test_request_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-3.2.1/tests/test_validation.py` & `flask_rebar-3.3.0/tests/test_validation.py`

 * *Files identical despite different names*

