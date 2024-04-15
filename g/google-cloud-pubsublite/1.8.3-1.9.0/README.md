# Comparing `tmp/google-cloud-pubsublite-1.8.3.tar.gz` & `tmp/google-cloud-pubsublite-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-pubsublite-1.8.3.tar", last modified: Wed Jul  5 15:45:38 2023, max compression
+gzip compressed data, was "google-cloud-pubsublite-1.9.0.tar", last modified: Thu Dec 14 00:07:47 2023, max compression
```

## Comparing `google-cloud-pubsublite-1.8.3.tar` & `google-cloud-pubsublite-1.9.0.tar`

### file list

```diff
@@ -1,229 +1,227 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.311065 google-cloud-pubsublite-1.8.3/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5227 2023-07-05 15:45:38.311065 google-cloud-pubsublite-1.8.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4352 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.275061 google-cloud-pubsublite-1.8.3/google/
--rw-rw-r--   0 root         (0)     1003      666 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.275061 google-cloud-pubsublite-1.8.3/google/cloud/
--rw-rw-r--   0 root         (0)     1003      666 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.279062 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/
--rw-rw-r--   0 root         (0)     1003     8752 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/__init__.py
--rw-rw-r--   0 root         (0)     1003     6054 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/admin_client.py
--rw-rw-r--   0 root         (0)     1003     5709 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/admin_client_interface.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.279062 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/
--rw-rw-r--   0 root         (0)     1003     1344 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.283062 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/
--rw-rw-r--   0 root         (0)     1003        0 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/__init__.py
--rw-rw-r--   0 root         (0)     1003     1717 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/ack_set_tracker.py
--rw-rw-r--   0 root         (0)     1003     2672 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/ack_set_tracker_impl.py
--rw-rw-r--   0 root         (0)     1003     4853 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/assigning_subscriber.py
--rw-rw-r--   0 root         (0)     1003     2060 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/async_publisher_impl.py
--rw-rw-r--   0 root         (0)     1003     4070 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/client_multiplexer.py
--rw-rw-r--   0 root         (0)     1003     4752 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/make_publisher.py
--rw-rw-r--   0 root         (0)     1003     9698 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/make_subscriber.py
--rw-rw-r--   0 root         (0)     1003     2846 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/managed_event_loop.py
--rw-rw-r--   0 root         (0)     1003     2608 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_async_publisher_client.py
--rw-rw-r--   0 root         (0)     1003     3037 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_async_subscriber_client.py
--rw-rw-r--   0 root         (0)     1003     3054 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_publisher_client.py
--rw-rw-r--   0 root         (0)     1003     3387 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_subscriber_client.py
--rw-rw-r--   0 root         (0)     1003     1864 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/publisher_impl.py
--rw-rw-r--   0 root         (0)     1003     6240 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/single_partition_subscriber.py
--rw-rw-r--   0 root         (0)     1003     2475 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/single_publisher.py
--rw-rw-r--   0 root         (0)     1003     1758 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/single_subscriber.py
--rw-rw-r--   0 root         (0)     1003      492 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/sorted_list.py
--rw-rw-r--   0 root         (0)     1003     1037 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/streaming_pull_manager.py
--rw-rw-r--   0 root         (0)     1003     4029 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/subscriber_impl.py
--rw-rw-r--   0 root         (0)     1003     1971 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/wrapped_message.py
--rw-rw-r--   0 root         (0)     1003     1559 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/message_transformer.py
--rw-rw-r--   0 root         (0)     1003     4968 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/message_transforms.py
--rw-rw-r--   0 root         (0)     1003     1682 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/nack_handler.py
--rw-rw-r--   0 root         (0)     1003     7396 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/publisher_client.py
--rw-rw-r--   0 root         (0)     1003     2982 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/publisher_client_interface.py
--rw-rw-r--   0 root         (0)     1003     2870 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/reassignment_handler.py
--rw-rw-r--   0 root         (0)     1003     8343 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/subscriber_client.py
--rw-rw-r--   0 root         (0)     1003     3877 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/subscriber_client_interface.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.283062 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/
--rw-rw-r--   0 root         (0)     1003        0 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/__init__.py
--rw-rw-r--   0 root         (0)     1003     1259 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/constructable_from_service_account.py
--rw-rw-r--   0 root         (0)     1003      731 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/endpoints.py
--rw-rw-r--   0 root         (0)     1003      247 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/fast_serialize.py
--rw-rw-r--   0 root         (0)     1003      764 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/publish_sequence_number.py
--rw-rw-r--   0 root         (0)     1003      661 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/publisher_client_id.py
--rw-rw-r--   0 root         (0)     1003     1150 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/require_started.py
--rw-rw-r--   0 root         (0)     1003     1236 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/routing_metadata.py
--rw-rw-r--   0 root         (0)     1003      953 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/status_codes.py
--rw-rw-r--   0 root         (0)     1003      895 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wait_ignore_cancelled.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.291063 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/
--rw-rw-r--   0 root         (0)     1003        0 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/__init__.py
--rw-rw-r--   0 root         (0)     1003     8187 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/admin_client_impl.py
--rw-rw-r--   0 root         (0)     1003     1079 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/assigner.py
--rw-rw-r--   0 root         (0)     1003     4997 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/assigner_impl.py
--rw-rw-r--   0 root         (0)     1003     1402 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/client_cache.py
--rw-rw-r--   0 root         (0)     1003     1355 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/committer.py
--rw-rw-r--   0 root         (0)     1003     6115 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/committer_impl.py
--rw-rw-r--   0 root         (0)     1003     1703 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/connection.py
--rw-rw-r--   0 root         (0)     1003     1746 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/connection_reinitializer.py
--rw-rw-r--   0 root         (0)     1003     1811 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/default_routing_policy.py
--rw-rw-r--   0 root         (0)     1003     1407 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/fixed_set_assigner.py
--rw-rw-r--   0 root         (0)     1003     3150 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/flow_control_batcher.py
--rw-rw-r--   0 root         (0)     1003     3518 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/gapic_connection.py
--rw-rw-r--   0 root         (0)     1003     5248 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/make_publisher.py
--rw-rw-r--   0 root         (0)     1003      999 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/merge_metadata.py
--rw-rw-r--   0 root         (0)     1003      829 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/partition_count_watcher.py
--rw-rw-r--   0 root         (0)     1003     2880 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/partition_count_watcher_impl.py
--rw-rw-r--   0 root         (0)     1003     3821 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/partition_count_watching_publisher.py
--rw-rw-r--   0 root         (0)     1003     3699 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/permanent_failable.py
--rw-rw-r--   0 root         (0)     1003     1292 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/publisher.py
--rw-rw-r--   0 root         (0)     1003     1974 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/pubsub_context.py
--rw-rw-r--   0 root         (0)     1003     1648 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/reset_signal.py
--rw-rw-r--   0 root         (0)     1003     6860 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/retrying_connection.py
--rw-rw-r--   0 root         (0)     1003     1098 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/routing_policy.py
--rw-rw-r--   0 root         (0)     1003     1833 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/routing_publisher.py
--rw-rw-r--   0 root         (0)     1003     2697 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/serial_batcher.py
--rw-rw-r--   0 root         (0)     1003     8546 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/single_partition_publisher.py
--rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/subscriber.py
--rw-rw-r--   0 root         (0)     1003     7806 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/subscriber_impl.py
--rw-rw-r--   0 root         (0)     1003     1004 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/subscriber_reset_handler.py
--rw-rw-r--   0 root         (0)     1003     1007 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/work_item.py
--rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.291063 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/testing/
--rw-rw-r--   0 root         (0)     1003        0 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/testing/__init__.py
--rw-rw-r--   0 root         (0)     1003     1681 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/testing/test_reset_signal.py
--rw-rw-r--   0 root         (0)     1003     2127 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/testing/test_utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.291063 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/
--rw-rw-r--   0 root         (0)     1003     1207 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1155 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/backlog_location.py
--rw-rw-r--   0 root         (0)     1003      806 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/flow_control_settings.py
--rw-rw-r--   0 root         (0)     1003     1529 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/location.py
--rw-rw-r--   0 root         (0)     1003     2100 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/message_metadata.py
--rw-rw-r--   0 root         (0)     1003      651 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/partition.py
--rw-rw-r--   0 root         (0)     1003     4396 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/paths.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.291063 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/
--rw-rw-r--   0 root         (0)     1003     7473 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     9172 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.291063 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.295064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/
--rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   101163 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   114019 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/client.py
--rw-rw-r--   0 root         (0)     1003    25935 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.295064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15053 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    37275 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    38010 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.295064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    29952 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37810 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/client.py
--rw-rw-r--   0 root         (0)     1003     5948 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.295064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9058 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17750 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18016 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.299064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/
--rw-rw-r--   0 root         (0)     1003      817 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    22024 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    29824 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.299064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/
--rw-rw-r--   0 root         (0)     1003     1310 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6998 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15711 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15943 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.299064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    21620 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    29591 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.299064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/transports/
--rw-rw-r--   0 root         (0)     1003     1212 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6892 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15822 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16029 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.299064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    20997 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28956 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.299064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/transports/
--rw-rw-r--   0 root         (0)     1003     1221 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6911 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15174 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15396 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.303064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    28085 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37275 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.303064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/transports/
--rw-rw-r--   0 root         (0)     1003     1221 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8036 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18104 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18374 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.303064 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/
--rw-rw-r--   0 root         (0)     1003     4740 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    22581 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/admin.py
--rw-rw-r--   0 root         (0)     1003    18703 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003     8775 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/cursor.py
--rw-rw-r--   0 root         (0)     1003     8507 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/publisher.py
--rw-rw-r--   0 root         (0)     1003    12772 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/subscriber.py
--rw-rw-r--   0 root         (0)     1003     6264 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/topic_stats.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.303064 google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/
--rw-r--r--   0 root         (0)     1003     5227 2023-07-05 15:45:38.000000 google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    11313 2023-07-05 15:45:38.000000 google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:45:38.000000 google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:45:38.000000 google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:45:38.000000 google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      223 2023-07-05 15:45:38.000000 google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:45:38.000000 google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:45:38.315066 google-cloud-pubsublite-1.8.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2861 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.307065 google-cloud-pubsublite-1.8.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.307065 google-cloud-pubsublite-1.8.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.307065 google-cloud-pubsublite-1.8.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.307065 google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   264729 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_admin_service.py
--rw-rw-r--   0 root         (0)     1003    95788 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_cursor_service.py
--rw-rw-r--   0 root         (0)     1003    76930 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_partition_assignment_service.py
--rw-rw-r--   0 root         (0)     1003    74710 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_publisher_service.py
--rw-rw-r--   0 root         (0)     1003    74920 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_subscriber_service.py
--rw-rw-r--   0 root         (0)     1003    89793 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_topic_stats_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.307065 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/
--rw-rw-r--   0 root         (0)     1003        0 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.307065 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/
--rw-rw-r--   0 root         (0)     1003        0 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.311065 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/
--rw-rw-r--   0 root         (0)     1003        0 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/__init__.py
--rw-rw-r--   0 root         (0)     1003     2924 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/ack_set_tracker_impl_test.py
--rw-rw-r--   0 root         (0)     1003     8020 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/assigning_subscriber_test.py
--rw-rw-r--   0 root         (0)     1003     2481 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/async_client_multiplexer_test.py
--rw-rw-r--   0 root         (0)     1003     2303 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/client_multiplexer_test.py
--rw-rw-r--   0 root         (0)     1003     3290 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/multiplexed_async_subscriber_client_test.py
--rw-rw-r--   0 root         (0)     1003     2755 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/multiplexed_publisher_client_test.py
--rw-rw-r--   0 root         (0)     1003     1521 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/publisher_impl_test.py
--rw-rw-r--   0 root         (0)     1003    10673 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/single_partition_subscriber_test.py
--rw-rw-r--   0 root         (0)     1003     3924 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/subscriber_impl_test.py
--rw-rw-r--   0 root         (0)     1003     7111 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/message_transforms_test.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.311065 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/
--rw-rw-r--   0 root         (0)     1003        0 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:45:38.311065 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/
--rw-rw-r--   0 root         (0)     1003        0 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/__init__.py
--rw-rw-r--   0 root         (0)     1003     7623 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/assigner_impl_test.py
--rw-rw-r--   0 root         (0)     1003    13347 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/committer_impl_test.py
--rw-rw-r--   0 root         (0)     1003     1341 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/default_routing_policy_test.py
--rw-rw-r--   0 root         (0)     1003     2227 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/flow_control_batcher_test.py
--rw-rw-r--   0 root         (0)     1003     1851 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/gapic_connection_test.py
--rw-rw-r--   0 root         (0)     1003     3033 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/partition_count_watcher_impl_test.py
--rw-rw-r--   0 root         (0)     1003     4921 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/partition_count_watching_publisher_test.py
--rw-rw-r--   0 root         (0)     1003     2525 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/reset_signal_test.py
--rw-rw-r--   0 root         (0)     1003     4881 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/retrying_connection_test.py
--rw-rw-r--   0 root         (0)     1003     1068 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/routing_tests.json
--rw-rw-r--   0 root         (0)     1003    17473 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/single_partition_publisher_test.py
--rw-rw-r--   0 root         (0)     1003    18197 2023-07-05 15:42:58.000000 google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/subscriber_impl_test.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.016415 google-cloud-pubsublite-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5641 2023-12-14 00:07:47.016415 google-cloud-pubsublite-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4352 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.964404 google-cloud-pubsublite-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.964404 google-cloud-pubsublite-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.972406 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/
+-rw-rw-r--   0 root         (0)     1003     8752 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6054 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/admin_client.py
+-rw-rw-r--   0 root         (0)     1003     5709 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/admin_client_interface.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.972406 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.980407 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1717 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/ack_set_tracker.py
+-rw-rw-r--   0 root         (0)     1003     2672 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/ack_set_tracker_impl.py
+-rw-rw-r--   0 root         (0)     1003     4853 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/assigning_subscriber.py
+-rw-rw-r--   0 root         (0)     1003     2060 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/async_publisher_impl.py
+-rw-rw-r--   0 root         (0)     1003     4070 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/client_multiplexer.py
+-rw-rw-r--   0 root         (0)     1003     4752 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/make_publisher.py
+-rw-rw-r--   0 root         (0)     1003     9698 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/make_subscriber.py
+-rw-rw-r--   0 root         (0)     1003     2846 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/managed_event_loop.py
+-rw-rw-r--   0 root         (0)     1003     2608 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_async_publisher_client.py
+-rw-rw-r--   0 root         (0)     1003     3037 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_async_subscriber_client.py
+-rw-rw-r--   0 root         (0)     1003     3054 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_publisher_client.py
+-rw-rw-r--   0 root         (0)     1003     3387 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_subscriber_client.py
+-rw-rw-r--   0 root         (0)     1003     1864 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/publisher_impl.py
+-rw-rw-r--   0 root         (0)     1003     6240 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/single_partition_subscriber.py
+-rw-rw-r--   0 root         (0)     1003     2475 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/single_publisher.py
+-rw-rw-r--   0 root         (0)     1003     1758 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/single_subscriber.py
+-rw-rw-r--   0 root         (0)     1003      492 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/sorted_list.py
+-rw-rw-r--   0 root         (0)     1003     1037 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/streaming_pull_manager.py
+-rw-rw-r--   0 root         (0)     1003     4029 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/subscriber_impl.py
+-rw-rw-r--   0 root         (0)     1003     1971 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/wrapped_message.py
+-rw-rw-r--   0 root         (0)     1003     1559 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/message_transformer.py
+-rw-rw-r--   0 root         (0)     1003     4968 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/message_transforms.py
+-rw-rw-r--   0 root         (0)     1003     1682 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/nack_handler.py
+-rw-rw-r--   0 root         (0)     1003     7396 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/publisher_client.py
+-rw-rw-r--   0 root         (0)     1003     2982 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/publisher_client_interface.py
+-rw-rw-r--   0 root         (0)     1003     2870 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/reassignment_handler.py
+-rw-rw-r--   0 root         (0)     1003     8343 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/subscriber_client.py
+-rw-rw-r--   0 root         (0)     1003     3877 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/subscriber_client_interface.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.980407 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1259 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/constructable_from_service_account.py
+-rw-rw-r--   0 root         (0)     1003      731 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/endpoints.py
+-rw-rw-r--   0 root         (0)     1003      247 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/fast_serialize.py
+-rw-rw-r--   0 root         (0)     1003      764 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/publish_sequence_number.py
+-rw-rw-r--   0 root         (0)     1003      661 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/publisher_client_id.py
+-rw-rw-r--   0 root         (0)     1003     1150 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/require_started.py
+-rw-rw-r--   0 root         (0)     1003     1236 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/routing_metadata.py
+-rw-rw-r--   0 root         (0)     1003      953 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/status_codes.py
+-rw-rw-r--   0 root         (0)     1003      895 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wait_ignore_cancelled.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.988409 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8187 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/admin_client_impl.py
+-rw-rw-r--   0 root         (0)     1003     1079 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/assigner.py
+-rw-rw-r--   0 root         (0)     1003     4997 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/assigner_impl.py
+-rw-rw-r--   0 root         (0)     1003     1402 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/client_cache.py
+-rw-rw-r--   0 root         (0)     1003     1355 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/committer.py
+-rw-rw-r--   0 root         (0)     1003     6115 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/committer_impl.py
+-rw-rw-r--   0 root         (0)     1003     1703 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/connection.py
+-rw-rw-r--   0 root         (0)     1003     1746 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/connection_reinitializer.py
+-rw-rw-r--   0 root         (0)     1003     1811 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/default_routing_policy.py
+-rw-rw-r--   0 root         (0)     1003     1407 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/fixed_set_assigner.py
+-rw-rw-r--   0 root         (0)     1003     3150 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/flow_control_batcher.py
+-rw-rw-r--   0 root         (0)     1003     3518 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/gapic_connection.py
+-rw-rw-r--   0 root         (0)     1003     5248 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/make_publisher.py
+-rw-rw-r--   0 root         (0)     1003      999 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/merge_metadata.py
+-rw-rw-r--   0 root         (0)     1003      829 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/partition_count_watcher.py
+-rw-rw-r--   0 root         (0)     1003     2880 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/partition_count_watcher_impl.py
+-rw-rw-r--   0 root         (0)     1003     3821 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/partition_count_watching_publisher.py
+-rw-rw-r--   0 root         (0)     1003     3699 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/permanent_failable.py
+-rw-rw-r--   0 root         (0)     1003     1292 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/publisher.py
+-rw-rw-r--   0 root         (0)     1003     1746 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/pubsub_context.py
+-rw-rw-r--   0 root         (0)     1003     1648 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/reset_signal.py
+-rw-rw-r--   0 root         (0)     1003     6860 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/retrying_connection.py
+-rw-rw-r--   0 root         (0)     1003     1098 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/routing_policy.py
+-rw-rw-r--   0 root         (0)     1003     1833 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/routing_publisher.py
+-rw-rw-r--   0 root         (0)     1003     2697 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/serial_batcher.py
+-rw-rw-r--   0 root         (0)     1003     8546 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/single_partition_publisher.py
+-rw-rw-r--   0 root         (0)     1003     1414 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/subscriber.py
+-rw-rw-r--   0 root         (0)     1003     7806 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/subscriber_impl.py
+-rw-rw-r--   0 root         (0)     1003     1004 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/subscriber_reset_handler.py
+-rw-rw-r--   0 root         (0)     1003     1007 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/work_item.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.988409 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/testing/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/testing/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1681 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/testing/test_reset_signal.py
+-rw-rw-r--   0 root         (0)     1003     2127 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/testing/test_utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.988409 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/
+-rw-rw-r--   0 root         (0)     1003     1207 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1155 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/backlog_location.py
+-rw-rw-r--   0 root         (0)     1003      806 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/flow_control_settings.py
+-rw-rw-r--   0 root         (0)     1003     1529 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/location.py
+-rw-rw-r--   0 root         (0)     1003     2100 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/message_metadata.py
+-rw-rw-r--   0 root         (0)     1003      651 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/partition.py
+-rw-rw-r--   0 root         (0)     1003     4396 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/paths.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.992410 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/
+-rw-rw-r--   0 root         (0)     1003     7473 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9172 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.992410 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.992410 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/
+-rw-rw-r--   0 root         (0)     1003      761 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   101477 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   114040 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/client.py
+-rw-rw-r--   0 root         (0)     1003    25935 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.992410 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15007 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    37229 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    37964 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.996411 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30096 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37827 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5948 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.996411 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9074 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17766 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18032 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.996411 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/
+-rw-rw-r--   0 root         (0)     1003      817 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22135 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    29840 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.996411 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1310 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7014 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15727 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15959 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:46.996411 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21731 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    29607 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.000412 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1212 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6908 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15838 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16045 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.000412 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21108 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28972 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.000412 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1221 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6927 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15190 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15412 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.000412 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28218 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37291 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.004413 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1221 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8052 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18120 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18390 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.004413 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4740 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22581 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/admin.py
+-rw-rw-r--   0 root         (0)     1003    18703 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     8775 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/cursor.py
+-rw-rw-r--   0 root         (0)     1003     8509 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/publisher.py
+-rw-rw-r--   0 root         (0)     1003    12774 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/subscriber.py
+-rw-rw-r--   0 root         (0)     1003     6264 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/topic_stats.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.004413 google-cloud-pubsublite-1.9.0/google_cloud_pubsublite.egg-info/
+-rw-r--r--   0 root         (0)     1003     5641 2023-12-14 00:07:46.000000 google-cloud-pubsublite-1.9.0/google_cloud_pubsublite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    11242 2023-12-14 00:07:46.000000 google-cloud-pubsublite-1.9.0/google_cloud_pubsublite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-12-14 00:07:46.000000 google-cloud-pubsublite-1.9.0/google_cloud_pubsublite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-12-14 00:07:46.000000 google-cloud-pubsublite-1.9.0/google_cloud_pubsublite.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      276 2023-12-14 00:07:46.000000 google-cloud-pubsublite-1.9.0/google_cloud_pubsublite.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-12-14 00:07:46.000000 google-cloud-pubsublite-1.9.0/google_cloud_pubsublite.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-12-14 00:07:47.016415 google-cloud-pubsublite-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2837 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.004413 google-cloud-pubsublite-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.008414 google-cloud-pubsublite-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.008414 google-cloud-pubsublite-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.008414 google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   264777 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_admin_service.py
+-rw-rw-r--   0 root         (0)     1003    95836 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_cursor_service.py
+-rw-rw-r--   0 root         (0)     1003    76978 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_partition_assignment_service.py
+-rw-rw-r--   0 root         (0)     1003    74758 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_publisher_service.py
+-rw-rw-r--   0 root         (0)     1003    74968 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_subscriber_service.py
+-rw-rw-r--   0 root         (0)     1003    89841 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_topic_stats_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.008414 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.008414 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.012415 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2924 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/ack_set_tracker_impl_test.py
+-rw-rw-r--   0 root         (0)     1003     8020 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/assigning_subscriber_test.py
+-rw-rw-r--   0 root         (0)     1003     2481 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/async_client_multiplexer_test.py
+-rw-rw-r--   0 root         (0)     1003     2303 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/client_multiplexer_test.py
+-rw-rw-r--   0 root         (0)     1003     3290 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/multiplexed_async_subscriber_client_test.py
+-rw-rw-r--   0 root         (0)     1003     2755 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/multiplexed_publisher_client_test.py
+-rw-rw-r--   0 root         (0)     1003     1521 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/publisher_impl_test.py
+-rw-rw-r--   0 root         (0)     1003    10673 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/single_partition_subscriber_test.py
+-rw-rw-r--   0 root         (0)     1003     3924 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/subscriber_impl_test.py
+-rw-rw-r--   0 root         (0)     1003     7111 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/message_transforms_test.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.012415 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-14 00:07:47.016415 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7623 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/assigner_impl_test.py
+-rw-rw-r--   0 root         (0)     1003    13347 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/committer_impl_test.py
+-rw-rw-r--   0 root         (0)     1003     1341 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/default_routing_policy_test.py
+-rw-rw-r--   0 root         (0)     1003     2227 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/flow_control_batcher_test.py
+-rw-rw-r--   0 root         (0)     1003     1851 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/gapic_connection_test.py
+-rw-rw-r--   0 root         (0)     1003     3033 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/partition_count_watcher_impl_test.py
+-rw-rw-r--   0 root         (0)     1003     4921 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/partition_count_watching_publisher_test.py
+-rw-rw-r--   0 root         (0)     1003     2525 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/reset_signal_test.py
+-rw-rw-r--   0 root         (0)     1003     4881 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/retrying_connection_test.py
+-rw-rw-r--   0 root         (0)     1003     1068 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/routing_tests.json
+-rw-rw-r--   0 root         (0)     1003    17473 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/single_partition_publisher_test.py
+-rw-rw-r--   0 root         (0)     1003    18197 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/subscriber_impl_test.py
+-rw-rw-r--   0 root         (0)     1003     1425 2023-12-14 00:05:10.000000 google-cloud-pubsublite-1.9.0/tests/unit/test_packaging.py
```

### Comparing `google-cloud-pubsublite-1.8.3/LICENSE` & `google-cloud-pubsublite-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/MANIFEST.in` & `google-cloud-pubsublite-1.9.0/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2020 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/PKG-INFO` & `google-cloud-pubsublite-1.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-pubsublite
-Version: 1.8.3
+Version: 1.9.0
 Summary: Google Cloud Pubsublite API client library
 Home-page: https://github.com/googleapis/python-pubsublite
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,18 +12,25 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: google-cloud-pubsub<3.0.0dev,>=2.10.0
+Requires-Dist: grpcio<2.0.0dev,>=1.38.1
+Requires-Dist: grpcio-status<2.0.0dev,>=1.38.1
+Requires-Dist: overrides<8.0.0,>=6.0.1
+Requires-Dist: overrides<8.0.0,>=7.0.1; python_version >= "3.12"
+Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,<3.0.0dev,>=1.33.2
 
 Python Client for Pub/Sub Lite API
 ==================================
 
 |stable| |pypi| |versions|
 
 `Pub/Sub Lite API`_: is designed to provide reliable,
```

### Comparing `google-cloud-pubsublite-1.8.3/README.rst` & `google-cloud-pubsublite-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/publisher_client_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2020 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     https://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pkg_resources
+from typing import NamedTuple
+
 
-pkg_resources.declare_namespace(__name__)
+class PublisherClientId(NamedTuple):
+    value: bytes
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/endpoints.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# -*- coding: utf-8 -*-
-#
 # Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     https://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pkg_resources
+from google.cloud.pubsublite.types import CloudRegion
+
 
-pkg_resources.declare_namespace(__name__)
+def regional_endpoint(region: CloudRegion):
+    return f"dns:///{region}-pubsublite.googleapis.com"
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/admin_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/admin_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/admin_client_interface.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/admin_client_interface.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/ack_set_tracker.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/ack_set_tracker.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/ack_set_tracker_impl.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/ack_set_tracker_impl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/assigning_subscriber.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/assigning_subscriber.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/async_publisher_impl.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/async_publisher_impl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/client_multiplexer.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/client_multiplexer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/make_publisher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/make_publisher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/make_subscriber.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/make_subscriber.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/managed_event_loop.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/managed_event_loop.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_async_publisher_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_async_publisher_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_async_subscriber_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_async_subscriber_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_publisher_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_publisher_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_subscriber_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/multiplexed_subscriber_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/publisher_impl.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/publisher_impl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/single_partition_subscriber.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/single_partition_subscriber.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/single_publisher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/single_publisher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/single_subscriber.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/single_subscriber.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/streaming_pull_manager.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/streaming_pull_manager.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/subscriber_impl.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/subscriber_impl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/internal/wrapped_message.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/internal/wrapped_message.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/message_transformer.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/message_transformer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/message_transforms.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/message_transforms.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/nack_handler.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/nack_handler.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/publisher_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/publisher_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/publisher_client_interface.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/publisher_client_interface.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/reassignment_handler.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/reassignment_handler.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/subscriber_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/subscriber_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/cloudpubsub/subscriber_client_interface.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/cloudpubsub/subscriber_client_interface.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/gapic_version.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.3"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/constructable_from_service_account.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/constructable_from_service_account.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/endpoints.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/partition.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from google.cloud.pubsublite.types import CloudRegion
+from typing import NamedTuple
 
 
-def regional_endpoint(region: CloudRegion):
-    return f"dns:///{region}-pubsublite.googleapis.com"
+class Partition(NamedTuple):
+    value: int
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/publish_sequence_number.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/publish_sequence_number.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/publisher_client_id.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/flow_control_settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Google LLC
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,9 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import NamedTuple
 
 
-class PublisherClientId(NamedTuple):
-    value: bytes
+class FlowControlSettings(NamedTuple):
+    messages_outstanding: int
+    bytes_outstanding: int
+
+
+_MAX_INT64 = 0x7FFFFFFFFFFFFFFF
+
+DISABLED_FLOW_CONTROL = FlowControlSettings(_MAX_INT64, _MAX_INT64)
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/require_started.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/require_started.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/routing_metadata.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/routing_metadata.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/status_codes.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/status_codes.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wait_ignore_cancelled.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wait_ignore_cancelled.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/admin_client_impl.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/admin_client_impl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/assigner.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/assigner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/assigner_impl.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/assigner_impl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/client_cache.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/client_cache.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/committer.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/committer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/committer_impl.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/committer_impl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/connection.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/connection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/connection_reinitializer.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/connection_reinitializer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/default_routing_policy.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/default_routing_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/fixed_set_assigner.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/fixed_set_assigner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/flow_control_batcher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/flow_control_batcher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/gapic_connection.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/gapic_connection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/make_publisher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/make_publisher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/merge_metadata.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/merge_metadata.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/partition_count_watcher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/partition_count_watcher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/partition_count_watcher_impl.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/partition_count_watcher_impl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/partition_count_watching_publisher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/partition_count_watching_publisher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/permanent_failable.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/permanent_failable.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/publisher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/publisher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/pubsub_context.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/pubsub_context.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,34 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from base64 import b64encode
 from typing import Mapping, Optional, NamedTuple
 
 import logging
-import pkg_resources
+
 from google.protobuf import struct_pb2  # pytype: disable=pyi-error
 
+from google.cloud.pubsublite import gapic_version
+
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class _Semver(NamedTuple):
     major: int
     minor: int
 
 
 def _version() -> _Semver:
-    try:
-        version = pkg_resources.get_distribution("google-cloud-pubsublite").version
-    except pkg_resources.DistributionNotFound:
-        _LOGGER.info(
-            "Failed to extract the google-cloud-pubsublite semver version. DistributionNotFound."
-        )
-        return _Semver(0, 0)
+    version = gapic_version.__version__
     splits = version.split(".")
     if len(splits) != 3:
         _LOGGER.info(f"Failed to extract semver from {version}.")
         return _Semver(0, 0)
     return _Semver(int(splits[0]), int(splits[1]))
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/reset_signal.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/reset_signal.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/retrying_connection.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/retrying_connection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/routing_policy.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/routing_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/routing_publisher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/routing_publisher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/serial_batcher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/serial_batcher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/single_partition_publisher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/single_partition_publisher.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/subscriber.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/subscriber.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/subscriber_impl.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/subscriber_impl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/subscriber_reset_handler.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/subscriber_reset_handler.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/internal/wire/work_item.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/internal/wire/work_item.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/testing/test_reset_signal.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/testing/test_reset_signal.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/testing/test_utils.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/backlog_location.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/backlog_location.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/flow_control_settings.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-# Copyright 2020 Google LLC
+# -*- coding: utf-8 -*-
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+from .client import TopicStatsServiceClient
+from .async_client import TopicStatsServiceAsyncClient
 
-from typing import NamedTuple
-
-
-class FlowControlSettings(NamedTuple):
-    messages_outstanding: int
-    bytes_outstanding: int
-
-
-_MAX_INT64 = 0x7FFFFFFFFFFFFFFF
-
-DISABLED_FLOW_CONTROL = FlowControlSettings(_MAX_INT64, _MAX_INT64)
+__all__ = (
+    "TopicStatsServiceClient",
+    "TopicStatsServiceAsyncClient",
+)
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/location.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/location.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/message_metadata.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/message_metadata.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/partition.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/gapic_version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-# Copyright 2020 Google LLC
+# -*- coding: utf-8 -*-
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from typing import NamedTuple
-
-
-class Partition(NamedTuple):
-    value: int
+#
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite/types/paths.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite/types/paths.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/gapic_metadata.json` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/async_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -29,29 +29,29 @@
 )
 
 from google.cloud.pubsublite_v1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
-from google.api_core import retry as retries
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 try:
-    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+    OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
-    OptionalRetry = Union[retries.Retry, object]  # type: ignore
+    OptionalRetry = Union[retries.AsyncRetry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.pubsublite_v1.services.admin_service import pagers
 from google.cloud.pubsublite_v1.types import admin
 from google.cloud.pubsublite_v1.types import common
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from .transports.base import AdminServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc_asyncio import AdminServiceGrpcAsyncIOTransport
 from .client import AdminServiceClient
 
 
 class AdminServiceAsyncClient:
@@ -284,15 +284,15 @@
                 the final component of the topic's name.
 
                 This value is structured like: ``my-topic-name``.
 
                 This corresponds to the ``topic_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.Topic:
@@ -387,15 +387,15 @@
             name (:class:`str`):
                 Required. The name of the topic whose
                 configuration to return.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.Topic:
@@ -487,15 +487,15 @@
             name (:class:`str`):
                 Required. The topic whose partition
                 information to return.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.TopicPartitions:
@@ -588,23 +588,24 @@
                 Required. The parent whose topics are to be listed.
                 Structured like
                 ``projects/{project_number}/locations/{location}``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListTopicsAsyncPager:
                 Response for ListTopics.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -707,15 +708,15 @@
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. A mask specifying the topic
                 fields to change.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.Topic:
@@ -807,15 +808,15 @@
             name (:class:`str`):
                 Required. The name of the topic to
                 delete.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -901,23 +902,24 @@
             name (:class:`str`):
                 Required. The name of the topic whose
                 subscriptions to list.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListTopicSubscriptionsAsyncPager:
                 Response for ListTopicSubscriptions.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1033,15 +1035,15 @@
                 become the final component of the subscription's name.
 
                 This value is structured like: ``my-sub-name``.
 
                 This corresponds to the ``subscription_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.Subscription:
@@ -1139,15 +1141,15 @@
                 Required. The name of the
                 subscription whose configuration to
                 return.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.Subscription:
@@ -1243,23 +1245,24 @@
                 Required. The parent whose subscriptions are to be
                 listed. Structured like
                 ``projects/{project_number}/locations/{location}``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListSubscriptionsAsyncPager:
                 Response for ListSubscriptions.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1362,15 +1365,15 @@
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. A mask specifying the
                 subscription fields to change.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.Subscription:
@@ -1464,15 +1467,15 @@
             name (:class:`str`):
                 Required. The name of the
                 subscription to delete.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1579,15 +1582,15 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.pubsublite_v1.types.SeekSubscriptionRequest, dict]]):
                 The request object. Request for SeekSubscription.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
@@ -1697,15 +1700,15 @@
                 become the final component of the reservation's name.
 
                 This value is structured like: ``my-reservation-name``.
 
                 This corresponds to the ``reservation_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.Reservation:
@@ -1803,15 +1806,15 @@
                 Required. The name of the reservation whose
                 configuration to return. Structured like:
                 projects/{project_number}/locations/{location}/reservations/{reservation_id}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.Reservation:
@@ -1907,23 +1910,24 @@
                 Required. The parent whose reservations are to be
                 listed. Structured like
                 ``projects/{project_number}/locations/{location}``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListReservationsAsyncPager:
                 Response for ListReservations.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -2026,15 +2030,15 @@
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. A mask specifying the
                 reservation fields to change.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.Reservation:
@@ -2129,15 +2133,15 @@
                 Required. The name of the reservation to delete.
                 Structured like:
                 projects/{project_number}/locations/{location}/reservations/{reservation_id}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -2224,23 +2228,24 @@
                 Required. The name of the reservation whose topics to
                 list. Structured like:
                 projects/{project_number}/locations/{location}/reservations/{reservation_id}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListReservationTopicsAsyncPager:
                 Response for ListReservationTopics.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -2303,15 +2308,15 @@
     ) -> operations_pb2.ListOperationsResponse:
         r"""Lists operations that match the specified filter in the request.
 
         Args:
             request (:class:`~.operations_pb2.ListOperationsRequest`):
                 The request object. Request message for
                 `ListOperations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.ListOperationsResponse:
                 Response message for ``ListOperations`` method.
@@ -2320,15 +2325,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.ListOperationsRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.list_operations,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -2357,15 +2362,15 @@
     ) -> operations_pb2.Operation:
         r"""Gets the latest state of a long-running operation.
 
         Args:
             request (:class:`~.operations_pb2.GetOperationRequest`):
                 The request object. Request message for
                 `GetOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.Operation:
                 An ``Operation`` object.
@@ -2374,15 +2379,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.GetOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.get_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -2416,15 +2421,15 @@
         If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.DeleteOperationRequest`):
                 The request object. Request message for
                 `DeleteOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -2432,15 +2437,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.DeleteOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.delete_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -2470,15 +2475,15 @@
         is not guaranteed.  If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.CancelOperationRequest`):
                 The request object. Request message for
                 `CancelOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -2486,15 +2491,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.CancelOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.cancel_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -47,15 +47,15 @@
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.pubsublite_v1.services.admin_service import pagers
 from google.cloud.pubsublite_v1.types import admin
 from google.cloud.pubsublite_v1.types import common
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from .transports.base import AdminServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import AdminServiceGrpcTransport
 from .transports.grpc_asyncio import AdminServiceGrpcAsyncIOTransport
 
 
 class AdminServiceClientMeta(type):
@@ -868,14 +868,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListTopicsPager:
                 Response for ListTopics.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1181,14 +1182,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListTopicSubscriptionsPager:
                 Response for ListTopicSubscriptions.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1523,14 +1525,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListSubscriptionsPager:
                 Response for ListSubscriptions.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -2188,14 +2191,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListReservationsPager:
                 Response for ListReservations.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -2505,14 +2509,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.admin_service.pagers.ListReservationTopicsPager:
                 Response for ListReservationTopics.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/pagers.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/transports/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/transports/base.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,15 +25,14 @@
 from google.api_core import retry as retries
 from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.pubsublite_v1.types import admin
 from google.cloud.pubsublite_v1.types import common
-from google.longrunning import operations_pb2
 from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/transports/grpc.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,15 +23,14 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.pubsublite_v1.types import admin
 from google.cloud.pubsublite_v1.types import common
-from google.longrunning import operations_pb2
 from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 from .base import AdminServiceTransport, DEFAULT_CLIENT_INFO
 
 
 class AdminServiceGrpcTransport(AdminServiceTransport):
     """gRPC backend transport for AdminService.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/admin_service/transports/grpc_asyncio.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/admin_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,15 +23,14 @@
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.pubsublite_v1.types import admin
 from google.cloud.pubsublite_v1.types import common
-from google.longrunning import operations_pb2
 from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 from .base import AdminServiceTransport, DEFAULT_CLIENT_INFO
 from .grpc import AdminServiceGrpcTransport
 
 
 class AdminServiceGrpcAsyncIOTransport(AdminServiceTransport):
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/async_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,26 +32,26 @@
 )
 
 from google.cloud.pubsublite_v1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
-from google.api_core import retry as retries
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 try:
-    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+    OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
-    OptionalRetry = Union[retries.Retry, object]  # type: ignore
+    OptionalRetry = Union[retries.AsyncRetry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.services.cursor_service import pagers
 from google.cloud.pubsublite_v1.types import cursor
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .transports.base import CursorServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc_asyncio import CursorServiceGrpcAsyncIOTransport
 from .client import CursorServiceClient
 
 
 class CursorServiceAsyncClient:
     """The service that a subscriber client application uses to
@@ -268,15 +268,15 @@
                 async for response in stream:
                     print(response)
 
         Args:
             requests (AsyncIterator[`google.cloud.pubsublite_v1.types.StreamingCommitCursorRequest`]):
                 The request object AsyncIterator. A request sent from the client to the
                 server on a stream.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             AsyncIterable[google.cloud.pubsublite_v1.types.StreamingCommitCursorResponse]:
@@ -338,15 +338,15 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.pubsublite_v1.types.CommitCursorRequest, dict]]):
                 The request object. Request for CommitCursor.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.CommitCursorResponse:
@@ -355,15 +355,15 @@
         # Create or coerce a protobuf request object.
         request = cursor.CommitCursorRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.commit_cursor,
-            default_retry=retries.Retry(
+            default_retry=retries.AsyncRetry(
                 initial=0.1,
                 maximum=60.0,
                 multiplier=1.3,
                 predicate=retries.if_exception_type(
                     core_exceptions.Aborted,
                     core_exceptions.DeadlineExceeded,
                     core_exceptions.InternalServerError,
@@ -441,23 +441,24 @@
                 Required. The subscription for which to retrieve
                 cursors. Structured like
                 ``projects/{project_number}/locations/{location}/subscriptions/{subscription_id}``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.cursor_service.pagers.ListPartitionCursorsAsyncPager:
                 Response for ListPartitionCursors
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -476,15 +477,15 @@
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.list_partition_cursors,
-            default_retry=retries.Retry(
+            default_retry=retries.AsyncRetry(
                 initial=0.1,
                 maximum=60.0,
                 multiplier=1.3,
                 predicate=retries.if_exception_type(
                     core_exceptions.Aborted,
                     core_exceptions.DeadlineExceeded,
                     core_exceptions.InternalServerError,
@@ -533,15 +534,15 @@
     ) -> operations_pb2.ListOperationsResponse:
         r"""Lists operations that match the specified filter in the request.
 
         Args:
             request (:class:`~.operations_pb2.ListOperationsRequest`):
                 The request object. Request message for
                 `ListOperations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.ListOperationsResponse:
                 Response message for ``ListOperations`` method.
@@ -550,15 +551,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.ListOperationsRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.list_operations,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -587,15 +588,15 @@
     ) -> operations_pb2.Operation:
         r"""Gets the latest state of a long-running operation.
 
         Args:
             request (:class:`~.operations_pb2.GetOperationRequest`):
                 The request object. Request message for
                 `GetOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.Operation:
                 An ``Operation`` object.
@@ -604,15 +605,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.GetOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.get_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -646,15 +647,15 @@
         If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.DeleteOperationRequest`):
                 The request object. Request message for
                 `DeleteOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -662,15 +663,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.DeleteOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.delete_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -700,15 +701,15 @@
         is not guaranteed.  If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.CancelOperationRequest`):
                 The request object. Request message for
                 `CancelOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -716,15 +717,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.CancelOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.cancel_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -46,15 +46,15 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.services.cursor_service import pagers
 from google.cloud.pubsublite_v1.types import cursor
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .transports.base import CursorServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import CursorServiceGrpcTransport
 from .transports.grpc_asyncio import CursorServiceGrpcAsyncIOTransport
 
 
 class CursorServiceClientMeta(type):
     """Metaclass for the CursorService client.
@@ -658,14 +658,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.services.cursor_service.pagers.ListPartitionCursorsPager:
                 Response for ListPartitionCursors
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/pagers.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/pagers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/transports/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/transports/base.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,15 +23,15 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.pubsublite_v1.types import cursor
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class CursorServiceTransport(abc.ABC):
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/transports/grpc.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.pubsublite_v1.types import cursor
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import CursorServiceTransport, DEFAULT_CLIENT_INFO
 
 
 class CursorServiceGrpcTransport(CursorServiceTransport):
     """gRPC backend transport for CursorService.
 
     The service that a subscriber client application uses to
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/cursor_service/transports/grpc_asyncio.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/cursor_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.pubsublite_v1.types import cursor
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import CursorServiceTransport, DEFAULT_CLIENT_INFO
 from .grpc import CursorServiceGrpcTransport
 
 
 class CursorServiceGrpcAsyncIOTransport(CursorServiceTransport):
     """gRPC AsyncIO backend transport for CursorService.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/async_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,25 +32,25 @@
 )
 
 from google.cloud.pubsublite_v1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
-from google.api_core import retry as retries
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 try:
-    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+    OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
-    OptionalRetry = Union[retries.Retry, object]  # type: ignore
+    OptionalRetry = Union[retries.AsyncRetry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .transports.base import PartitionAssignmentServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc_asyncio import PartitionAssignmentServiceGrpcAsyncIOTransport
 from .client import PartitionAssignmentServiceClient
 
 
 class PartitionAssignmentServiceAsyncClient:
     """The service that a subscriber client application uses to
@@ -277,15 +277,15 @@
                 async for response in stream:
                     print(response)
 
         Args:
             requests (AsyncIterator[`google.cloud.pubsublite_v1.types.PartitionAssignmentRequest`]):
                 The request object AsyncIterator. A request on the PartitionAssignment
                 stream.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             AsyncIterable[google.cloud.pubsublite_v1.types.PartitionAssignment]:
@@ -326,15 +326,15 @@
     ) -> operations_pb2.ListOperationsResponse:
         r"""Lists operations that match the specified filter in the request.
 
         Args:
             request (:class:`~.operations_pb2.ListOperationsRequest`):
                 The request object. Request message for
                 `ListOperations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.ListOperationsResponse:
                 Response message for ``ListOperations`` method.
@@ -343,15 +343,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.ListOperationsRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.list_operations,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -380,15 +380,15 @@
     ) -> operations_pb2.Operation:
         r"""Gets the latest state of a long-running operation.
 
         Args:
             request (:class:`~.operations_pb2.GetOperationRequest`):
                 The request object. Request message for
                 `GetOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.Operation:
                 An ``Operation`` object.
@@ -397,15 +397,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.GetOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.get_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -439,15 +439,15 @@
         If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.DeleteOperationRequest`):
                 The request object. Request message for
                 `DeleteOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -455,15 +455,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.DeleteOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.delete_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -493,15 +493,15 @@
         is not guaranteed.  If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.CancelOperationRequest`):
                 The request object. Request message for
                 `CancelOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -509,15 +509,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.CancelOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.cancel_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,15 +45,15 @@
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .transports.base import PartitionAssignmentServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import PartitionAssignmentServiceGrpcTransport
 from .transports.grpc_asyncio import PartitionAssignmentServiceGrpcAsyncIOTransport
 
 
 class PartitionAssignmentServiceClientMeta(type):
     """Metaclass for the PartitionAssignmentService client.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/base.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,15 +23,15 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class PartitionAssignmentServiceTransport(abc.ABC):
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/grpc.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import PartitionAssignmentServiceTransport, DEFAULT_CLIENT_INFO
 
 
 class PartitionAssignmentServiceGrpcTransport(PartitionAssignmentServiceTransport):
     """gRPC backend transport for PartitionAssignmentService.
 
     The service that a subscriber client application uses to
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/grpc_asyncio.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/partition_assignment_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import PartitionAssignmentServiceTransport, DEFAULT_CLIENT_INFO
 from .grpc import PartitionAssignmentServiceGrpcTransport
 
 
 class PartitionAssignmentServiceGrpcAsyncIOTransport(
     PartitionAssignmentServiceTransport
 ):
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/async_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,25 +32,25 @@
 )
 
 from google.cloud.pubsublite_v1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
-from google.api_core import retry as retries
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 try:
-    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+    OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
-    OptionalRetry = Union[retries.Retry, object]  # type: ignore
+    OptionalRetry = Union[retries.AsyncRetry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.types import publisher
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .transports.base import PublisherServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc_asyncio import PublisherServiceGrpcAsyncIOTransport
 from .client import PublisherServiceClient
 
 
 class PublisherServiceAsyncClient:
     """The service that a publisher client application uses to publish
@@ -273,15 +273,15 @@
                 async for response in stream:
                     print(response)
 
         Args:
             requests (AsyncIterator[`google.cloud.pubsublite_v1.types.PublishRequest`]):
                 The request object AsyncIterator. Request sent from the client to the
                 server on a stream.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             AsyncIterable[google.cloud.pubsublite_v1.types.PublishResponse]:
@@ -317,15 +317,15 @@
     ) -> operations_pb2.ListOperationsResponse:
         r"""Lists operations that match the specified filter in the request.
 
         Args:
             request (:class:`~.operations_pb2.ListOperationsRequest`):
                 The request object. Request message for
                 `ListOperations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.ListOperationsResponse:
                 Response message for ``ListOperations`` method.
@@ -334,15 +334,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.ListOperationsRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.list_operations,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -371,15 +371,15 @@
     ) -> operations_pb2.Operation:
         r"""Gets the latest state of a long-running operation.
 
         Args:
             request (:class:`~.operations_pb2.GetOperationRequest`):
                 The request object. Request message for
                 `GetOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.Operation:
                 An ``Operation`` object.
@@ -388,15 +388,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.GetOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.get_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -430,15 +430,15 @@
         If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.DeleteOperationRequest`):
                 The request object. Request message for
                 `DeleteOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -446,15 +446,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.DeleteOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.delete_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -484,15 +484,15 @@
         is not guaranteed.  If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.CancelOperationRequest`):
                 The request object. Request message for
                 `CancelOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -500,15 +500,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.CancelOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.cancel_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,15 +45,15 @@
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.types import publisher
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .transports.base import PublisherServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import PublisherServiceGrpcTransport
 from .transports.grpc_asyncio import PublisherServiceGrpcAsyncIOTransport
 
 
 class PublisherServiceClientMeta(type):
     """Metaclass for the PublisherService client.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/transports/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/transports/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/transports/base.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,15 +23,15 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.pubsublite_v1.types import publisher
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class PublisherServiceTransport(abc.ABC):
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/transports/grpc.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.pubsublite_v1.types import publisher
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import PublisherServiceTransport, DEFAULT_CLIENT_INFO
 
 
 class PublisherServiceGrpcTransport(PublisherServiceTransport):
     """gRPC backend transport for PublisherService.
 
     The service that a publisher client application uses to publish
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/publisher_service/transports/grpc_asyncio.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/publisher_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.pubsublite_v1.types import publisher
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import PublisherServiceTransport, DEFAULT_CLIENT_INFO
 from .grpc import PublisherServiceGrpcTransport
 
 
 class PublisherServiceGrpcAsyncIOTransport(PublisherServiceTransport):
     """gRPC AsyncIO backend transport for PublisherService.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/async_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,25 +32,25 @@
 )
 
 from google.cloud.pubsublite_v1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
-from google.api_core import retry as retries
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 try:
-    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+    OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
-    OptionalRetry = Union[retries.Retry, object]  # type: ignore
+    OptionalRetry = Union[retries.AsyncRetry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .transports.base import SubscriberServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc_asyncio import SubscriberServiceGrpcAsyncIOTransport
 from .client import SubscriberServiceClient
 
 
 class SubscriberServiceAsyncClient:
     """The service that a subscriber client application uses to
@@ -263,15 +263,15 @@
                 async for response in stream:
                     print(response)
 
         Args:
             requests (AsyncIterator[`google.cloud.pubsublite_v1.types.SubscribeRequest`]):
                 The request object AsyncIterator. A request sent from the client to the
                 server on a stream.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             AsyncIterable[google.cloud.pubsublite_v1.types.SubscribeResponse]:
@@ -307,15 +307,15 @@
     ) -> operations_pb2.ListOperationsResponse:
         r"""Lists operations that match the specified filter in the request.
 
         Args:
             request (:class:`~.operations_pb2.ListOperationsRequest`):
                 The request object. Request message for
                 `ListOperations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.ListOperationsResponse:
                 Response message for ``ListOperations`` method.
@@ -324,15 +324,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.ListOperationsRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.list_operations,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -361,15 +361,15 @@
     ) -> operations_pb2.Operation:
         r"""Gets the latest state of a long-running operation.
 
         Args:
             request (:class:`~.operations_pb2.GetOperationRequest`):
                 The request object. Request message for
                 `GetOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.Operation:
                 An ``Operation`` object.
@@ -378,15 +378,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.GetOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.get_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -420,15 +420,15 @@
         If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.DeleteOperationRequest`):
                 The request object. Request message for
                 `DeleteOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -436,15 +436,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.DeleteOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.delete_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -474,15 +474,15 @@
         is not guaranteed.  If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.CancelOperationRequest`):
                 The request object. Request message for
                 `CancelOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -490,15 +490,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.CancelOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.cancel_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,15 +45,15 @@
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .transports.base import SubscriberServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import SubscriberServiceGrpcTransport
 from .transports.grpc_asyncio import SubscriberServiceGrpcAsyncIOTransport
 
 
 class SubscriberServiceClientMeta(type):
     """Metaclass for the SubscriberService client.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/transports/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/transports/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/transports/base.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,15 +23,15 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class SubscriberServiceTransport(abc.ABC):
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/transports/grpc.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import SubscriberServiceTransport, DEFAULT_CLIENT_INFO
 
 
 class SubscriberServiceGrpcTransport(SubscriberServiceTransport):
     """gRPC backend transport for SubscriberService.
 
     The service that a subscriber client application uses to
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/subscriber_service/transports/grpc_asyncio.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/subscriber_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import SubscriberServiceTransport, DEFAULT_CLIENT_INFO
 from .grpc import SubscriberServiceGrpcTransport
 
 
 class SubscriberServiceGrpcAsyncIOTransport(SubscriberServiceTransport):
     """gRPC AsyncIO backend transport for SubscriberService.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/async_client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -29,26 +29,26 @@
 )
 
 from google.cloud.pubsublite_v1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
-from google.api_core import retry as retries
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 try:
-    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
+    OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
-    OptionalRetry = Union[retries.Retry, object]  # type: ignore
+    OptionalRetry = Union[retries.AsyncRetry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.types import common
 from google.cloud.pubsublite_v1.types import topic_stats
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import TopicStatsServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc_asyncio import TopicStatsServiceGrpcAsyncIOTransport
 from .client import TopicStatsServiceClient
 
 
 class TopicStatsServiceAsyncClient:
@@ -255,15 +255,15 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.pubsublite_v1.types.ComputeMessageStatsRequest, dict]]):
                 The request object. Compute statistics about a range of
                 messages in a given topic and partition.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.ComputeMessageStatsResponse:
@@ -343,15 +343,15 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.pubsublite_v1.types.ComputeHeadCursorRequest, dict]]):
                 The request object. Compute the current head cursor for a
                 partition.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.ComputeHeadCursorResponse:
@@ -426,15 +426,15 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.pubsublite_v1.types.ComputeTimeCursorRequest, dict]]):
                 The request object. Compute the corresponding cursor for
                 a publish or event time in a topic
                 partition.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.pubsublite_v1.types.ComputeTimeCursorResponse:
@@ -481,15 +481,15 @@
     ) -> operations_pb2.ListOperationsResponse:
         r"""Lists operations that match the specified filter in the request.
 
         Args:
             request (:class:`~.operations_pb2.ListOperationsRequest`):
                 The request object. Request message for
                 `ListOperations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.ListOperationsResponse:
                 Response message for ``ListOperations`` method.
@@ -498,15 +498,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.ListOperationsRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.list_operations,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -535,15 +535,15 @@
     ) -> operations_pb2.Operation:
         r"""Gets the latest state of a long-running operation.
 
         Args:
             request (:class:`~.operations_pb2.GetOperationRequest`):
                 The request object. Request message for
                 `GetOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             ~.operations_pb2.Operation:
                 An ``Operation`` object.
@@ -552,15 +552,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.GetOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.get_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -594,15 +594,15 @@
         If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.DeleteOperationRequest`):
                 The request object. Request message for
                 `DeleteOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -610,15 +610,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.DeleteOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.delete_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
@@ -648,15 +648,15 @@
         is not guaranteed.  If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.
 
         Args:
             request (:class:`~.operations_pb2.CancelOperationRequest`):
                 The request object. Request message for
                 `CancelOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors,
                     if any, should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         Returns:
             None
         """
@@ -664,15 +664,15 @@
         # The request isn't a proto-plus wrapped type,
         # so it must be constructed via keyword expansion.
         if isinstance(request, dict):
             request = operations_pb2.CancelOperationRequest(**request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
+        rpc = gapic_v1.method_async.wrap_method(
             self._client._transport.cancel_operation,
             default_timeout=None,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/client.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -44,15 +44,15 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.pubsublite_v1.types import common
 from google.cloud.pubsublite_v1.types import topic_stats
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import TopicStatsServiceTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import TopicStatsServiceGrpcTransport
 from .transports.grpc_asyncio import TopicStatsServiceGrpcAsyncIOTransport
 
 
 class TopicStatsServiceClientMeta(type):
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/transports/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/transports/base.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,15 +23,15 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.pubsublite_v1.types import topic_stats
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class TopicStatsServiceTransport(abc.ABC):
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/transports/grpc.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.pubsublite_v1.types import topic_stats
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import TopicStatsServiceTransport, DEFAULT_CLIENT_INFO
 
 
 class TopicStatsServiceGrpcTransport(TopicStatsServiceTransport):
     """gRPC backend transport for TopicStatsService.
 
     This service allows users to get stats about messages in
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/services/topic_stats_service/transports/grpc_asyncio.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/services/topic_stats_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.pubsublite_v1.types import topic_stats
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from .base import TopicStatsServiceTransport, DEFAULT_CLIENT_INFO
 from .grpc import TopicStatsServiceGrpcTransport
 
 
 class TopicStatsServiceGrpcAsyncIOTransport(TopicStatsServiceTransport):
     """gRPC AsyncIO backend transport for TopicStatsService.
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/__init__.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/admin.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/common.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/cursor.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/publisher.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,14 +45,15 @@
             The partition within the topic to which messages will be
             written. Partitions are zero indexed, so ``partition`` must
             be in the range [0, topic.num_partitions).
         client_id (bytes):
             Unique identifier for a publisher client. If
             set, enables publish idempotency within a
             publisher client session.
+
             The length of this field must be exactly 16
             bytes long and should be populated with a 128
             bit uuid, generated by standard uuid algorithms
             like uuid1 or uuid4. The same identifier should
             be reused following disconnections with
             retryable stream errors.
     """
@@ -118,14 +119,15 @@
             the batch. The cursors for any remaining
             messages in the batch are guaranteed to be
             sequential.
         cursor_ranges (MutableSequence[google.cloud.pubsublite_v1.types.MessagePublishResponse.CursorRange]):
             Cursors for messages published in the batch.
             There will exist multiple ranges when cursors
             are not contiguous within the batch.
+
             The cursor ranges may not account for all
             messages in the batch when publish idempotency
             is enabled. A missing range indicates that
             cursors could not be determined for messages
             within the range, as they were deduplicated and
             the necessary data was not available at publish
             time. These messages will have offsets when
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/subscriber.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/subscriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -310,23 +310,25 @@
     r"""The first request that must be sent on a newly-opened stream.
     The client must wait for the response before sending subsequent
     requests on the stream.
 
     Attributes:
         subscription (str):
             The subscription name. Structured like:
+
             projects/<project number>/locations/<zone
             name>/subscriptions/<subscription id>
         client_id (bytes):
             An opaque, unique client identifier. This
             field must be exactly 16 bytes long and is
             interpreted as an unsigned 128 bit integer.
             Other size values will be rejected and the
             stream will be failed with a non-retryable
             error.
+
             This field is large enough to fit a uuid from
             standard uuid algorithms like uuid1 or uuid4,
             which should be used to generate this number.
             The same identifier should be reused following
             disconnections with retryable stream errors.
     """
```

### Comparing `google-cloud-pubsublite-1.8.3/google/cloud/pubsublite_v1/types/topic_stats.py` & `google-cloud-pubsublite-1.9.0/google/cloud/pubsublite_v1/types/topic_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/PKG-INFO` & `google-cloud-pubsublite-1.9.0/google_cloud_pubsublite.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-pubsublite
-Version: 1.8.3
+Version: 1.9.0
 Summary: Google Cloud Pubsublite API client library
 Home-page: https://github.com/googleapis/python-pubsublite
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,18 +12,25 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: google-cloud-pubsub<3.0.0dev,>=2.10.0
+Requires-Dist: grpcio<2.0.0dev,>=1.38.1
+Requires-Dist: grpcio-status<2.0.0dev,>=1.38.1
+Requires-Dist: overrides<8.0.0,>=6.0.1
+Requires-Dist: overrides<8.0.0,>=7.0.1; python_version >= "3.12"
+Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,<3.0.0dev,>=1.33.2
 
 Python Client for Pub/Sub Lite API
 ==================================
 
 |stable| |pypi| |versions|
 
 `Pub/Sub Lite API`_: is designed to provide reliable,
```

### Comparing `google-cloud-pubsublite-1.8.3/google_cloud_pubsublite.egg-info/SOURCES.txt` & `google-cloud-pubsublite-1.9.0/google_cloud_pubsublite.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-google/__init__.py
-google/cloud/__init__.py
 google/cloud/pubsublite/__init__.py
 google/cloud/pubsublite/admin_client.py
 google/cloud/pubsublite/admin_client_interface.py
 google/cloud/pubsublite/gapic_version.py
 google/cloud/pubsublite/py.typed
 google/cloud/pubsublite/cloudpubsub/__init__.py
 google/cloud/pubsublite/cloudpubsub/message_transformer.py
@@ -146,20 +144,20 @@
 google/cloud/pubsublite_v1/types/cursor.py
 google/cloud/pubsublite_v1/types/publisher.py
 google/cloud/pubsublite_v1/types/subscriber.py
 google/cloud/pubsublite_v1/types/topic_stats.py
 google_cloud_pubsublite.egg-info/PKG-INFO
 google_cloud_pubsublite.egg-info/SOURCES.txt
 google_cloud_pubsublite.egg-info/dependency_links.txt
-google_cloud_pubsublite.egg-info/namespace_packages.txt
 google_cloud_pubsublite.egg-info/not-zip-safe
 google_cloud_pubsublite.egg-info/requires.txt
 google_cloud_pubsublite.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
+tests/unit/test_packaging.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/pubsublite_v1/__init__.py
 tests/unit/gapic/pubsublite_v1/test_admin_service.py
 tests/unit/gapic/pubsublite_v1/test_cursor_service.py
 tests/unit/gapic/pubsublite_v1/test_partition_assignment_service.py
 tests/unit/gapic/pubsublite_v1/test_publisher_service.py
 tests/unit/gapic/pubsublite_v1/test_subscriber_service.py
```

### Comparing `google-cloud-pubsublite-1.8.3/setup.py` & `google-cloud-pubsublite-1.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,35 +35,32 @@
 else:
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-cloud-pubsub >= 2.10.0, <3.0.0dev",
     "grpcio >= 1.38.1, <2.0.0dev",
     "grpcio-status >= 1.38.1, <2.0.0dev",
-    "overrides>=6.0.1, <7.0.0",
+    "overrides>=6.0.1, <8.0.0",
+    "overrides>=7.0.1, <8.0.0; python_version>='3.12'",
     "google-api-core[grpc] >= 1.33.2, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
 ]
 url = "https://github.com/googleapis/python-pubsublite"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 packages = [
     package
-    for package in setuptools.PEP420PackageFinder.find()
+    for package in setuptools.find_namespace_packages()
     if package.startswith("google")
 ]
 
-namespaces = ["google"]
-if "google.cloud" in packages:
-    namespaces.append("google.cloud")
-
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
     author_email="googleapis-packages@google.com",
@@ -75,18 +72,18 @@
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
         "Topic :: Internet",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     python_requires=">=3.8",
-    namespace_packages=namespaces,
     install_requires=dependencies,
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/__init__.py` & `google-cloud-pubsublite-1.9.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/__init__.py` & `google-cloud-pubsublite-1.9.0/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/gapic/__init__.py` & `google-cloud-pubsublite-1.9.0/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/__init__.py` & `google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_admin_service.py` & `google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_admin_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -43,15 +43,15 @@
 from google.auth.exceptions import MutualTLSChannelError
 from google.cloud.pubsublite_v1.services.admin_service import AdminServiceAsyncClient
 from google.cloud.pubsublite_v1.services.admin_service import AdminServiceClient
 from google.cloud.pubsublite_v1.services.admin_service import pagers
 from google.cloud.pubsublite_v1.services.admin_service import transports
 from google.cloud.pubsublite_v1.types import admin
 from google.cloud.pubsublite_v1.types import common
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import google.auth
 
 
@@ -6968,15 +6968,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_delete_operation_async(transport: str = "grpc"):
+async def test_delete_operation_async(transport: str = "grpc_asyncio"):
     client = AdminServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -7107,15 +7107,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_cancel_operation_async(transport: str = "grpc"):
+async def test_cancel_operation_async(transport: str = "grpc_asyncio"):
     client = AdminServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -7246,15 +7246,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.Operation)
 
 
 @pytest.mark.asyncio
-async def test_get_operation_async(transport: str = "grpc"):
+async def test_get_operation_async(transport: str = "grpc_asyncio"):
     client = AdminServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -7391,15 +7391,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.ListOperationsResponse)
 
 
 @pytest.mark.asyncio
-async def test_list_operations_async(transport: str = "grpc"):
+async def test_list_operations_async(transport: str = "grpc_asyncio"):
     client = AdminServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_cursor_service.py` & `google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_cursor_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -39,15 +39,15 @@
 from google.auth.exceptions import MutualTLSChannelError
 from google.cloud.pubsublite_v1.services.cursor_service import CursorServiceAsyncClient
 from google.cloud.pubsublite_v1.services.cursor_service import CursorServiceClient
 from google.cloud.pubsublite_v1.services.cursor_service import pagers
 from google.cloud.pubsublite_v1.services.cursor_service import transports
 from google.cloud.pubsublite_v1.types import common
 from google.cloud.pubsublite_v1.types import cursor
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account
 import google.auth
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
@@ -2022,15 +2022,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_delete_operation_async(transport: str = "grpc"):
+async def test_delete_operation_async(transport: str = "grpc_asyncio"):
     client = CursorServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -2161,15 +2161,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_cancel_operation_async(transport: str = "grpc"):
+async def test_cancel_operation_async(transport: str = "grpc_asyncio"):
     client = CursorServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -2300,15 +2300,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.Operation)
 
 
 @pytest.mark.asyncio
-async def test_get_operation_async(transport: str = "grpc"):
+async def test_get_operation_async(transport: str = "grpc_asyncio"):
     client = CursorServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -2445,15 +2445,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.ListOperationsResponse)
 
 
 @pytest.mark.asyncio
-async def test_list_operations_async(transport: str = "grpc"):
+async def test_list_operations_async(transport: str = "grpc_asyncio"):
     client = CursorServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_partition_assignment_service.py` & `google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_partition_assignment_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -41,15 +41,15 @@
     PartitionAssignmentServiceAsyncClient,
 )
 from google.cloud.pubsublite_v1.services.partition_assignment_service import (
     PartitionAssignmentServiceClient,
 )
 from google.cloud.pubsublite_v1.services.partition_assignment_service import transports
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account
 import google.auth
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
@@ -1446,15 +1446,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_delete_operation_async(transport: str = "grpc"):
+async def test_delete_operation_async(transport: str = "grpc_asyncio"):
     client = PartitionAssignmentServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1585,15 +1585,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_cancel_operation_async(transport: str = "grpc"):
+async def test_cancel_operation_async(transport: str = "grpc_asyncio"):
     client = PartitionAssignmentServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1724,15 +1724,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.Operation)
 
 
 @pytest.mark.asyncio
-async def test_get_operation_async(transport: str = "grpc"):
+async def test_get_operation_async(transport: str = "grpc_asyncio"):
     client = PartitionAssignmentServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1869,15 +1869,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.ListOperationsResponse)
 
 
 @pytest.mark.asyncio
-async def test_list_operations_async(transport: str = "grpc"):
+async def test_list_operations_async(transport: str = "grpc_asyncio"):
     client = PartitionAssignmentServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_publisher_service.py` & `google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_publisher_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -40,15 +40,15 @@
 from google.cloud.pubsublite_v1.services.publisher_service import (
     PublisherServiceAsyncClient,
 )
 from google.cloud.pubsublite_v1.services.publisher_service import PublisherServiceClient
 from google.cloud.pubsublite_v1.services.publisher_service import transports
 from google.cloud.pubsublite_v1.types import common
 from google.cloud.pubsublite_v1.types import publisher
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account
 from google.protobuf import timestamp_pb2  # type: ignore
 import google.auth
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
@@ -1419,15 +1419,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_delete_operation_async(transport: str = "grpc"):
+async def test_delete_operation_async(transport: str = "grpc_asyncio"):
     client = PublisherServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1558,15 +1558,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_cancel_operation_async(transport: str = "grpc"):
+async def test_cancel_operation_async(transport: str = "grpc_asyncio"):
     client = PublisherServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1697,15 +1697,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.Operation)
 
 
 @pytest.mark.asyncio
-async def test_get_operation_async(transport: str = "grpc"):
+async def test_get_operation_async(transport: str = "grpc_asyncio"):
     client = PublisherServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1842,15 +1842,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.ListOperationsResponse)
 
 
 @pytest.mark.asyncio
-async def test_list_operations_async(transport: str = "grpc"):
+async def test_list_operations_async(transport: str = "grpc_asyncio"):
     client = PublisherServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_subscriber_service.py` & `google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_subscriber_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -42,15 +42,15 @@
 )
 from google.cloud.pubsublite_v1.services.subscriber_service import (
     SubscriberServiceClient,
 )
 from google.cloud.pubsublite_v1.services.subscriber_service import transports
 from google.cloud.pubsublite_v1.types import common
 from google.cloud.pubsublite_v1.types import subscriber
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account
 import google.auth
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
@@ -1420,15 +1420,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_delete_operation_async(transport: str = "grpc"):
+async def test_delete_operation_async(transport: str = "grpc_asyncio"):
     client = SubscriberServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1559,15 +1559,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_cancel_operation_async(transport: str = "grpc"):
+async def test_cancel_operation_async(transport: str = "grpc_asyncio"):
     client = SubscriberServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1698,15 +1698,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.Operation)
 
 
 @pytest.mark.asyncio
-async def test_get_operation_async(transport: str = "grpc"):
+async def test_get_operation_async(transport: str = "grpc_asyncio"):
     client = SubscriberServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1843,15 +1843,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.ListOperationsResponse)
 
 
 @pytest.mark.asyncio
-async def test_list_operations_async(transport: str = "grpc"):
+async def test_list_operations_async(transport: str = "grpc_asyncio"):
     client = SubscriberServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/gapic/pubsublite_v1/test_topic_stats_service.py` & `google-cloud-pubsublite-1.9.0/tests/unit/gapic/pubsublite_v1/test_topic_stats_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -42,15 +42,15 @@
 )
 from google.cloud.pubsublite_v1.services.topic_stats_service import (
     TopicStatsServiceClient,
 )
 from google.cloud.pubsublite_v1.services.topic_stats_service import transports
 from google.cloud.pubsublite_v1.types import common
 from google.cloud.pubsublite_v1.types import topic_stats
-from google.longrunning import operations_pb2
+from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account
 from google.protobuf import timestamp_pb2  # type: ignore
 import google.auth
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
@@ -1851,15 +1851,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_delete_operation_async(transport: str = "grpc"):
+async def test_delete_operation_async(transport: str = "grpc_asyncio"):
     client = TopicStatsServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -1990,15 +1990,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
-async def test_cancel_operation_async(transport: str = "grpc"):
+async def test_cancel_operation_async(transport: str = "grpc_asyncio"):
     client = TopicStatsServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -2129,15 +2129,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.Operation)
 
 
 @pytest.mark.asyncio
-async def test_get_operation_async(transport: str = "grpc"):
+async def test_get_operation_async(transport: str = "grpc_asyncio"):
     client = TopicStatsServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
@@ -2274,15 +2274,15 @@
         assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, operations_pb2.ListOperationsResponse)
 
 
 @pytest.mark.asyncio
-async def test_list_operations_async(transport: str = "grpc"):
+async def test_list_operations_async(transport: str = "grpc_asyncio"):
     client = TopicStatsServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
```

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/ack_set_tracker_impl_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/ack_set_tracker_impl_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/assigning_subscriber_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/assigning_subscriber_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/async_client_multiplexer_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/async_client_multiplexer_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/client_multiplexer_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/client_multiplexer_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/multiplexed_async_subscriber_client_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/multiplexed_async_subscriber_client_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/multiplexed_publisher_client_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/multiplexed_publisher_client_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/publisher_impl_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/publisher_impl_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/single_partition_subscriber_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/single_partition_subscriber_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/internal/subscriber_impl_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/internal/subscriber_impl_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/cloudpubsub/message_transforms_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/cloudpubsub/message_transforms_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/assigner_impl_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/assigner_impl_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/committer_impl_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/committer_impl_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/default_routing_policy_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/default_routing_policy_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/flow_control_batcher_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/flow_control_batcher_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/gapic_connection_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/gapic_connection_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/partition_count_watcher_impl_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/partition_count_watcher_impl_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/partition_count_watching_publisher_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/partition_count_watching_publisher_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/reset_signal_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/reset_signal_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/retrying_connection_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/retrying_connection_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/routing_tests.json` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/routing_tests.json`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/single_partition_publisher_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/single_partition_publisher_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-pubsublite-1.8.3/tests/unit/pubsublite/internal/wire/subscriber_impl_test.py` & `google-cloud-pubsublite-1.9.0/tests/unit/pubsublite/internal/wire/subscriber_impl_test.py`

 * *Files identical despite different names*

