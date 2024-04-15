# Comparing `tmp/vectice-24.1.9.0.tar.gz` & `tmp/vectice-24.2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-24.1.9.0.tar", last modified: Mon Mar 25 10:18:31 2024, max compression
+gzip compressed data, was "vectice-24.2.1.0.tar", last modified: Mon Apr 15 11:27:31 2024, max compression
```

## Comparing `vectice-24.1.9.0.tar` & `vectice-24.2.1.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.498698 vectice-24.1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-25 10:18:27.000000 vectice-24.1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-25 10:18:31.498698 vectice-24.1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-25 10:18:27.000000 vectice-24.1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-25 10:18:27.000000 vectice-24.1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-25 10:18:31.498698 vectice-24.1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-03-25 10:18:27.000000 vectice-24.1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.450698 vectice-24.1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.458698 vectice-24.1.9.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.466698 vectice-24.1.9.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.474698 vectice-24.1.9.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/json_to_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.474698 vectice-24.1.9.0/src/vectice/autolog/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.474698 vectice-24.1.9.0/src/vectice/autolog/asset_services/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/catboost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/keras_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/lightgbm_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/metric_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/pandas_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/pyspark_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/sklearn_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/asset_services/vectice_asset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/autolog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/autolog_asset_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    25431 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/autolog_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/autolog/model_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.478698 vectice-24.1.9.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/model_exp_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/model_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.482698 vectice-24.1.9.0/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.482698 vectice-24.1.9.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/pyspark_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/no_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/resource/snowflake_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice/services/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/services/iteration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/services/phase_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice/types/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/code_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-25 10:18:27.000000 vectice-24.1.9.0/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:18:31.486698 vectice-24.1.9.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 10:18:31.000000 vectice-24.1.9.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.995369 vectice-24.2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 11:27:27.000000 vectice-24.2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-15 11:27:30.995369 vectice-24.2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 11:27:27.000000 vectice-24.2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-15 11:27:27.000000 vectice-24.2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 11:27:30.995369 vectice-24.2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-15 11:27:27.000000 vectice-24.2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.955368 vectice-24.2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.955368 vectice-24.2.1.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.963368 vectice-24.2.1.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.967368 vectice-24.2.1.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/json_to_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.971368 vectice-24.2.1.0/src/vectice/autolog/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.971368 vectice-24.2.1.0/src/vectice/autolog/asset_services/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/catboost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/keras_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/lightgbm_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/pandas_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/pyspark_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/sklearn_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/vectice_asset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/autolog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/autolog_asset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29286 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/autolog_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/model_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.975369 vectice-24.2.1.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19789 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/model_exp_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/model_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.975369 vectice-24.2.1.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.979369 vectice-24.2.1.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/pyspark_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/no_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/snowflake_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/services/iteration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/services/phase_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/code_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-24.1.9.0/LICENSE` & `vectice-24.2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/PKG-INFO` & `vectice-24.2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.1.9.0
+Version: 24.2.1.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-24.1.9.0/pyproject.toml` & `vectice-24.2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/setup.py` & `vectice-24.2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/__init__.py` & `vectice-24.2.1.0/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/__init__.py` & `vectice-24.2.1.0/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/_auth.py` & `vectice-24.2.1.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/attachment.py` & `vectice-24.2.1.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/client.py` & `vectice-24.2.1.0/src/vectice/api/client.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/gql_api.py` & `vectice-24.2.1.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/gql_dataset.py` & `vectice-24.2.1.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/gql_entity_file.py` & `vectice-24.2.1.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/gql_feature_flag.py` & `vectice-24.2.1.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/gql_metric.py` & `vectice-24.2.1.0/src/vectice/api/gql_metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/gql_model.py` & `vectice-24.2.1.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/gql_organization.py` & `vectice-24.2.1.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/gql_property.py` & `vectice-24.2.1.0/src/vectice/api/gql_property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-24.2.1.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/http_error.py` & `vectice-24.2.1.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/http_error_handlers.py` & `vectice-24.2.1.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/iteration.py` & `vectice-24.2.1.0/src/vectice/api/iteration.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 if TYPE_CHECKING:
     from vectice.api.json.iteration import IterationContextInput, IterationInput, IterationOutput
 
 _logger = logging.getLogger(__name__)
 
 _RETURNS_LIST = """vecticeId
             index
+            name
             status
             owner {
                 id
                 name
             }
             starred
             __typename
             """
 
 _RETURNS_PAGE = PAGINATE_OUTPUT.format(_RETURNS_LIST)
 
 _BASE_RETURNS = """vecticeId
             index
+            name
             status
             starred
             __typename
             """
 _BASE_PARENT = """
             phase {
                     vecticeId
```

### Comparing `vectice-24.1.9.0/src/vectice/api/json/__init__.py` & `vectice-24.2.1.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/artifact_version.py` & `vectice-24.2.1.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/code.py` & `vectice-24.2.1.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/code_version.py` & `vectice-24.2.1.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/dataset_register.py` & `vectice-24.2.1.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/dataset_representation.py` & `vectice-24.2.1.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/dataset_version.py` & `vectice-24.2.1.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/dataset_version_representation.py` & `vectice-24.2.1.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/files_metadata.py` & `vectice-24.2.1.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/iteration.py` & `vectice-24.2.1.0/src/vectice/api/json/iteration.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,14 +145,18 @@
         return str(self["vecticeId"])
 
     @property
     def index(self) -> int:
         return int(self["index"])
 
     @property
+    def name(self) -> str:
+        return str(self["name"])
+
+    @property
     def sections(self) -> PagedResponse[StepOutput]:
         from vectice.api.gql_api import Parser
 
         return Parser().parse_paged_response(self["sections"])
 
     @property
     def steps(self) -> list[StepOutput]:
```

### Comparing `vectice-24.1.9.0/src/vectice/api/json/json_to_class.py` & `vectice-24.2.1.0/src/vectice/api/json/json_to_class.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/last_assets.py` & `vectice-24.2.1.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/metric.py` & `vectice-24.2.1.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/model.py` & `vectice-24.2.1.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/model_register.py` & `vectice-24.2.1.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/model_representation.py` & `vectice-24.2.1.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/model_version.py` & `vectice-24.2.1.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/model_version_representation.py` & `vectice-24.2.1.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/paged_response.py` & `vectice-24.2.1.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/phase.py` & `vectice-24.2.1.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/project.py` & `vectice-24.2.1.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/property.py` & `vectice-24.2.1.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/public_config.py` & `vectice-24.2.1.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/step.py` & `vectice-24.2.1.0/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/user_and_workspace.py` & `vectice-24.2.1.0/src/vectice/api/json/user_and_workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/json/workspace.py` & `vectice-24.2.1.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/phase.py` & `vectice-24.2.1.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/project.py` & `vectice-24.2.1.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/rest_api.py` & `vectice-24.2.1.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/step.py` & `vectice-24.2.1.0/src/vectice/api/step.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/version.py` & `vectice-24.2.1.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/api/workspace.py` & `vectice-24.2.1.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/autolog/asset_services/__init__.py` & `vectice-24.2.1.0/src/vectice/autolog/asset_services/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/autolog/asset_services/catboost_service.py` & `vectice-24.2.1.0/src/vectice/autolog/asset_services/catboost_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/autolog/asset_services/keras_service.py` & `vectice-24.2.1.0/src/vectice/autolog/asset_services/keras_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     from keras.models import Model as KerasModel
 
 
 class AutologKerasService(MetricService):
     def __init__(self, key: str, asset: KerasModel, data: dict):
         self._asset = asset
         self._key = key
+
         super().__init__(cell_data=data)
 
     def get_asset(self):
         model_metrics = self._get_model_metrics(self._cell_data)
         training_metrics = self._get_keras_training_metrics(self._asset)
         return {
             "variable": self._key,
```

### Comparing `vectice-24.1.9.0/src/vectice/autolog/asset_services/lightgbm_service.py` & `vectice-24.2.1.0/src/vectice/autolog/asset_services/lightgbm_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/autolog/asset_services/metric_service.py` & `vectice-24.2.1.0/src/vectice/autolog/asset_services/metric_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/autolog/asset_services/sklearn_service.py` & `vectice-24.2.1.0/src/vectice/autolog/asset_services/sklearn_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/autolog/asset_services/vectice_asset_service.py` & `vectice-24.2.1.0/src/vectice/autolog/asset_services/vectice_asset_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,24 @@
 from typing import TypedDict, TypeVar
 
 from vectice.models.dataset import Dataset
 from vectice.models.model import Model
 from vectice.models.table import Table
 
 VecticeObjectTypes = TypeVar("VecticeObjectTypes", Dataset, Model, Table)
-TVecticeObjects = TypedDict("TVecticeObjects", {"variable": str, "vectice_object": VecticeObjectTypes})
+TVecticeObjects = TypedDict(
+    "TVecticeObjects",
+    {"variable": str, "vectice_object": VecticeObjectTypes},
+)
 VecticeObjectClasses = (Dataset, Model, Table)
 
 
 class AutologVecticeAssetService:
     def __init__(self, key: str, asset: VecticeObjectTypes):
         self._asset = asset
         self._key = key
 
     def get_asset(self):
-        return {"variable": self._key, "vectice_object": self._asset}
+        return {
+            "variable": self._key,
+            "vectice_object": self._asset,
+        }
```

### Comparing `vectice-24.1.9.0/src/vectice/autolog/autolog.py` & `vectice-24.2.1.0/src/vectice/autolog/autolog.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 2.** Supported libraries and environment:**
     Vectice automatically identifies and log assets encapsulated within a specified list of supported libraries and environement mentioned below
 
 NOTE: **Supported libraries and environment**
     - Dataframe: Pandas, Spark.
     - Model: Scikit, Xgboost, Lightgbm, Catboost, Keras.
     - Graphs: Matplotlib, Seaborn, Plotly.
-    - Environments: Colab, Jupyter, Vertex, SageMaker, Databricks and VScode notebook.
+    - Environments: Colab, Jupyter, Vertex, SageMaker, Databricks, Pycharm and VScode notebook.
 
 3.** General behavior:**
     Vectice autolog provides three methods: autolog.config, autolog.notebook, and autolog.cell. These methods are designed to log every asset to Vectice existing as a variable in the notebook's memory. It is important to review the specific behaviors outlined in the documentation for each of these three methods.
 
 NOTE: **IMPORTANT INFORMATION**
     - For GRAPHS, ensure they are saved as files to be automatically logged in the iteration i.e:
         - plt.savefig("my figure.png") (for seaborn or matploltlib)
@@ -44,14 +44,15 @@
 from typing import TYPE_CHECKING
 
 from typing_extensions import TypedDict
 
 if TYPE_CHECKING:
     from IPython.core.interactiveshell import InteractiveShell
 
+    from vectice.connection import Connection
     from vectice.models import Phase
 
 
 class Login(TypedDict):
     phase: Phase | None
 
 
@@ -98,16 +99,47 @@
         "\nFor detailed information, supported libraries and environments please consult the documentation: https://api-docs.vectice.com/reference/vectice/autolog/"
     )
     from vectice.autolog.autolog_class import start_listen
 
     start_listen()
 
 
+def phase_config(phase: str | None = None) -> None:
+    """Update the phase in which autolog is logging assets. (This method will update the configured phase defined in autolog.config).
+
+    If phase is None, the method print the current configured phase.
+
+    NOTE: **Ensure that you have configured the autolog with your Vectice API token before using this method.**
+
+    ```python
+    # After autolog is configured
+    autolog.phase_config(
+        phase = 'PHA-XXX'   # Paste your Phase Id
+    )
+    ```
+
+    Parameters:
+            phase: The ID of the phase in which you wish to autolog your work as an iteration.
+
+    """
+    if LOGIN["phase"] is None:
+        _logger.warning("\nAutolog needs to be configured before using this method. Please run autolog.config() first.")
+    else:
+        if phase is None:
+            _logger.info(
+                f"\nCurrent configured phase name is: `{LOGIN['phase'].name}`"
+                f"\nCurrent configured phase ID is: `{LOGIN['phase'].id}`"
+            )
+            return None
+        else:
+            LOGIN["phase"] = LOGIN["phase"].connection.phase(phase)
+
+
 # Log the whole notebook inside Vectice iteration
-def notebook(note: str | None = None, capture_schema_only: bool = True) -> None:
+def notebook(note: str | None = None, capture_schema_only: bool = True, capture_comments: bool = True) -> None:
     """Automatically log all supported models, dataframes, and graphs from your notebook within the Vectice App as assets.
 
     NOTE: **IMPORTANT INFORMATION**
         Autolog must be configured at the beginning of your notebook to capture all relevant information. Cells executed prior to configuring autolog may not have their assets recorded by the autolog.notebook() method and may need to be run again.
 
     ```python
                                    ...
@@ -116,23 +148,28 @@
     ```
 
     NOTE: **Ensure that the required assets are in memory before calling this method.**
 
     Parameters:
         note: the note or comment to log to your iteration associated with the autolog.notebook
         capture_schema_only: A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes. If set to False, both the schema and column statistics of the dataframes will be captured. Please note that this option may require additional processing time due to the computation of statistics.
-
+        capture_comments: A boolean parameter indicating whether comments should be automatically logged as notes inside Vectice. If set to True, autolog will capture all comments that start with '##'.
     """
     from vectice.autolog.autolog_class import Autolog
 
     # TODO add notebook parsing of content
-    Autolog(LOGIN["phase"], _check_if_notebook(), True, True, note, capture_schema_only)
+    Autolog(LOGIN["phase"], _check_if_notebook(), True, True, note, capture_schema_only, capture_comments)
 
 
-def cell(create_new_iteration: bool = False, note: str | None = None, capture_schema_only: bool = True):
+def cell(
+    create_new_iteration: bool = False,
+    note: str | None = None,
+    capture_schema_only: bool = True,
+    capture_comments: bool = True,
+):
     """Automatically logs all supported models, dataframes, and graphs from a specific notebook cell within the Vectice platform.
 
     This method facilitates the selective logging of assets within a particular notebook cell, allowing users to precisely choose the assets to log to Vectice with an optional control to log assets inside a new iteration.
 
     NOTE: **Ensure that you have configured the autolog with your Vectice API token and the relevant phase ID before using this method.**
 
     ```python
@@ -143,19 +180,40 @@
 
     NOTE: **Place the command at the end of the desired cell to log all assets within that cell.**
 
     Parameters:
         create_new_iteration: If set to False, logging of assets will happen in the last updated iteration. Otherwise, it will create a new iteration for logging the cell's assets.
         note: the note or comment to log to your iteration associated with the autolog.cell
         capture_schema_only: A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes. If set to False, both the schema and column statistics of the dataframes will be captured. Please note that this option may require additional processing time due to the computation of statistics.
+        capture_comments: A boolean parameter indicating whether comments should be automatically logged as notes inside Vectice. If set to True, autolog will capture all comments that start with '##'.
 
     """
     from vectice.autolog.autolog_class import Autolog
 
-    Autolog(LOGIN["phase"], _check_if_notebook(), False, create_new_iteration, note, capture_schema_only)
+    Autolog(
+        LOGIN["phase"], _check_if_notebook(), False, create_new_iteration, note, capture_schema_only, capture_comments
+    )
+
+
+def get_connection() -> Connection:
+    """Get the Connection from autolog.config(...) to interact with the Vectice base Python API.
+
+    NOTE: **Ensure that you have configured the autolog with your Vectice API token and the relevant phase ID before using this method.**
+
+    ```python
+                                   ...
+    #After autolog is configured
+    connect = autolog.get_connection()
+    ```
+    """
+    phase = LOGIN["phase"]
+    if phase:
+        return phase.connection
+
+    raise ConnectionError("Autolog needs to be configured before using this method. Please run autolog.config() first.")
 
 
 def _check_if_notebook() -> InteractiveShell:
     from IPython.core.getipython import get_ipython
 
     ipython = get_ipython()
```

### Comparing `vectice-24.1.9.0/src/vectice/autolog/autolog_asset_factory.py` & `vectice-24.2.1.0/src/vectice/autolog/autolog_asset_factory.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/autolog/autolog_class.py` & `vectice-24.2.1.0/src/vectice/autolog/autolog_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from typing_extensions import TypedDict
 
 from vectice.api.http_error_handlers import VecticeException
 from vectice.autolog.autolog_asset_factory import AssetFactory
 from vectice.autolog.model_library import ModelLibrary
 from vectice.models.dataset import Dataset
 from vectice.models.table import Table
-from vectice.utils.code_parser import VariableVisitor, preprocess_code
+from vectice.utils.code_parser import VariableVisitor, parse_comments, preprocess_code
 
 if TYPE_CHECKING:
     from tempfile import TemporaryDirectory
 
     from catboost.core import CatBoost
     from keras import Model as KerasModel
     from keras.layers import InputLayer
@@ -35,17 +35,28 @@
 
     # Vectice Object types
     from vectice.autolog.asset_services import TVecticeObjects
     from vectice.models import Phase
     from vectice.models.resource.metadata.db_metadata import TableType
 
     ModelTypes = TypeVar("ModelTypes", BaseEstimator, Booster, CatBoost, KerasModel)
-    TModel = TypedDict("TModel", {"variable": str, "model": ModelTypes, "library": ModelLibrary, "metrics": dict})
+    TModel = TypedDict(
+        "TModel",
+        {
+            "variable": str,
+            "model": ModelTypes,
+            "library": ModelLibrary,
+            "metrics": dict,
+        },
+    )
     DataframeTypes = TypeVar("DataframeTypes", SparkDF, DataFrame)
-    TDataset = TypedDict("TDataset", {"variable": str, "dataframe": DataframeTypes, "type": TableType})
+    TDataset = TypedDict(
+        "TDataset",
+        {"variable": str, "dataframe": DataframeTypes, "type": TableType},
+    )
 
 
 try:
     from IPython.core.getipython import get_ipython
     from IPython.core.interactiveshell import InteractiveShell
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
@@ -200,14 +211,15 @@
         self,
         phase: Phase | None,
         ipy: InteractiveShell,
         is_notebook: bool,
         create: bool = True,
         note: str | None = None,
         capture_schema_only: bool = True,
+        capture_comments: bool = True,
     ):
         from vectice.services.phase_service import PhaseService
 
         if phase is None:
             raise ValueError("Login")
 
         if create is True:
@@ -218,52 +230,56 @@
             ).get_active_iteration_or_create(phase)
 
         self._iteration = iteration
         self._iteration_service = iteration._service  # pyright: ignore[reportPrivateUsage]
         self._capture_schema_only = capture_schema_only
         self._ip = ipy
         self._local_vars = self._ip.user_global_ns
+        self._capture_comments = capture_comments
         self._cell_content = self._get_notebook_cell_content() if is_notebook is True else self._get_cell_content()
         self._vectice_data = self._get_variable_matches(self._local_vars)
         self._failed_assets = []
 
         # Get back objects to log
         self._assets = self._get_assets()
         graphs = self._get_graphs(is_notebook)
 
         if note:
             self._iteration_service.log_comment(note)
-            _logger.info(f"Note logged in iteration {self._iteration.index!r}.")
+            _logger.info(f"Note logged in iteration {self._iteration.name!r}.")
 
         # Log objects
+
         self._log_assets(self._assets)
 
         if graphs:
             for graph in graphs:
                 try:
                     self._iteration_service.log_image_or_file(graph)
                     graph = graph if isinstance(graph, str) else graph.filename
-                    _logger.info(f"Graph {graph!r} logged in iteration {self._iteration.index!r}.")
+                    _logger.info(f"Graph {graph!r} logged in iteration {self._iteration.name!r}.")
                 except Exception as e:
                     self._failed_assets.append({"reason": e, "asset": graph, "type": "Graph"})
 
         if len(self._failed_assets):
             _logger.warning("The following assets failed to log:")
         for failed_asset in self._failed_assets:
             _logger.warning(f"{failed_asset['type']} {failed_asset['asset']!r}, reason: {failed_asset['reason']}")
 
     def _get_variable_matches(self, local_vars: dict[str, Any]) -> list[dict[Any, Any]]:
         vectice_data = []
         all_vectice_calls = set()
         for cell_not_processed in self._cell_content:
             cell = preprocess_code(cell_not_processed)
+            variable_comments = parse_comments(cell_not_processed) if self._capture_comments else []
             vectice_match = {}
             all_vars: OrderedDict[str, Any] = OrderedDict()
 
             vectice_match["cell"] = cell
+            vectice_match["comments"] = variable_comments
 
             # Parse the cell content using the VariableVisitor
             try:
                 tree = ast.parse(cell)
             except SyntaxError as err:
                 raise SyntaxError(
                     "Autolog is unable to parse the code. Make sure all non-Python syntax, such as bash commands, are properly indented and preceded by '%' or '!'. If the error persist, please contact your sales representative."
@@ -283,29 +299,40 @@
             vectice_data.append(vectice_match)
         clean_vectice_data = []
         for data in vectice_data:
             for var in all_vectice_calls:
                 # the order of cells misses vars
                 if var in data["variables"]:
                     del data["variables"][var]
-            # check that there are vars for the cell and then append
-            if len(data["variables"]) >= 1:
+            # check that there are vars for the cell and then append or if there are comments
+            if len(data["variables"]) >= 1 or len(data["comments"]) >= 1:
                 clean_vectice_data.append(data)
         return clean_vectice_data
 
     def _get_notebook_cell_content(self) -> list[Any]:
         return list(NOTEBOOK_CELLS.values())
 
     def _get_cell_content(self) -> list[Any]:
         """Used by autolog cell to get the content of the cell. This is used to parse for variables."""
         cell_content = self._ip.get_parent()["content"]["code"]  # pyright: ignore[reportAttributeAccessIssue]
         if cell_content is None:
             raise ValueError("Failed to get cell content.")
         return [cell_content]
 
+    def _get_asset_comments(self, comments: dict, key: str) -> tuple[str | None, str | None]:
+        try:
+            comment_before = comments["comment_matches_before"][key]["comment"]
+        except KeyError:
+            comment_before = None
+        try:
+            comment_after = comments["comment_matches_after"][key]["comment"]
+        except KeyError:
+            comment_after = None
+        return comment_before, comment_after
+
     def _get_assets(self) -> list[TModel | TDataset | TVecticeObjects]:
         assets = []
         for data in self._vectice_data:
             for key in data["variables"].keys():
                 # skip cell inputs/outputs
                 if key.startswith("_"):
                     continue
@@ -398,30 +425,91 @@
 
     def _get_keras_info(self, model: KerasModel) -> tuple[str, dict[str, Any]] | tuple[None, None]:
         try:
             return "keras", self._format_keras_params(model)
         except Exception:
             return None, None
 
+    def _get_all_cells_comments(self) -> list[dict]:
+        # Get all comments from all cells
+        all_comments_and_variables = []
+        for data in self._vectice_data:
+            if data["comments"]:
+                for comments in data["comments"]:
+                    all_comments_and_variables.append(comments)
+        return all_comments_and_variables
+
+    def _get_comments_before(
+        self, all_comments_and_variables: list[dict], asset: TModel | TDataset | TVecticeObjects, comments_logged: list
+    ):
+        comments_to_log = []
+        for data in all_comments_and_variables:
+            # If we find the variable we log all the comments found
+            if data["variable"] == asset["variable"]:
+                return comments_to_log
+            # We only want comments remaining
+            if data["comment"] not in comments_logged:
+                comments_to_log.append(data["comment"])
+        # return nothing if we don't see the asset
+        return []
+
+    def _log_comments_before_asset(
+        self, all_comments_and_variables: list[dict], asset: TModel | TDataset | TVecticeObjects, comments_logged: list
+    ) -> list:
+        # Get comments to log before each asset
+        comments_before = self._get_comments_before(all_comments_and_variables, asset, comments_logged)
+        # Log comments before each asset
+        if comments_before:
+            for comment in comments_before:
+                if comment:
+                    self._iteration_service.log_comment(comment)
+            # Keep track of what's logged
+            return comments_logged + comments_before
+        return comments_logged
+
+    def _log_remaining_comments(self, all_unique_comments: set, comments_logged: list) -> None:
+        # Ensure last asset comments are filtered out
+        all_comments_logged = set(comments_logged)
+        still_comments_to_log = list(all_unique_comments - all_comments_logged)
+        # Log remaining comments after last asset
+        if still_comments_to_log:
+            for comment in still_comments_to_log:
+                if comment:
+                    self._iteration_service.log_comment(comment)
+        # Logging for comments captured
+        all_comments_logged.discard(None)
+        filtered_comments = list(filter(lambda comment: comment is not None, still_comments_to_log))
+        if filtered_comments or all_comments_logged:
+            _logger.info(f"Comments logged in iteration {self._iteration.name!r}.")
+
     def _log_assets(
         self,
         assets: list[TModel | TDataset | TVecticeObjects],
     ):
+        # all comments and variables
+        all_comments_and_variables = self._get_all_cells_comments()
+        # Unique comment set
+        all_unique_comments = set([data["comment"] for data in all_comments_and_variables])
+        # Keep track of what is logged
+        comments_logged = []
         for asset in assets:
             try:
+                comments_logged = self._log_comments_before_asset(all_comments_and_variables, asset, comments_logged)
                 if "vectice_object" in asset:
                     self._log_vectice_asset(asset)
                 elif "model" in asset:
                     self._log_model(asset)
                 elif "dataframe" in asset:
                     self._log_dataset(asset)
             except Exception as e:
                 self._failed_assets.append(
                     {"reason": e, "asset": asset["variable"], "type": "Model" if "model" in asset else "Dataset"}
                 )
+        # Log the remaining comments
+        self._log_remaining_comments(all_unique_comments, comments_logged)
 
     def _get_catboost_info(self, model: CatBoost) -> tuple[str, dict[str, Any]] | tuple[None, None]:
         try:
             params = {str(key): value for key, value in model.get_all_params().items() if value is not None}
             return "catboost", params
         except AttributeError:
             return None, None
@@ -500,37 +588,37 @@
                 metrics=model_metrics,
                 properties=params,
                 name=model_name,
                 predictor=model["model"],
                 attachments=temp_file_path,
             )
         )
-        _logger.info(f"Model {model_name!r} logged in iteration {self._iteration.index!r}.")
+        _logger.info(f"Model {model_name!r} logged in iteration {self._iteration.name!r}.")
 
         if temp_dir is not None:
             temp_dir.cleanup()
 
     def _log_vectice_asset(self, asset: TVecticeObjects) -> None:
         asset_to_log = asset["vectice_object"]
         asset_name = asset["variable"]
         if isinstance(asset_to_log, Dataset):
             dataset = asset_to_log
             dataset_name = dataset.name if dataset.name else asset_name
             self._iteration_service.log_dataset(asset_to_log)
-            _logger.info(f"Dataset {dataset_name!r} logged in iteration {self._iteration.index!r}.")
+            _logger.info(f"Dataset {dataset_name!r} logged in iteration {self._iteration.name!r}.")
         elif isinstance(asset_to_log, Table):
             table = asset_to_log
             table_name = table.name if table.name else asset_name
             self._iteration_service.log_table(asset_to_log)
-            _logger.info(f"Table {table_name!r} logged in iteration {self._iteration.index!r}.")
+            _logger.info(f"Table {table_name!r} logged in iteration {self._iteration.name!r}.")
         else:
             model = asset_to_log
             model_name = model.name if model.name else asset_name
             self._iteration_service.log_model(asset_to_log)
-            _logger.info(f"Model {model_name!r} logged in iteration {self._iteration.index!r}.")
+            _logger.info(f"Model {model_name!r} logged in iteration {self._iteration.name!r}.")
 
     def _log_dataset(self, dataset: TDataset) -> None:
         from vectice import Dataset, DatasetType, FileResource, NoResource
 
         resource = self._get_dataset_resource(dataset)
         dataset_name = f"{self._iteration.phase.id}-{dataset['variable']}"
         no_resource_dataset = Dataset(
@@ -556,15 +644,15 @@
             )
         else:
             vec_dataset = no_resource_dataset
         try:
             self._iteration_service.log_dataset(vec_dataset)
         except FileNotFoundError:
             self._iteration_service.log_dataset(no_resource_dataset)
-        _logger.info(f"Dataset {dataset_name!r} logged in iteration {self._iteration.index!r}.")
+        _logger.info(f"Dataset {dataset_name!r} logged in iteration {self._iteration.name!r}.")
 
     def _get_dataset_resource(self, dataset: TDataset) -> str | None:
         import re
 
         if not self._cell_content:
             return None
         try:
```

### Comparing `vectice-24.1.9.0/src/vectice/connection.py` & `vectice-24.2.1.0/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/__init__.py` & `vectice-24.2.1.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/additional_info.py` & `vectice-24.2.1.0/src/vectice/models/additional_info.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/attachment_container.py` & `vectice-24.2.1.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/code_version.py` & `vectice-24.2.1.0/src/vectice/models/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/dataset.py` & `vectice-24.2.1.0/src/vectice/models/dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/iteration.py` & `vectice-24.2.1.0/src/vectice/models/iteration.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     iteration = phase.create_iteration()
     ```
     """
 
     __slots__: ClassVar[list[str]] = [
         "_id",
         "_index",
+        "_name",
         "_phase",
         "_status",
         "_client",
         "_steps",
         "_service",
         "__dict__",
     ]
@@ -100,22 +101,23 @@
         output: IterationOutput,
         phase: Phase,
         client: Client,
     ):
         self.__dict__ = {}
         self._id = output.id
         self._index = output.index
+        self._name = output.name
         self._phase = phase
         self._status = output.status
         self._client = client
         self._steps = self._populate_steps()
         self._service = IterationService(self, self._client)
 
-    def __repr__(self):
-        return f"Iteration (index={self._index}, status={get_iteration_status(self._status)})"
+    def __repr__(self) -> str:
+        return f"Iteration (name={self._name}, status={get_iteration_status(self._status)})"
 
     def __eq__(self, other: object):
         if not isinstance(other, Iteration):
             return NotImplemented
         return self.id == other.id
 
     def _populate_steps(self) -> dict[str, Step]:
@@ -134,15 +136,16 @@
             step = self._client.get_step_by_name(step_item.name, self.id)
             return get_step_type(step_output=step, iteration=self)
         raise AttributeError(f"The attribute '{item}' does not exist.")
 
     def __setattr__(self, attr_name: str, attr_value: Any):
         if hasattr(self, "_steps") and attr_name in super().__getattribute__("_steps"):
             self._steps[attr_name] = self._steps[attr_name].step_factory_and_update(value=attr_value)
-        elif hasattr(self, "__dict__") and attr_name not in self.__slots__:
+        # adding name handling but not sure this raise condition is necessary, don't want to break other things
+        elif hasattr(self, "__dict__") and attr_name not in self.__slots__ and attr_name != "name":
             raise AttributeError(f"The attribute '{attr_name}' does not exist.")
         else:
             super().__setattr__(attr_name, attr_value)
 
     @property
     def id(self) -> str:
         """The iteration's identifier.
@@ -168,14 +171,27 @@
 
         Returns:
             The iteration's index.
         """
         return self._index
 
     @property
+    def name(self) -> str:
+        """The iteration's name.
+
+        Returns:
+            The iteration's name.
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name: str):
+        self._name = name
+
+    @property
     def status(self) -> str:
         """The iteration's status.
 
         Returns:
             The iteration's status.
         """
         return get_iteration_status(self._status)
@@ -187,20 +203,20 @@
         Returns:
             Whether the iteration is completed.
         """
         return self._status is IterationStatus.Completed
 
     @property
     def properties(self) -> dict[str, int | str]:
-        """The iteration's identifier and index.
+        """The iteration's identifier, index and name.
 
         Returns:
-            A dictionary containing the `id` and `index` items.
+            A dictionary containing the `id`, `index` and `name` items.
         """
-        return {"id": self.id, "index": self.index}
+        return {"id": self.id, "index": self.index, "name": self.name}
 
     def list_phase_requirements(self) -> None:
         """Prints a list of phase requirements in a tabular format, limited to the first 10 requirements. A link is provided to view the remaining requirements.
 
         Returns:
             None
         """
@@ -242,15 +258,15 @@
 
         if iteration_output.artifacts_count > 0:
             rich_table.add_row("None ('Assets without section')", str(iteration_output.artifacts_count))
 
         for section in iteration_output.sections.list:
             rich_table.add_row(section.name, str(section.artifacts_count))
 
-        description = f"""There are {iteration_output.sections.total} sections in the iteration {self.index!r} and a maximum of 10 sections are displayed in the table below:"""
+        description = f"""There are {iteration_output.sections.total} sections in the iteration {self.name!r} and a maximum of 10 sections are displayed in the table below:"""
         link = dedent(
             f"""
                 >> To log an asset to a specific section, use iteration.log()
                 For quick access to the iteration in the Vectice web app, visit:
                 {self._client.auth.api_base_url}/browse/iteration/{self.id}
             """
         ).lstrip()
@@ -275,34 +291,34 @@
         """
 
     def cancel(self) -> None:
         """Cancel the iteration."""
         iteration_input = IterationInput(status=IterationStatus.Abandoned.name)
         self._client.update_iteration(self.id, iteration_input)
         self._status = IterationStatus.Abandoned
-        _logger.info(f"Iteration with index {self.index} cancelled.")
+        _logger.info(f"Iteration {self.name} cancelled.")
 
     def complete(self) -> None:
         """Mark the iteration as completed."""
         iteration_input = IterationInput(status=IterationStatus.Completed.name)
         self._client.update_iteration(self.id, iteration_input)
         self._status = IterationStatus.Completed
         logging_output = dedent(
             f"""
-                        Iteration with index {self.index} completed.
+                        Iteration {self.name!r} completed.
 
                         For quick access to the Iteration in the Vectice web app, visit:
                         {self._client.auth.api_base_url}/browse/iteration/{self.id}"""
         ).lstrip()
         _logger.info(logging_output)
 
     def delete(self) -> None:
         """Permanently deletes the iteration."""
         self._client.delete_iteration(self.id)
-        _logger.info(f"Iteration with index {self.index} was deleted.")
+        _logger.info(f"Iteration {self.name} was deleted.")
 
     @property
     def connection(self) -> Connection:
         """The connection to which this iteration belongs.
 
         Returns:
             The connection to which this iteration belongs.
@@ -363,15 +379,29 @@
         """Delete all assets from the iteration. This action is irreversible, and the deleted assets cannot be recovered.
 
         ```python
         iteration.delete_assets_from_iteration()
         ```
         """
         self._client.remove_iteration_assets(iteration_id=self._id, all=True)
-        _logger.info(f"All assets from iteration {self.index!r} are deleted.")
+        _logger.info(f"All assets from iteration {self.name!r} are deleted.")
+
+    def update(
+        self,
+        name: str | None = None,
+    ) -> None:
+        """Update the Iteration from the API.
+
+        Parameters:
+            name: The new name of the iteration.
+
+        Returns:
+            None
+        """
+        self._service.update(name)
 
     def log(self, asset: Any, section: str | None = None) -> None:
         """Log an asset to an iteration. Assets can be organized into sections for improved clarity within the iteration.
 
         ```python
         from vectice import Model
         my_model = Model(name="my_model")
```

### Comparing `vectice-24.1.9.0/src/vectice/models/metric.py` & `vectice-24.2.1.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/model.py` & `vectice-24.2.1.0/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/model_exp_tracker.py` & `vectice-24.2.1.0/src/vectice/models/model_exp_tracker.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/model_mlflow.py` & `vectice-24.2.1.0/src/vectice/models/model_mlflow.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/phase.py` & `vectice-24.2.1.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/project.py` & `vectice-24.2.1.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/property.py` & `vectice-24.2.1.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/representation/dataset_representation.py` & `vectice-24.2.1.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/representation/dataset_version_representation.py` & `vectice-24.2.1.0/src/vectice/models/representation/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/representation/model_representation.py` & `vectice-24.2.1.0/src/vectice/models/representation/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/representation/model_version_representation.py` & `vectice-24.2.1.0/src/vectice/models/representation/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/__init__.py` & `vectice-24.2.1.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/base.py` & `vectice-24.2.1.0/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-24.2.1.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/databricks_table_resource.py` & `vectice-24.2.1.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/description.py` & `vectice-24.2.1.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/file_resource.py` & `vectice-24.2.1.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/gcs_resource.py` & `vectice-24.2.1.0/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/base.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/metadata/source.py` & `vectice-24.2.1.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/no_resource.py` & `vectice-24.2.1.0/src/vectice/models/resource/no_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/s3_resource.py` & `vectice-24.2.1.0/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/resource/snowflake_resource.py` & `vectice-24.2.1.0/src/vectice/models/resource/snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/step.py` & `vectice-24.2.1.0/src/vectice/models/step.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/step_dataset.py` & `vectice-24.2.1.0/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/step_image.py` & `vectice-24.2.1.0/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/step_model.py` & `vectice-24.2.1.0/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/step_number.py` & `vectice-24.2.1.0/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/step_string.py` & `vectice-24.2.1.0/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/table.py` & `vectice-24.2.1.0/src/vectice/models/table.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/models/workspace.py` & `vectice-24.2.1.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/services/iteration_service.py` & `vectice-24.2.1.0/src/vectice/services/iteration_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from io import BufferedReader, IOBase
 from typing import TYPE_CHECKING, Any, Hashable
 
 from PIL.Image import Image
 
 from vectice.api.http_error_handlers import VecticeException
 from vectice.api.json.iteration import (
+    IterationInput,
     IterationStepArtifactEntityMetadataInput,
     IterationStepArtifactInput,
     IterationStepArtifactType,
 )
 from vectice.utils.common_utils import (
     check_string_sanity,
     get_image_or_file_variables,
@@ -76,14 +77,23 @@
             iteration_id=self._iteration.id,
             code_version=code_version,
             section=section,
         )
         attachments_output = set_dataset_attachments(self._client, asset, dataset_output.dataset_version)
         return dataset_output, attachments_output
 
+    def update(self, name: str | None = None):
+        if name is not None:
+            self._update_name(name)
+
+    def _update_name(self, name: str):
+        self._client.update_iteration(self._iteration.id, IterationInput(name=name))
+        self._iteration.name = name
+        _logger.info(f"Iteration {self._iteration.id!r} name successfully updated.")
+
     def _create_image_or_file_artifact(
         self, value: str | IOBase | Image, section: str | None = None
     ) -> tuple[IterationStepArtifactInput, str]:
         is_image_or_file, filename = get_image_or_file_variables(value)
         try:
             artifact, *_ = self._client.upsert_iteration_attachments(
                 files=[("file", (filename, is_image_or_file))], iteration_id=self._iteration.id, step_name=section
```

### Comparing `vectice-24.1.9.0/src/vectice/services/phase_service.py` & `vectice-24.2.1.0/src/vectice/services/phase_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,22 +45,22 @@
             None
 
         """
         iteration_outputs = self._client.list_iterations(phase.id, only_mine, statuses)
         rich_table = Table(expand=True, show_edge=False)
 
         rich_table.add_column("Id", justify="left", no_wrap=True, min_width=3, max_width=20)
-        rich_table.add_column("Index", justify="left", no_wrap=True, min_width=5, max_width=10)
+        rich_table.add_column("Name", justify="left", no_wrap=True, min_width=5, max_width=20)
         rich_table.add_column("Status", justify="left", no_wrap=True, min_width=3, max_width=15)
         rich_table.add_column("Owner", justify="left", no_wrap=True, min_width=5, max_width=15)
 
         for iteration in iteration_outputs.list:
             rich_table.add_row(
                 str(iteration.id),
-                str(iteration.index),
+                iteration.name,
                 get_iteration_status(iteration.status, iteration.starred),
                 iteration.ownername,
             )
 
         iteration_statuses_log = (
             " | ".join(list(map(lambda status: get_iteration_status(status), statuses)))
             if statuses is not None and len(statuses) > 0
@@ -137,15 +137,15 @@
             An iteration.
         """
         from vectice.models.iteration import Iteration
 
         iteration_output = self._client.create_iteration(phase_id=phase.id)
         logging_output = dedent(
             f"""
-        New Iteration number {iteration_output.index!r} created.
+        New Iteration {iteration_output.name!r} created.
 
         For quick access to the Iteration in the Vectice web app, visit:
         {self._client.auth.api_base_url}/browse/iteration/{iteration_output.id}"""
         ).lstrip()
         _logger.info(logging_output)
 
         iteration = Iteration(iteration_output, phase, self._client)
@@ -165,15 +165,15 @@
         iteration_output = self._client.get_active_iteration_or_create(phase.id)
         return self._build_iteration_from_output_and_log(phase=phase, iteration_output=iteration_output)
 
     def _build_iteration_from_output_and_log(self, phase: Phase, iteration_output: IterationOutput) -> Iteration:
         from vectice.models.iteration import Iteration
 
         iteration = Iteration(iteration_output, phase, self._client)
-        base_log = dedent(f"Iteration number {iteration.index!r} successfully retrieved.")
+        base_log = dedent(f"Iteration {iteration.name!r} successfully retrieved.")
         if iteration_output.status in [IterationStatus.Completed, IterationStatus.Abandoned]:
             base_log += dedent(
                 f"""
                 WARN: Iteration is {iteration.status}."""
             )
 
         logging_output = dedent(
```

### Comparing `vectice-24.1.9.0/src/vectice/types/version.py` & `vectice-24.2.1.0/src/vectice/types/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/utils/common_utils.py` & `vectice-24.2.1.0/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/utils/configuration.py` & `vectice-24.2.1.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/utils/deprecation.py` & `vectice-24.2.1.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/utils/instance_helper.py` & `vectice-24.2.1.0/src/vectice/utils/instance_helper.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice/utils/last_assets.py` & `vectice-24.2.1.0/src/vectice/utils/last_assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 def _get_iteration_log(iteration: Iteration, section: str | None = None, existing_asset: bool = False):
     iteration_id = iteration.id
     url = iteration._client.auth.api_base_url  # pyright: ignore[reportPrivateUsage] OK to ignore deprecated code
     hyper_link = f"{url}/browse/iteration/{iteration_id}"
     assignment_type = "reassigned to" if existing_asset else "in"
     to_section = f", {assignment_type} section: {section!r}." if section else "."
-    return f"to iteration: {iteration.index}{to_section}", f"Link to iteration: {hyper_link}"
+    return f"to iteration: {iteration.name!r}{to_section}", f"Link to iteration: {hyper_link}"
 
 
 def _get_image_or_file_artifact_reference(filename: str) -> str:
     _, ext = os.path.splitext(filename)
     pillow_extensions = {exten for exten in Image.registered_extensions()}
     return "image" if (ext in pillow_extensions and ext != ".pdf") else "file"
```

### Comparing `vectice-24.1.9.0/src/vectice/utils/logging_utils.py` & `vectice-24.2.1.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice.egg-info/PKG-INFO` & `vectice-24.2.1.0/src/vectice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.1.9.0
+Version: 24.2.1.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-24.1.9.0/src/vectice.egg-info/SOURCES.txt` & `vectice-24.2.1.0/src/vectice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vectice-24.1.9.0/src/vectice.egg-info/requires.txt` & `vectice-24.2.1.0/src/vectice.egg-info/requires.txt`

 * *Files identical despite different names*

