# Comparing `tmp/waylay_sdk_resources_types-8.1.0.20240415.tar.gz` & `tmp/waylay_sdk_resources_types-8.1.0a20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_resources_types-8.1.0.20240415.tar", last modified: Mon Apr 15 09:59:09 2024, max compression
+gzip compressed data, was "waylay_sdk_resources_types-8.1.0a20240415.tar", last modified: Mon Apr 15 08:05:31 2024, max compression
```

## Comparing `waylay_sdk_resources_types-8.1.0.20240415.tar` & `waylay_sdk_resources_types-8.1.0a20240415.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.407788 waylay_sdk_resources_types-8.1.0.20240415/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-15 09:59:09.407788 waylay_sdk_resources_types-8.1.0.20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:59:09.407788 waylay_sdk_resources_types-8.1.0.20240415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.383787 waylay_sdk_resources_types-8.1.0.20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.379788 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.379788 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.379788 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.403788 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/array_must_contain_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/array_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/array_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/attribute_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_operation_enqueued.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_operation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_operation_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_resource_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_resource_operation_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_resource_operation_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_resource_operation_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_resource_operation_query_ids_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_running_resource_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/boolean_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/boolean_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/changed_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/changed_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/cloud_metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/cloud_metadata_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/cloud_metadata_event_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/cloud_metadata_event_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/constraint_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/constraint_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/constraint_status_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/create_delete_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/create_delete_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/discovered_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/discovered_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/failure_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/generic_metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/get_stream_event_format_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_page_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_children.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_listing_all_of_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_type_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_self_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_self_links_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_self_links_links_self.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_self_links_links_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/halid_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/list_constraints200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/metadata_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/metadata_entity_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/metadata_entity_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/nd_json_response_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/numeric_enum_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/numeric_enum_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/numeric_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/numeric_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/object_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/object_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/operation_result_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/operation_result_object_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/pagination_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/pagination_links_next.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/pagination_links_prev.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/pagination_links_self.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/paging_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/paging_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/patch_resource_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/patch_resource_type_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_change_change.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_changes_paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_constraint_creation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_constraint_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_constraint_with_id_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_creation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metadata_event_all_of_object_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric_metric_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of1.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of2.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of3.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of4.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_ref_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_ref_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_sensor_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_creation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_with_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_with_id_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_types_changes_paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_with_id_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resourcetype_metadata_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resourcetype_metadata_event_all_of_object_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/schema_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/ss_event_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/string_enum_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/string_value_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/string_value_constraint_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/success_operation_result_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/task_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/task_configuration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/validation_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/with_id_required.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.403788 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/metadata_events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/resource_constraint_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-15 09:59:04.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/resource_type_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.407788 waylay_sdk_resources_types-8.1.0.20240415/src/waylay_sdk_resources_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-15 09:59:09.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay_sdk_resources_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-04-15 09:59:09.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay_sdk_resources_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:59:09.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay_sdk_resources_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-15 09:59:09.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay_sdk_resources_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 09:59:09.000000 waylay_sdk_resources_types-8.1.0.20240415/src/waylay_sdk_resources_types.egg-info/top_level.txt
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.260614 waylay_sdk_resources_types-8.1.0a20240415/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      745 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/LICENSE.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     5024 2024-04-15 08:05:31.260093 waylay_sdk_resources_types-8.1.0a20240415/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2744 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/README.md
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1824 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/pyproject.toml
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)       38 2024-04-15 08:05:31.260688 waylay_sdk_resources_types-8.1.0a20240415/setup.cfg
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.155325 waylay_sdk_resources_types-8.1.0a20240415/src/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.154690 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.154822 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.155134 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.243506 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    11903 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      484 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/array_must_contain_inner.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1718 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/array_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      448 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/array_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      963 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/attribute_item.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      943 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_enqueued.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1754 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_result.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      668 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_status_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      977 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      458 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_action.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      494 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      907 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_query.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      605 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_query_ids_inner.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1590 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      977 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      528 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      761 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/boolean_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      456 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/boolean_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      903 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/changed_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      434 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/changed_event_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1062 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1112 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      590 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data_source.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1330 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1144 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      989 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_error.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1636 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_status.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      498 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_status_status.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      716 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/create_delete_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      466 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/create_delete_event_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      880 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/discovered_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      448 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/discovered_event_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      794 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/error_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      884 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/failure_operation_result_value.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      763 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/generic_metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      515 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/get_stream_event_format_parameter.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      680 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_link.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      729 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_page_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     3036 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      813 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_embedded.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1210 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      736 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_children.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      810 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_parent.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      822 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_resource_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1337 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_listing.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      832 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_listing_all_of_embedded.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2378 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_type_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      716 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      746 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      708 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links_self.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      788 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links_value.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      762 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/halid_link.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1140 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/list_constraints200_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1815 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      906 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity_location.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      536 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity_value.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      628 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      596 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/nd_json_response_stream.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1124 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_enum_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      458 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_enum_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1094 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      456 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      154 2024-04-15 07:53:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/object.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      948 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/object_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      452 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/object_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      845 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/operation_result_object.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1199 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/operation_result_object_results.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      951 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      704 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_next.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      704 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_prev.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      704 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_self.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      735 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/paging_count.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      937 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/paging_result.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1341 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/patch_resource_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1416 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/patch_resource_type_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:52:48.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/py.typed
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1666 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_change.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      492 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_change_change.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1093 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_changes_paged_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      881 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_creation_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1843 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1775 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_with_id_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      861 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_creation_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2701 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      564 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_id.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1135 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_listing.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1377 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      478 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metadata_event_all_of_object_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2349 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1145 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      483 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      492 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of1.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      458 2024-04-15 08:02:52.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of2.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      587 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of3.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      564 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of4.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      607 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_parent.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1520 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_ref_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      472 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_ref_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1201 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_reference.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      862 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_sensor.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1455 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_sensor_sensor.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      610 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1765 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_change.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      882 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_creation_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2277 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      581 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_id.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1112 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_listing.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2627 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_with_constraints.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2781 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_with_id_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1116 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_types_changes_paged_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2679 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_with_id_entity.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1271 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resourcetype_metadata_event.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      494 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resourcetype_metadata_event_all_of_object_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      985 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/schema_validation_error.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      576 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/ss_event_stream.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1089 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_enum_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1158 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_value_constraint.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      452 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_value_constraint_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      787 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/success_operation_result_value.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      900 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/task_configuration.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      526 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/task_configuration_type.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1025 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/validation_failure.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      655 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/version_response.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      628 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/with_id_required.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.248467 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      645 2024-04-15 07:52:48.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/__init__.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      758 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/about_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1124 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/batch_operations_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     1296 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/metadata_events_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 07:52:48.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/py.typed
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)    10002 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     2862 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_constraint_api.py
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     6976 2024-04-15 08:02:53.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_type_api.py
+drwxr-xr-x   0 simonschoonjans   (501) staff       (20)        0 2024-04-15 08:05:31.258751 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     5024 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/PKG-INFO
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)     8840 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/SOURCES.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        1 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/dependency_links.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)      326 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/requires.txt
+-rw-r--r--   0 simonschoonjans   (501) staff       (20)        7 2024-04-15 08:05:31.000000 waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/LICENSE.txt` & `waylay_sdk_resources_types-8.1.0a20240415/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/PKG-INFO` & `waylay_sdk_resources_types-8.1.0a20240415/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-resources-types
-Version: 8.1.0.20240415
+Version: 8.1.0a20240415
 Summary: Waylay Resources Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -21,15 +21,15 @@
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-resources-py.git
 Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/resources.html
 Keywords: Waylay Resources,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: waylay-sdk-core~=0.2.0
-Requires-Dist: waylay-sdk-resources==8.1.0.20240415
+Requires-Dist: waylay-sdk-resources==8.1.0a20240415
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/README.md` & `waylay_sdk_resources_types-8.1.0a20240415/README.md`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/pyproject.toml` & `waylay_sdk_resources_types-8.1.0a20240415/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-resources-types"
-version = "8.1.0.20240415"
+version = "8.1.0a20240415"
 description = "Waylay Resources Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Resources" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
     "waylay-sdk-core ~= 0.2.0",
-    "waylay-sdk-resources == 8.1.0.20240415",
+    "waylay-sdk-resources == 8.1.0a20240415",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/__init__.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 This service manages  [Waylay Resources](/#/features/resources/?id=resource) and related entities.  A _Waylay Resource_ models a real-world device or abstract entity of your IoT solution, and provides a context when processing data in the Rule Engine.  You'll interact with the _Waylay Resources_ API to create this _Digital Twin_ model,  a process that's also called _resource provisioning_.
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "8.1.0.20240415"
+__version__ = "8.1.0a20240415"
 
 # import models into model package
 from .array_must_contain_inner import ArrayMustContainInner
 from .array_value_constraint import ArrayValueConstraint
 from .array_value_constraint_type import ArrayValueConstraintType
 from .attribute_item import AttributeItem
 from .batch_operation_enqueued import BatchOperationEnqueued
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/array_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/array_value_constraint.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/attribute_item.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/attribute_item.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_operation_enqueued.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_enqueued.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_operation_result.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_operation_status_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_operation_status_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_resource_operation.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_resource_operation_query.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_query.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_resource_operation_query_ids_inner.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_resource_operation_query_ids_inner.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_running_resource_operation.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/batch_running_resource_operation_operation_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/boolean_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/boolean_value_constraint.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/changed_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/changed_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/cloud_metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/cloud_metadata_event_data.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/cloud_metadata_event_data_source.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data_source.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/cloud_metadata_event_data_type.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/cloud_metadata_event_data_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/constraint_error.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_error.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/constraint_status.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/constraint_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/create_delete_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/create_delete_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/discovered_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/discovered_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/error_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/error_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/failure_operation_result_value.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/failure_operation_result_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/generic_metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/generic_metadata_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/get_stream_event_format_parameter.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/get_stream_event_format_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_link.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_page_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_page_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_embedded.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_embedded.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_children.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_children.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_parent.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_parent.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_resource_type.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_entity_all_of_links_resource_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_listing.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_listing_all_of_embedded.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_listing_all_of_embedded.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_resource_type_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_resource_type_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_self_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_self_links_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_self_links_links_self.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links_self.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/hal_self_links_links_value.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/hal_self_links_links_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/halid_link.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/halid_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/list_constraints200_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/list_constraints200_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/metadata_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/metadata_entity_location.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity_location.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/metadata_entity_value.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_entity_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/metadata_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/nd_json_response_stream.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/nd_json_response_stream.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/numeric_enum_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_enum_value_constraint.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/numeric_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/numeric_value_constraint.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/object_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/object_value_constraint.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/operation_result_object.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/operation_result_object.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/operation_result_object_results.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/operation_result_object_results.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/pagination_links.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/pagination_links_next.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_next.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/pagination_links_prev.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_prev.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/pagination_links_self.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/pagination_links_self.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/paging_count.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/paging_count.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/paging_result.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/paging_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/patch_resource_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/patch_resource_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/patch_resource_type_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/patch_resource_type_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_change.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_change.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_changes_paged_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_changes_paged_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_constraint_creation_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_creation_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_constraint_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_constraint_with_id_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_constraint_with_id_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_creation_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_creation_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_id.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_listing.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metadata_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric_metric_type.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of3.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of3.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of4.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_metric_metric_type_one_of4.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_parent.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_parent.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_ref_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_ref_value_constraint.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_reference.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_reference.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_sensor.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_sensor.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_sensor_sensor.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_sensor_sensor.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_change.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_change.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_creation_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_creation_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_id.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_id.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_listing.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_with_constraints.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_with_constraints.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_type_with_id_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_type_with_id_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_types_changes_paged_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_types_changes_paged_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resource_with_id_entity.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resource_with_id_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/resourcetype_metadata_event.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/resourcetype_metadata_event.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/schema_validation_error.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/schema_validation_error.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/ss_event_stream.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/ss_event_stream.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/string_enum_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_enum_value_constraint.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/string_value_constraint.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/string_value_constraint.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/success_operation_result_value.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/success_operation_result_value.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/task_configuration.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/task_configuration.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/task_configuration_type.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/task_configuration_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/validation_failure.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/validation_failure.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/version_response.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/version_response.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/models/with_id_required.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/models/with_id_required.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/__init__.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/about_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/about_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/batch_operations_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/batch_operations_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/metadata_events_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/metadata_events_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/resource_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/resource_constraint_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_constraint_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay/services/resources/queries/resource_type_api.py` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay/services/resources/queries/resource_type_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay_sdk_resources_types.egg-info/PKG-INFO` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-resources-types
-Version: 8.1.0.20240415
+Version: 8.1.0a20240415
 Summary: Waylay Resources Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -21,15 +21,15 @@
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-resources-py.git
 Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/resources.html
 Keywords: Waylay Resources,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: waylay-sdk-core~=0.2.0
-Requires-Dist: waylay-sdk-resources==8.1.0.20240415
+Requires-Dist: waylay-sdk-resources==8.1.0a20240415
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay_sdk_resources_types-8.1.0.20240415/src/waylay_sdk_resources_types.egg-info/SOURCES.txt` & `waylay_sdk_resources_types-8.1.0a20240415/src/waylay_sdk_resources_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

