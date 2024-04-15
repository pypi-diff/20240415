# Comparing `tmp/gaboost-1.8.1.tar.gz` & `tmp/gaboost-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaboost-1.8.1.tar", last modified: Wed Jan  3 10:18:15 2024, max compression
+gzip compressed data, was "gaboost-1.8.2.tar", last modified: Mon Apr 15 10:36:30 2024, max compression
```

## Comparing `gaboost-1.8.1.tar` & `gaboost-1.8.2.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.768431 gaboost-1.8.1/
--rw-rw-rw-   0        0        0    11558 2022-08-02 07:14:48.000000 gaboost-1.8.1/LICENSE
--rw-rw-rw-   0        0        0       68 2023-03-29 06:23:28.000000 gaboost-1.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1462 2024-01-03 10:18:15.766296 gaboost-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0    22066 2023-04-20 03:18:22.000000 gaboost-1.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.406012 gaboost-1.8.1/funboost/
--rw-rw-rw-   0        0        0    20789 2023-04-20 03:46:06.000000 gaboost-1.8.1/funboost/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.408191 gaboost-1.8.1/funboost/assist/
--rw-rw-rw-   0        0        0     2858 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/assist/user_custom_broker_register.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.410719 gaboost-1.8.1/funboost/beggar_version_implementation/
--rw-rw-rw-   0        0        0     3930 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/beggar_version_implementation/beggar_redis_consumer.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.438953 gaboost-1.8.1/funboost/concurrent_pool/
--rw-rw-rw-   0        0        0      689 2023-06-29 07:38:24.000000 gaboost-1.8.1/funboost/concurrent_pool/__init__.py
--rw-rw-rw-   0        0        0     3256 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/concurrent_pool/async_helper.py
--rw-rw-rw-   0        0        0     7227 2023-03-29 02:20:08.000000 gaboost-1.8.1/funboost/concurrent_pool/async_pool_executor.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.447119 gaboost-1.8.1/funboost/concurrent_pool/backup/
--rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/concurrent_pool/backup/__init__.py
--rw-rw-rw-   0        0        0     9548 2023-03-29 02:20:08.000000 gaboost-1.8.1/funboost/concurrent_pool/backup/async_pool_executor0223.py
--rw-rw-rw-   0        0        0     9568 2023-03-29 02:20:08.000000 gaboost-1.8.1/funboost/concurrent_pool/backup/async_pool_executor_back.py
--rw-rw-rw-   0        0        0     5728 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/concurrent_pool/backup/async_pool_executor_janus.py
--rw-rw-rw-   0        0        0     4723 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py
--rw-rw-rw-   0        0        0     3011 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/concurrent_pool/bounded_processpoolexcutor_py36.py
--rw-rw-rw-   0        0        0     1571 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/concurrent_pool/bounded_threadpoolexcutor.py
--rw-rw-rw-   0        0        0     1693 2023-06-29 08:14:12.000000 gaboost-1.8.1/funboost/concurrent_pool/concurrent_pool_with_multi_process.py
--rw-rw-rw-   0        0        0        0 2023-03-28 13:05:23.000000 gaboost-1.8.1/funboost/concurrent_pool/custom_evenlet_pool_executor.py
--rw-rw-rw-   0        0        0     4273 2023-06-29 07:45:55.000000 gaboost-1.8.1/funboost/concurrent_pool/custom_gevent_pool_executor.py
--rw-rw-rw-   0        0        0    11504 2023-11-13 07:25:20.000000 gaboost-1.8.1/funboost/concurrent_pool/custom_threadpool_executor.py
--rw-rw-rw-   0        0        0     9317 2022-08-02 08:43:39.000000 gaboost-1.8.1/funboost/concurrent_pool/custom_threadpool_executor000.py
--rw-rw-rw-   0        0        0      373 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/concurrent_pool/single_thread_executor.py
--rw-rw-rw-   0        0        0     5629 2023-06-29 07:32:16.000000 gaboost-1.8.1/funboost/constant.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.515052 gaboost-1.8.1/funboost/consumers/
--rw-rw-rw-   0        0        0      126 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/__init__.py
--rw-rw-rw-   0        0        0    93184 2023-12-14 14:35:31.000000 gaboost-1.8.1/funboost/consumers/base_consumer.py
--rw-rw-rw-   0        0        0     5877 2023-04-20 03:18:22.000000 gaboost-1.8.1/funboost/consumers/confirm_mixin.py
--rw-rw-rw-   0        0        0     2045 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/http_consumer.py
--rw-rw-rw-   0        0        0     4463 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/http_consumer000.py
--rw-rw-rw-   0        0        0     1058 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/httpsqs_consumer.py
--rw-rw-rw-   0        0        0     4294 2023-07-26 10:08:26.000000 gaboost-1.8.1/funboost/consumers/kafka_consumer.py
--rw-rw-rw-   0        0        0     6640 2024-01-03 09:36:12.000000 gaboost-1.8.1/funboost/consumers/kafka_consumer_manually_commit.py
--rw-rw-rw-   0        0        0     5082 2023-03-29 02:23:37.000000 gaboost-1.8.1/funboost/consumers/kombu_consumer.py
--rw-rw-rw-   0        0        0     1356 2023-07-26 10:46:53.000000 gaboost-1.8.1/funboost/consumers/local_python_queue_consumer.py
--rw-rw-rw-   0        0        0     1069 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/mongomq_consumer.py
--rw-rw-rw-   0        0        0     2208 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/mqtt_consumer.py
--rw-rw-rw-   0        0        0     1054 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/consumers/nats_consumer.py
--rw-rw-rw-   0        0        0     1440 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/nsq_consumer.py
--rw-rw-rw-   0        0        0     1218 2023-04-20 03:18:22.000000 gaboost-1.8.1/funboost/consumers/peewee_conusmer.py
--rw-rw-rw-   0        0        0      982 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/persist_queue_consumer.py
--rw-rw-rw-   0        0        0     1791 2023-04-20 03:18:22.000000 gaboost-1.8.1/funboost/consumers/pulsar_consumer.py
--rw-rw-rw-   0        0        0     1901 2023-11-07 08:00:36.000000 gaboost-1.8.1/funboost/consumers/rabbitmq_amqpstorm_consumer.py
--rw-rw-rw-   0        0        0     5412 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/rabbitmq_pika_consumer.py
--rw-rw-rw-   0        0        0     4653 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/rabbitmq_pika_consumerv0.py
--rw-rw-rw-   0        0        0     1239 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/rabbitmq_rabbitpy_consumer.py
--rw-rw-rw-   0        0        0     3067 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/redis_brpoplpush_consumer.py
--rw-rw-rw-   0        0        0     2928 2023-12-14 13:56:53.000000 gaboost-1.8.1/funboost/consumers/redis_consumer.py
--rw-rw-rw-   0        0        0     4338 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/redis_consumer_ack_able.py
--rw-rw-rw-   0        0        0     1109 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/redis_consumer_simple.py
--rw-rw-rw-   0        0        0     7190 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/redis_filter.py
--rw-rw-rw-   0        0        0     1184 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/redis_pubsub_consumer.py
--rw-rw-rw-   0        0        0     6740 2023-12-14 13:56:53.000000 gaboost-1.8.1/funboost/consumers/redis_stream_consumer.py
--rw-rw-rw-   0        0        0     1633 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/rocketmq_consumer.py
--rw-rw-rw-   0        0        0     1289 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/sqlachemy_consumer.py
--rw-rw-rw-   0        0        0     2025 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/tcp_consumer.py
--rw-rw-rw-   0        0        0     1322 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/txt_file_consumer.py
--rw-rw-rw-   0        0        0     1625 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/udp_consumer.py
--rw-rw-rw-   0        0        0     4137 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/consumers/zeromq_consumer.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.520833 gaboost-1.8.1/funboost/contrib/
--rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/contrib/__init__.py
--rw-rw-rw-   0        0        0     4703 2023-04-20 03:18:22.000000 gaboost-1.8.1/funboost/contrib/queue2queue.py
--rw-rw-rw-   0        0        0     1817 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/contrib/redis_consume_latest_msg_broker.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.525965 gaboost-1.8.1/funboost/factories/
--rw-rw-rw-   0        0        0      178 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/factories/__init__.py
--rw-rw-rw-   0        0        0     2512 2024-01-03 09:38:08.000000 gaboost-1.8.1/funboost/factories/consumer_factory.py
--rw-rw-rw-   0        0        0     4429 2024-01-03 10:16:33.000000 gaboost-1.8.1/funboost/factories/publisher_factotry.py
--rw-rw-rw-   0        0        0     6684 2023-04-20 03:18:22.000000 gaboost-1.8.1/funboost/funboost_config_deafult.py
--rw-rw-rw-   0        0        0    14118 2023-04-20 03:21:07.000000 gaboost-1.8.1/funboost/helpers.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.586643 gaboost-1.8.1/funboost/publishers/
--rw-rw-rw-   0        0        0      131 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/__init__.py
--rw-rw-rw-   0        0        0    14959 2023-07-26 10:16:58.000000 gaboost-1.8.1/funboost/publishers/base_publisher.py
--rw-rw-rw-   0        0        0     3541 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/confluent_kafka_publisher.py
--rw-rw-rw-   0        0        0      777 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/http_publisher.py
--rw-rw-rw-   0        0        0     2783 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/httpsqs_publisher.py
--rw-rw-rw-   0        0        0     2160 2023-04-20 03:18:22.000000 gaboost-1.8.1/funboost/publishers/kafka_publisher.py
--rw-rw-rw-   0        0        0     4567 2023-03-29 02:23:37.000000 gaboost-1.8.1/funboost/publishers/kombu_publisher.py
--rw-rw-rw-   0        0        0     1365 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/local_python_queue_publisher.py
--rw-rw-rw-   0        0        0     1874 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/mongomq_publisher.py
--rw-rw-rw-   0        0        0     3050 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/mqtt_publisher.py
--rw-rw-rw-   0        0        0     7881 2023-07-26 09:34:20.000000 gaboost-1.8.1/funboost/publishers/msg_result_getter.py
--rw-rw-rw-   0        0        0      776 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/publishers/nats_publisher.py
--rw-rw-rw-   0        0        0     1302 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/nsq_publisher.py
--rw-rw-rw-   0        0        0     1095 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/peewee_publisher.py
--rw-rw-rw-   0        0        0     2540 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/persist_queue_publisher.py
--rw-rw-rw-   0        0        0     1085 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/pulsar_publisher.py
--rw-rw-rw-   0        0        0     2687 2023-04-20 03:18:22.000000 gaboost-1.8.1/funboost/publishers/rabbitmq_amqpstorm_publisher.py
--rw-rw-rw-   0        0        0     2343 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/rabbitmq_pika_publisher.py
--rw-rw-rw-   0        0        0     1953 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/rabbitmq_rabbitpy_publisher.py
--rw-rw-rw-   0        0        0     3950 2023-03-29 02:04:48.000000 gaboost-1.8.1/funboost/publishers/redis_publisher.py
--rw-rw-rw-   0        0        0      278 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/redis_publisher_lpush.py
--rw-rw-rw-   0        0        0      872 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/redis_publisher_simple.py
--rw-rw-rw-   0        0        0      721 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/redis_pubsub_publisher.py
--rw-rw-rw-   0        0        0     2141 2022-09-01 07:50:53.000000 gaboost-1.8.1/funboost/publishers/redis_stream_publisher.py
--rw-rw-rw-   0        0        0     2343 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/rocketmq_publisher.py
--rw-rw-rw-   0        0        0     1215 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/sqla_queue_publisher.py
--rw-rw-rw-   0        0        0     1359 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/tcp_publisher.py
--rw-rw-rw-   0        0        0     1380 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/txt_file_publisher.py
--rw-rw-rw-   0        0        0     1218 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/publishers/udp_publisher.py
--rw-rw-rw-   0        0        0     1002 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/publishers/zeromq_publisher.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.592028 gaboost-1.8.1/funboost/queues/
--rw-rw-rw-   0        0        0        0 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/queues/__init__.py
--rw-rw-rw-   0        0        0     4982 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/queues/peewee_queue.py
--rw-rw-rw-   0        0        0    11186 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/queues/sqla_queue.py
--rw-rw-rw-   0        0        0     9134 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/set_frame_config.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.599761 gaboost-1.8.1/funboost/timing_job/
--rw-rw-rw-   0        0        0     4098 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/timing_job/__init__.py
--rw-rw-rw-   0        0        0      418 2023-04-20 03:18:22.000000 gaboost-1.8.1/funboost/timing_job/apscheduler_use_mysql_store.py
--rw-rw-rw-   0        0        0      868 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/timing_job/apscheduler_use_redis_store.py
--rw-rw-rw-   0        0        0      996 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/timing_job/push_fun_for_apscheduler_use_db.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.639520 gaboost-1.8.1/funboost/utils/
--rw-rw-rw-   0        0        0     1951 2023-07-26 09:32:51.000000 gaboost-1.8.1/funboost/utils/__init__.py
--rw-rw-rw-   0        0        0     3124 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/apscheduler_monkey.py
--rw-rw-rw-   0        0        0       96 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/block_exit.py
--rw-rw-rw-   0        0        0    10063 2022-08-09 01:46:39.000000 gaboost-1.8.1/funboost/utils/bulk_operation.py
--rw-rw-rw-   0        0        0     5923 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/custom_pysnooper.py
--rw-rw-rw-   0        0        0    24240 2024-01-03 10:12:17.000000 gaboost-1.8.1/funboost/utils/decorators.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.641475 gaboost-1.8.1/funboost/utils/dependency_packages/
--rw-rw-rw-   0        0        0        0 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/dependency_packages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.653345 gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/
--rw-rw-rw-   0        0        0      131 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/__init__.py
--rw-rw-rw-   0        0        0     2486 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/lock.py
--rw-rw-rw-   0        0        0     7902 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/mongomq.py
--rw-rw-rw-   0        0        0     7867 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/mongomq0000.py
--rw-rw-rw-   0        0        0     4811 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/test.py
--rw-rw-rw-   0        0        0      377 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.656889 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.661884 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/__pycache__/
--rw-rw-rw-   0        0        0      324 2023-03-29 02:15:53.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-310.pyc
--rw-rw-rw-   0        0        0      481 2023-06-29 08:08:35.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-311.pyc
--rw-rw-rw-   0        0        0      341 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.684178 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/
--rw-rw-rw-   0        0        0     1282 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.712557 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/
--rw-rw-rw-   0        0        0     1214 2023-03-29 02:15:56.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1702 2023-06-29 08:08:38.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0   156125 2023-03-29 02:15:56.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-310.pyc
--rw-rw-rw-   0        0        0   238828 2023-06-29 08:08:38.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-311.pyc
--rw-rw-rw-   0        0        0      358 2023-03-29 02:15:56.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-310.pyc
--rw-rw-rw-   0        0        0      445 2023-06-29 08:08:38.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-311.pyc
--rw-rw-rw-   0        0        0    42622 2023-03-29 02:15:56.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-310.pyc
--rw-rw-rw-   0        0        0    79452 2023-06-29 08:08:38.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-311.pyc
--rw-rw-rw-   0        0        0     2907 2023-03-29 02:15:56.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-310.pyc
--rw-rw-rw-   0        0        0     4286 2023-06-29 08:08:38.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-311.pyc
--rw-rw-rw-   0        0        0    10275 2023-03-29 02:15:56.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-310.pyc
--rw-rw-rw-   0        0        0    14354 2023-06-29 08:08:38.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-311.pyc
--rw-rw-rw-   0        0        0     2053 2023-03-29 02:15:56.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     2932 2023-06-29 08:08:38.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-   0        0        0   187456 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py
--rw-rw-rw-   0        0        0      191 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py
--rw-rw-rw-   0        0        0    63907 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py
--rw-rw-rw-   0        0        0     1682 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py
--rw-rw-rw-   0        0        0    11957 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py
--rw-rw-rw-   0        0        0      442 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/log.py
--rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/py.typed
--rw-rw-rw-   0        0        0      617 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md
--rw-rw-rw-   0        0        0    12865 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py
--rw-rw-rw-   0        0        0     1345 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.724124 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/
--rw-rw-rw-   0        0        0     5379 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py
--rw-rw-rw-   0        0        0      603 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.743107 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/
--rw-rw-rw-   0        0        0     5094 2023-03-29 02:20:11.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-310.pyc
--rw-rw-rw-   0        0        0     6490 2023-06-29 08:08:39.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-311.pyc
--rw-rw-rw-   0        0        0      775 2023-03-29 02:20:11.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      863 2023-06-29 08:08:39.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     7995 2023-03-29 02:20:11.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-310.pyc
--rw-rw-rw-   0        0        0    11453 2023-06-29 08:08:39.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-311.pyc
--rw-rw-rw-   0        0        0     3742 2023-03-29 02:20:11.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-310.pyc
--rw-rw-rw-   0        0        0     4598 2023-06-29 08:08:39.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-311.pyc
--rw-rw-rw-   0        0        0      315 2023-03-29 02:20:11.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-310.pyc
--rw-rw-rw-   0        0        0      363 2023-06-29 08:08:39.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-311.pyc
--rw-rw-rw-   0        0        0     9531 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py
--rw-rw-rw-   0        0        0     4072 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py
--rw-rw-rw-   0        0        0      176 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py
--rw-rw-rw-   0        0        0      287 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py
--rw-rw-rw-   0        0        0      545 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/readme.md
--rw-rw-rw-   0        0        0      251 2022-08-02 08:43:39.000000 gaboost-1.8.1/funboost/utils/develop_log.py
--rw-rw-rw-   0        0        0     2984 2023-04-20 03:18:22.000000 gaboost-1.8.1/funboost/utils/mongo_util.py
--rw-rw-rw-   0        0        0     7367 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/monkey_color_log.py
--rw-rw-rw-   0        0        0     2882 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/monkey_patches.py
--rw-rw-rw-   0        0        0     3199 2022-08-02 08:43:39.000000 gaboost-1.8.1/funboost/utils/mqtt_util.py
--rw-rw-rw-   0        0        0     4901 2022-08-02 08:43:39.000000 gaboost-1.8.1/funboost/utils/paramiko_util.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.753495 gaboost-1.8.1/funboost/utils/pysnooper_ydf/
--rw-rw-rw-   0        0        0      909 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/pysnooper_ydf/__init__.py
--rw-rw-rw-   0        0        0     2243 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/pysnooper_ydf/pycompat.py
--rw-rw-rw-   0        0        0    19131 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/pysnooper_ydf/tracer.py
--rw-rw-rw-   0        0        0     2753 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/pysnooper_ydf/utils.py
--rw-rw-rw-   0        0        0     3693 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/pysnooper_ydf/variables.py
--rw-rw-rw-   0        0        0     2963 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/rabbitmq_factory.py
--rw-rw-rw-   0        0        0     4856 2024-01-03 10:15:30.000000 gaboost-1.8.1/funboost/utils/redis_manager.py
--rw-rw-rw-   0        0        0     5532 2023-03-28 12:34:36.000000 gaboost-1.8.1/funboost/utils/resource_monitoring.py
--rw-rw-rw-   0        0        0     1418 2023-03-29 02:20:08.000000 gaboost-1.8.1/funboost/utils/restart_python.py
--rw-rw-rw-   0        0        0     1204 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/simple_data_class.py
--rw-rw-rw-   0        0        0     5407 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/time_util.py
--rw-rw-rw-   0        0        0      408 2022-08-02 07:14:48.000000 gaboost-1.8.1/funboost/utils/un_strict_json_dumps.py
-drwxrwxrwx   0        0        0        0 2024-01-03 10:18:15.764193 gaboost-1.8.1/gaboost.egg-info/
--rw-rw-rw-   0        0        0     1462 2024-01-03 10:18:15.000000 gaboost-1.8.1/gaboost.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9477 2024-01-03 10:18:15.000000 gaboost-1.8.1/gaboost.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-03 10:18:15.000000 gaboost-1.8.1/gaboost.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      283 2024-01-03 10:18:15.000000 gaboost-1.8.1/gaboost.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-03 10:18:15.000000 gaboost-1.8.1/gaboost.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-03 10:18:15.769512 gaboost-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0     4004 2024-01-03 10:17:50.000000 gaboost-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.453699 gaboost-1.8.2/
+-rw-rw-rw-   0        0        0    11558 2022-08-02 07:14:48.000000 gaboost-1.8.2/LICENSE
+-rw-rw-rw-   0        0        0       68 2023-03-29 06:23:28.000000 gaboost-1.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1462 2024-04-15 10:36:30.447200 gaboost-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0    22066 2023-04-20 03:18:22.000000 gaboost-1.8.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:29.826648 gaboost-1.8.2/funboost/
+-rw-rw-rw-   0        0        0    20789 2023-04-20 03:46:06.000000 gaboost-1.8.2/funboost/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:29.828608 gaboost-1.8.2/funboost/assist/
+-rw-rw-rw-   0        0        0     2858 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/assist/user_custom_broker_register.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:29.831030 gaboost-1.8.2/funboost/beggar_version_implementation/
+-rw-rw-rw-   0        0        0     3930 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/beggar_version_implementation/beggar_redis_consumer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:29.857723 gaboost-1.8.2/funboost/concurrent_pool/
+-rw-rw-rw-   0        0        0      689 2023-06-29 07:38:24.000000 gaboost-1.8.2/funboost/concurrent_pool/__init__.py
+-rw-rw-rw-   0        0        0     3256 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/concurrent_pool/async_helper.py
+-rw-rw-rw-   0        0        0     7227 2023-03-29 02:20:08.000000 gaboost-1.8.2/funboost/concurrent_pool/async_pool_executor.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:29.868284 gaboost-1.8.2/funboost/concurrent_pool/backup/
+-rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/concurrent_pool/backup/__init__.py
+-rw-rw-rw-   0        0        0     9548 2023-03-29 02:20:08.000000 gaboost-1.8.2/funboost/concurrent_pool/backup/async_pool_executor0223.py
+-rw-rw-rw-   0        0        0     9568 2023-03-29 02:20:08.000000 gaboost-1.8.2/funboost/concurrent_pool/backup/async_pool_executor_back.py
+-rw-rw-rw-   0        0        0     5728 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/concurrent_pool/backup/async_pool_executor_janus.py
+-rw-rw-rw-   0        0        0     4723 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py
+-rw-rw-rw-   0        0        0     3011 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/concurrent_pool/bounded_processpoolexcutor_py36.py
+-rw-rw-rw-   0        0        0     1571 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/concurrent_pool/bounded_threadpoolexcutor.py
+-rw-rw-rw-   0        0        0     1693 2023-06-29 08:14:12.000000 gaboost-1.8.2/funboost/concurrent_pool/concurrent_pool_with_multi_process.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 13:05:23.000000 gaboost-1.8.2/funboost/concurrent_pool/custom_evenlet_pool_executor.py
+-rw-rw-rw-   0        0        0     4273 2023-06-29 07:45:55.000000 gaboost-1.8.2/funboost/concurrent_pool/custom_gevent_pool_executor.py
+-rw-rw-rw-   0        0        0    11504 2023-11-13 07:25:20.000000 gaboost-1.8.2/funboost/concurrent_pool/custom_threadpool_executor.py
+-rw-rw-rw-   0        0        0     9317 2022-08-02 08:43:39.000000 gaboost-1.8.2/funboost/concurrent_pool/custom_threadpool_executor000.py
+-rw-rw-rw-   0        0        0      373 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/concurrent_pool/single_thread_executor.py
+-rw-rw-rw-   0        0        0     5629 2023-06-29 07:32:16.000000 gaboost-1.8.2/funboost/constant.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:29.985067 gaboost-1.8.2/funboost/consumers/
+-rw-rw-rw-   0        0        0      126 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/__init__.py
+-rw-rw-rw-   0        0        0    93184 2023-12-14 14:35:31.000000 gaboost-1.8.2/funboost/consumers/base_consumer.py
+-rw-rw-rw-   0        0        0     5877 2023-04-20 03:18:22.000000 gaboost-1.8.2/funboost/consumers/confirm_mixin.py
+-rw-rw-rw-   0        0        0     2045 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/http_consumer.py
+-rw-rw-rw-   0        0        0     4463 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/http_consumer000.py
+-rw-rw-rw-   0        0        0     1058 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/httpsqs_consumer.py
+-rw-rw-rw-   0        0        0     4326 2024-04-15 10:33:18.000000 gaboost-1.8.2/funboost/consumers/kafka_consumer.py
+-rw-rw-rw-   0        0        0     6640 2024-01-03 09:36:12.000000 gaboost-1.8.2/funboost/consumers/kafka_consumer_manually_commit.py
+-rw-rw-rw-   0        0        0     5082 2023-03-29 02:23:37.000000 gaboost-1.8.2/funboost/consumers/kombu_consumer.py
+-rw-rw-rw-   0        0        0     1356 2023-07-26 10:46:53.000000 gaboost-1.8.2/funboost/consumers/local_python_queue_consumer.py
+-rw-rw-rw-   0        0        0     1069 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/mongomq_consumer.py
+-rw-rw-rw-   0        0        0     2208 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/mqtt_consumer.py
+-rw-rw-rw-   0        0        0     1054 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/consumers/nats_consumer.py
+-rw-rw-rw-   0        0        0     1440 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/nsq_consumer.py
+-rw-rw-rw-   0        0        0     1218 2023-04-20 03:18:22.000000 gaboost-1.8.2/funboost/consumers/peewee_conusmer.py
+-rw-rw-rw-   0        0        0      982 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/persist_queue_consumer.py
+-rw-rw-rw-   0        0        0     1791 2023-04-20 03:18:22.000000 gaboost-1.8.2/funboost/consumers/pulsar_consumer.py
+-rw-rw-rw-   0        0        0     1901 2023-11-07 08:00:36.000000 gaboost-1.8.2/funboost/consumers/rabbitmq_amqpstorm_consumer.py
+-rw-rw-rw-   0        0        0     5412 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/rabbitmq_pika_consumer.py
+-rw-rw-rw-   0        0        0     4653 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/rabbitmq_pika_consumerv0.py
+-rw-rw-rw-   0        0        0     1239 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/rabbitmq_rabbitpy_consumer.py
+-rw-rw-rw-   0        0        0     3067 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/redis_brpoplpush_consumer.py
+-rw-rw-rw-   0        0        0     2960 2024-04-15 10:31:03.000000 gaboost-1.8.2/funboost/consumers/redis_consumer.py
+-rw-rw-rw-   0        0        0     4338 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/redis_consumer_ack_able.py
+-rw-rw-rw-   0        0        0     1109 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/redis_consumer_simple.py
+-rw-rw-rw-   0        0        0     7190 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/redis_filter.py
+-rw-rw-rw-   0        0        0     1184 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/redis_pubsub_consumer.py
+-rw-rw-rw-   0        0        0     6772 2024-04-15 10:33:18.000000 gaboost-1.8.2/funboost/consumers/redis_stream_consumer.py
+-rw-rw-rw-   0        0        0     1633 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/rocketmq_consumer.py
+-rw-rw-rw-   0        0        0     1289 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/sqlachemy_consumer.py
+-rw-rw-rw-   0        0        0     2025 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/tcp_consumer.py
+-rw-rw-rw-   0        0        0     1322 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/txt_file_consumer.py
+-rw-rw-rw-   0        0        0     1625 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/udp_consumer.py
+-rw-rw-rw-   0        0        0     4137 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/consumers/zeromq_consumer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:29.993522 gaboost-1.8.2/funboost/contrib/
+-rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/contrib/__init__.py
+-rw-rw-rw-   0        0        0     4703 2023-04-20 03:18:22.000000 gaboost-1.8.2/funboost/contrib/queue2queue.py
+-rw-rw-rw-   0        0        0     1817 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/contrib/redis_consume_latest_msg_broker.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.001994 gaboost-1.8.2/funboost/factories/
+-rw-rw-rw-   0        0        0      178 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/factories/__init__.py
+-rw-rw-rw-   0        0        0     2512 2024-01-03 09:38:08.000000 gaboost-1.8.2/funboost/factories/consumer_factory.py
+-rw-rw-rw-   0        0        0     4429 2024-01-03 10:16:33.000000 gaboost-1.8.2/funboost/factories/publisher_factotry.py
+-rw-rw-rw-   0        0        0     6684 2023-04-20 03:18:22.000000 gaboost-1.8.2/funboost/funboost_config_deafult.py
+-rw-rw-rw-   0        0        0    14118 2023-04-20 03:21:07.000000 gaboost-1.8.2/funboost/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.101044 gaboost-1.8.2/funboost/publishers/
+-rw-rw-rw-   0        0        0      131 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/__init__.py
+-rw-rw-rw-   0        0        0    14991 2024-04-15 10:33:48.000000 gaboost-1.8.2/funboost/publishers/base_publisher.py
+-rw-rw-rw-   0        0        0     3541 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/confluent_kafka_publisher.py
+-rw-rw-rw-   0        0        0      777 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/http_publisher.py
+-rw-rw-rw-   0        0        0     2783 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/httpsqs_publisher.py
+-rw-rw-rw-   0        0        0     2160 2023-04-20 03:18:22.000000 gaboost-1.8.2/funboost/publishers/kafka_publisher.py
+-rw-rw-rw-   0        0        0     4567 2023-03-29 02:23:37.000000 gaboost-1.8.2/funboost/publishers/kombu_publisher.py
+-rw-rw-rw-   0        0        0     1365 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/local_python_queue_publisher.py
+-rw-rw-rw-   0        0        0     1874 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/mongomq_publisher.py
+-rw-rw-rw-   0        0        0     3050 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/mqtt_publisher.py
+-rw-rw-rw-   0        0        0     7881 2023-07-26 09:34:20.000000 gaboost-1.8.2/funboost/publishers/msg_result_getter.py
+-rw-rw-rw-   0        0        0      776 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/publishers/nats_publisher.py
+-rw-rw-rw-   0        0        0     1302 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/nsq_publisher.py
+-rw-rw-rw-   0        0        0     1095 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/peewee_publisher.py
+-rw-rw-rw-   0        0        0     2540 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/persist_queue_publisher.py
+-rw-rw-rw-   0        0        0     1085 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/pulsar_publisher.py
+-rw-rw-rw-   0        0        0     2687 2023-04-20 03:18:22.000000 gaboost-1.8.2/funboost/publishers/rabbitmq_amqpstorm_publisher.py
+-rw-rw-rw-   0        0        0     2343 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/rabbitmq_pika_publisher.py
+-rw-rw-rw-   0        0        0     1953 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/rabbitmq_rabbitpy_publisher.py
+-rw-rw-rw-   0        0        0     3950 2023-03-29 02:04:48.000000 gaboost-1.8.2/funboost/publishers/redis_publisher.py
+-rw-rw-rw-   0        0        0      278 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/redis_publisher_lpush.py
+-rw-rw-rw-   0        0        0      872 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/redis_publisher_simple.py
+-rw-rw-rw-   0        0        0      721 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/redis_pubsub_publisher.py
+-rw-rw-rw-   0        0        0     2141 2022-09-01 07:50:53.000000 gaboost-1.8.2/funboost/publishers/redis_stream_publisher.py
+-rw-rw-rw-   0        0        0     2343 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/rocketmq_publisher.py
+-rw-rw-rw-   0        0        0     1215 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/sqla_queue_publisher.py
+-rw-rw-rw-   0        0        0     1359 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/tcp_publisher.py
+-rw-rw-rw-   0        0        0     1380 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/txt_file_publisher.py
+-rw-rw-rw-   0        0        0     1218 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/publishers/udp_publisher.py
+-rw-rw-rw-   0        0        0     1002 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/publishers/zeromq_publisher.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.116434 gaboost-1.8.2/funboost/queues/
+-rw-rw-rw-   0        0        0        0 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/queues/__init__.py
+-rw-rw-rw-   0        0        0     4982 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/queues/peewee_queue.py
+-rw-rw-rw-   0        0        0    11186 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/queues/sqla_queue.py
+-rw-rw-rw-   0        0        0     9134 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/set_frame_config.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.126436 gaboost-1.8.2/funboost/timing_job/
+-rw-rw-rw-   0        0        0     4098 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/timing_job/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-04-20 03:18:22.000000 gaboost-1.8.2/funboost/timing_job/apscheduler_use_mysql_store.py
+-rw-rw-rw-   0        0        0      868 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/timing_job/apscheduler_use_redis_store.py
+-rw-rw-rw-   0        0        0      996 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/timing_job/push_fun_for_apscheduler_use_db.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.178569 gaboost-1.8.2/funboost/utils/
+-rw-rw-rw-   0        0        0     1951 2023-07-26 09:32:51.000000 gaboost-1.8.2/funboost/utils/__init__.py
+-rw-rw-rw-   0        0        0     3124 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/apscheduler_monkey.py
+-rw-rw-rw-   0        0        0       96 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/block_exit.py
+-rw-rw-rw-   0        0        0    10063 2022-08-09 01:46:39.000000 gaboost-1.8.2/funboost/utils/bulk_operation.py
+-rw-rw-rw-   0        0        0     5923 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/custom_pysnooper.py
+-rw-rw-rw-   0        0        0    24240 2024-01-03 10:12:17.000000 gaboost-1.8.2/funboost/utils/decorators.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.181517 gaboost-1.8.2/funboost/utils/dependency_packages/
+-rw-rw-rw-   0        0        0        0 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/dependency_packages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.202004 gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/
+-rw-rw-rw-   0        0        0      131 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/__init__.py
+-rw-rw-rw-   0        0        0     2486 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/lock.py
+-rw-rw-rw-   0        0        0     7902 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/mongomq.py
+-rw-rw-rw-   0        0        0     7867 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/mongomq0000.py
+-rw-rw-rw-   0        0        0     4811 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/test.py
+-rw-rw-rw-   0        0        0      377 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.207867 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.214341 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/__pycache__/
+-rw-rw-rw-   0        0        0      324 2023-03-29 02:15:53.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-310.pyc
+-rw-rw-rw-   0        0        0      481 2023-06-29 08:08:35.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/__pycache__/add_to_pythonpath.cpython-311.pyc
+-rw-rw-rw-   0        0        0      341 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/add_to_pythonpath.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.250624 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/
+-rw-rw-rw-   0        0        0     1282 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.318157 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/
+-rw-rw-rw-   0        0        0     1214 2023-03-29 02:15:56.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1702 2023-06-29 08:08:38.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0   156125 2023-03-29 02:15:56.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-310.pyc
+-rw-rw-rw-   0        0        0   238828 2023-06-29 08:08:38.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-311.pyc
+-rw-rw-rw-   0        0        0      358 2023-03-29 02:15:56.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-310.pyc
+-rw-rw-rw-   0        0        0      445 2023-06-29 08:08:38.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/compat.cpython-311.pyc
+-rw-rw-rw-   0        0        0    42622 2023-03-29 02:15:56.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-310.pyc
+-rw-rw-rw-   0        0        0    79452 2023-06-29 08:08:38.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2907 2023-03-29 02:15:56.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4286 2023-06-29 08:08:38.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10275 2023-03-29 02:15:56.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-310.pyc
+-rw-rw-rw-   0        0        0    14354 2023-06-29 08:08:38.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2053 2023-03-29 02:15:56.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2932 2023-06-29 08:08:38.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0   187456 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py
+-rw-rw-rw-   0        0        0      191 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/compat.py
+-rw-rw-rw-   0        0        0    63907 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py
+-rw-rw-rw-   0        0        0     1682 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py
+-rw-rw-rw-   0        0        0    11957 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py
+-rw-rw-rw-   0        0        0      442 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/log.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/py.typed
+-rw-rw-rw-   0        0        0      617 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md
+-rw-rw-rw-   0        0        0    12865 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py
+-rw-rw-rw-   0        0        0     1345 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.335880 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/
+-rw-rw-rw-   0        0        0     5379 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py
+-rw-rw-rw-   0        0        0      603 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.373568 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/
+-rw-rw-rw-   0        0        0     5094 2023-03-29 02:20:11.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6490 2023-06-29 08:08:39.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-311.pyc
+-rw-rw-rw-   0        0        0      775 2023-03-29 02:20:11.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      863 2023-06-29 08:08:39.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7995 2023-03-29 02:20:11.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11453 2023-06-29 08:08:39.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3742 2023-03-29 02:20:11.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4598 2023-06-29 08:08:39.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-311.pyc
+-rw-rw-rw-   0        0        0      315 2023-03-29 02:20:11.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-310.pyc
+-rw-rw-rw-   0        0        0      363 2023-06-29 08:08:39.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9531 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py
+-rw-rw-rw-   0        0        0     4072 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py
+-rw-rw-rw-   0        0        0      176 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/py2_raise.py
+-rw-rw-rw-   0        0        0      287 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/py3_raise.py
+-rw-rw-rw-   0        0        0      545 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/readme.md
+-rw-rw-rw-   0        0        0      251 2022-08-02 08:43:39.000000 gaboost-1.8.2/funboost/utils/develop_log.py
+-rw-rw-rw-   0        0        0     2984 2023-04-20 03:18:22.000000 gaboost-1.8.2/funboost/utils/mongo_util.py
+-rw-rw-rw-   0        0        0     7367 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/monkey_color_log.py
+-rw-rw-rw-   0        0        0     2882 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/monkey_patches.py
+-rw-rw-rw-   0        0        0     3199 2022-08-02 08:43:39.000000 gaboost-1.8.2/funboost/utils/mqtt_util.py
+-rw-rw-rw-   0        0        0     4901 2022-08-02 08:43:39.000000 gaboost-1.8.2/funboost/utils/paramiko_util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.394022 gaboost-1.8.2/funboost/utils/pysnooper_ydf/
+-rw-rw-rw-   0        0        0      909 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/pysnooper_ydf/__init__.py
+-rw-rw-rw-   0        0        0     2243 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/pysnooper_ydf/pycompat.py
+-rw-rw-rw-   0        0        0    19131 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/pysnooper_ydf/tracer.py
+-rw-rw-rw-   0        0        0     2753 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/pysnooper_ydf/utils.py
+-rw-rw-rw-   0        0        0     3693 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/pysnooper_ydf/variables.py
+-rw-rw-rw-   0        0        0     2963 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/rabbitmq_factory.py
+-rw-rw-rw-   0        0        0     4856 2024-01-03 10:15:30.000000 gaboost-1.8.2/funboost/utils/redis_manager.py
+-rw-rw-rw-   0        0        0     5532 2023-03-28 12:34:36.000000 gaboost-1.8.2/funboost/utils/resource_monitoring.py
+-rw-rw-rw-   0        0        0     1418 2023-03-29 02:20:08.000000 gaboost-1.8.2/funboost/utils/restart_python.py
+-rw-rw-rw-   0        0        0     1204 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/simple_data_class.py
+-rw-rw-rw-   0        0        0     5407 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/time_util.py
+-rw-rw-rw-   0        0        0      408 2022-08-02 07:14:48.000000 gaboost-1.8.2/funboost/utils/un_strict_json_dumps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:36:30.444173 gaboost-1.8.2/gaboost.egg-info/
+-rw-rw-rw-   0        0        0     1462 2024-04-15 10:36:29.000000 gaboost-1.8.2/gaboost.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9477 2024-04-15 10:36:29.000000 gaboost-1.8.2/gaboost.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 10:36:29.000000 gaboost-1.8.2/gaboost.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      283 2024-04-15 10:36:29.000000 gaboost-1.8.2/gaboost.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 10:36:29.000000 gaboost-1.8.2/gaboost.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 10:36:30.453699 gaboost-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     4004 2024-04-15 10:35:16.000000 gaboost-1.8.2/setup.py
```

### Comparing `gaboost-1.8.1/LICENSE` & `gaboost-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/PKG-INFO` & `gaboost-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaboost
-Version: 1.8.1
+Version: 1.8.2
 Summary: fork funboost
 Author: ziko
 License: BSD License
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `gaboost-1.8.1/README.md` & `gaboost-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/__init__.py` & `gaboost-1.8.2/funboost/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/assist/user_custom_broker_register.py` & `gaboost-1.8.2/funboost/assist/user_custom_broker_register.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/beggar_version_implementation/beggar_redis_consumer.py` & `gaboost-1.8.2/funboost/beggar_version_implementation/beggar_redis_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/__init__.py` & `gaboost-1.8.2/funboost/concurrent_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/async_helper.py` & `gaboost-1.8.2/funboost/concurrent_pool/async_helper.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/async_pool_executor.py` & `gaboost-1.8.2/funboost/concurrent_pool/async_pool_executor.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/backup/async_pool_executor0223.py` & `gaboost-1.8.2/funboost/concurrent_pool/backup/async_pool_executor0223.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/backup/async_pool_executor_back.py` & `gaboost-1.8.2/funboost/concurrent_pool/backup/async_pool_executor_back.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/backup/async_pool_executor_janus.py` & `gaboost-1.8.2/funboost/concurrent_pool/backup/async_pool_executor_janus.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py` & `gaboost-1.8.2/funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/bounded_processpoolexcutor_py36.py` & `gaboost-1.8.2/funboost/concurrent_pool/bounded_processpoolexcutor_py36.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/bounded_threadpoolexcutor.py` & `gaboost-1.8.2/funboost/concurrent_pool/bounded_threadpoolexcutor.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/concurrent_pool_with_multi_process.py` & `gaboost-1.8.2/funboost/concurrent_pool/concurrent_pool_with_multi_process.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/custom_gevent_pool_executor.py` & `gaboost-1.8.2/funboost/concurrent_pool/custom_gevent_pool_executor.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/custom_threadpool_executor.py` & `gaboost-1.8.2/funboost/concurrent_pool/custom_threadpool_executor.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/concurrent_pool/custom_threadpool_executor000.py` & `gaboost-1.8.2/funboost/concurrent_pool/custom_threadpool_executor000.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/constant.py` & `gaboost-1.8.2/funboost/constant.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/base_consumer.py` & `gaboost-1.8.2/funboost/consumers/base_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/confirm_mixin.py` & `gaboost-1.8.2/funboost/consumers/confirm_mixin.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/http_consumer.py` & `gaboost-1.8.2/funboost/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/http_consumer000.py` & `gaboost-1.8.2/funboost/consumers/http_consumer000.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/httpsqs_consumer.py` & `gaboost-1.8.2/funboost/consumers/httpsqs_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/kafka_consumer.py` & `gaboost-1.8.2/funboost/consumers/kafka_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,8 +70,8 @@
             kw = {'consumer': consumer, 'message': message, 'body': orjson.loads(message.value)}
             self._submit_task(kw)
 
     def _confirm_consume(self, kw):
         pass  # 使用kafka的自动commit模式。
 
     def _requeue(self, kw):
-        self._producer.send(self._queue_name, orjson.dumps(kw['body']))
+        self._producer.send(self._queue_name, orjson.dumps(kw['body'], option=orjson.OPT_NON_STR_KEYS))
```

### Comparing `gaboost-1.8.1/funboost/consumers/kafka_consumer_manually_commit.py` & `gaboost-1.8.2/funboost/consumers/kafka_consumer_manually_commit.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/kombu_consumer.py` & `gaboost-1.8.2/funboost/consumers/kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/local_python_queue_consumer.py` & `gaboost-1.8.2/funboost/consumers/local_python_queue_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/mongomq_consumer.py` & `gaboost-1.8.2/funboost/consumers/mongomq_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/mqtt_consumer.py` & `gaboost-1.8.2/funboost/consumers/mqtt_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/nats_consumer.py` & `gaboost-1.8.2/funboost/consumers/nats_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/nsq_consumer.py` & `gaboost-1.8.2/funboost/consumers/nsq_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/peewee_conusmer.py` & `gaboost-1.8.2/funboost/consumers/peewee_conusmer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/persist_queue_consumer.py` & `gaboost-1.8.2/funboost/consumers/persist_queue_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/pulsar_consumer.py` & `gaboost-1.8.2/funboost/consumers/pulsar_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/rabbitmq_amqpstorm_consumer.py` & `gaboost-1.8.2/funboost/consumers/rabbitmq_amqpstorm_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/rabbitmq_pika_consumer.py` & `gaboost-1.8.2/funboost/consumers/rabbitmq_pika_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/rabbitmq_pika_consumerv0.py` & `gaboost-1.8.2/funboost/consumers/rabbitmq_pika_consumerv0.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/rabbitmq_rabbitpy_consumer.py` & `gaboost-1.8.2/funboost/consumers/rabbitmq_rabbitpy_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/redis_brpoplpush_consumer.py` & `gaboost-1.8.2/funboost/consumers/redis_brpoplpush_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/redis_consumer.py` & `gaboost-1.8.2/funboost/consumers/redis_consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,8 +57,8 @@
             if self._stop_flag:
                 break
 
     def _confirm_consume(self, kw):
         pass  # redis没有确认消费的功能。
 
     def _requeue(self, kw):
-        self.redis_db_frame.rpush(self._queue_name, orjson.dumps(kw['body']))
+        self.redis_db_frame.rpush(self._queue_name, orjson.dumps(kw['body'], option=orjson.OPT_NON_STR_KEYS))
```

### Comparing `gaboost-1.8.1/funboost/consumers/redis_consumer_ack_able.py` & `gaboost-1.8.2/funboost/consumers/redis_consumer_ack_able.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/redis_consumer_simple.py` & `gaboost-1.8.2/funboost/consumers/redis_consumer_simple.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/redis_filter.py` & `gaboost-1.8.2/funboost/consumers/redis_filter.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/redis_pubsub_consumer.py` & `gaboost-1.8.2/funboost/consumers/redis_pubsub_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/redis_stream_consumer.py` & `gaboost-1.8.2/funboost/consumers/redis_stream_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         with self.redis_db_frame_version3.pipeline() as pipe:
             pipe.xack(self._queue_name, self.GROUP, kw['msg_id'])
             pipe.xdel(self._queue_name, kw['msg_id'])  # 直接删除不需要保留， 便于xlen
             pipe.execute()
 
     def _requeue(self, kw):
         self.redis_db_frame_version3.xack(self._queue_name, self.GROUP, kw['msg_id'])
-        self.redis_db_frame_version3.xadd(self._queue_name, {'': orjson.dumps(kw['body']).decode()})
+        self.redis_db_frame_version3.xadd(self._queue_name, {'': orjson.dumps(kw['body'], option=orjson.OPT_NON_STR_KEYS).decode()})
         # print(self.redis_db_frame_version3.xclaim(self._queue_name,
         #                                     'distributed_frame_group', self.consumer_identification,
         #                                     min_idle_time=0, message_ids=[kw['msg_id']]))
 
     def _requeue_tasks_which_unconfirmed(self):
         lock_key = f'funboost_lock__requeue_tasks_which_unconfirmed:{self._queue_name}'
         with decorators.RedisDistributedLockContextManager(self.redis_db_frame, lock_key, ) as lock:
```

### Comparing `gaboost-1.8.1/funboost/consumers/rocketmq_consumer.py` & `gaboost-1.8.2/funboost/consumers/rocketmq_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/sqlachemy_consumer.py` & `gaboost-1.8.2/funboost/consumers/sqlachemy_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/tcp_consumer.py` & `gaboost-1.8.2/funboost/consumers/tcp_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/txt_file_consumer.py` & `gaboost-1.8.2/funboost/consumers/txt_file_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/udp_consumer.py` & `gaboost-1.8.2/funboost/consumers/udp_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/consumers/zeromq_consumer.py` & `gaboost-1.8.2/funboost/consumers/zeromq_consumer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/contrib/queue2queue.py` & `gaboost-1.8.2/funboost/contrib/queue2queue.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/contrib/redis_consume_latest_msg_broker.py` & `gaboost-1.8.2/funboost/contrib/redis_consume_latest_msg_broker.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/factories/consumer_factory.py` & `gaboost-1.8.2/funboost/factories/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/factories/publisher_factotry.py` & `gaboost-1.8.2/funboost/factories/publisher_factotry.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/funboost_config_deafult.py` & `gaboost-1.8.2/funboost/funboost_config_deafult.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/helpers.py` & `gaboost-1.8.2/funboost/helpers.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/base_publisher.py` & `gaboost-1.8.2/funboost/publishers/base_publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         task_id = task_id or f'{self._queue_name}_result:{uuid.uuid4()}'
         msg['extra'] = extra_params = {'task_id': task_id, 'publish_time': round(time.time(), 4),
                                        'publish_time_format': time.strftime('%Y-%m-%d %H:%M:%S')}
         if priority_control_config:
             extra_params.update(priority_control_config.to_dict())
         t_start = time.time()
         decorators.handle_exception(retry_times=10, is_throw_error=True, time_sleep=0.1)(
-            self.concrete_realization_of_publish)(orjson.dumps(msg))
+            self.concrete_realization_of_publish)(orjson.dumps(msg, option=orjson.OPT_NON_STR_KEYS))
         self.logger.debug(f'向{self._queue_name} 队列，推送消息 耗时{round(time.time() - t_start, 4)}秒  {msg_function_kw}')  # 显示msg太长了。
         with self._lock_for_count:
             self.count_per_minute += 1
             self.publish_msg_num_total += 1
             if time.time() - self._current_time > 10:
                 self.logger.info(
                     f'10秒内推送了 {self.count_per_minute} 条消息,累计推送了 {self.publish_msg_num_total} 条消息到 {self._queue_name} 队列中')
```

### Comparing `gaboost-1.8.1/funboost/publishers/confluent_kafka_publisher.py` & `gaboost-1.8.2/funboost/publishers/confluent_kafka_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/http_publisher.py` & `gaboost-1.8.2/funboost/publishers/http_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/httpsqs_publisher.py` & `gaboost-1.8.2/funboost/publishers/httpsqs_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/kafka_publisher.py` & `gaboost-1.8.2/funboost/publishers/kafka_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/kombu_publisher.py` & `gaboost-1.8.2/funboost/publishers/kombu_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/local_python_queue_publisher.py` & `gaboost-1.8.2/funboost/publishers/local_python_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/mongomq_publisher.py` & `gaboost-1.8.2/funboost/publishers/mongomq_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/mqtt_publisher.py` & `gaboost-1.8.2/funboost/publishers/mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/msg_result_getter.py` & `gaboost-1.8.2/funboost/publishers/msg_result_getter.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/nats_publisher.py` & `gaboost-1.8.2/funboost/publishers/nats_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/nsq_publisher.py` & `gaboost-1.8.2/funboost/publishers/nsq_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/peewee_publisher.py` & `gaboost-1.8.2/funboost/publishers/peewee_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/persist_queue_publisher.py` & `gaboost-1.8.2/funboost/publishers/persist_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/pulsar_publisher.py` & `gaboost-1.8.2/funboost/publishers/pulsar_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/rabbitmq_amqpstorm_publisher.py` & `gaboost-1.8.2/funboost/publishers/rabbitmq_amqpstorm_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/rabbitmq_pika_publisher.py` & `gaboost-1.8.2/funboost/publishers/rabbitmq_pika_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/rabbitmq_rabbitpy_publisher.py` & `gaboost-1.8.2/funboost/publishers/rabbitmq_rabbitpy_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/redis_publisher.py` & `gaboost-1.8.2/funboost/publishers/redis_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/redis_publisher_simple.py` & `gaboost-1.8.2/funboost/publishers/redis_publisher_simple.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/redis_pubsub_publisher.py` & `gaboost-1.8.2/funboost/publishers/redis_pubsub_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/redis_stream_publisher.py` & `gaboost-1.8.2/funboost/publishers/redis_stream_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/rocketmq_publisher.py` & `gaboost-1.8.2/funboost/publishers/rocketmq_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/sqla_queue_publisher.py` & `gaboost-1.8.2/funboost/publishers/sqla_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/tcp_publisher.py` & `gaboost-1.8.2/funboost/publishers/tcp_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/txt_file_publisher.py` & `gaboost-1.8.2/funboost/publishers/txt_file_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/udp_publisher.py` & `gaboost-1.8.2/funboost/publishers/udp_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/publishers/zeromq_publisher.py` & `gaboost-1.8.2/funboost/publishers/zeromq_publisher.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/queues/peewee_queue.py` & `gaboost-1.8.2/funboost/queues/peewee_queue.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/queues/sqla_queue.py` & `gaboost-1.8.2/funboost/queues/sqla_queue.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/set_frame_config.py` & `gaboost-1.8.2/funboost/set_frame_config.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/timing_job/__init__.py` & `gaboost-1.8.2/funboost/timing_job/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/timing_job/apscheduler_use_redis_store.py` & `gaboost-1.8.2/funboost/timing_job/apscheduler_use_redis_store.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/timing_job/push_fun_for_apscheduler_use_db.py` & `gaboost-1.8.2/funboost/timing_job/push_fun_for_apscheduler_use_db.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/__init__.py` & `gaboost-1.8.2/funboost/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/apscheduler_monkey.py` & `gaboost-1.8.2/funboost/utils/apscheduler_monkey.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/bulk_operation.py` & `gaboost-1.8.2/funboost/utils/bulk_operation.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/custom_pysnooper.py` & `gaboost-1.8.2/funboost/utils/custom_pysnooper.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/decorators.py` & `gaboost-1.8.2/funboost/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/lock.py` & `gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/lock.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/mongomq.py` & `gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/mongomq.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/mongomq0000.py` & `gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/mongomq0000.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages/mongomq/test.py` & `gaboost-1.8.2/funboost/utils/dependency_packages/mongomq/test.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/connection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/lock.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/client.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/connection.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/lock.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/readme.md`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/sentinel.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/aioredis/utils.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/StoppableThread.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/StoppableThread.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/dafunc.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-310.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-311.pyc` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/dafunc.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/func_timeout/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/dependency_packages_in_pythonpath/readme.md` & `gaboost-1.8.2/funboost/utils/dependency_packages_in_pythonpath/readme.md`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/mongo_util.py` & `gaboost-1.8.2/funboost/utils/mongo_util.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/monkey_color_log.py` & `gaboost-1.8.2/funboost/utils/monkey_color_log.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/monkey_patches.py` & `gaboost-1.8.2/funboost/utils/monkey_patches.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/mqtt_util.py` & `gaboost-1.8.2/funboost/utils/mqtt_util.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/paramiko_util.py` & `gaboost-1.8.2/funboost/utils/paramiko_util.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/pysnooper_ydf/__init__.py` & `gaboost-1.8.2/funboost/utils/pysnooper_ydf/__init__.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/pysnooper_ydf/pycompat.py` & `gaboost-1.8.2/funboost/utils/pysnooper_ydf/pycompat.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/pysnooper_ydf/tracer.py` & `gaboost-1.8.2/funboost/utils/pysnooper_ydf/tracer.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/pysnooper_ydf/utils.py` & `gaboost-1.8.2/funboost/utils/pysnooper_ydf/utils.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/pysnooper_ydf/variables.py` & `gaboost-1.8.2/funboost/utils/pysnooper_ydf/variables.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/rabbitmq_factory.py` & `gaboost-1.8.2/funboost/utils/rabbitmq_factory.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/redis_manager.py` & `gaboost-1.8.2/funboost/utils/redis_manager.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/resource_monitoring.py` & `gaboost-1.8.2/funboost/utils/resource_monitoring.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/restart_python.py` & `gaboost-1.8.2/funboost/utils/restart_python.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/simple_data_class.py` & `gaboost-1.8.2/funboost/utils/simple_data_class.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/funboost/utils/time_util.py` & `gaboost-1.8.2/funboost/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/gaboost.egg-info/PKG-INFO` & `gaboost-1.8.2/gaboost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaboost
-Version: 1.8.1
+Version: 1.8.2
 Summary: fork funboost
 Author: ziko
 License: BSD License
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `gaboost-1.8.1/gaboost.egg-info/SOURCES.txt` & `gaboost-1.8.2/gaboost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaboost-1.8.1/setup.py` & `gaboost-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='gaboost',  #
-    version='1.8.1',
+    version='1.8.2',
     description=(
         'fork funboost'
     ),
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     # keywords=["funboost", "distributed-framework", "function-scheduling", "rabbitmq", "rocketmq", "kafka", "nsq", "redis", "disk",
     #           "sqlachemy", "consume-confirm", "timing", "task-scheduling", "apscheduler", "pulsar", "mqtt", "kombu"],
     #long_description_content_type="text/markdown",
```

