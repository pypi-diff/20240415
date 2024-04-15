# Comparing `tmp/oarepo_model_builder-4.0.84.tar.gz` & `tmp/oarepo-model-builder-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo_model_builder-4.0.84.tar", last modified: Mon Apr 15 11:15:51 2024, max compression
+gzip compressed data, was "oarepo-model-builder-4.0.9.tar", last modified: Tue May 30 18:25:02 2023, max compression
```

## Comparing `oarepo_model_builder-4.0.84.tar` & `oarepo-model-builder-4.0.9.tar`

### file list

```diff
@@ -1,220 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.957401 oarepo_model_builder-4.0.84/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-15 11:15:51.957401 oarepo_model_builder-4.0.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.925401 oarepo_model_builder-4.0.84/oarepo_model_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.929401 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/json_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/model_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/pyproject_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/python.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/python_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/setup_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.929401 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/templates/setup.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.929401 oarepo_model_builder-4.0.84/oarepo_model_builder/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/builtin_models/invenio.json
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.929401 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.929401 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.933400 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.933400 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.937401 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/blueprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/edtf_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/ext_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/model_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/pid.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/record_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/record_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/record_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/search_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.937401 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/sort/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/sort/field.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/sort/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.941401 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/containers/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/containers/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/containers/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/containers/nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/containers/object.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/primitive_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/generate_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.945401 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/edtf_interval_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_api_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_app_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_ext_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_resource_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_search_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_ui_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_script_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.949401 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/api_views.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/app_views.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/edtf_interval_record_dumper.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/ext.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/ext_resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/proxies.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/record_item.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/record_list.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/resource_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/version.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.949401 oarepo_model_builder-4.0.84/oarepo_model_builder/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/loaders/extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/merger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.953401 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/json_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/python.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/toml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.953401 oarepo_model_builder-4.0.84/oarepo_model_builder/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/profiles/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.953401 oarepo_model_builder-4.0.84/oarepo_model_builder/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/settings/opensearch.json
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/settings/python.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.953401 oarepo_model_builder-4.0.84/oarepo_model_builder/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.957401 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/absolute_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/camelcase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.957401 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/indented_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/mergers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/simple_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/facet_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/import_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/python_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/utils/verbose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.957401 oarepo_model_builder-4.0.84/oarepo_model_builder/validation/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/validation/extensibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/validation/model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/validation/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/oarepo_model_builder/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:15:51.957401 oarepo_model_builder-4.0.84/oarepo_model_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-15 11:15:51.000000 oarepo_model_builder-4.0.84/oarepo_model_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-04-15 11:15:51.000000 oarepo_model_builder-4.0.84/oarepo_model_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:15:51.000000 oarepo_model_builder-4.0.84/oarepo_model_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7510 2024-04-15 11:15:51.000000 oarepo_model_builder-4.0.84/oarepo_model_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-15 11:15:51.000000 oarepo_model_builder-4.0.84/oarepo_model_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 11:15:51.000000 oarepo_model_builder-4.0.84/oarepo_model_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-15 11:15:51.961401 oarepo_model_builder-4.0.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 11:11:44.000000 oarepo_model_builder-4.0.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.369763 oarepo-model-builder-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-30 18:25:02.369763 oarepo-model-builder-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.341763 oarepo-model-builder-4.0.9/oarepo_model_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.345763 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/json_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/pyproject_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/python_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/setup_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.345763 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/templates/setup.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.345763 oarepo-model-builder-4.0.9/oarepo_model_builder/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/builtin_models/invenio.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.345763 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.345763 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.349763 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.349763 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.353763 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.353763 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/containers/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/containers/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/containers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/containers/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/primitive_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/generate_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.357763 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_api_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_app_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_resource_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_ui_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_script_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.357763 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/api_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/app_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/ext.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/imports.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/proxies.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/resource.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/resource_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/service_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/version.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.357763 oarepo-model-builder-4.0.9/oarepo_model_builder/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.357763 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/json_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.361763 oarepo-model-builder-4.0.9/oarepo_model_builder/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/profiles/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/profiles/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.361763 oarepo-model-builder-4.0.9/oarepo_model_builder/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/settings/opensearch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/settings/python.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.361763 oarepo-model-builder-4.0.9/oarepo_model_builder/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.361763 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/absolute_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/camelcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.361763 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/indented_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/simple_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/facet_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/python_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/utils/verbose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.361763 oarepo-model-builder-4.0.9/oarepo_model_builder/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/validation/extensibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/validation/model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/oarepo_model_builder/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.345763 oarepo-model-builder-4.0.9/oarepo_model_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-30 18:25:02.000000 oarepo-model-builder-4.0.9/oarepo_model_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-30 18:25:02.000000 oarepo-model-builder-4.0.9/oarepo_model_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:25:02.000000 oarepo-model-builder-4.0.9/oarepo_model_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-30 18:25:02.000000 oarepo-model-builder-4.0.9/oarepo_model_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-30 18:25:02.000000 oarepo-model-builder-4.0.9/oarepo_model_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 18:25:02.000000 oarepo-model-builder-4.0.9/oarepo_model_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-30 18:25:02.369763 oarepo-model-builder-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:25:02.369763 oarepo-model-builder-4.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/faker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/multilang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_builder_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_cfg_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_datatype_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_datatype_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_empty_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   396304 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29556 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_fulltext_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_jsonchema_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_mapping_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_marshmallow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_marshmallow_ui_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23543 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_overwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_plugin_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_python_mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_sample_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_schema_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_simple_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_template_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_type_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-30 18:24:05.000000 oarepo-model-builder-4.0.9/tests/utils.py
```

### Comparing `oarepo_model_builder-4.0.84/LICENSE` & `oarepo-model-builder-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builder.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Type, Union
 
 from .builders import OutputBuilder
 from .fs import AbstractFileSystem, FileSystem
 from .outputs import OutputBase
 from .schema import ModelSchema
+from .utils.dict import dict_get, dict_setdefault
 from .utils.import_class import import_class
 
 
 class ModelBuilder:
     """
     Processes a model file and generates/updates sources for the model
     """
@@ -73,16 +74,14 @@
         and return it. If the builder on the path has already been requested, return
         the same instance of the builder.
 
         :param output_type: @see FileBuilder.output_type
         :param path: relative path to output_dir, set in build()
         :return:    instance of FileBuilder for the path
         """
-        if path is None:
-            raise AssertionError("Can not have a null path in a builder output")
         if not isinstance(path, Path):
             path = Path(path)
         path = self.output_dir.joinpath(path)
 
         output = self.outputs.get(path, None)
         if output:
             assert output_type == self.outputs[path].TYPE
@@ -112,35 +111,36 @@
         :return:            the outputs (self.outputs)
         """
 
         # deep copy the model
         if self.overwrite:
             self.filesystem.overwrite = True
 
+        current_model = dict_setdefault(model.schema, model_path, default={})
+
         self.set_schema(model)
         self.filtered_output_classes = {
             o.TYPE: o
-            for o in self._filter_classes(self.output_classes, model.schema, "output")
+            for o in self._filter_classes(self.output_classes, current_model, "output")
         }
         self.output_dir = Path(output_dir).absolute()
         self.outputs = {}
-        context = context or {}
-        context.setdefault("profile", profile)
+
         self._run_output_builders(model, profile, model_path, context or {})
 
         self._save_outputs()
 
         return self.outputs
 
     def _run_output_builders(
         self, model: ModelSchema, profile: str, model_path: Iterable[str], context
     ):
         output_builder_class: Type[OutputBuilder]
         for output_builder_class in self._filter_classes(
-            self.output_builder_classes, model.schema, "builder"
+            self.output_builder_classes, dict_get(model.schema, model_path), "builder"
         ):
             output_builder = output_builder_class(builder=self)
             current_model = model.get_schema_section(profile, model_path, context)
             output_builder.build(current_model=current_model, schema=model.schema)
 
     def _save_outputs(self):
         for output in sorted(self.outputs.values(), key=lambda x: x.path):
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builders/__init__.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builders/json_base.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builders/json_base.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builders/jsonschema.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builders/jsonschema.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builders/mapping.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builders/mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,35 +21,33 @@
             return True
     return False
 
 
 class MappingBuilder(JSONBaseBuilder):
     TYPE = "mapping"
     output_file_type = "mapping"
-    output_file_name = ["mapping", "file"]
-    skip = ["mapping", "skip"]
+    output_file_name = ["mapping-settings", "file"]
+    skip = ["mapping-settings", "skip"]
     parent_module_root_name = "mappings"
     create_parent_packages = True
 
     def build_node(self, node):
-        skip = dict_get(self.current_model.definition, ["mapping", "skip"], False)
+        skip = dict_get(
+            self.current_model.definition, ["mapping-settings", "skip"], False
+        )
         if skip:
             return
         generated = self.generate_model(node)
         generated.pop("enabled", None)
-        template = dict_get(self.current_model.definition, ["mapping", "template"], {})
-        if template:
-            self.output.merge(template)
         self.output.merge(generated)
 
     def generate_model(self, node):
         generated = self.generate(node)
         generated.pop("enabled", None)
         generated.pop("type", None)
-        node.section_global_mapping.config.pop("properties", None)
 
         return {**node.section_global_mapping.config, "mappings": generated}
 
     def generate(self, node, parent_enabled=True):
         mapping: Section = node.section_mapping
         facets: Section = node.section_facets
         ret = {**mapping.config}
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builders/model_saver.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builders/model_saver.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builders/python.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builders/python.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builders/python_structure.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builders/python_structure.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builders/setup_cfg.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builders/setup_cfg.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,45 +14,41 @@
         output.setdefault(
             "metadata",
             "name",
             self.current_model.definition["module"]["base"].replace("_", "-"),
         )
         version = self.schema.get("version", "1.0.0dev1")
         output.setdefault("metadata", "version", version)
-        try:
-            if parse_version(output.get("metadata", "version").value) < parse_version(
-                version
-            ):
-                output.set("metadata", "version", version)
-        except:
-            # may be, for example, attr:..., so ignore exception
-            pass
+        if parse_version(output.get("metadata", "version").value) < parse_version(
+            version
+        ):
+            output.set("metadata", "version", version)
         output.setdefault(
             "metadata",
             "description",
             f"Repository model for {self.current_model.definition['model-name']}",
         )
         output.setdefault("metadata", "authors", "")
 
         output.setdefault("options", "python", ">=3.9")
-
+        try:
+            ov = int(self.settings["oarepo-version"])
+            output.add_dependency("oarepo", f">={ov},<{ov+1}")
+        except ValueError:
+            output.add_dependency("oarepo", self.settings["oarepo-version"])
         output.add_dependency("oarepo-runtime", ">=1.0.0")
 
         output.setdefault("options", "packages", "find:")
 
         output.setdefault(
             "options.package_data", "*", "*.json, *.rst, *.md, *.json5, *.jinja2"
         )
 
         if "runtime-dependencies" in self.schema:
             for dep, value in self.schema["runtime-dependencies"].items():
-                if value[0] not in (">", "<", "="):
-                    value = ">=" + value
-                output.add_dependency(dep, value)
+                output.add_dependency(dep, ">=" + value)
 
         if "dev-dependencies" in self.schema:
             for dep, value in self.schema["dev-dependencies"].items():
-                if value[0] not in (">", "<", "="):
-                    value = ">=" + value
                 output.add_dependency(
-                    dep, value, group="options.extras_require", section="devs"
+                    dep, ">=" + value, group="options.extras_require", section="devs"
                 )
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builders/utils.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builders/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/builtin_models/invenio.json` & `oarepo-model-builder-4.0.9/oarepo_model_builder/builtin_models/invenio.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8291666666666666%*

 * *Differences: {"'marshmallow'": "{'base-classes': ['InvenioBaseRecordSchema'], delete: ['imports']}",*

 * * "'properties'": "{'id': {'facets': {delete: ['facet']}}, 'created': {'facets': {delete: "*

 * *                 "['facet']}}, 'updated': {'facets': {delete: ['facet']}}, '$schema': {'facets': "*

 * *                 "{delete: ['facet']}}}",*

 * * "'ui'": "{'marshmallow': {'base-classes': ['InvenioUISchema'], 'imports': "*

 * *         "[OrderedDict([('import', 'oarepo_runtime.ui.marshmallow.InvenioUISchema')])]}}"}*

```diff
@@ -1,18 +1,16 @@
 {
     "marshmallow": {
         "base-classes": [
-            "oarepo_runtime.services.schema.marshmallow.BaseRecordSchema"
-        ],
-        "imports": []
+            "InvenioBaseRecordSchema"
+        ]
     },
     "properties": {
         "$schema": {
             "facets": {
-                "facet": false,
                 "searchable": true
             },
             "marshmallow": {
                 "read": false,
                 "write": false
             },
             "sample": {
@@ -24,15 +22,14 @@
                     "read": false,
                     "write": false
                 }
             }
         },
         "created": {
             "facets": {
-                "facet": false,
                 "searchable": true
             },
             "marshmallow": {
                 "read": false,
                 "write": false
             },
             "sample": {
@@ -44,15 +41,14 @@
                     "read": false,
                     "write": false
                 }
             }
         },
         "id": {
             "facets": {
-                "facet": false,
                 "searchable": true
             },
             "marshmallow": {
                 "read": false,
                 "write": false
             },
             "sample": {
@@ -64,15 +60,14 @@
                     "read": false,
                     "write": false
                 }
             }
         },
         "updated": {
             "facets": {
-                "facet": false,
                 "searchable": true
             },
             "marshmallow": {
                 "read": false,
                 "write": false
             },
             "sample": {
@@ -86,13 +81,17 @@
                 }
             }
         }
     },
     "ui": {
         "marshmallow": {
             "base-classes": [
-                "oarepo_runtime.services.schema.ui.InvenioUISchema"
+                "InvenioUISchema"
             ],
-            "imports": []
+            "imports": [
+                {
+                    "import": "oarepo_runtime.ui.marshmallow.InvenioUISchema"
+                }
+            ]
         }
     }
 }
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/cli.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     type=bool,
     default=False,
     help="Do not merge with content in already existing files, overwrite them",
 )
 @click.option(
     "--profile",
     help="Run the builder with this profile",
-    default=[],
+    default=["record"],
     multiple=True,
 )
 @click.argument("model_filename", type=click.Path(exists=True), required=True)
 @click.argument(
     "included_models", nargs=-1, type=click.Path(exists=True), required=False
 )
 def run(
@@ -201,16 +201,14 @@
         sets,
         merged_models=included_models,
         extra_included=includes,
     )
     if save_model:
         with open(save_model, "w") as f:
             yaml.dump(json.loads(json.dumps(model.schema)), f)
-    if not profiles:
-        profiles = model.schema.get("profiles", ["record"])
 
     # for each profile on the command line, render it
     profiles_to_render = [y.strip() for x in profiles for y in x.split(",")]
     for profile in profiles_to_render:
         # load the builder
         builder = create_builder_from_entrypoints(profile=profile, overwrite=overwrite)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/__init__.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,38 +6,37 @@
 
 boolean:
   no constraints supported
 
 date, time, datetime
   no constraints supported
 
-edtf, edtf-time, edtf-time-interval, edtf-interval
+edtf, edtf-interval
   no constraints supported
 
 fulltext, keyword, fulltext+keyword:
   minLength, maxLength, pattern
 
 flatten:
   object represented as flatten type in elasticsearch
 """
 
+
 from .containers import (  # noqa
     ArrayDataType,
-    FlatObjectDataType,
+    FlattenDataType,
     NestedDataType,
     ObjectDataType,
 )
-from .datatypes import DataType, DataTypeComponent, Section, datatypes  # noqa
+from .datatypes import DataType, DataTypeComponent, Import, Section, datatypes  # noqa
 from .dates import (  # noqa
     DateDataType,
     DateTimeDataType,
     EDTFDataType,
     EDTFIntervalType,
-    EDTFTimeDataType,
-    EDTFTimeIntervalType,
     TimeDataType,
 )
 from .model import ModelDataType  # noqa
 from .primitive_types import NumberDataType  # noqa , just for export
 from .primitive_types import (
     BooleanDataType,
     DoubleDataType,
@@ -47,34 +46,30 @@
 from .strings import StringDataType  # noqa , just for export
 from .strings import (  # noqa
     FulltextDataType,
     FulltextKeywordDataType,
     KeywordDataType,
     URLDataType,
     UUIDDataType,
-    HtmlDataType
 )
 
 DEFAULT_DATATYPES = [
     IntegerDataType,
     FloatDataType,
     DoubleDataType,
     BooleanDataType,
     DateDataType,
     TimeDataType,
     DateTimeDataType,
     EDTFDataType,
     EDTFIntervalType,
-    EDTFTimeIntervalType,
-    EDTFTimeDataType,
     FulltextDataType,
     KeywordDataType,
     FulltextKeywordDataType,
     UUIDDataType,
     ObjectDataType,
     NestedDataType,
-    FlatObjectDataType,
+    FlattenDataType,
     ArrayDataType,
     URLDataType,
     ModelDataType,
-    HtmlDataType
 ]
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/__init__.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 from .enum import EnumComponent
 from .facets.array import ArrayFacetsComponent
 from .facets.field import RegularFacetsComponent
 from .facets.nested import NestedFacetsComponent
 from .facets.object import ObjectFacetsComponent
 from .marshmallow import (
     ArrayMarshmallowComponent,
-    NumberMarshmallowComponent,
     ObjectMarshmallowComponent,
     RegularMarshmallowComponent,
-    StringMarshmallowComponent,
     UIArrayMarshmallowComponent,
     UIMarshmallowComponent,
     UIObjectMarshmallowComponent,
 )
 from .model import (
     AppModelComponent,
     BlueprintsModelComponent,
     DefaultsModelComponent,
-    EDTFIntervalDumperModelComponent,
-    ExtResourceModelComponent,
     FacetsModelComponent,
     JSONSchemaModelComponent,
     MappingModelComponent,
     MarshmallowModelComponent,
     PermissionsModelComponent,
     PIDModelComponent,
+    PluginsModelComponent,
     ProxyModelComponent,
     RecordDumperModelComponent,
-    RecordItemModelComponent,
-    RecordListModelComponent,
     RecordMetadataModelComponent,
     RecordModelComponent,
     ResourceModelComponent,
     SampleModelComponent,
     SavedModelComponent,
     SearchOptionsModelComponent,
     ServiceModelComponent,
     UIMarshmallowModelComponent,
     UIModelComponent,
 )
 from .sample import ArraySampleComponent, RegularSampleComponent
-from .sort import FieldSortComponent, RegularSortComponent
 from .ui import ObjectUIComponent, RegularUIComponent
 
 DEFAULT_COMPONENTS = [
     SearchOptionsModelComponent,
     ArraySampleComponent,
     RegularSampleComponent,
     RegularMarshmallowComponent,
@@ -71,20 +65,13 @@
     SampleModelComponent,
     SavedModelComponent,
     ServiceModelComponent,
     UIMarshmallowModelComponent,
     UIModelComponent,
     DefaultsModelComponent,
     ProxyModelComponent,
+    PluginsModelComponent,
     ObjectFacetsComponent,
     NestedFacetsComponent,
     RegularFacetsComponent,
     ArrayFacetsComponent,
-    ExtResourceModelComponent,
-    RegularSortComponent,
-    FieldSortComponent,
-    StringMarshmallowComponent,
-    NumberMarshmallowComponent,
-    EDTFIntervalDumperModelComponent,
-    RecordListModelComponent,
-    RecordItemModelComponent,
 ]
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/enum.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/enum.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,16 @@
             ma.fields.Raw, metadata={"doc": "A list of possible values"}
         )
 
     def process_marshmallow(self, datatype, section, **kwargs):
         enum = datatype.definition.get("enum")
         if enum:
             section.config.setdefault("validators", []).append(
-                f"{{{{marshmallow.validate.OneOf}}}}({repr(enum)})"
+                f"ma_validate.OneOf({repr(enum)})"
             )
 
     def process_ui(self, datatype, section, **kwargs):
         enum = datatype.definition.get("enum")
         if enum:
             section.config.setdefault("marshmallow", {}).setdefault(
                 "validators", []
-            ).append(f"{{{{marshmallow.validate.OneOf}}}}({repr(enum)})")
+            ).append(f"ma_validate.OneOf({repr(enum)})")
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/array.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/array.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/field.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/field.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,50 +5,28 @@
 from oarepo_model_builder.utils.facet_helpers import facet_name, flatten
 from oarepo_model_builder.validation.utils import ImportSchema
 
 from ...datatypes import DataTypeComponent
 from . import FacetDefinition
 
 
-class FacetGroupsDict(fields.Dict):
-    def _deserialize(self, value, attr, data, **kwargs):
-        transformed_value = {}
-        if isinstance(value, list):
-            for val in value:
-                if isinstance(val, str):
-                    transformed_value[val] = 100000
-                else:
-                    transformed_value.update(val)
-        else:
-            transformed_value = value
-        return super()._deserialize(transformed_value, attr, data, **kwargs)
-
-
 class FacetsSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
     searchable = ma.fields.Bool(required=False)
     key = fields.String(required=False)
     field = fields.String(required=False)
     facet_class = fields.String(
         required=False, data_key="facet-class", attribute="facet-class"
     )
     args = fields.List(fields.String(), required=False)
     imports = fields.List(fields.Nested(ImportSchema), required=False)
     path = fields.String(required=False)
     keyword = fields.String(required=False)
-    facet_groups = FacetGroupsDict(
-        keys=fields.String(),
-        values=fields.Integer(),
-        required=False,
-        data_key="facet-groups",
-        attribute="facet-groups",
-    )
-    facet = ma.fields.Bool(required=False)
 
 
 class RegularFacetsComponent(DataTypeComponent):
     eligible_datatypes = []
 
     class ModelSchema(ma.Schema):
         facets = ma.fields.Nested(
@@ -70,16 +48,14 @@
 
         path = self.facet_path(datatype, facet_section)
         facet_definition = FacetDefinition(
             path=facet_section.get("key", facet_name(datatype.path)),
             dot_path=datatype.path,
             searchable=facet_section.get("searchable"),
             imports=facet_section.get("imports", []),
-            facet=facet_section.get("facet", None),
-            facet_groups=facet_section.get("facet-groups", {"_default": 100000}),
         )
 
         # set the field on the definition
         label = facet_section.get("label", f'{datatype.path.replace(".", "/")}.label')
         facet_definition.set_field(
             facet_section,
             arguments=[
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/nested.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/nested.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/facets/object.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/facets/object.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/__init__.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from .array import ArrayMarshmallowComponent
 from .field import (
     MarshmallowField,
     PropertyMarshmallowSchema,
     RegularMarshmallowComponent,
 )
-from .numbers import NumberMarshmallowComponent
 from .object import (
     ExtraField,
     ObjectMarshmallowComponent,
     ObjectMarshmallowExtraSchema,
     ObjectMarshmallowMixin,
     ObjectMarshmallowSchema,
 )
-from .strings import StringMarshmallowComponent
 from .ui_array import UIArrayMarshmallowComponent
 from .ui_field import UIMarshmallowComponent
 from .ui_object import UIObjectMarshmallowComponent
 
 __all__ = [
     "RegularMarshmallowComponent",
     "MarshmallowField",
@@ -26,10 +24,8 @@
     "ObjectMarshmallowExtraSchema",
     "ObjectMarshmallowMixin",
     "ObjectMarshmallowSchema",
     "ArrayMarshmallowComponent",
     "UIMarshmallowComponent",
     "UIObjectMarshmallowComponent",
     "UIArrayMarshmallowComponent",
-    "StringMarshmallowComponent",
-    "NumberMarshmallowComponent",
 ]
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/graph.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses
 from typing import List, Optional, Set
 
 from oarepo_model_builder.validation import InvalidModelException
 
-from ....utils.python_name import Import, base_name, package_name
+from ....utils.python_name import base_name, package_name
+from ...datatypes import Import
 
 
 @dataclasses.dataclass
 class MarshmallowField:
     key: str
     definition: str
     imports: List[Import] = dataclasses.field(default_factory=list)
@@ -42,15 +43,15 @@
 
 @dataclasses.dataclass
 class MarshmallowClass:
     class_name: str
     base_classes: List[str]
     imports: List[Import]
     fields: List[MarshmallowField]
-    unknown: str
+    strict: bool
     order: Optional[int] = None
 
     references: List[MarshmallowReference] = dataclasses.field(default_factory=list)
 
     def collect_references(self, classes):
         references = []
         for fld in self.fields:
@@ -91,15 +92,15 @@
         to_process = for_another_round
     classes_list.sort(key=lambda x: [-x.order, x.class_name])
 
 
 def collect_imports(current_module, classes_list: List[MarshmallowClass]):
     for cls in classes_list:
         for fld in cls.fields:
-            if not fld.reference or not fld.reference.reference:
+            if not fld.reference:
                 continue
             if fld.reference.accessor:
                 # local accessor handles its own imports inside the accessor
                 continue
             # if from different package,
             if package_name(fld.reference.reference) != current_module:
                 fld.imports.append(Import(import_path=fld.reference.reference))
@@ -132,29 +133,27 @@
         pd = PackageWithDependencies(p)
         package_dependencies.append(pd)
         for pc in classes_by_package[p]:
             for fld in pc.fields:
                 if not fld.reference:
                     continue
                 referenced_package = package_name(fld.reference.reference)
-                if referenced_package != p and referenced_package in classes_by_package:
+                if referenced_package in classes_by_package:
                     pd.add_dependency(referenced_package)
     to_process = list(package_dependencies)
     processed_dependencies = set()
     while to_process:
         for_another_round = []
         for c in to_process:
             if c.dependencies:
                 for_another_round.append(c)
             else:
                 processed_dependencies.add(c.package)
         if len(for_another_round) == len(to_process):
-            raise InvalidModelException(
-                f"Cycle found in packages, code missing: {to_process}"
-            )
+            raise InvalidModelException("Cycle found in packages, code missing")
         else:
             for c in for_another_round:
                 c.remove_dependencies(processed_dependencies)
         to_process = for_another_round
 
     for p in package_dependencies:
         for cls in classes_by_package[p.package]:
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/object.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import List
 
 import marshmallow as ma
-import marshmallow.validate
 from marshmallow import fields
 
 from oarepo_model_builder.datatypes import DataType, ObjectDataType, datatypes
 from oarepo_model_builder.utils.absolute_class import convert_to_absolute_class_name
 from oarepo_model_builder.utils.python_name import (
     base_name,
     convert_name_to_python_class,
@@ -60,18 +59,14 @@
         fields.Nested(ExtraField),
         required=False,
         data_key="extra-fields",
         attribute="extra-fields",
         metadata={"doc": "Extra fields to generate into the marshmallow class"},
     )
     skip = fields.Boolean()
-    unknown = fields.Str(
-        validate=[marshmallow.validate.OneOf(["RAISE", "INCLUDE", "EXCLUDE"])],
-        default="RAISE",
-    )
 
 
 class ObjectMarshmallowSchema(PropertyMarshmallowSchema, ObjectMarshmallowExtraSchema):
     pass
 
 
 class ObjectMarshmallowMixin:
@@ -105,16 +100,14 @@
                 marshmallow_config["class"] = qualified_schema_class
                 definition_marshmallow["class"] = qualified_schema_class
                 schema_class = qualified_schema_class
             if not generate:
                 if fingerprint not in classes:
                     classes[fingerprint] = schema_class
                 return
-        if marshmallow_config.get("field") and not schema_class and not generate:
-            return
 
         fingerprint_schema_class = classes.get(fingerprint)
         if fingerprint_schema_class:
             # reuse, do not generate again, even if schema_class was specified
             schema_class = fingerprint_schema_class
             marshmallow_config["generate"] = False
             definition_marshmallow["generate"] = False
@@ -179,41 +172,32 @@
 
         raise InvalidModelException(
             f"Too many marshmallow classes with name {class_name}{suffix}, defined on path {datatype.path}. "
             "Please specify your own class name for marshmallow at this path"
         )
 
     def _build_class(
-        self,
-        datatype,
-        marshmallow,
-        children,
-        field_generator,
-        classes,
-        default_base_class,  # NOSONAR
+        self, datatype, marshmallow, children, field_generator, classes  # NOSONAR
     ):
         fields = []
         for _, c in sorted(children.items()):
             datatypes.call_components(c, field_generator, fields=fields)
         extra_fields = [
             MarshmallowField(f["name"], f["value"])
             for f in marshmallow.get("extra-fields", [])
         ]
         fields = [*fields, *extra_fields]
         fields.sort(key=lambda x: (not x.key.startswith("_"), x.key))
-        base_classes = marshmallow.get("base-classes", [])
-        if not base_classes:
-            base_classes = [default_base_class]
         classes.append(
             MarshmallowClass(
                 class_name=marshmallow["class"],
-                base_classes=base_classes,
+                base_classes=marshmallow.get("base-classes", []) or ["ma.Schema"],
                 imports=Import.from_config(marshmallow.get("imports", [])),
                 fields=fields,
-                unknown=marshmallow.get("unknown", "RAISE"),
+                strict=True,
             )
         )
 
 
 class ObjectMarshmallowComponent(ObjectMarshmallowMixin, RegularMarshmallowComponent):
     eligible_datatypes = [ObjectDataType]
 
@@ -258,29 +242,24 @@
     def marshmallow_build_class(self, *, datatype, classes, **kwargs):
         self._build_class(
             datatype,
             datatype.section_marshmallow.config,
             datatype.section_marshmallow.children,
             "marshmallow_field",
             classes,
-            default_base_class=datatype.schema.settings["marshmallow"][
-                "schema-base-class"
-            ],
         )
 
     def marshmallow_field(
         self, datatype: DataType, *, fields: List[MarshmallowField], **kwargs
     ):
         section = datatype.section_marshmallow
         f = []
         super().marshmallow_field(datatype, fields=f)
-        if not f:
-            return
         fld: MarshmallowField = f[0]
-        fld.reference = MarshmallowReference(reference=section.config.get("class"))
+        fld.reference = MarshmallowReference(reference=section.config["class"])
         fields.append(fld)
 
     def _marshmallow_field_arguments(self, datatype, section, marshmallow, field_name):
         return [
             "__reference__",
             *super()._marshmallow_field_arguments(
                 datatype, section, marshmallow, field_name
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,30 +50,25 @@
     def ui_marshmallow_build_class(self, *, datatype, classes, **__kwargs):
         self._build_class(
             datatype,
             datatype.section_ui.config.setdefault("marshmallow", {}),
             datatype.section_ui.children,
             "ui_marshmallow_field",
             classes,
-            default_base_class=datatype.schema.settings["marshmallow"][
-                "ui-schema-base-class"
-            ],
         )
 
     def ui_marshmallow_field(
         self, datatype: DataType, *, fields: List[MarshmallowField], **__kwargs
     ):
         section = datatype.section_ui
         f = []
         super().ui_marshmallow_field(datatype, fields=f)
-        if not f:
-            return
         fld: MarshmallowField = f[0]
         fld.reference = MarshmallowReference(
-            reference=section.config["marshmallow"].get("class")
+            reference=section.config["marshmallow"]["class"]
         )
         fields.append(fld)
 
     def _marshmallow_field_arguments(self, datatype, section, marshmallow, field_name):
         return [
             "__reference__",
             *super()._marshmallow_field_arguments(
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/__init__.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from .app import AppModelComponent
 from .blueprints import BlueprintsModelComponent
 from .defaults import DefaultsModelComponent
-from .edtf_interval import EDTFIntervalDumperModelComponent
-from .ext_resource import ExtResourceModelComponent
 from .facets import FacetsModelComponent
 from .jsonschema import JSONSchemaModelComponent
 from .mapping import MappingModelComponent
 from .marshmallow import MarshmallowModelComponent
 from .model_saver import SavedModelComponent
 from .permissions import PermissionsModelComponent
 from .pid import PIDModelComponent
+from .plugins import PluginsModelComponent
 from .proxy import ProxyModelComponent
 from .record import RecordModelComponent
 from .record_dumper import RecordDumperModelComponent
-from .record_item import RecordItemModelComponent
-from .record_list import RecordListModelComponent
 from .record_metadata import RecordMetadataModelComponent
 from .resource import ResourceModelComponent
 from .sample import SampleModelComponent
 from .search_options import SearchOptionsModelComponent
 from .service import ServiceModelComponent
-from .sort import SortModelComponent
 from .ui import UIModelComponent
 from .ui_marshmallow import UIMarshmallowModelComponent
 
 __all__ = [
     "AppModelComponent",
     "BlueprintsModelComponent",
     "FacetsModelComponent",
@@ -41,13 +37,9 @@
     "SampleModelComponent",
     "SavedModelComponent",
     "ServiceModelComponent",
     "UIMarshmallowModelComponent",
     "UIModelComponent",
     "DefaultsModelComponent",
     "ProxyModelComponent",
-    "ExtResourceModelComponent",
-    "SortModelComponent",
-    "EDTFIntervalDumperModelComponent",
-    "RecordListModelComponent",
-    "RecordItemModelComponent",
+    "PluginsModelComponent",
 ]
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/app.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,27 +62,28 @@
             ConfigSchema, metadata={"doc": "Application config details"}
         )
         ext = ma.fields.Nested(
             ExtSchema, metadata={"doc": "Application extension details"}
         )
 
     def before_model_prepare(self, datatype, **kwargs):
+        prefix = datatype.definition["module"]["prefix"]
+        alias = datatype.definition["module"]["alias"]
         module = datatype.definition["module"]["qualified"]
-        base_title = datatype.definition["module"]["base-title"]
 
         config = set_default(datatype, "config", {})
 
         config.setdefault("generate", True)
         config.setdefault("module", f"{module}.config")
         config.setdefault("extra_code", "")
         config.setdefault("imports", [])
 
         ext = set_default(datatype, "ext", {})
 
         ext.setdefault("generate", True)
         ext_module = ext.setdefault("module", f"{module}.ext")
-        ext.setdefault("class", f"{ext_module}.{base_title}Ext")
+        ext.setdefault("class", f"{ext_module}.{prefix}Ext")
         ext.setdefault("base-classes", [])
         ext.setdefault("extra_code", "")
-        ext.setdefault("alias", module)
+        ext.setdefault("alias", alias)
         ext.setdefault("imports", [])
         convert_config_to_qualified_name(ext)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/blueprints.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/blueprints.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/defaults.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,15 @@
         metadata={"doc": "Base name of the module (if the module has dot)"}
     )
     base_upper = ma.fields.String(
         attribute="base-upper",
         data_key="base-upper",
         metadata={"doc": "Uppercase of the base name"},
     )
-    base_title = ma.fields.String(
-        attribute="base-title",
-        data_key="base-title",
-        metadata={"doc": "Capitalized base name"},
-    )
+
     kebab_module = ma.fields.String(
         attribute="kebab-module",
         data_key="kebab-module",
         metadata={"doc": "Kebab case of the module"},
     )
 
     prefix = ma.fields.String(
@@ -96,18 +92,14 @@
             split_base_name(module),
         )
         module_container.setdefault(
             "base-upper",
             module_base.upper(),
         )
         module_container.setdefault(
-            "base-title",
-            module_base.capitalize(),
-        )
-        module_container.setdefault(
             "kebab-module",
             module.replace(".", "-").replace("_", "-"),
         )
 
         prefix = module_container.setdefault(
             "prefix",
             camel_case(module_base),
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/edtf_interval.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/record_dumper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import marshmallow as ma
 
 from oarepo_model_builder.datatypes import DataTypeComponent, ModelDataType
 from oarepo_model_builder.utils.python_name import parent_module
 from oarepo_model_builder.validation.utils import ImportSchema
 
 from .defaults import DefaultsModelComponent
-from .record_dumper import RecordDumperModelComponent
+from .record import RecordModelComponent
 from .utils import set_default
 
 
-class EDTFIntervalDumperClassSchema(ma.Schema):
+class RecordDumperClassSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
     generate = ma.fields.Bool(metadata={"doc": "Generate the dumper class"})
     class_ = ma.fields.Str(
         attribute="class",
         data_key="class",
@@ -21,55 +21,49 @@
     )
     base_classes = ma.fields.List(
         ma.fields.Str(),
         attribute="base-classes",
         data_key="base-classes",
         metadata={"doc": "List of base classes"},
     )
+    extensions = ma.fields.List(
+        ma.fields.Str(), metadata={"doc": "List of dumper extensions"}
+    )
     extra_code = ma.fields.Str(
         attribute="extra-code",
         data_key="extra-code",
         metadata={"doc": "Extra code to be copied to the bottom of the dumper file"},
     )
     module = ma.fields.String(metadata={"doc": "Class module"})
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
     skip = ma.fields.Boolean()
 
 
-class EDTFIntervalDumperModelComponent(DataTypeComponent):
+class RecordDumperModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
-    depends_on = [
-        DefaultsModelComponent,
-        RecordDumperModelComponent,
-    ]
+    depends_on = [DefaultsModelComponent, RecordModelComponent]
 
     class ModelSchema(ma.Schema):
-        edtf_interval_dumper = ma.fields.Nested(
-            EDTFIntervalDumperClassSchema,
-            attribute="edtf-interval-dumper",
-            data_key="edtf-interval-dumper",
-            metadata={"doc": "Settings for edtf interval dumper"},
+        record_dumper = ma.fields.Nested(
+            RecordDumperClassSchema,
+            attribute="record-dumper",
+            data_key="record-dumper",
+            metadata={"doc": "Settings for record dumper"},
         )
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
         record_module = parent_module(datatype.definition["record"]["module"])
         prefix = datatype.definition["module"]["prefix"]
 
-        dumper = set_default(datatype, "edtf-interval-dumper", {})
+        dumper = set_default(datatype, "record-dumper", {})
         dumper.setdefault("generate", True)
 
-        dumper_module = dumper.setdefault("module", f"{record_module}.dumpers.edtf")
-        ext_class = f"{dumper_module}.{prefix}EDTFIntervalDumperExt"
-        dumper.setdefault("class", ext_class)
-        dumper.setdefault(
-            "base-classes",
-            ["oarepo_runtime.records.dumpers.edtf_interval.EDTFIntervalDumperExt"],
-        )
+        dumper_module = dumper.setdefault("module", f"{record_module}.dumper")
+        dumper.setdefault("class", f"{dumper_module}.{prefix}Dumper")
+        dumper.setdefault("base-classes", ["SearchDumper"])
         dumper.setdefault("extra-code", "")
         dumper.setdefault("extensions", [])
-        dumper.setdefault("imports", [])
-
-        datatype.definition["record-dumper"]["extensions"].append(
-            "{{" + ext_class + "}}()"
+        dumper.setdefault(
+            "imports", [{"import": "invenio_records.dumpers.SearchDumper"}]
         )
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/facets.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/facets.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,24 +20,14 @@
         metadata={"doc": "Extra code to be pasted to search options module"},
     )
     module = ma.fields.String(
         metadata={"doc": "Module where the facets will be placed"}
     )
     generate = ma.fields.Boolean()
     skip = ma.fields.Boolean()
-    facet_groups = ma.fields.Dict(
-        attribute="facet-groups",
-        data_key="facet-groups",
-        keys=ma.fields.String(),
-        values=ma.fields.Dict(keys=ma.fields.String(), values=ma.fields.Integer()),
-        metadata={
-            "doc": "Groups of facets in the form of {group_name: {facet_path: priority}}. Will merge with facet "
-            "groups declared on the individual fields."
-        },
-    )
 
 
 class FacetsModelComponent(ObjectFacetsComponent):
     eligible_datatypes = [ModelDataType]
     depends_on = [DefaultsModelComponent]
 
     class ModelSchema(ma.Schema):
@@ -51,24 +41,20 @@
         profile_module = context["profile_module"]
 
         facets = set_default(datatype, "facets", {})
         facets.setdefault("generate", True)
         facets.setdefault("module", f"{module}.services.{profile_module}.facets")
 
         facets.setdefault("extra-code", "")
-        facets.setdefault("groups", True)
 
     def build_facet_definition(
         self,
         datatype,
         facet_definition: FacetDefinition,
     ):
         if facet_definition.searchable is None:
             facet_definition.searchable = datatype.definition.get("searchable", True)
-        if (
-            facet_definition.searchable is not False
-            and facet_definition.facet is not False
-        ):
+        if facet_definition.searchable is not False:
             return [facet_definition]
         else:
             # facet will not be generated
             return []
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/jsonschema.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/jsonschema.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             data_key="json-schema-settings",
             attribute="json-schema-settings",
             metadata={
                 "doc": "JSON Schema section of the model. Properties will be generated automatically"
             },
         )
 
-    def before_model_prepare(self, datatype, *, context, **kwargs):
+    def before_model_prepare(self, datatype, **kwargs):
         prefix_snake = datatype.definition["module"]["prefix-snake"]
         alias = datatype.definition["module"]["alias"]
         records_path = module_to_path(
             parent_module(datatype.definition["record"]["module"])
         )
 
         json_schema = set_default(datatype, "json-schema-settings", {})
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/mapping.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/mapping.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,20 +27,14 @@
 
     # mapping
     template = ma.fields.Nested(
         PermissiveSchema,
         metadata={"doc": "Mapping template, merged with generated mapping"},
     )
     skip = ma.fields.Boolean()
-    index_field_arguments = ma.fields.List(
-        ma.fields.String(),
-        data_key="index-field-arguments",
-        attribute="index-field-arguments",
-        metadata={"doc": "Other arguments for index field"},
-    )
 
     class Meta:
         unknown = ma.RAISE
 
 
 class MappingModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
@@ -49,33 +43,33 @@
         RecordModelComponent,
         JSONSchemaModelComponent,
     ]
 
     class ModelSchema(ma.Schema):
         mapping = ma.fields.Nested(
             ModelMappingSchema,
-            attribute="mapping",
-            data_key="mapping",
+            attribute="mapping-settings",
+            data_key="mapping-settings",
             metadata={"doc": "Mapping definition"},
         )
         searchable = ma.fields.Bool(
             load_default=True,
             metadata={
                 "doc": "Will the mapping/indexing be generated on model? (can be overriden on individual properties)"
             },
         )
 
-    def before_model_prepare(self, datatype, *, context, **kwargs):
+    def before_model_prepare(self, datatype, **kwargs):
         prefix_snake = datatype.definition["module"]["prefix-snake"]
         alias = datatype.definition["module"]["alias"]
         records_path = module_to_path(
             parent_module(datatype.definition["record"]["module"])
         )
 
-        mapping = set_default(datatype, "mapping", {})
+        mapping = set_default(datatype, "mapping-settings", {})
         mapping.setdefault("generate", True)
         alias = mapping.setdefault("alias", alias)
         mapping.setdefault(
             "module",
             f'{parent_module(datatype.definition["record"]["module"])}.mappings',
         )
         short_index_name = (
@@ -91,8 +85,7 @@
                 records_path,
                 "mappings",
                 "os-v2",
                 alias,
                 f"{short_index_name}.json",
             ),
         )
-        mapping.setdefault("index-field-args", [])
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/marshmallow.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/marshmallow.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,33 +70,33 @@
     class ModelSchema(ma.Schema):
         marshmallow = ma.fields.Nested(ModelMarshmallowSchema)
 
     def marshmallow_register_class_names(self, *, datatype, classes, **kwargs):
         marshmallow_def = dict_get(datatype.definition, self.model_marshmallow_section)
         classes[marshmallow_def["class"]].append((True, datatype))
 
-    def before_model_prepare(self, datatype, *, context, **kwargs):
+    def before_model_prepare(self, datatype, **kwargs):
         prefix = datatype.definition["module"]["prefix"]
         services_module = parent_module(datatype.definition["service"]["module"])
 
         marshmallow: Dict = set_default(datatype, "marshmallow", {})
         marshmallow.setdefault("generate", True)
         module = marshmallow.setdefault("module", f"{services_module}.schema")
         marshmallow.setdefault("class", f"{module}.{prefix}Schema")
         marshmallow.setdefault("extra-code", "")
-        marshmallow.setdefault("base-classes", ["marshmallow.Schema"])
+        marshmallow.setdefault("base-classes", ["ma.Schema"])
         convert_config_to_qualified_name(marshmallow)
 
         if "properties" in datatype.definition and "metadata" in (
             datatype.definition["properties"] or {}
         ):
             metadata_marshmallow = set_default(
                 datatype, "properties", "metadata", "marshmallow", {}
             )
             metadata_module = metadata_marshmallow.setdefault("module", module)
             metadata_marshmallow.setdefault("generate", True)
             metadata_marshmallow.setdefault(
                 "class", f"{metadata_module}.{prefix}MetadataSchema"
             )
             metadata_marshmallow.setdefault("extra-code", "")
-            metadata_marshmallow.setdefault("base-classes", ["marshmallow.Schema"])
+            metadata_marshmallow.setdefault("base-classes", ["ma.Schema"])
             convert_config_to_qualified_name(metadata_marshmallow)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/model_saver.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/model_saver.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,25 +28,22 @@
     depends_on = [DefaultsModelComponent]
 
     class ModelSchema(ma.Schema):
         saved_model = ma.fields.Nested(
             SavedModelSchema, attribute="saved-model", data_key="saved-model"
         )
 
-    def before_model_prepare(self, datatype, context=None, **kwargs):
-        profile = context.get("profile_module")
-        file = f"{profile}.json"
-
+    def before_model_prepare(self, datatype, **kwargs):
         module_path = datatype.definition["module"]["path"]
         module = datatype.definition["module"]["qualified"]
 
         saved_model = set_default(datatype, "saved-model", {})
 
         saved_model.setdefault(
             "file",
-            os.path.join(module_path, "models", file),
+            os.path.join(module_path, "models", "model.json"),
         )
         saved_model.setdefault(
             "module",
             f"{module}.models",
         )
         saved_model.setdefault("alias", datatype.definition["module"]["alias"])
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/permissions.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,13 +72,13 @@
         )
         permissions.setdefault(
             "class",
             f"{permissions_module}.{prefix}PermissionPolicy",
         )
         permissions.setdefault(
             "base-classes",
-            ["invenio_records_permissions.RecordPermissionPolicy"],
+            ["RecordPermissionPolicy"],
         )
         permissions.setdefault(
             "imports",
-            [],
+            [{"import": "invenio_records_permissions.RecordPermissionPolicy"}],
         )
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/pid.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/pid.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,19 +52,14 @@
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "A list of python imports"}
     )
     module = ma.fields.String(
         metadata={"doc": "Module where the pid provider will be placed"}
     )
     skip = ma.fields.Boolean()
-    extra_code = ma.fields.String(
-        attribute="extra-code",
-        data_key="extra-code",
-        metadata={"doc": "Extra code to be copied below the permission class"},
-    )
 
 
 class PIDModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
     depends_on = [DefaultsModelComponent, RecordModelComponent]
 
     class ModelSchema(ma.Schema):
@@ -82,32 +77,31 @@
             "module",
             f"{record_module}.api",
         )
         pid.setdefault(
             "provider-class",
             f"{pid_module}.{prefix}IdProvider",
         )
-        pid.setdefault(
-            "provider-base-classes",
-            ["invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"],
-        )
+        pid.setdefault("provider-base-classes", ["RecordIdProviderV2"])
 
-        pid.setdefault(
-            "field-class", "invenio_records_resources.records.systemfields.pid.PIDField"
-        )
-        pid.setdefault(
-            "context-class",
-            "invenio_records_resources.records.systemfields.pid.PIDFieldContext",
-        )
+        pid.setdefault("field-class", "PIDField")
+        pid.setdefault("context-class", "PIDFieldContext")
         pid.setdefault("field-args", ["create=True"])
         pid.setdefault(
             "imports",
-            [],
+            [
+                {
+                    "import": "invenio_records_resources.records.systemfields.pid.PIDField"
+                },
+                {
+                    "import": "invenio_records_resources.records.systemfields.pid.PIDFieldContext"
+                },
+                {"import": "invenio_pidstore.providers.recordid_v2.RecordIdProviderV2"},
+            ],
         )
-        pid.setdefault("extra-code", "")
 
 
 def process_pid_type(pid_base):
     pid_base = re.sub(r"[\s_-]", "", pid_base).lower()
     if len(pid_base) > 6:
         pid_base = re.sub(r"[AEIOU]", "", pid_base, flags=re.IGNORECASE)
     if len(pid_base) > 6:
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/proxy.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/proxy.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/record.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/record.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,19 +32,14 @@
         metadata={"doc": "Extra code to copy to record file"},
     )
     module = ma.fields.String(metadata={"doc": "Class module"})
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
     skip = ma.fields.Boolean()
-    fields = ma.fields.Dict(
-        attribute="fields",
-        data_key="fields",
-        metadata={"doc": "Extra fields to add to the class"},
-    )
 
 
 class RecordModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
     depends_on = [DefaultsModelComponent]
 
     class ModelSchema(ma.Schema):
@@ -57,18 +52,19 @@
         profile_module = context["profile_module"]
         record_prefix = datatype.definition["module"]["prefix"]
 
         record = set_default(datatype, "record", {})
         record.setdefault("generate", True)
         records_module = record.setdefault("module", f"{module}.{profile_module}.api")
         record.setdefault("class", f"{records_module}.{record_prefix}Record")
-        record.setdefault(
-            "base-classes",
-            ["invenio_records_resources.records.api.Record{InvenioRecord}"],
-        )
+        record.setdefault("base-classes", ["InvenioRecord"])
         record.setdefault(
             "imports",
-            [],
+            [
+                {
+                    "import": "invenio_records_resources.records.api.Record",
+                    "alias": "InvenioRecord",
+                }
+            ],
         )
         record.setdefault("extra-code", "")
-        record.setdefault("fields", {})
         convert_config_to_qualified_name(record)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/record_dumper.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/record_metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,65 +5,79 @@
 from oarepo_model_builder.validation.utils import ImportSchema
 
 from .defaults import DefaultsModelComponent
 from .record import RecordModelComponent
 from .utils import set_default
 
 
-class RecordDumperClassSchema(ma.Schema):
+class RecordMetadataClassSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
-    generate = ma.fields.Bool(metadata={"doc": "Generate the dumper class"})
+    alias = ma.fields.Str(
+        metadata={"doc": "Alias under which the metadata is registered in setup.cfg"}
+    )
+    generate = ma.fields.Bool(metadata={"doc": "True to generate the metadata class"})
+    module = ma.fields.String(
+        metadata={"doc": "Module where the metadata class resides"}
+    )
     class_ = ma.fields.Str(
         attribute="class",
         data_key="class",
         metadata={"doc": "Qualified name of the class"},
     )
     base_classes = ma.fields.List(
         ma.fields.Str(),
         attribute="base-classes",
         data_key="base-classes",
-        metadata={"doc": "List of base classes"},
-    )
-    extensions = ma.fields.List(
-        ma.fields.Str(), metadata={"doc": "List of dumper extensions"}
+        metadata={"doc": "A list of base classes"},
     )
     extra_code = ma.fields.Str(
         attribute="extra-code",
         data_key="extra-code",
-        metadata={"doc": "Extra code to be copied to the bottom of the dumper file"},
+        metadata={"doc": "Extra code to be put below the record"},
     )
-    module = ma.fields.String(metadata={"doc": "Class module"})
+    table = ma.fields.Str(
+        attribute="table",
+        data_key="table",
+        metadata={"doc": "Name of the database table"},
+    )
+    alembic = ma.fields.Str(metadata={"doc": "module where alembic files are stored"})
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
     skip = ma.fields.Boolean()
 
 
-class RecordDumperModelComponent(DataTypeComponent):
+class RecordMetadataModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
     depends_on = [DefaultsModelComponent, RecordModelComponent]
 
     class ModelSchema(ma.Schema):
-        record_dumper = ma.fields.Nested(
-            RecordDumperClassSchema,
-            attribute="record-dumper",
-            data_key="record-dumper",
-            metadata={"doc": "Settings for record dumper"},
+        record_metadata = ma.fields.Nested(
+            RecordMetadataClassSchema,
+            attribute="record-metadata",
+            data_key="record-metadata",
+            metadata={"doc": "Record metadata settings"},
         )
 
-    def before_model_prepare(self, datatype, *, context, **kwargs):
-        record_module = parent_module(datatype.definition["record"]["module"])
+    def before_model_prepare(self, datatype, **kwargs):
+        records_module = parent_module(datatype.definition["record"]["module"])
         prefix = datatype.definition["module"]["prefix"]
+        alias = datatype.definition["module"]["alias"]
 
-        dumper = set_default(datatype, "record-dumper", {})
-        dumper.setdefault("generate", True)
-
-        dumper_module = dumper.setdefault("module", f"{record_module}.dumpers.dumper")
-        dumper.setdefault("class", f"{dumper_module}.{prefix}Dumper")
-        dumper.setdefault(
-            "base-classes", ["oarepo_runtime.records.dumpers.SearchDumper"]
+        metadata = set_default(datatype, "record-metadata", {})
+        metadata.setdefault("generate", True)
+        metadata_module = metadata.setdefault("module", f"{records_module}.models")
+        metadata.setdefault("class", f"{metadata_module}.{prefix}Metadata")
+        metadata.setdefault("base-classes", ["db.Model", "RecordMetadataBase"])
+        metadata.setdefault("extra-code", "")
+        metadata.setdefault(
+            "imports",
+            [
+                {"import": "invenio_records.models.RecordMetadataBase"},
+                {"import": "invenio_db.db"},
+            ],
         )
-        dumper.setdefault("extra-code", "")
-        dumper.setdefault("extensions", [])
-        dumper.setdefault("imports", [])
+        metadata.setdefault("table", f"{prefix.lower()}_metadata")
+        metadata.setdefault("alembic", f"{records_module}.alembic")
+        metadata.setdefault("alias", alias)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/record_item.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/search_options.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,74 @@
 import marshmallow as ma
 
 from oarepo_model_builder.datatypes import DataTypeComponent, ModelDataType
-from oarepo_model_builder.utils.python_name import (
-    convert_config_to_qualified_name,
-    package_name,
-)
+from oarepo_model_builder.datatypes.components.model.utils import set_default
 from oarepo_model_builder.validation.utils import ImportSchema
 
-from .service import ServiceModelComponent
-from .utils import set_default
+from .defaults import DefaultsModelComponent
 
 
-class RecordItemClassSchema(ma.Schema):
+class RecordSearchOptionsSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
-    generate = ma.fields.Bool(metadata={"doc": "Generate the record item class"})
+    extra_code = ma.fields.String(
+        attribute="extra-code",
+        data_key="extra-code",
+        metadata={"doc": "Extra code to be pasted to search options module"},
+    )
+    module = ma.fields.String(
+        metadata={"doc": "Module where the facets will be placed"}
+    )
+    generate = ma.fields.Boolean()
+    skip = ma.fields.Boolean()
     class_ = ma.fields.Str(
         attribute="class",
         data_key="class",
-        metadata={"doc": "Qualified name of the record item class"},
+        metadata={"doc": "Qualified name of the class"},
     )
     base_classes = ma.fields.List(
         ma.fields.Str(),
         attribute="base-classes",
         data_key="base-classes",
-        metadata={"doc": "List of base classes"},
-    )
-    extra_code = ma.fields.Str(
-        attribute="extra-code",
-        data_key="extra-code",
-        metadata={"doc": "Extra code to be put below the record item class"},
-    )
-    components = ma.fields.List(
-        ma.fields.String(), metadata={"doc": "List of record item components"}
+        metadata={"doc": "Model base classes"},
     )
-    module = ma.fields.String(metadata={"doc": "Class module"})
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
-    skip = ma.fields.Boolean()
 
 
-class RecordItemModelComponent(DataTypeComponent):
+class SearchOptionsModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
-    depends_on = [ServiceModelComponent]
+    depends_on = [DefaultsModelComponent]
 
     class ModelSchema(ma.Schema):
-        record_item = ma.fields.Nested(
-            RecordItemClassSchema,
-            attribute="record-item",
-            data_key="record-item",
-            metadata={"doc": "Record item class settings"},
+        search_options = ma.fields.Nested(
+            RecordSearchOptionsSchema,
+            required=False,
         )
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
-        record_prefix = datatype.definition["module"]["prefix"]
-
-        service_package = package_name(datatype.definition["service-config"]["module"])
-
-        record_item_config = set_default(datatype, "record-item", {})
-
-        record_item_config.setdefault("generate", True)
-        record_item_module = record_item_config.setdefault(
-            "module",
-            f"{service_package}.results",
+        module = datatype.definition["module"]["qualified"]
+        profile_module = context["profile_module"]
+        record_search_prefix = datatype.definition["module"]["prefix"]
+
+        record_search_options = set_default(datatype, "search-options", {})
+        record_search_options.setdefault("generate", True)
+        module = record_search_options.setdefault(
+            "module", f"{module}.services.{profile_module}.search"
         )
-        record_item_config.setdefault(
-            "class",
-            f"{record_item_module}.{record_prefix}RecordItem",
+
+        record_search_options.setdefault("extra-code", "")
+        record_search_options.setdefault(
+            "class", f"{module}.{record_search_prefix}SearchOptions"
         )
-        record_item_config.setdefault("extra-code", "")
-        record_item_config.setdefault(
-            "base-classes",
+        record_search_options.setdefault("base-classes", ["InvenioSearchOptions"])
+        record_search_options.setdefault(
+            "imports",
             [
-                "oarepo_runtime.services.results.RecordItem",
+                {
+                    "import": "invenio_records_resources.services.SearchOptions",
+                    "alias": "InvenioSearchOptions",
+                }
             ],
         )
-        record_item_config.setdefault("components", [])
-        record_item_config.setdefault(
-            "imports",
-            [],
-        )
-        convert_config_to_qualified_name(record_item_config)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/resource.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/resource.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,41 +37,27 @@
         data_key="extra-code",
         metadata={"doc": "Extra code to be put to the bottom of the generated file"},
     )
     module = ma.fields.String(metadata={"doc": "Class module"})
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
-    additional_args = ma.fields.List(
-        ma.fields.String(),
-        attribute="additional-args",
-        data_key="additional-args",
-        metadata={
-            "doc": "List of additional arguments that will be passed to the resource constructor"
-        },
-    )
     skip = ma.fields.Boolean()
 
 
 class ResourceConfigClassSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
     base_url = ma.fields.String(
         data_key="base-url",
         attribute="base-url",
         metadata={"doc": "The base url of the resource"},
     )
 
-    base_html_url = ma.fields.String(
-        data_key="base-html-url",
-        attribute="base-html-url",
-        metadata={"doc": "The base html url of the resource"},
-    )
-
     generate = ma.fields.Bool(
         metadata={"doc": "Generate the resource config class (default)"}
     )
     config_key = ma.fields.Str(
         metadata={
             "doc": "Name of the config entry that holds the current resource class name"
         }
@@ -92,22 +78,14 @@
         data_key="extra-code",
         metadata={"doc": "Extra code to be put below the generated config class"},
     )
     module = ma.fields.String(metadata={"doc": "Class module"})
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
-    additional_args = ma.fields.List(
-        ma.fields.String(),
-        attribute="additional-args",
-        data_key="additional-args",
-        metadata={
-            "doc": "List of additional arguments that will be passed to the resource config constructor"
-        },
-    )
     skip = ma.fields.Boolean()
 
 
 class ResourceModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
     depends_on = [DefaultsModelComponent]
 
@@ -142,41 +120,34 @@
             f"{resource_module}.{module_container['prefix']}Resource",
         )
         resource.setdefault(
             "proxy",
             "current_resource",
         )
         resource.setdefault("extra-code", "")
-        resource.setdefault(
-            "base-classes", ["invenio_records_resources.resources.RecordResource"]
-        )
+        resource.setdefault("base-classes", ["RecordResource"])
         resource.setdefault(
             "imports",
-            [],
+            [{"import": "invenio_records_resources.resources.RecordResource"}],
         )
-        resource.setdefault("additional-args", [])
         convert_config_to_qualified_name(resource)
 
         config = set_default(datatype, "resource-config", {})
         config.setdefault("generate", True)
         config.setdefault("base-url", f"/{module_container['kebab-module']}/")
-        config.setdefault("base-html-url", f"/{module_container['kebab-module']}/")
         config.setdefault(
             "config-key",
             f"{module_container['base-upper']}_{context['profile_upper']}_RESOURCE_CONFIG",
         )
         config_module = config.setdefault("module", f"{resource_package}.config")
         config.setdefault(
             "class",
             f"{config_module}.{module_container['prefix']}ResourceConfig",
         )
         config.setdefault("extra-code", "")
 
-        config.setdefault(
-            "base-classes", ["invenio_records_resources.resources.RecordResourceConfig"]
-        )
+        config.setdefault("base-classes", ["RecordResourceConfig"])
         config.setdefault(
             "imports",
-            [],
+            [{"import": "invenio_records_resources.resources.RecordResourceConfig"}],
         )
-        config.setdefault("additional-args", [])
         convert_config_to_qualified_name(config)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/sample.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/sample.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/service.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,22 +36,14 @@
         data_key="extra-code",
         metadata={"doc": "Extra code to be put below the generated service class"},
     )
     module = ma.fields.String(metadata={"doc": "Class module"})
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
-    additional_args = ma.fields.List(
-        ma.fields.String(),
-        attribute="additional-args",
-        data_key="additional-args",
-        metadata={
-            "doc": "List of additional arguments that will be passed to the service constructor"
-        },
-    )
     skip = ma.fields.Boolean()
 
 
 class ServiceConfigClassSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
@@ -85,22 +77,14 @@
     components = ma.fields.List(
         ma.fields.String(), metadata={"doc": "List of service components"}
     )
     module = ma.fields.String(metadata={"doc": "Class module"})
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
-    additional_args = ma.fields.List(
-        ma.fields.String(),
-        attribute="additional-args",
-        data_key="additional-args",
-        metadata={
-            "doc": "List of additional arguments that will be passed to the service config constructor"
-        },
-    )
     skip = ma.fields.Boolean()
 
 
 class ServiceModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
     depends_on = [DefaultsModelComponent, AppModelComponent]
 
@@ -116,14 +100,15 @@
         )
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
         profile_module = context["profile_module"]
         module = datatype.definition["module"]["qualified"]
         module_base_upper = datatype.definition["module"]["base-upper"]
         record_prefix = datatype.definition["module"]["prefix"]
+        flask_extension_name = datatype.definition["ext"]["alias"]
 
         service_package = f"{module}.services.{profile_module}"
 
         config = set_default(datatype, "service-config", {})
 
         config.setdefault("generate", True)
         config.setdefault(
@@ -135,40 +120,49 @@
             f"{service_package}.config",
         )
         config.setdefault(
             "class",
             f"{config_module}.{record_prefix}ServiceConfig",
         )
         config.setdefault("extra-code", "")
-        config.setdefault("service-id", datatype.definition["module"]["suffix-snake"])
+        config.setdefault("service-id", flask_extension_name)
         config.setdefault(
             "base-classes",
+            ["PermissionsPresetsConfigMixin", "InvenioRecordServiceConfig"],
+        )
+        config.setdefault("components", [])
+        config.setdefault(
+            "imports",
             [
-                "oarepo_runtime.services.config.service.PermissionsPresetsConfigMixin",
-                "invenio_records_resources.services.RecordServiceConfig{InvenioRecordServiceConfig}",
+                {
+                    "import": "invenio_records_resources.services.RecordServiceConfig",
+                    "alias": "InvenioRecordServiceConfig",
+                },
+                {
+                    "import": "oarepo_runtime.config.service.PermissionsPresetsConfigMixin"
+                },
             ],
         )
-        config.setdefault("components", [])
-        config.setdefault("additional-args", [])
         convert_config_to_qualified_name(config)
 
         service = set_default(datatype, "service", {})
 
         service.setdefault("generate", True)
         service.setdefault(
             "config-key",
             f"{module_base_upper}_{context['profile_upper']}_SERVICE_CLASS",
         )
         service.setdefault("proxy", "current_service")
         service_module = service.setdefault("module", f"{service_package}.service")
         service.setdefault("class", f"{service_module}.{record_prefix}Service")
         service.setdefault("extra-code", "")
-        service.setdefault(
-            "base-classes",
-            ["invenio_records_resources.services.RecordService{InvenioRecordService}"],
-        )
+        service.setdefault("base-classes", ["InvenioRecordService"])
         service.setdefault(
             "imports",
-            [],
+            [
+                {
+                    "import": "invenio_records_resources.services.RecordService",
+                    "alias": "InvenioRecordService",
+                }
+            ],
         )
-        service.setdefault("additional-args", [])
         convert_config_to_qualified_name(service)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/ui.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+
 import marshmallow as ma
 
 from oarepo_model_builder.datatypes import ModelDataType
 from oarepo_model_builder.utils.python_name import parent_module
-from oarepo_model_builder.validation.extensibility import ExtensibleSchema
 from oarepo_model_builder.validation.utils import ImportSchema
 
 from ..ui import ObjectUIComponent, ObjectUIExtraSchema
 from .marshmallow import ModelMarshmallowSchema
 from .resource import ResourceModelComponent
 from .utils import set_default
 
@@ -32,29 +32,14 @@
     extra_code = ma.fields.Str(
         attribute="extra-code",
         data_key="extra-code",
         metadata={
             "doc": "Extra code to be put below the generated ui serializer class"
         },
     )
-    list_schema_cls = ma.fields.Str(
-        attribute="list-schema-cls",
-        data_key="list-schema-cls",
-        metadata={"doc": "Marshmallow class for list serialization"},
-    )
-    format_serializer_cls = ma.fields.Str(
-        attribute="format-serializer-cls",
-        data_key="format-serializer-cls",
-        metadata={"doc": "Class for serializing the resulting json"},
-    )
-    schema_context_args = ma.fields.Dict(
-        attribute="schema-context-args",
-        data_key="schema-context-args",
-        metadata={"doc": "Extra args for ui marshmallow schema context"},
-    )
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
     skip = ma.fields.Boolean()
     generate = ma.fields.Boolean()
 
 
@@ -63,17 +48,15 @@
 
 
 class UIModelComponent(ObjectUIComponent):
     eligible_datatypes = [ModelDataType]
     depends_on = [ResourceModelComponent]
 
     class ModelSchema(ma.Schema):
-        ui = ma.fields.Nested(
-            ExtensibleSchema("ui.model", ModelUISchema), metadata={"doc": "UI settings"}
-        )
+        ui = ma.fields.Nested(ModelUISchema, metadata={"doc": "UI settings"})
         json_serializer = ma.fields.Nested(
             JSONSerializerSchema,
             attribute="json-serializer",
             data_key="json-serializer",
         )
 
     def before_model_prepare(self, datatype, **kwargs):
@@ -81,24 +64,18 @@
         resources_module = parent_module(datatype.definition["resource"]["module"])
 
         set_default(datatype, "ui", {})
 
         json = set_default(datatype, "json-serializer", {})
         json_module = json.setdefault("module", f"{resources_module}.ui")
         json.setdefault("class", f"{json_module}.{prefix}UIJSONSerializer")
-        json.setdefault(
-            "base-classes", ["oarepo_runtime.resources.LocalizedUIJSONSerializer"]
-        )
+        json.setdefault("base-classes", ["MarshmallowSerializer"])
         json.setdefault(
             "imports",
-            [],
+            [
+                {"import": "flask_resources.BaseListSchema"},
+                {"import": "flask_resources.MarshmallowSerializer"},
+                {"import": "flask_resources.serializers.JSONSerializer"},
+            ],
         )
         json.setdefault("extra-code", "")
         json.setdefault("generate", True)
-        json.setdefault("list_schema_cls", "flask_resources.BaseListSchema")
-        json.setdefault(
-            "format_serializer_cls", "flask_resources.serializers.JSONSerializer"
-        )
-        json.setdefault(
-            "schema-context-args",
-            {'"object_key"': '"ui"', '"identity"': "{{ flask.g{g.identity} }}"},
-        )
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,27 +32,27 @@
         services_module = parent_module(datatype.definition["service"]["module"])
 
         marshmallow: Dict = set_default(datatype, "ui", "marshmallow", {})
         marshmallow.setdefault("generate", True)
         module = marshmallow.setdefault("module", f"{services_module}.ui_schema")
         marshmallow.setdefault("class", f"{module}.{prefix}UISchema")
         marshmallow.setdefault("extra-code", "")
+        marshmallow.setdefault("base-classes", ["InvenioUISchema"])
         marshmallow.setdefault(
-            "base-classes", ["oarepo_runtime.services.schema.ui.InvenioUISchema"]
+            "imports", [{"import": "oarepo_runtime.ui.marshmallow.InvenioUISchema"}]
         )
-        marshmallow.setdefault("imports", [])
         convert_config_to_qualified_name(marshmallow)
 
         if "properties" in datatype.definition and "metadata" in (
             datatype.definition["properties"] or {}
         ):
             metadata_marshmallow = set_default(
                 datatype, "properties", "metadata", "ui", "marshmallow", {}
             )
             metadata_marshmallow.setdefault("generate", True)
             metadata_module = metadata_marshmallow.setdefault("module", module)
             metadata_marshmallow.setdefault(
                 "class", f"{metadata_module}.{prefix}MetadataUISchema"
             )
             metadata_marshmallow.setdefault("extra-code", "")
-            metadata_marshmallow.setdefault("base-classes", ["marshmallow.Schema"])
+            metadata_marshmallow.setdefault("base-classes", ["ma.Schema"])
             convert_config_to_qualified_name(metadata_marshmallow)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/model/utils.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/components/ui.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/containers/array.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/containers/array.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 
 class ArrayDataType(DataType):
     model_type = "array"
 
     ui = {
         "marshmallow": {
-            "field-class": "marshmallow.fields{ma_fields.List}",
+            "field-class": "ma_fields.List",
         }
     }
     marshmallow = {
-        "field-class": "marshmallow.fields{ma_fields.List}",
+        "field-class": "ma_fields.List",
     }
     json_schema = {"type": "array"}
 
     class ModelSchema(DataType.ModelSchema):
         items = fields.Nested(FieldSchema)
+        uniqueItems = fields.Boolean(required=False)
         minItems = fields.Integer(required=False)
         maxItems = fields.Integer(required=False)
 
     def prepare(self, context):
         from ..datatypes import datatypes
 
         items = self.definition.get("items", {})
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/containers/object.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/containers/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,19 +126,19 @@
 
 
 class ObjectDataType(DataType):
     model_type = "object"
 
     ui = {
         "marshmallow": {
-            "field-class": "marshmallow.fields{ma_fields.Nested}",
+            "field-class": "ma_fields.Nested",
         }
     }
     marshmallow = {
-        "field-class": "marshmallow.fields{ma_fields.Nested}",
+        "field-class": "ma_fields.Nested",
     }
     json_schema = {"type": "object"}
     mapping = {"type": "object"}
 
     class ModelSchema(DataType.ModelSchema):
         properties = ObjectPropertiesField()
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/datatypes.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,44 @@
 import copy
 import dataclasses
 import json
 from collections.abc import Mapping
 from functools import cached_property, lru_cache
-from typing import Any, Dict, List, Type, Union
+from typing import Any, Dict, List, Optional, Type, Union
 
 import importlib_metadata
 import marshmallow as ma
 from marshmallow import fields
 
 from ..utils.deepmerge import deepmerge
 from ..utils.import_class import import_class
 from ..utils.properties import class_property
 from ..validation.utils import PermissiveSchema
 
 
 @dataclasses.dataclass
+class Import:
+    import_path: str
+    alias: Optional[str] = None
+
+    @staticmethod
+    def from_config(d):
+        if isinstance(d, dict):
+            return Import(d["import"], d.get("alias"))
+        elif isinstance(d, (tuple, list)):
+            return [Import.from_config(x) for x in d]
+
+    def __hash__(self):
+        return hash(self.import_path) ^ hash(self.alias)
+
+    def __eq__(self, o):
+        return self.import_path == o.import_path and self.alias == o.alias
+
+
+@dataclasses.dataclass
 class Section:
     section_name: str
     config: Dict[str, Any]
     children: Dict[str, "AbstractDataType"] = dataclasses.field(default_factory=dict)
     item: "AbstractDataType" = None
 
     @cached_property
@@ -84,15 +103,14 @@
         self.parent = parent
         self.children = {}
         self.definition = definition
         self.key = key
         self.model = model
         self.schema = schema
         self._sections = {}
-        self.skip_in_path = False
 
     def copy(self, without_children=False):
         ret = type(self)(
             # shallow copy of the definition to enable overwriting pieces of it
             self.parent,
             {**self.definition},
             self.key,
@@ -179,41 +197,31 @@
                 section=section,
             )
         self._sections[section_key] = section
         return section
 
     @cached_property
     def path(self):
-        if not self.parent or not self.parent.path:
-            return self.path_element or ""
-
-        p = self.parent.path  # recursion
-        if self.path_element:
-            return p + f".{self.path_element}"
-        return p
-
-    @property
-    def path_element(self):
-        if self.skip_in_path:
-            return None
-        return self.key
+        ret = []
+        p = self
+        while p:
+            if p.key:
+                ret.append(p.key)
+            p = p.parent
+        return ".".join(reversed(ret))
 
     @cached_property
     def stack(self):
         ret = []
         p = self
         while p:
             ret.append(p)
             p = p.parent
         return tuple(reversed(ret))
 
-    @property
-    def root(self):
-        return self.stack[0]
-
 
 class DataType(AbstractDataType):
     model_type = None
 
     class ModelSchema(ma.Schema):
         type = fields.String(required=True)
         required = fields.Bool()
@@ -231,25 +239,21 @@
 
     @class_property
     def validator(cls):
         validators = list(
             datatypes.call_class_components(datatype=cls, method="model_schema")
         ) + list(datatypes.get_class_components(cls, "ModelSchema"))
         validators = [x for x in validators if x]
-        unique_validators = []
-        for v in validators:
-            if v not in unique_validators:
-                unique_validators.append(v)
 
         class Meta:
             unknown = ma.RAISE
 
         ret = type(
             f"{cls.__name__}ModelValidator",
-            (*unique_validators, cls.ModelSchema),
+            (*validators, cls.ModelSchema),
             {"Meta": Meta},
         )
         return ret
 
     def deep_iter(self):
         yield self
 
@@ -284,15 +288,14 @@
             for component in entry.load():
                 c.append(component())
         return c
 
     @lru_cache(maxsize=1024)
     def _get_components(self, datatype_class):
         datatype_components = []
-
         for component in self.components:
             if not component.eligible_datatypes:
                 datatype_components.append(component)
             else:
                 for depends_on in component.eligible_datatypes:
                     if isinstance(depends_on, str):
                         depends_on = import_class(depends_on)
@@ -306,39 +309,24 @@
         for c in datatype_components:
             non_leaf_components.update(type(c).mro()[1:])
 
         for c in datatype_components:
             if type(c) not in non_leaf_components:
                 unsorted_components.append(c)
 
-        dependency_remaps = {}
-        for c in unsorted_components:
-            remap = getattr(c, "dependency_remap", None)
-            if remap:
-                dependency_remaps[remap] = type(c)
         # sort by dependencies
         depsort_map = {}
-
-        def get_dependent_component(component):
-            return (
-                dependency_remaps[component]
-                if component in dependency_remaps
-                else component
-            )
-
         for c in unsorted_components:
             dependencies_classes = depsort_map.setdefault(type(c), [])
             depsort_map[type(c)] = dependencies_classes
             for depends_on in getattr(c, "depends_on", []):
-                depends_on = get_dependent_component(depends_on)
                 if isinstance(depends_on, str):
                     depends_on = import_class(depends_on)
                 dependencies_classes.append(depends_on)
             for affects in getattr(c, "affects", []):
-                affects = get_dependent_component(affects)
                 if isinstance(affects, str):
                     affects = import_class(affects)
                 depsort_map.setdefault(affects, []).append(type(c))
 
         sorted_components = []
         while unsorted_components:
             new_unsorted_components = []
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/model.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import dataclasses
 from typing import List
 
 import marshmallow as ma
 
-from ..datatypes import Section, datatypes
-from ..utils.links import url_prefix2link
-from ..utils.python_name import Import
+from ..datatypes import Import, Section, datatypes
 from .containers import ObjectDataType
 
 
 @dataclasses.dataclass
 class Link:
     name: str
     link_class: str = "RecordLink"
@@ -45,50 +43,36 @@
 
     @property
     def section_global_mapping(self):
         return self.default_section_mapping
 
     @property
     def links(self):
-        url_prefix = url_prefix2link(self.definition["resource-config"]["base-url"])
-        html_url_prefix = url_prefix2link(
-            self.definition["resource-config"]["base-html-url"]
-        )
         return {
             "links_item": [
                 Link(
                     name="self",
                     link_class="RecordLink",
-                    link_args=[f'"{{+api}}{url_prefix}{{id}}"'],
-                    imports=[Import("invenio_records_resources.services.RecordLink")],
-                ),
-                Link(
-                    name="self_html",
-                    link_class="RecordLink",
-                    link_args=[
-                        f'"{{+ui}}{html_url_prefix}{{id}}"',
-                    ],
+                    link_args=['"{self.url_prefix}{id}"'],
                     imports=[Import("invenio_records_resources.services.RecordLink")],
                 ),
             ],
             "links_search": [
                 Link(
                     name=None,
                     link_class="pagination_links",
-                    link_args=[f'"{{+api}}{url_prefix}{{?args*}}"'],
+                    link_args=['"{self.url_prefix}{?args*}"'],
                     imports=[
                         Import("invenio_records_resources.services.pagination_links")
                     ],
                 ),
             ],
         }
 
     def prepare(self, context):
-        if "profile" in context:
-            self.profile = context["profile"]
         datatypes.call_components(
             datatype=self, method="before_model_prepare", context=context
         )
         super().prepare(context)
         datatypes.call_components(
             datatype=self, method="after_model_prepare", context=context
         )
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/primitive_types.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/primitive_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from marshmallow import fields
 
 from .datatypes import DataType
 
 
 class NumberDataType(DataType):
     facets = {
-        "facet-class": "invenio_records_resources.services.records.facets.TermsFacet",
+        "facet-class": "TermsFacet",
+        "imports": [
+            {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
+        ],
     }
 
 
 class IntegerDataType(NumberDataType):
     model_type = "integer"
 
     ui = {
         "marshmallow": {
-            "field-class": "marshmallow.fields{ma_fields.Integer}",
+            "field-class": "ma_fields.Integer",
         }
     }
     marshmallow = {
-        "field-class": "marshmallow.fields{ma_fields.Integer}",
+        "field-class": "ma_fields.Integer",
     }
     json_schema = {"type": "integer"}
 
     class ModelSchema(DataType.ModelSchema):
         minimum = fields.Integer(required=False)
         exclusiveMinimum = fields.Integer(required=False)
         maximum = fields.Integer(required=False)
@@ -31,19 +34,19 @@
 
 
 class FloatDataType(NumberDataType):
     model_type = "float"
 
     ui = {
         "marshmallow": {
-            "field-class": "marshmallow.fields{ma_fields.Float}",  # NOSONAR
+            "field-class": "ma_fields.Float",  # NOSONAR
         }
     }
     marshmallow = {
-        "field-class": "marshmallow.fields{ma_fields.Float}",
+        "field-class": "ma_fields.Float",
     }
     json_schema = {"type": "number"}
 
     class ModelSchema(DataType.ModelSchema):
         minimum = fields.Float(required=False)
         exclusiveMinimum = fields.Float(required=False)
         maximum = fields.Float(required=False)
@@ -52,19 +55,19 @@
 
 
 class DoubleDataType(NumberDataType):
     model_type = "double"
 
     ui = {
         "marshmallow": {
-            "field-class": "marshmallow.fields{ma_fields.Float}",
+            "field-class": "ma_fields.Float",
         }
     }
     marshmallow = {
-        "field-class": "marshmallow.fields{ma_fields.Float}",
+        "field-class": "ma_fields.Float",
     }
     json_schema = {"type": "number"}
 
     class ModelSchema(DataType.ModelSchema):
         minimum = fields.Float(required=False)
         exclusiveMinimum = fields.Float(required=False)
         maximum = fields.Float(required=False)
@@ -73,17 +76,20 @@
 
 
 class BooleanDataType(DataType):
     model_type = "boolean"
 
     ui = {
         "marshmallow": {
-            "field-class": "marshmallow.fields{ma_fields.Boolean}",
+            "field-class": "ma_fields.Boolean",
         }
     }
     marshmallow = {
-        "field-class": "marshmallow.fields{ma_fields.Boolean}",
+        "field-class": "ma_fields.Boolean",
     }
     json_schema = {"type": "boolean"}
     facets = {
-        "facet-class": "invenio_records_resources.services.records.facets.TermsFacet",
+        "facet-class": "TermsFacet",
+        "imports": [
+            {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
+        ],
     }
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/datatypes/strings.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/strings.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,19 +16,19 @@
             f"Regex '{value}' is not valid. Reported error: '{str(e)}'"
         )
 
 
 class StringDataType(DataType):
     ui = {
         "marshmallow": {
-            "field-class": "marshmallow.fields{ma_fields.String}",
+            "field-class": "ma_fields.String",
         }
     }
     marshmallow = {
-        "field-class": "marshmallow.fields{ma_fields.String}",
+        "field-class": "ma_fields.String",
     }
     json_schema = {"type": "string"}
 
     class ModelSchema(DataType.ModelSchema):
         minLength = fields.Integer(required=False)
         maxLength = fields.Integer(required=False)
         regex = fields.String(required=False, validate=validate_regex)
@@ -37,39 +37,43 @@
 class FulltextDataType(StringDataType):
     model_type = "fulltext"
     mapping = {"type": "text"}
 
 
 class KeywordDataType(StringDataType):
     model_type = "keyword"
-    mapping = {"type": "keyword", "ignore_above": 1024}
+    mapping = {"type": "keyword"}
     facets = {
-        "facet-class": "invenio_records_resources.services.records.facets.TermsFacet",
+        "facet-class": "TermsFacet",
+        "imports": [
+            {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
+        ],
     }
 
 
 class UUIDDataType(StringDataType):
     model_type = "uuid"
     mapping = {"type": "keyword"}
 
 
 class FulltextKeywordDataType(StringDataType):
     model_type = "fulltext+keyword"
-    mapping = {
-        "type": "text",
-        "fields": {"keyword": {"type": "keyword", "ignore_above": 256}},
+    mapping = {"type": "text", "fields": {"keyword": {"type": "keyword"}}}
+    facets = {
+        "facet-class": "TermsFacet",
+        "keyword": True,
+        # "path": "_keyword",
+        "imports": [
+            {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
+        ],
     }
-    facets = {"facet": False}
 
 
 class URLDataType(StringDataType):
     model_type = "url"
-    mapping = {"type": "keyword", "ignore_above": 1024}
+    mapping = {"type": "keyword"}
     facets = {
-        "facet-class": "invenio_records_resources.services.records.facets.TermsFacet",
-    }
-
-class HtmlDataType(FulltextDataType):
-    model_type = "html"
-    marshmallow = {
-        "field-class": "marshmallow_utils.fields.SanitizedHTML",
+        "facet-class": "TermsFacet",
+        "imports": [
+            {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
+        ],
     }
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/entrypoints.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/entrypoints.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+import importlib.resources
 import sys
 from functools import reduce
 from importlib import import_module
 from pathlib import Path
 
 import importlib_metadata
 
 from oarepo_model_builder.builder import ModelBuilder
 from oarepo_model_builder.schema import ModelSchema, remove_star_keys
-from oarepo_model_builder.validation import InvalidModelException
 
 
 def create_builder_from_entrypoints(profile="record", **kwargs):
     # output classes do not depend on profile
     output_classes = load_entry_points_list("oarepo_model_builder.outputs", None)
     builder_classes = load_entry_points_list("oarepo_model_builder.builders", profile)
 
@@ -59,34 +59,25 @@
 def load_model_from_entrypoint(ep: importlib_metadata.EntryPoint):
     def load(schema):
         try:
             loaded_schema = ep.load()
         except:  # NOSONAR intentionally broad
             module = import_module(ep.module)
             split_attr = ep.attr.split(".")
-            for split_point in range(len(split_attr) - 1, -1, -1):
-                base_path = split_attr[:split_point]
-                file_name = ".".join(split_attr[split_point:])
-                if base_path:
-                    file_name = (
-                        reduce(lambda x, y: x / y, [Path(x) for x in base_path])
-                        / file_name
-                    )
-
-                module_path = getattr(module, "__path__", [])
-                if module_path:
-                    full_fn = Path(module_path[0]) / file_name
-                else:
-                    full_fn = Path(file_name)
-                if not full_fn.exists():
-                    continue
-                loaded_schema = schema._load(full_fn, content=full_fn.read_text())
-                break
+            fn = f"{split_attr[-2]}.{split_attr[-1]}"
+            if len(split_attr) > 2:
+                fn = reduce(lambda x, y: Path(x) / Path(y), split_attr[:-2]) / fn
+            module_path = getattr(module, "__path__", [])
+            if module_path:
+                full_fn = Path(module_path[0]) / fn
             else:
-                raise InvalidModelException(f"Could not load entry point {ep}")
+                full_fn = fn
+            content = importlib.resources.open_text(module, fn, encoding="utf-8").read()
+            loaded_schema = schema._load(full_fn, content=content)
+
         remove_star_keys(loaded_schema)
         return loaded_schema
 
     return load
 
 
 def load_included_models_from_entry_points():
@@ -113,36 +104,14 @@
         included_models.update(extra_included)
     schema = ModelSchema(
         model_filename,
         content=model_content,
         loaders=loaders,
         included_models=included_models,
         merged_models=merged_models,
-        reference_processors={
-            ModelSchema.REF_KEYWORD: load_entry_points_list(
-                "oarepo_model_builder.loaders.ref", None
-            ),
-            ModelSchema.USE_KEYWORD: load_entry_points_list(
-                "oarepo_model_builder.loaders.use", None
-            ),
-            ModelSchema.EXTEND_KEYWORD: load_entry_points_list(
-                "oarepo_model_builder.loaders.extend", None
-            ),
-        },
-        post_reference_processors={
-            ModelSchema.REF_KEYWORD: load_entry_points_list(
-                "oarepo_model_builder.loaders.post.ref", None
-            ),
-            ModelSchema.USE_KEYWORD: load_entry_points_list(
-                "oarepo_model_builder.loaders.post.use", None
-            ),
-            ModelSchema.EXTEND_KEYWORD: load_entry_points_list(
-                "oarepo_model_builder.loaders.post.extend", None
-            ),
-        },
     )
     for config in configs:
         load_config(schema, config, loaders)
     for s in sets:
         k, v = s.split("=", 1)
         schema.schema[k] = v
     check_plugin_packages(schema)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/fs.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/fs.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/generate_doc.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/generate_doc.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/__init__.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,12 +15,9 @@
     "version": "templates/version.py.jinja2",
     "config": "templates/config.py.jinja2",
     "ext": "templates/ext.py.jinja2",
     "proxies": "templates/proxies.py.jinja2",
     "record-facets": "templates/invenio_record_facets.py.jinja2",
     "pid-provider": "templates/pid_provider.py.jinja2",
     # utils and included
-    "ext-resource": "templates/ext_resource.py.jinja2",
-    "edtf-interval-record-dumper": "templates/edtf_interval_record_dumper.py.jinja2",
-    "record-item": "templates/record_item.py.jinja2",
-    "record-list": "templates/record_list.py.jinja2",
+    "imports": "templates/imports.py.jinja2",
 }
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_base.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,37 +26,31 @@
             and not dict_get(
                 self.current_model.definition, [self.section, "generate"], False
             )
         ):
             return False
         return True
 
-    @property
-    def vars(self):
-        section = getattr(
-            self.current_model,
-            f"section_mb_{self.TYPE.replace('-', '_')}",
-        )
-
-        vars = MergedAttrDict(section.config, self.current_model.definition)
-        return vars
-
     def finish(self, **extra_kwargs):
         super().finish()
         if not self.generate:
             return
-
         module = self._get_output_module()
         python_path = Path(module_to_path(module) + ".py")
 
+        section = getattr(
+            self.current_model,
+            f"section_mb_{self.TYPE.replace('-', '_')}",
+        )
+        merged = MergedAttrDict(section.config, self.current_model.definition)
         self.process_template(
             python_path,
             self.template,
             current_module=module,
-            vars=self.vars,
+            vars=merged,
             **extra_kwargs,
         )
 
     def _get_output_module(self):
         module = self.current_model.definition[self.section]["module"]
         return module
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_facets.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_facets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict
+from typing import List
 
 from oarepo_model_builder.datatypes import DataType
 
 from ..datatypes.components.facets import FacetDefinition
 from .invenio_base import InvenioBaseClassPythonBuilder
 
 
@@ -12,30 +12,22 @@
     template = "record-facets"
 
     def build_node(self, node: DataType):
         # everything is done in finish
         pass
 
     def finish(self, **extra_kwargs):
-        facets = get_distinct_facets(self.current_model)
+        facets: List[FacetDefinition] = []
+        for node in self.current_model.deep_iter():
+            facets.extend(node.section_facets.config["facets"])
         package = self.current_model.definition["facets"]["module"]
 
         imports = []
         for f in facets:
             imports.extend(f.imports)
 
         return super().finish(
             current_package_name=package,
             facets=facets,
-            facet_imports=imports,
+            imports=imports,
             **extra_kwargs,
         )
-
-
-def get_distinct_facets(current_model):
-    facets_dict: Dict[str, FacetDefinition] = {}
-    for node in current_model.deep_iter():
-        facet: FacetDefinition
-        for facet in node.section_facets.config["facets"]:
-            if facet.path not in facets_dict:
-                facets_dict[facet.path] = facet
-    return list(facets_dict.values())
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_marshmallow.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_marshmallow.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,15 @@
         imports = [*self.extra_imports]
 
         for cls in package_classes:
             imports.extend(cls.imports)
             for fld in cls.fields:
                 imports.extend(fld.imports)
 
-        imports = list(
-            sorted(set(imports), key=lambda x: (x.import_path or "", x.alias or ""))
-        )
+        imports = list(sorted(set(imports), key=lambda x: (x.import_path, x.alias)))
 
         self.process_template(
             python_path,
             self.template,
             current_module=package_name,
             imports=imports,
             generated_classes=package_classes,
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 class InvenioRecordMetadataAlembicSetupCfgBuilder(OutputBuilder):
     TYPE = "invenio_record_metadata_alembic_setup_cfg"
 
     def finish(self):
         super().finish()
 
         output: CFGOutput = self.builder.get_output("cfg", "setup.cfg")
-        if "alembic" not in self.current_model.definition["record-metadata"]:
-            return
-
         alembic_module_parent, alembic_module = split_package_base_name(
             self.current_model.definition["record-metadata"]["alembic"]
         )
         output.add_entry_point(
             "invenio_db.alembic",
             self.current_model.definition["record-metadata"]["alias"],
             f"{alembic_module_parent}:{alembic_module}",
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_record_service_config.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_record_service_config.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/invenio_script_sample_data.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/invenio_script_sample_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from typing import Callable
-import random
+
 import faker
 import faker.providers
 from faker import Faker
 
 from oarepo_model_builder.datatypes import (
     ArrayDataType,
     DataType,
@@ -36,60 +36,14 @@
         rnd = self.generator.random.randrange(-100, 100 + 1, 1)
         return rnd / 10
 
     def random_boolean(self):
         rnd = self.generator.random.randrange(0, 2, 1)
         return rnd == 1
 
-    def random_html(self):
-        html = ""
-        i = 0
-        while i < 4:
-            tag = random.choice(["<p>", "<div>", "<span>"])
-            content = ''.join(Faker().sentence())
-            html += f"{tag}{content}{tag[0]}/{tag[1:]}"
-            i = i + 1
-        return html
-
-    def datetime(self):
-        return self.generator.date_time_this_decade(
-            tzinfo=self.generator.pytimezone()
-        ).isoformat()
-
-    def edtf(self):
-        rnd = self.generator.random.randrange(0, 3)
-        if rnd == 0:
-            return self.generator.date()
-        if rnd == 1:
-            return self.generator.date("%Y")
-        if rnd == 2:
-            return self.generator.date("%Y-%m")
-
-    def edtf_interval(self):
-        a = [self.edtf(), self.edtf()]
-        a.sort()
-        return "/".join(a)
-
-    def edtf_time(self):
-        rnd = self.generator.random.randrange(0, 3)
-        if rnd == 0:
-            return self.generator.date()
-        if rnd == 1:
-            return self.generator.date("%Y")
-        if rnd == 2:
-            return self.generator.date("%Y-%m")
-
-    def edtf_time_interval(self):
-        a = [self.edtf(), self.edtf()]
-        a.sort()
-        return "/".join(a)
-
-    def time(self):
-        return self.generator.time()
-
     def sample_object(self):
         return {
             self.generator.word(): self.generator.word()
             for _ in range(self.generator.random.randrange(1, 5, 1))
         }
 
     def constant(self, value=None):
@@ -207,36 +161,22 @@
             method = node.key
         else:
             data_type = node.model_type
             if data_type == "integer":
                 method = "random_int"
             elif data_type == "number":
                 method = "random_float"
-            elif data_type == "html":
-                method = "random_html"
             elif data_type == "double":
                 method = "random_float"
             elif data_type == "float":
                 method = "random_float"
             elif data_type == "boolean":
                 method = "random_boolean"
             elif data_type == "date":
                 method = "date"
-            elif data_type == "datetime":
-                method = "datetime"
-            elif data_type == "time":
-                method = "time"
-            elif data_type == "edtf":
-                method = "edtf"
-            elif data_type == "edtf-interval":
-                method = "edtf_interval"
-            elif data_type == "edtf-time-interval":
-                method = "edtf_time_interval"
-            elif data_type == "edtf-time":
-                method = "edtf_time"
             elif data_type == "object":
                 # it is an object with unknown properties, return a sample object
                 method = "sample_object"
             elif data_type in ("string", "keyword", "fulltext", "fulltext+keyword"):
                 method = "sentence"
             else:
                 print(
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/api_views.py.jinja2` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/app_views.py.jinja2`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from flask import Blueprint
 
-def {{ vars.api_blueprint.function|base_name }}(app):
-    """Create {{ vars.record.class|base_name }} blueprint."""
-    blueprint = app.extensions["{{ vars.ext.alias }}"].{{ ext.ext_resource_name }}.as_blueprint()
-    blueprint.record_once(init_{{ vars.api_blueprint.function|base_name }})
+def {{ vars.app_blueprint.function|base_name }}(app):
+    blueprint = Blueprint("{{ vars.app_blueprint.alias }}_app", __name__, url_prefix="{{ vars.resource_config.base_url }}")
+    blueprint.record_once(init_{{ vars.app_blueprint.function|base_name }})
 
     #calls record_once for all other functions starting with "init_addons_"
     #https://stackoverflow.com/questions/58785162/how-can-i-call-function-with-string-value-that-equals-to-function-name
     funcs = globals()
     funcs = [v for k, v in funcs.items() if k.startswith("init_addons_{{ vars.module.suffix_snake }}") and callable(v)]
     for func in funcs:
         blueprint.record_once(func)
 
     return blueprint
 
-def init_{{ vars.api_blueprint.function|base_name }}(state):
+def init_{{ vars.app_blueprint.function|base_name }}(state):
     """Init app."""
     app = state.app
     ext = app.extensions["{{ vars.ext.alias }}"]
 
     {%  if not vars.service_config.skip %}
     # register service
     sregistry = app.extensions["invenio-records-resources"].registry
-    sregistry.register(ext.{{ ext.ext_service_name }}, service_id=ext.{{ ext.ext_service_name }}.config.service_id)
+    sregistry.register(ext.service, service_id="{{ vars.service_config.service_id }}")
     {% endif  %}
 
-    {%  if not vars.mapping.skip %}
+    {%  if not vars.mapping_settings.skip %}
     # Register indexer
-    if hasattr(ext.{{ ext.ext_service_name }}, "indexer"):
+    if hasattr(ext.service, "indexer"):
         iregistry = app.extensions["invenio-indexer"].registry
-        iregistry.register(ext.{{ ext.ext_service_name }}.indexer, indexer_id=ext.{{ ext.ext_service_name }}.config.service_id)
+        iregistry.register(ext.service.indexer, indexer_id="{{ vars.ext.alias }}")
     {% endif  %}
 
-{{ vars.api_blueprint|extra_code }}
+{{ vars.app_blueprint.extra_code }}
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/app_views.py.jinja2` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/api_views.py.jinja2`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from flask import Blueprint
 
-def {{ vars.app_blueprint.function|base_name }}(app):
-    blueprint = Blueprint("{{ vars.app_blueprint.alias }}_app", __name__, url_prefix="{{ vars.resource_config.base_url }}")
-    blueprint.record_once(init_{{ vars.app_blueprint.function|base_name }})
+def {{ vars.api_blueprint.function|base_name }}(app):
+    """Create {{ vars.record.class|base_name }} blueprint."""
+    blueprint = app.extensions["{{ vars.ext.alias }}"].resource.as_blueprint()
+    blueprint.record_once(init_{{ vars.api_blueprint.function|base_name }})
 
     #calls record_once for all other functions starting with "init_addons_"
     #https://stackoverflow.com/questions/58785162/how-can-i-call-function-with-string-value-that-equals-to-function-name
     funcs = globals()
     funcs = [v for k, v in funcs.items() if k.startswith("init_addons_{{ vars.module.suffix_snake }}") and callable(v)]
     for func in funcs:
         blueprint.record_once(func)
 
     return blueprint
 
-def init_{{ vars.app_blueprint.function|base_name }}(state):
+def init_{{ vars.api_blueprint.function|base_name }}(state):
     """Init app."""
     app = state.app
     ext = app.extensions["{{ vars.ext.alias }}"]
 
     {%  if not vars.service_config.skip %}
     # register service
     sregistry = app.extensions["invenio-records-resources"].registry
-    sregistry.register(ext.{{ ext.ext_service_name }}, service_id=ext.{{ ext.ext_service_name }}.config.service_id)
+    sregistry.register(ext.service, service_id="{{ vars.service_config.service_id }}")
     {% endif  %}
 
-    {%  if not vars.mapping.skip %}
+    {%  if not vars.mapping_settings.skip %}
     # Register indexer
-    if hasattr(ext.{{ ext.ext_service_name }}, "indexer"):
+    if hasattr(ext.service, "indexer"):
         iregistry = app.extensions["invenio-indexer"].registry
-        iregistry.register(ext.{{ ext.ext_service_name }}.indexer, indexer_id=ext.{{ ext.ext_service_name }}.config.service_id)
+        iregistry.register(ext.service.indexer, indexer_id="{{ vars.ext.alias }}")
     {% endif  %}
 
-{{ vars.app_blueprint|extra_code }}
+{{ vars.api_blueprint.extra_code }}
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/config.py.jinja2` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/config.py.jinja2`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-{{ vars.config|imports }}
-
-{{ vars.service_config.class|imports }}
-{{ vars.service.class|imports }}
-{{ vars.resource_config.class|imports }}
-{{ vars.resource.class|imports }}
+{{ vars.service_config|generate_import }}
+{{ vars.service|generate_import }}
+{{ vars.resource_config|generate_import }}
+{{ vars.resource|generate_import }}
 
 {% if not vars.resource_config.skip %}
 {{ vars.resource_config.config_key }} = {{ vars.resource_config.class|base_name }}
 {% endif  %}
 
 {% if not vars.resource.skip %}
 {{ vars.resource.config_key }} = {{ vars.resource.class|base_name }}
@@ -16,8 +14,8 @@
 {% if not vars.service_config.skip %}
 {{ vars.service_config.config_key }} = {{ vars.service_config.class|base_name }}
 {% endif  %}
 {% if not vars.service.skip %}
 {{ vars.service.config_key }} = {{ vars.service.class|base_name }}
 {% endif  %}
 
-{{ vars.config|extra_code }}
+{{ vars.config.extra_code }}
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/record.py.jinja2` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/record.py.jinja2`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,33 @@
 from invenio_records.systemfields import ConstantField
 from invenio_records_resources.records.systemfields import IndexField
 
-{{ vars.pid.provider_class|imports }}
-{{ vars.pid.field_class|imports }}
-{{ vars.pid.context_class|imports }}
-
-{{ vars.record_metadata.class|imports }}
-{{ vars.record_dumper.class|imports }}
-{{ vars.record|imports }}
-
-{% for extra_field_value in vars.record.fields.values() %}
-{{ extra_field_value|code_imports }}
-{% endfor %}
-
+{{ vars.pid|generate_import('provider-class') }}
+{{ vars.pid.imports|generate_import }}
+{{ vars.record_metadata|generate_import }}
+{{ vars.record_dumper|generate_import }}
+{{ vars.record.imports|generate_import }}
 
 class {{ vars.record|class_header }}:
 {% if not vars.record_metadata.skip %}
     model_cls = {{ vars.record_metadata.class|base_name }}
 {% endif %}
 {% if not vars.json_schema_settings.skip %}
     schema = ConstantField("$schema", "{{ settings.schema_server }}{{ vars.json_schema_settings.name }}")
 {% endif %}
-{% if not vars.mapping.skip %}
-    index = IndexField("{{ vars.mapping.index }}", {% if vars.mapping.index_field_args %}
-                {{ vars.mapping.index_field_args|generate_list }}
-            {% endif %})
+{% if not vars.mapping_settings.skip %}
+    index = IndexField("{{ vars.mapping_settings.index }}")
 {% endif %}
 {% if not vars.pid.skip %}
-    pid = {{ vars.pid.field_class|base_name }}(
+    pid = {{ vars.pid.field_class }}(
         provider={{ vars.pid.provider_class|base_name }},
-        context_cls={{ vars.pid.context_class|base_name }}{% if vars.pid.field_args %},
+        context_cls={{ vars.pid.context_class }}{% if vars.pid.field_args %},
         {{ vars.pid.field_args|generate_list }}
     {% endif %}
     )
 {% endif %}
 {% if not vars.record_dumper.skip %}
-    dumper = {{ vars.record_dumper.class|base_name }}()
+    dumper_extensions = [ {{ vars.record.dumper_extensions|generate_list }} ]
+    dumper = {{ vars.record_dumper.class|base_name }}(extensions=dumper_extensions)
 {% endif %}
-{% for extra_field_name, extra_field_value in vars.record.fields.items() %}
-    {{ extra_field_name }} = {{ extra_field_value|extra_code }}
-{% endfor %}
 
-{{ vars.record|extra_code }}
+{{ vars.record.extra_code }}
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/invenio/templates/resource_config.py.jinja2` & `oarepo-model-builder-4.0.9/oarepo_model_builder/invenio/templates/resource_config.py.jinja2`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib_metadata
 from flask_resources import ResponseHandler
 
-{{ vars.json_serializer.class|imports }}
-{{ vars.resource_config|imports }}
+{{ vars.json_serializer.class|generate_import }}
+{{ vars.resource_config.imports|generate_import }}
 
 class {{ vars.resource_config|class_header }}:
     """{{ vars.record.class|base_name }} resource config."""
 
     blueprint_name = '{{ vars.api_blueprint.alias }}'
     url_prefix = '{{ vars.resource_config.base_url }}'
 
@@ -17,8 +17,8 @@
             entrypoint_response_handlers.update(x.load())
         return {
             "application/vnd.inveniordm.v1+json": ResponseHandler({{vars.json_serializer.class|base_name}}()),
             **super().response_handlers,
             **entrypoint_response_handlers
         }
 
-{{ vars.resource_config|extra_code }}
+{{ vars.resource_config.extra_code }}
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/loaders/__init__.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/merger.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,17 @@
         for fn in source.glob("**/*"):
             if not fn.is_file():
                 continue
             relative_fn = fn.relative_to(source)
             merge_file(
                 fn,
                 destination.joinpath(relative_fn),
-                (
-                    result.joinpath(relative_fn)
-                    if result
-                    else destination.joinpath(relative_fn)
-                ),
+                result.joinpath(relative_fn)
+                if result
+                else destination.joinpath(relative_fn),
                 destination_first,
                 overwrite,
             )
 
 
 def merge_file(
     source: Path,
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/cfg.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/diff.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/diff.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/json.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/json.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/json_stack.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/json_stack.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/python.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/python.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,18 @@
 
 from oarepo_model_builder.outputs import OutputBase
 from oarepo_model_builder.templates import templates
 from oarepo_model_builder.utils.cst import PythonContext, merge
 from oarepo_model_builder.utils.jinja import (
     base_name,
     class_header,
-    generate_dict,
-    generate_extra_code,
-    generate_extra_code_imports,
     generate_import,
     generate_list,
     in_different_package,
     package_name,
-    repr_filter,
 )
 from oarepo_model_builder.utils.verbose import log
 
 
 class PythonOutput(OutputBase):
     TYPE = "python"
     cst = None
@@ -111,28 +107,23 @@
             print("====")
             print(self.original_data)
             raise
 
     @staticmethod
     def register_default_filters(env):
         env.filters["generate_import"] = generate_import
-        env.filters["imports"] = generate_import
-        env.filters["extra_code"] = generate_extra_code
-        env.filters["code_imports"] = generate_extra_code_imports
         env.filters["generate_list"] = generate_list
-        env.filters["generate_dict"] = generate_dict
         env.filters["class_header"] = class_header
         env.filters["package_name"] = package_name
         env.filters["base_name"] = pass_context(lambda context, value: base_name(value))
         env.tests["in_different_package"] = pass_context(
             lambda context, value: in_different_package(
                 context["current_module"], value
             )
         )
-        env.filters["repr"] = repr_filter
 
 
 class AttrDict(dict):
     def __getattr__(self, item):
         try:
             return self[item]
         except KeyError as e:
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/text.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/text.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/toml.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/toml.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/outputs/yaml.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/schema.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,27 +10,24 @@
 from .utils.deepmerge import deepmerge
 from .validation import validate_model
 
 
 class ModelSchema:
     USE_KEYWORD = "use"
     REF_KEYWORD = "$ref"
-    EXTEND_KEYWORD = "extend"
 
     def __init__(
         self,
         file_path,
         content=None,
         included_models: Dict[str, Callable] = None,
         merged_models: List[Union[str, Path]] = None,
         loaders=None,
         validate=True,
         source_locations=None,
-        reference_processors=None,
-        post_reference_processors=None,
     ):
         """
         Creates and parses model schema
 
         :param file_paths: list of paths on the filesystem to the model schema files. The content of these files will be merged before the processing.
         :param content:   if set, use this content, otherwise load the file_path
         :param included_models: a dictionary of file_id to callable that returns included json.
@@ -39,67 +36,33 @@
 
         self.file_path = file_path
         self.included_schemas = included_models or {}
         self.loaders = loaders
         self.source_locations = [*(source_locations or [])]
         self.source_locations.append(os.path.abspath(os.curdir))
         self.source_locations.append(os.path.dirname(os.path.abspath(self.file_path)))
-        self._reference_processors = deepmerge(
-            {
-                self.REF_KEYWORD: [],
-                self.USE_KEYWORD: [],
-                self.EXTEND_KEYWORD: [],
-            },
-            reference_processors or {},
-        )
-        self._post_reference_processors = deepmerge(
-            {
-                self.REF_KEYWORD: [],
-                self.USE_KEYWORD: [],
-                self.EXTEND_KEYWORD: [],
-            },
-            post_reference_processors or {},
-        )
 
         if content is not None:
             self.schema = content
         else:
             self.schema = copy.deepcopy(self._load(file_path))
             for fp in merged_models or []:
                 self.schema = deepmerge(self.schema, copy.deepcopy(self._load(fp)))
 
-        reference_count = 1
-        while reference_count:
-            reference_count = self._resolve_references(
-                self.schema,
-                [],
-                {
-                    self.REF_KEYWORD,
-                    self.USE_KEYWORD,
-                },
-            )
-            reference_count += self._resolve_references(
-                self.schema,
-                [],
-                {
-                    self.EXTEND_KEYWORD,
-                },
-            )
+        self._resolve_references(self.schema, [])
 
         self._resolve_shortcuts(self.schema)
 
         # any star keys should be kept
         use_star_keys(self.schema)
 
         self.schema.setdefault("settings", {})
 
         self._sections = {}
 
-        self._strip_ignored_elements()
-
         if validate:
             validate_model(self)
 
     @property
     def settings(self):
         return self.schema.get("settings", {})
 
@@ -197,81 +160,45 @@
         if isinstance(element, dict):
             for v in element.values():
                 self._resolve_shortcuts(v)
         elif isinstance(element, list):
             for v in element:
                 self._resolve_shortcuts(v)
 
-    def _resolve_references(self, element, stack, only_keys):
-        resolved_count = 0
+    def _resolve_references(self, element, stack):
         if isinstance(element, dict):
-            # find a reference and if there is one, resolve it
-            modified = True
-            while modified:
-                modified = False
-                for key in list(element.keys()):
-                    if key not in only_keys:
-                        continue
-                    resolved_count += self._resolve_reference_key(
-                        element, key, stack, only_keys
-                    )
-                    # it is possible that the reference introduced another reference,
-                    # so try it once again
-                    modified = True
-
+            if self.USE_KEYWORD in element or self.REF_KEYWORD in element:
+                for key in element:
+                    if key in (self.USE_KEYWORD, self.REF_KEYWORD):
+                        break
+                included_name = element[key]
+
+                # if it is a dictionary, then probably it is a name of a property,
+                # so keep it
+                if isinstance(included_name, dict):
+                    return self._resolve_references(element, stack)
+
+                element.pop(self.USE_KEYWORD, None)
+                element.pop(self.REF_KEYWORD, None)
+
+                if not isinstance(included_name, list):
+                    included_name = [included_name]
+                for name in included_name:
+                    if not name:
+                        raise IncludedFileNotFoundException(
+                            f"No file for use at path {'/'.join(stack)}"
+                        )
+                    included_data = self._load_included_file(name)
+                    deepmerge(element, included_data, [], listmerge="keep")
+                return self._resolve_references(element, stack)
             for k, v in element.items():
-                resolved_count += self._resolve_references(v, stack + [k], only_keys)
-
+                self._resolve_references(v, stack + [k])
         elif isinstance(element, list):
             for v in element:
-                resolved_count += self._resolve_references(v, stack, only_keys)
-        return resolved_count
-
-    def _resolve_reference_key(self, element, key, stack, only_keys):
-        included_name = element[key]
-
-        # if it is a dictionary, then probably it is a name of a property,
-        # so keep it
-        if isinstance(included_name, dict):
-            return self._resolve_references(element, stack, only_keys)
-
-        # not a dict, so pop the key
-        element.pop(key)
-
-        if not isinstance(included_name, list):
-            included_name = [included_name]
-        for name in included_name:
-            if not name:
-                raise IncludedFileNotFoundException(
-                    f"No file for use at path {'/'.join(stack)}"
-                )
-            self._load_and_merge_reference(element, key, name, stack)
-        # it was resolved => return number of resolved references (1)
-        return 1
-
-    def _load_and_merge_reference(self, element, key, name, stack):
-        included_data = self._load_included_file(name)
-
-        context = {}
-        for rp in self._reference_processors[key]:
-            included_data = rp(
-                included_data,
-                element=element,
-                key=key,
-                name=name,
-                context=context,
-            )
-        deepmerge(element, included_data, [], listmerge="keep")
-        for rp in self._post_reference_processors[key]:
-            rp(
-                element=element,
-                key=key,
-                name=name,
-                context=context,
-            )
+                self._resolve_references(v, stack)
 
     @property
     def abs_path(self):
         return Path(self.file_path).absolute()
 
     def get_schema_section(self, profile, section, prepare_context=None):
         if not isinstance(section, (tuple, list)):
@@ -302,39 +229,14 @@
         prepare_context.setdefault("profile", profile)
         prepare_context.setdefault("profile_module", profile + "s")
         prepare_context.setdefault("profile_upper", profile.upper())
         parsed_section.prepare(prepare_context)
         self._sections[key] = parsed_section
         return parsed_section
 
-    def _strip_ignored_elements(self):
-        extension_elements = self.schema.get("settings", {}).get(
-            "extension-elements", []
-        )
-        extension_elements = [
-            *extension_elements,
-            *[f"^{x}" for x in extension_elements],
-        ]
-        if not extension_elements:
-            return
-
-        def remove_extension_elements(d):
-            if isinstance(d, dict):
-                for k, v in list(d.items()):
-                    if k in extension_elements:
-                        del d[k]
-                    elif isinstance(v, (dict, list)):
-                        remove_extension_elements(v)
-            elif isinstance(d, list):
-                for v in d:
-                    if isinstance(v, (dict, list)):
-                        remove_extension_elements(v)
-
-        remove_extension_elements(self.schema)
-
 
 def resolve_id(json, element_id):
     if isinstance(json, dict):
         if "$id" in json and json["$id"] == element_id:
             return json
         continue_with = json.values()
     elif isinstance(json, (tuple, list)):
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/templates/__init__.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/call.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/call.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/collections.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/collections.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/common.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/common.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/indented_nodes.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/indented_nodes.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/mergers.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/mergers.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/cst/simple_nodes.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/cst/simple_nodes.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/deepmerge.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/deepmerge.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,45 @@
 import copy
-from typing import Union
 
 
-def deepmerge(
-    target,
-    source,
-    stack=None,
-    listmerge: Union[str, callable] = "overwrite",
-    dictmerge=None,
-):
+def deepmerge(target, source, stack=None, listmerge="overwrite"):
     if stack is None:
         stack = []
 
     if isinstance(target, dict):
         if source is not None:
             if not isinstance(source, dict):
                 raise AttributeError(
                     f"Incompatible source and target on path {stack}: source {source}, target {target}"
                 )
-            if dictmerge:
-                merged = dictmerge(target, source, stack)
-            else:
-                merged = None
-            if merged is None:
-                for k, v in source.items():
-                    if k not in target:
-                        target[k] = source[k]
-                    else:
-                        target[k] = deepmerge(
-                            target[k],
-                            source[k],
-                            stack + [k],
-                            listmerge=listmerge,
-                            dictmerge=dictmerge,
-                        )
+            for k, v in source.items():
+                if k not in target:
+                    target[k] = source[k]
+                else:
+                    target[k] = deepmerge(
+                        target[k], source[k], stack + [k], listmerge=listmerge
+                    )
     elif isinstance(target, list):
         if source is not None:
             if not isinstance(source, list):
                 raise AttributeError(
                     f"Incompatible source and target on path {stack}: source {source}, target {target}"
                 )
             if listmerge == "overwrite":
                 for idx in range(min(len(source), len(target))):
                     target[idx] = deepmerge(
-                        target[idx],
-                        source[idx],
-                        stack + [idx],
-                        listmerge=listmerge,
-                        dictmerge=dictmerge,
+                        target[idx], source[idx], stack + [idx], listmerge=listmerge
                     )
                 for idx in range(len(target), len(source)):
                     target.append(source[idx])
             elif listmerge == "extend":
                 target.extend(source)
             elif listmerge == "keep":
                 if len(source) > len(target):
                     target.extend(source[len(target) :])
-            elif callable(listmerge):
-                listmerge(target, source, stack)
             else:
                 raise AttributeError(
                     'listmerge must be one of "overwrite", "extend" or "keep"'
                 )
     elif target is None:
         return copy.deepcopy(source)
     return target
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/facet_helpers.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/facet_helpers.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/properties.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/properties.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/utils/verbose.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/utils/verbose.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/validation/__init__.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/validation/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,11 +24,10 @@
         model.schema = model_validator.validate(model.schema)
         return True
     except ValidationError as e:
         msg = []
         for err, path in flatten_errors(e.messages_dict, ""):
             if path.endswith("._schema") and err == "Unknown field.":
                 continue
-            path = path.replace(".value.", ".")
             msg.append(f"{path}: {err}")
         msg = "\n    ".join(msg)
         raise InvalidModelException(f"Invalid model: \n    {msg}")
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/validation/extensibility.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/validation/extensibility.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/validation/model_validation.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/validation/model_validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import marshmallow as ma
 
 from .extensibility import ExtensibleSchema
-from .plugins import PluginsSchema
 
 
 def get_model_schema():
     from ..datatypes.model import ModelDataType
 
     return ModelDataType.validator()
 
@@ -33,46 +32,24 @@
 class SettingsOpenSearchSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
     version = ma.fields.String(load_default="os-v2")
 
 
-class MarshmallowSettingsSchema(ma.Schema):
-    schema_base_class = ma.fields.String(
-        attribute="schema-base-class",
-        data_key="schema-base-class",
-        default="oarepo_runtime.services.schema.marshmallow.DictOnlySchema",
-    )
-    ui_schema_base_class = ma.fields.String(
-        attribute="ui-schema-base-class",
-        data_key="ui-schema-base-class",
-        default="oarepo_runtime.services.schema.marshmallow.DictOnlySchema",
-    )
-
-
 class SettingsSchema(ma.Schema):
     python = ma.fields.Nested(ExtensibleSchema("settings.python", SettingsPythonSchema))
     opensearch = ma.fields.Nested(
         ExtensibleSchema("settings.opensearch", SettingsOpenSearchSchema)
     )
     schema_server = ma.fields.String(
         attribute="schema-server", data_key="schema-server", load_default="local://"
     )
-    extension_elements = ma.fields.List(
-        ma.fields.String(),
-        attribute="extension-elements",
-        data_key="extension-elements",
-    )
-    marshmallow = ma.fields.Nested(
-        MarshmallowSettingsSchema,
-        load_default=lambda: {
-            "schema-base-class": "oarepo_runtime.services.schema.marshmallow.DictOnlySchema",
-            "ui-schema-base-class": "oarepo_runtime.services.schema.marshmallow.DictOnlySchema",
-        },
+    oarepo_version = ma.fields.String(
+        attribute="oarepo-version", data_key="oarepo-version", load_default="11"
     )
 
     class Meta:
         unknown = ma.RAISE
 
 
 class ModelFileSchema(ma.Schema):
@@ -99,19 +76,14 @@
     )
     dev_dependencies = ma.fields.Dict(
         ma.fields.String(),
         ma.fields.String(),
         attribute="dev-dependencies",
         data_key="dev-dependencies",
     )
-    plugins = ma.fields.Nested(
-        ExtensibleSchema("plugins", PluginsSchema),
-        metadata={"doc": "Plugins to load, enable, disable"},
-    )
-    profiles = ma.fields.List(ma.fields.String())
 
 
 class ModelValidator:
     def validate(self, data):
         complete_model_schema = ExtensibleSchema("model_file", ModelFileSchema)
         validator = complete_model_schema()
         return validator.load(data)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/validation/plugins.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/datatypes/components/model/plugins.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 import marshmallow as ma
 
+from oarepo_model_builder.datatypes import DataTypeComponent, ModelDataType
+
 
 class PluginEnableDisableField(ma.fields.List):
     def deserialize(self, value, attr, data, **kwargs):
         if value == "__all__":
             return value
         return super().deserialize(value, attr, data, **kwargs)
 
 
 class PluginSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
+    packages = ma.fields.List(ma.fields.String())
     include = ma.fields.List(ma.fields.String())
     enable = PluginEnableDisableField(ma.fields.String())
     disable = PluginEnableDisableField(ma.fields.String())
 
 
 class PluginsSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
-    packages = ma.fields.List(ma.fields.String())
     output = ma.fields.Nested(PluginSchema)
     builder = ma.fields.Nested(PluginSchema)
+
+
+class PluginsModelComponent(DataTypeComponent):
+    eligible_datatypes = [ModelDataType]
+
+    class ModelSchema(ma.Schema):
+        plugins = ma.fields.Nested(PluginsSchema)
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder/validation/utils.py` & `oarepo-model-builder-4.0.9/oarepo_model_builder/validation/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder.egg-info/SOURCES.txt` & `oarepo-model-builder-4.0.9/oarepo_model_builder.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 oarepo_model_builder/__init__.py
 oarepo_model_builder/builder.py
 oarepo_model_builder/cli.py
@@ -16,14 +15,15 @@
 oarepo_model_builder.egg-info/PKG-INFO
 oarepo_model_builder.egg-info/SOURCES.txt
 oarepo_model_builder.egg-info/dependency_links.txt
 oarepo_model_builder.egg-info/entry_points.txt
 oarepo_model_builder.egg-info/requires.txt
 oarepo_model_builder.egg-info/top_level.txt
 oarepo_model_builder/builders/__init__.py
+oarepo_model_builder/builders/extend.py
 oarepo_model_builder/builders/json_base.py
 oarepo_model_builder/builders/jsonschema.py
 oarepo_model_builder/builders/mapping.py
 oarepo_model_builder/builders/model_saver.py
 oarepo_model_builder/builders/pyproject_toml.py
 oarepo_model_builder/builders/python.py
 oarepo_model_builder/builders/python_structure.py
@@ -49,71 +49,58 @@
 oarepo_model_builder/datatypes/components/facets/field.py
 oarepo_model_builder/datatypes/components/facets/nested.py
 oarepo_model_builder/datatypes/components/facets/object.py
 oarepo_model_builder/datatypes/components/marshmallow/__init__.py
 oarepo_model_builder/datatypes/components/marshmallow/array.py
 oarepo_model_builder/datatypes/components/marshmallow/field.py
 oarepo_model_builder/datatypes/components/marshmallow/graph.py
-oarepo_model_builder/datatypes/components/marshmallow/numbers.py
 oarepo_model_builder/datatypes/components/marshmallow/object.py
-oarepo_model_builder/datatypes/components/marshmallow/strings.py
 oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
 oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
 oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
 oarepo_model_builder/datatypes/components/model/__init__.py
 oarepo_model_builder/datatypes/components/model/app.py
 oarepo_model_builder/datatypes/components/model/blueprints.py
 oarepo_model_builder/datatypes/components/model/defaults.py
-oarepo_model_builder/datatypes/components/model/edtf_interval.py
-oarepo_model_builder/datatypes/components/model/ext_resource.py
 oarepo_model_builder/datatypes/components/model/facets.py
 oarepo_model_builder/datatypes/components/model/jsonschema.py
 oarepo_model_builder/datatypes/components/model/mapping.py
 oarepo_model_builder/datatypes/components/model/marshmallow.py
 oarepo_model_builder/datatypes/components/model/model_saver.py
 oarepo_model_builder/datatypes/components/model/permissions.py
 oarepo_model_builder/datatypes/components/model/pid.py
+oarepo_model_builder/datatypes/components/model/plugins.py
 oarepo_model_builder/datatypes/components/model/proxy.py
 oarepo_model_builder/datatypes/components/model/record.py
 oarepo_model_builder/datatypes/components/model/record_dumper.py
-oarepo_model_builder/datatypes/components/model/record_item.py
-oarepo_model_builder/datatypes/components/model/record_list.py
 oarepo_model_builder/datatypes/components/model/record_metadata.py
 oarepo_model_builder/datatypes/components/model/resource.py
 oarepo_model_builder/datatypes/components/model/sample.py
 oarepo_model_builder/datatypes/components/model/search_options.py
 oarepo_model_builder/datatypes/components/model/service.py
-oarepo_model_builder/datatypes/components/model/sort.py
 oarepo_model_builder/datatypes/components/model/ui.py
 oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
 oarepo_model_builder/datatypes/components/model/utils.py
-oarepo_model_builder/datatypes/components/sort/__init__.py
-oarepo_model_builder/datatypes/components/sort/field.py
-oarepo_model_builder/datatypes/components/sort/object.py
 oarepo_model_builder/datatypes/containers/__init__.py
 oarepo_model_builder/datatypes/containers/array.py
 oarepo_model_builder/datatypes/containers/flatten.py
 oarepo_model_builder/datatypes/containers/nested.py
 oarepo_model_builder/datatypes/containers/object.py
 oarepo_model_builder/invenio/__init__.py
-oarepo_model_builder/invenio/edtf_interval_dumper.py
 oarepo_model_builder/invenio/invenio_api_views.py
 oarepo_model_builder/invenio/invenio_app_views.py
 oarepo_model_builder/invenio/invenio_base.py
 oarepo_model_builder/invenio/invenio_config.py
 oarepo_model_builder/invenio/invenio_ext.py
-oarepo_model_builder/invenio/invenio_ext_resource.py
 oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
 oarepo_model_builder/invenio/invenio_proxies.py
 oarepo_model_builder/invenio/invenio_record.py
 oarepo_model_builder/invenio/invenio_record_dumper.py
 oarepo_model_builder/invenio/invenio_record_facets.py
-oarepo_model_builder/invenio/invenio_record_item.py
 oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
-oarepo_model_builder/invenio/invenio_record_list.py
 oarepo_model_builder/invenio/invenio_record_marshmallow.py
 oarepo_model_builder/invenio/invenio_record_metadata.py
 oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_permissions.py
 oarepo_model_builder/invenio/invenio_record_pid_provider.py
 oarepo_model_builder/invenio/invenio_record_resource.py
@@ -127,70 +114,100 @@
 oarepo_model_builder/invenio/invenio_record_ui_serializer.py
 oarepo_model_builder/invenio/invenio_script_sample_data.py
 oarepo_model_builder/invenio/invenio_version.py
 oarepo_model_builder/invenio/templates/__init__.py
 oarepo_model_builder/invenio/templates/api_views.py.jinja2
 oarepo_model_builder/invenio/templates/app_views.py.jinja2
 oarepo_model_builder/invenio/templates/config.py.jinja2
-oarepo_model_builder/invenio/templates/edtf_interval_record_dumper.py.jinja2
 oarepo_model_builder/invenio/templates/ext.py.jinja2
-oarepo_model_builder/invenio/templates/ext_resource.py.jinja2
+oarepo_model_builder/invenio/templates/imports.py.jinja2
 oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
 oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
 oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
 oarepo_model_builder/invenio/templates/permissions.py.jinja2
 oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
 oarepo_model_builder/invenio/templates/proxies.py.jinja2
 oarepo_model_builder/invenio/templates/record.py.jinja2
 oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
-oarepo_model_builder/invenio/templates/record_item.py.jinja2
-oarepo_model_builder/invenio/templates/record_list.py.jinja2
 oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
 oarepo_model_builder/invenio/templates/resource.py.jinja2
 oarepo_model_builder/invenio/templates/resource_config.py.jinja2
 oarepo_model_builder/invenio/templates/service.py.jinja2
 oarepo_model_builder/invenio/templates/service_config.py.jinja2
 oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
 oarepo_model_builder/invenio/templates/version.py.jinja2
 oarepo_model_builder/loaders/__init__.py
-oarepo_model_builder/loaders/extend.py
 oarepo_model_builder/outputs/__init__.py
 oarepo_model_builder/outputs/cfg.py
 oarepo_model_builder/outputs/diff.py
 oarepo_model_builder/outputs/json.py
 oarepo_model_builder/outputs/json_stack.py
 oarepo_model_builder/outputs/jsonschema.py
 oarepo_model_builder/outputs/mapping.py
 oarepo_model_builder/outputs/python.py
 oarepo_model_builder/outputs/text.py
 oarepo_model_builder/outputs/toml.py
 oarepo_model_builder/outputs/yaml.py
 oarepo_model_builder/profiles/__init__.py
+oarepo_model_builder/profiles/extend.py
 oarepo_model_builder/profiles/record.py
 oarepo_model_builder/settings/__init__.py
 oarepo_model_builder/settings/opensearch.json
 oarepo_model_builder/settings/python.json
 oarepo_model_builder/templates/__init__.py
 oarepo_model_builder/utils/__init__.py
 oarepo_model_builder/utils/absolute_class.py
 oarepo_model_builder/utils/camelcase.py
 oarepo_model_builder/utils/deepmerge.py
 oarepo_model_builder/utils/dict.py
 oarepo_model_builder/utils/facet_helpers.py
 oarepo_model_builder/utils/import_class.py
 oarepo_model_builder/utils/jinja.py
-oarepo_model_builder/utils/links.py
 oarepo_model_builder/utils/properties.py
 oarepo_model_builder/utils/python_name.py
 oarepo_model_builder/utils/verbose.py
 oarepo_model_builder/utils/cst/__init__.py
 oarepo_model_builder/utils/cst/call.py
 oarepo_model_builder/utils/cst/collections.py
 oarepo_model_builder/utils/cst/common.py
 oarepo_model_builder/utils/cst/indented_nodes.py
 oarepo_model_builder/utils/cst/mergers.py
 oarepo_model_builder/utils/cst/simple_nodes.py
 oarepo_model_builder/validation/__init__.py
 oarepo_model_builder/validation/extensibility.py
 oarepo_model_builder/validation/model_validation.py
-oarepo_model_builder/validation/plugins.py
-oarepo_model_builder/validation/utils.py
+oarepo_model_builder/validation/utils.py
+tests/__init__.py
+tests/conftest.py
+tests/faker_constant.py
+tests/multilang.py
+tests/test_builder.py
+tests/test_builder_from_entrypoints.py
+tests/test_cfg_builders.py
+tests/test_datatype_prepare.py
+tests/test_datatype_validator.py
+tests/test_dependencies.py
+tests/test_empty_metadata.py
+tests/test_extend.py
+tests/test_facets.py
+tests/test_fulltext_keyword.py
+tests/test_jsonchema_builder.py
+tests/test_loading.py
+tests/test_mapping_builder.py
+tests/test_marshmallow_builder.py
+tests/test_marshmallow_ui_builder.py
+tests/test_merge.py
+tests/test_model_saver.py
+tests/test_overwrite.py
+tests/test_pid_provider.py
+tests/test_plugin_configuration.py
+tests/test_python_mergers.py
+tests/test_raw.py
+tests/test_sample_builder.py
+tests/test_schema_props.py
+tests/test_search_options.py
+tests/test_shortcuts.py
+tests/test_simple_builders.py
+tests/test_template_registry.py
+tests/test_type_shortcuts.py
+tests/test_validation.py
+tests/utils.py
```

### Comparing `oarepo_model_builder-4.0.84/oarepo_model_builder.egg-info/entry_points.txt` & `oarepo-model-builder-4.0.9/oarepo_model_builder.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,91 +19,79 @@
 plugins = oarepo_model_builder.validation.schemas:plugins.json5
 settings = oarepo_model_builder.validation.schemas:settings.json5
 sort = oarepo_model_builder.validation.schemas:sort.json5
 
 [oarepo.models]
 invenio = oarepo_model_builder.builtin_models:invenio.json
 
-[oarepo_model_builder.builders.base]
+[oarepo_model_builder.builders.extend]
+1000-model = oarepo_model_builder.builders.extend:ExtendBuilder
+
+[oarepo_model_builder.builders.record]
+0020-jsonschema = oarepo_model_builder.builders.jsonschema:JSONSchemaBuilder
+0030-mapping = oarepo_model_builder.builders.mapping:MappingBuilder
 0050-setup-cfg = oarepo_model_builder.builders.setup_cfg:SetupCfgBuilder
 0060-setup-py = oarepo_model_builder.builders.setup_py:SetupPyBuilder
 0070-pyproject-toml = oarepo_model_builder.builders.pyproject_toml:PyprojectTOMLBuilder
 0100-python_structure = oarepo_model_builder.builders.python_structure:PythonStructureBuilder
+0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 0110-invenio_record = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 0120-invenio_record_metadata = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 0130-invenio_record_marshmallow = oarepo_model_builder.invenio.invenio_record_marshmallow:InvenioRecordMarshmallowBuilder
 0140-invenio_record_ui_marshmallow = oarepo_model_builder.invenio.invenio_record_ui_marshmallow:InvenioRecordUIMarshmallowBuilder
+0200-invenio_record_permissions = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
+0300-invenio_record_search_facets = oarepo_model_builder.invenio.invenio_record_facets:InvenioRecordSearchFacetsBuilder
+0305-invenio_record_search_options = oarepo_model_builder.invenio.invenio_record_search_options:InvenioRecordSearchOptionsBuilder
 0310-invenio_record_service_config = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 0320-invenio_record_service = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
+0340-invenio_record_dumper = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 0400-invenio_record_resource_config = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
 0410-invenio_record_resource = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
 0420-invenio_api_views = oarepo_model_builder.invenio.invenio_api_views:InvenioAPIViewsBuilder
 0421-invenio_app_views = oarepo_model_builder.invenio.invenio_app_views:InvenioAPPViewsBuilder
 0430-ui_serializer = oarepo_model_builder.invenio.invenio_record_ui_serializer:InvenioRecordUISerializerBuilder
 0500-invenio_config = oarepo_model_builder.invenio.invenio_config:InvenioConfigBuilder
 0600-invenio_ext = oarepo_model_builder.invenio.invenio_ext:InvenioExtBuilder
-0605-invenio_ext_resource = oarepo_model_builder.invenio.invenio_ext_resource:InvenioExtResourceBuilder
 0610-invenio_ext_setup_cfg = oarepo_model_builder.invenio.invenio_ext_setup_cfg:InvenioExtSetupCfgBuilder
-0700-invenio_proxies = oarepo_model_builder.invenio.invenio_proxies:InvenioProxiesBuilder
+0700-invenio_ext = oarepo_model_builder.invenio.invenio_proxies:InvenioProxiesBuilder
+0910-invenio_record_metadata_alembic_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_alembic_setup_cfg:InvenioRecordMetadataAlembicSetupCfgBuilder
 0920-invenio_record_metadata_models_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_models_setup_cfg:InvenioRecordMetadataModelsSetupCfgBuilder
 0930-invenio_resource_setup_cfg = oarepo_model_builder.invenio.invenio_record_resource_setup_cfg:InvenioRecordResourceSetupCfgBuilder
-
-[oarepo_model_builder.builders.record]
-0020-jsonschema = oarepo_model_builder.builders.jsonschema:JSONSchemaBuilder
-0030-mapping = oarepo_model_builder.builders.mapping:MappingBuilder
-0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
-0200-invenio_record_permissions = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
-0300-invenio_record_search_facets = oarepo_model_builder.invenio.invenio_record_facets:InvenioRecordSearchFacetsBuilder
-0305-invenio_record_search_options = oarepo_model_builder.invenio.invenio_record_search_options:InvenioRecordSearchOptionsBuilder
-0340-invenio_record_dumper = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
-0350-edtf_interval-dumper = oarepo_model_builder.invenio.edtf_interval_dumper:EDTFIntervalDumperBuilder
-0910-invenio_record_metadata_alembic_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_alembic_setup_cfg:InvenioRecordMetadataAlembicSetupCfgBuilder
 0940-invenio_record_search_setup_cfg = oarepo_model_builder.invenio.invenio_record_search_setup_cfg:InvenioRecordSearchSetupCfgBuilder
 0950-invenio_record_jsonschemas_setup_cfg = oarepo_model_builder.invenio.invenio_record_jsonschemas_setup_cfg:InvenioRecordJSONSchemasSetupCfgBuilder
 1030-invenio_script_sample_data = oarepo_model_builder.invenio.invenio_script_sample_data:SampleDataBuilder
 1050-invenio_version = oarepo_model_builder.invenio.invenio_version:InvenioVersionBuilder
 2000-model_saver = oarepo_model_builder.builders.model_saver:ModelSaverBuilder
 2010-model_registration = oarepo_model_builder.builders.model_saver:ModelRegistrationBuilder
-2020-invenio_record_item = oarepo_model_builder.invenio.invenio_record_item:InvenioRecordItemBuilder
-2030-invenio_record_list = oarepo_model_builder.invenio.invenio_record_list:InvenioRecordListBuilder
-
-[oarepo_model_builder.builders.record.inherit]
-0100-model = oarepo_model_builder.builders.base
 
 [oarepo_model_builder.datatypes]
 0100-default-datatypes = oarepo_model_builder.datatypes:DEFAULT_DATATYPES
 
 [oarepo_model_builder.datatypes.components]
 0100-default-datatypes = oarepo_model_builder.datatypes.components:DEFAULT_COMPONENTS
 
 [oarepo_model_builder.loaders]
 json = oarepo_model_builder.loaders:json_loader
 json5 = oarepo_model_builder.loaders:json_loader
 yaml = oarepo_model_builder.loaders:yaml_loader
 yml = oarepo_model_builder.loaders:yaml_loader
 
-[oarepo_model_builder.loaders.extend]
-0100-extract_record = oarepo_model_builder.loaders.extend:extract_extended_record
-1000-modify-marshmallow = oarepo_model_builder.loaders.extend:extend_modify_marshmallow
-
-[oarepo_model_builder.loaders.post.extend]
-1000-modify-marshmallow = oarepo_model_builder.loaders.extend:post_extend_modify_marshmallow
-
 [oarepo_model_builder.outputs]
 cfg = oarepo_model_builder.outputs.cfg:CFGOutput
 diff = oarepo_model_builder.outputs.diff:DiffOutput
 json = oarepo_model_builder.outputs.json:JSONOutput
 jsonschema = oarepo_model_builder.outputs.jsonschema:JSONSchemaOutput
 mapping = oarepo_model_builder.outputs.mapping:MappingOutput
 python = oarepo_model_builder.outputs.python:PythonOutput
 text = oarepo_model_builder.outputs.text:TextOutput
 toml = oarepo_model_builder.outputs.toml:TOMLOutput
 yaml = oarepo_model_builder.outputs.yaml:YAMLOutput
 
 [oarepo_model_builder.profiles]
+extend = oarepo_model_builder.profiles.extend:ExtendProfile
 record = oarepo_model_builder.profiles.record:RecordProfile
 
 [oarepo_model_builder.settings]
 1000-python = oarepo_model_builder.settngs:python.json
 2000-opensearch = oarepo_model_builder.settngs:opensearch.json
 
 [oarepo_model_builder.templates]
```

### Comparing `oarepo_model_builder-4.0.84/setup.cfg` & `oarepo-model-builder-4.0.9/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder
-version = 4.0.84
+version = 4.0.9
 description = A utility library that generates OARepo required data model files from a JSON specification file
 authors = Miroslav Bauer <bauer@cesnet.cz>, Miroslav Simek <simeki@vscht.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -27,18 +27,14 @@
 	marshmallow
 	marshmallow-union
 	marshmallow-oneofschema
 	autoflake
 	frozendict
 packages = find:
 
-[options.packages.find]
-exclude = 
-	tests
-
 [options.extras_require]
 devs = 
 	pytest>=7.1.2
 	black
 	isort
 tests = 
 	pytest>=7.1.2
@@ -91,62 +87,54 @@
 	toml  = oarepo_model_builder.outputs.toml:TOMLOutput
 	yaml  = oarepo_model_builder.outputs.yaml:YAMLOutput
 oarepo_model_builder.templates = 
 	99-base_generic_templates  = oarepo_model_builder.builders
 	99-base_invenio_templates  = oarepo_model_builder.invenio
 oarepo_model_builder.profiles = 
 	record = oarepo_model_builder.profiles.record:RecordProfile
-oarepo_model_builder.builders.record.inherit = 
-	0100-model = oarepo_model_builder.builders.base
+	extend = oarepo_model_builder.profiles.extend:ExtendProfile
 oarepo_model_builder.builders.record = 
 	0020-jsonschema  = oarepo_model_builder.builders.jsonschema:JSONSchemaBuilder
 	0030-mapping  = oarepo_model_builder.builders.mapping:MappingBuilder
-	0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
-	0200-invenio_record_permissions  = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
-	0300-invenio_record_search_facets  = oarepo_model_builder.invenio.invenio_record_facets:InvenioRecordSearchFacetsBuilder
-	0305-invenio_record_search_options  = oarepo_model_builder.invenio.invenio_record_search_options:InvenioRecordSearchOptionsBuilder
-	0340-invenio_record_dumper  = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
-	0350-edtf_interval-dumper  = oarepo_model_builder.invenio.edtf_interval_dumper:EDTFIntervalDumperBuilder
-	0910-invenio_record_metadata_alembic_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_alembic_setup_cfg:InvenioRecordMetadataAlembicSetupCfgBuilder
-	0940-invenio_record_search_setup_cfg  = oarepo_model_builder.invenio.invenio_record_search_setup_cfg:InvenioRecordSearchSetupCfgBuilder
-	0950-invenio_record_jsonschemas_setup_cfg = oarepo_model_builder.invenio.invenio_record_jsonschemas_setup_cfg:InvenioRecordJSONSchemasSetupCfgBuilder
-	1030-invenio_script_sample_data  = oarepo_model_builder.invenio.invenio_script_sample_data:SampleDataBuilder
-	1050-invenio_version  = oarepo_model_builder.invenio.invenio_version:InvenioVersionBuilder
-	2000-model_saver  = oarepo_model_builder.builders.model_saver:ModelSaverBuilder
-	2010-model_registration  = oarepo_model_builder.builders.model_saver:ModelRegistrationBuilder
-	2020-invenio_record_item = oarepo_model_builder.invenio.invenio_record_item:InvenioRecordItemBuilder
-	2030-invenio_record_list = oarepo_model_builder.invenio.invenio_record_list:InvenioRecordListBuilder
-oarepo_model_builder.builders.base = 
 	0050-setup-cfg  = oarepo_model_builder.builders.setup_cfg:SetupCfgBuilder
 	0060-setup-py  = oarepo_model_builder.builders.setup_py:SetupPyBuilder
 	0070-pyproject-toml  = oarepo_model_builder.builders.pyproject_toml:PyprojectTOMLBuilder
 	0100-python_structure  = oarepo_model_builder.builders.python_structure:PythonStructureBuilder
+	0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 	0110-invenio_record  = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 	0120-invenio_record_metadata  = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 	0130-invenio_record_marshmallow  = oarepo_model_builder.invenio.invenio_record_marshmallow:InvenioRecordMarshmallowBuilder
 	0140-invenio_record_ui_marshmallow  = oarepo_model_builder.invenio.invenio_record_ui_marshmallow:InvenioRecordUIMarshmallowBuilder
+	0200-invenio_record_permissions  = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
+	0300-invenio_record_search_facets  = oarepo_model_builder.invenio.invenio_record_facets:InvenioRecordSearchFacetsBuilder
+	0305-invenio_record_search_options  = oarepo_model_builder.invenio.invenio_record_search_options:InvenioRecordSearchOptionsBuilder
+	
 	0310-invenio_record_service_config  = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 	0320-invenio_record_service  = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
+	0340-invenio_record_dumper  = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 	0400-invenio_record_resource_config  = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
 	0410-invenio_record_resource  = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
 	0420-invenio_api_views  = oarepo_model_builder.invenio.invenio_api_views:InvenioAPIViewsBuilder
 	0421-invenio_app_views  = oarepo_model_builder.invenio.invenio_app_views:InvenioAPPViewsBuilder
 	0430-ui_serializer  = oarepo_model_builder.invenio.invenio_record_ui_serializer:InvenioRecordUISerializerBuilder
 	0500-invenio_config  = oarepo_model_builder.invenio.invenio_config:InvenioConfigBuilder
 	0600-invenio_ext  = oarepo_model_builder.invenio.invenio_ext:InvenioExtBuilder
-	0605-invenio_ext_resource = oarepo_model_builder.invenio.invenio_ext_resource:InvenioExtResourceBuilder
 	0610-invenio_ext_setup_cfg  = oarepo_model_builder.invenio.invenio_ext_setup_cfg:InvenioExtSetupCfgBuilder
-	0700-invenio_proxies  = oarepo_model_builder.invenio.invenio_proxies:InvenioProxiesBuilder
+	0700-invenio_ext  = oarepo_model_builder.invenio.invenio_proxies:InvenioProxiesBuilder
+	0910-invenio_record_metadata_alembic_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_alembic_setup_cfg:InvenioRecordMetadataAlembicSetupCfgBuilder
 	0920-invenio_record_metadata_models_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_models_setup_cfg:InvenioRecordMetadataModelsSetupCfgBuilder
 	0930-invenio_resource_setup_cfg  = oarepo_model_builder.invenio.invenio_record_resource_setup_cfg:InvenioRecordResourceSetupCfgBuilder
-oarepo_model_builder.loaders.extend = 
-	0100-extract_record = oarepo_model_builder.loaders.extend:extract_extended_record
-	1000-modify-marshmallow = oarepo_model_builder.loaders.extend:extend_modify_marshmallow
-oarepo_model_builder.loaders.post.extend = 
-	1000-modify-marshmallow = oarepo_model_builder.loaders.extend:post_extend_modify_marshmallow
+	0940-invenio_record_search_setup_cfg  = oarepo_model_builder.invenio.invenio_record_search_setup_cfg:InvenioRecordSearchSetupCfgBuilder
+	0950-invenio_record_jsonschemas_setup_cfg = oarepo_model_builder.invenio.invenio_record_jsonschemas_setup_cfg:InvenioRecordJSONSchemasSetupCfgBuilder
+	1030-invenio_script_sample_data  = oarepo_model_builder.invenio.invenio_script_sample_data:SampleDataBuilder
+	1050-invenio_version  = oarepo_model_builder.invenio.invenio_version:InvenioVersionBuilder
+	2000-model_saver  = oarepo_model_builder.builders.model_saver:ModelSaverBuilder
+	2010-model_registration  = oarepo_model_builder.builders.model_saver:ModelRegistrationBuilder
+oarepo_model_builder.builders.extend = 
+	1000-model  = oarepo_model_builder.builders.extend:ExtendBuilder
 oarepo_model_builder.settings = 
 	1000-python  = oarepo_model_builder.settngs:python.json
 	2000-opensearch  = oarepo_model_builder.settngs:opensearch.json
 
 [tool:pytest]
 testpaths = 
 	tests
```

