# Comparing `tmp/faststream-0.5.0rc1.tar.gz` & `tmp/faststream-0.5.0rc2.tar.gz`

## Comparing `faststream-0.5.0rc1.tar` & `faststream-0.5.0rc2.tar`

### file list

```diff
@@ -1,323 +1,322 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/SECURITY.md
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/serve.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/__main__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/annotations.py
--rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/py.typed
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/security.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/__init__.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/message.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/proto.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/router.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/schemas.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/types.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    12951 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/message.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/parser.py
--rw-r--r--   0        0        0    19994 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/security.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/testing.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    19107 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    64895 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0    99679 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/message.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/parser.py
--rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/security.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/testing.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    29222 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    65255 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   111507 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/log/logging.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/annotations.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/message.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/parser.py
--rw-r--r--   0        0        0    12261 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/router.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/security.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/testing.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    26786 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    11855 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36215 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/router.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    19378 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/message.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/parser.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/router.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/security.py
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27539 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    17110 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0    21150 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/testing/app.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/data.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/README.md
--rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/SECURITY.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/annotations.py
+-rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/security.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/types.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    64951 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/security.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    28966 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    65311 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   111563 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/log/logging.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/annotations.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/helpers.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/message.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/parser.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/security.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    14872 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/message.py
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/security.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15687 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27558 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    21257 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/testing/app.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/README.md
+-rw-r--r--   0        0        0    10240 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    19960 2020-02-02 00:00:00.000000 faststream-0.5.0rc2/PKG-INFO
```

### Comparing `faststream-0.5.0rc1/.pre-commit-config.yaml` & `faststream-0.5.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.secrets.baseline` & `faststream-0.5.0rc2/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/CITATION.cff` & `faststream-0.5.0rc2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/CODE_OF_CONDUCT.md` & `faststream-0.5.0rc2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/CONTRIBUTING.md` & `faststream-0.5.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/SECURITY.md` & `faststream-0.5.0rc2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.0rc2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/dependabot.yml` & `faststream-0.5.0rc2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.0rc2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.0rc2/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/workflows/codeql.yml` & `faststream-0.5.0rc2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/workflows/dependency-review.yaml` & `faststream-0.5.0rc2/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/workflows/deploy-docs.yaml` & `faststream-0.5.0rc2/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/workflows/publish_coverage.yml` & `faststream-0.5.0rc2/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/workflows/publish_pypi.yml` & `faststream-0.5.0rc2/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/workflows/test.yaml` & `faststream-0.5.0rc2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/.github/workflows/update_release_notes.yaml` & `faststream-0.5.0rc2/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/e02_1_basic_publisher.py` & `faststream-0.5.0rc2/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/e02_2_basic_publisher.py` & `faststream-0.5.0rc2/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/e02_3_basic_publisher.py` & `faststream-0.5.0rc2/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/e03_miltiple_pubsub.py` & `faststream-0.5.0rc2/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/e04_msg_filter.py` & `faststream-0.5.0rc2/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/e07_ack_immediately.py` & `faststream-0.5.0rc2/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/e09_testing_mocks.py` & `faststream-0.5.0rc2/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/e10_middlewares.py` & `faststream-0.5.0rc2/examples/e10_middlewares.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from contextlib import asynccontextmanager
 from types import TracebackType
-from typing import Optional, Type
+from typing import Any, Awaitable, Callable, Optional, Type
 
 from faststream import BaseMiddleware, FastStream
-from faststream.rabbit import RabbitBroker
-from faststream.types import DecodedMessage
+from faststream.rabbit import RabbitBroker, RabbitMessage
 
 
 class TopLevelMiddleware(BaseMiddleware):
     async def on_receive(self) -> None:
         print(f"call toplevel middleware with msg: {self.msg}")
         return await super().on_receive()
 
@@ -18,29 +16,33 @@
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> bool:
         print("highlevel middleware out")
         return await super().after_processed(exc_type, exc_val, exc_tb)
 
 
-@asynccontextmanager
-async def HandlerMiddleware(msg: DecodedMessage) -> DecodedMessage:
+async def subscriber_middleware(
+    call_next: Callable[[Any], Awaitable[Any]],
+    msg: RabbitMessage,
+) -> Any:
     print(f"call handler middleware with body: {msg}")
-    yield "fake message"
+    msg.decoded_body = "fake message"
+    result = await call_next(msg)
     print("handler middleware out")
+    return result
 
 
 broker = RabbitBroker(
     "amqp://guest:guest@localhost:5672/",
     middlewares=(TopLevelMiddleware,),
 )
 app = FastStream(broker)
 
 
-@broker.subscriber("test", middlewares=(HandlerMiddleware,))
+@broker.subscriber("test", middlewares=(subscriber_middleware,))
 async def handle(msg):
     assert msg == "fake message"
 
 
 @app.after_startup
 async def test_publish():
     await broker.publish("message", "test")
```

### Comparing `faststream-0.5.0rc1/examples/e11_settings.py` & `faststream-0.5.0rc2/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/fastapi_integration/testing.py` & `faststream-0.5.0rc2/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/howto/structlogs.py` & `faststream-0.5.0rc2/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/kafka/testing.py` & `faststream-0.5.0rc2/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/nats/e03_publisher.py` & `faststream-0.5.0rc2/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/nats/e04_js_basic.py` & `faststream-0.5.0rc2/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/nats/e05_basic_and_js.py` & `faststream-0.5.0rc2/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/nats/e06_key_value.py` & `faststream-0.5.0rc2/examples/nats/e06_key_value.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/nats/e07_object_storage.py` & `faststream-0.5.0rc2/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/rabbit/direct.py` & `faststream-0.5.0rc2/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/rabbit/fanout.py` & `faststream-0.5.0rc2/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/rabbit/header.py` & `faststream-0.5.0rc2/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/rabbit/topic.py` & `faststream-0.5.0rc2/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/redis/channel_sub_pattern.py` & `faststream-0.5.0rc2/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/redis/rpc.py` & `faststream-0.5.0rc2/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/router/basic_publish.py` & `faststream-0.5.0rc2/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/serialization/avro/avro.py` & `faststream-0.5.0rc2/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/serialization/msgpack/pack.py` & `faststream-0.5.0rc2/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.0rc2/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/__init__.py` & `faststream-0.5.0rc2/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/_compat.py` & `faststream-0.5.0rc2/faststream/_compat.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/app.py` & `faststream-0.5.0rc2/faststream/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/exceptions.py` & `faststream-0.5.0rc2/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/security.py` & `faststream-0.5.0rc2/faststream/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/types.py` & `faststream-0.5.0rc2/faststream/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,21 @@
 
 F_Return = TypeVar("F_Return")
 F_Spec = ParamSpec("F_Spec")
 
 AnyCallable: TypeAlias = Callable[..., Any]
 NoneCallable: TypeAlias = Callable[..., None]
 AsyncFunc: TypeAlias = Callable[..., Awaitable[Any]]
+AsyncFuncAny: TypeAlias = Callable[[Any], Awaitable[Any]]
 
 DecoratedCallable: TypeAlias = AnyCallable
 DecoratedCallableNone: TypeAlias = NoneCallable
 
+Decorator: TypeAlias = Callable[[AnyCallable], AnyCallable]
+
 JsonArray: TypeAlias = Sequence["DecodedMessage"]
 
 JsonTable: TypeAlias = Dict[str, "DecodedMessage"]
 
 JsonDecodable: TypeAlias = Union[
     bool,
     bytes,
```

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/abc.py` & `faststream-0.5.0rc2/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/generate.py` & `faststream-0.5.0rc2/faststream/asyncapi/generate.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/message.py` & `faststream-0.5.0rc2/faststream/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/proto.py` & `faststream-0.5.0rc2/faststream/asyncapi/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/site.py` & `faststream-0.5.0rc2/faststream/asyncapi/site.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/utils.py` & `faststream-0.5.0rc2/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/channels.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/info.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/main.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/message.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/operations.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/security.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/servers.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/utils.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.0rc2/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.0rc2/faststream/broker/acknowledgement_watcher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/message.py` & `faststream-0.5.0rc2/faststream/broker/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/router.py` & `faststream-0.5.0rc2/faststream/broker/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/schemas.py` & `faststream-0.5.0rc2/faststream/broker/schemas.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/types.py` & `faststream-0.5.0rc2/faststream/broker/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import (
     Any,
-    AsyncContextManager,
     Awaitable,
     Callable,
     Optional,
     Protocol,
     TypeVar,
     Union,
 )
 
 from typing_extensions import ParamSpec, TypeAlias
 
 from faststream.broker.message import StreamMessage
 from faststream.broker.middlewares import BaseMiddleware
-from faststream.types import DecodedMessage, SendableMessage
+from faststream.types import AsyncFunc, AsyncFuncAny
 
 MsgType = TypeVar("MsgType")
 StreamMsg = TypeVar("StreamMsg", bound=StreamMessage[Any])
 ConnectionType = TypeVar("ConnectionType")
 
 
 SyncFilter: TypeAlias = Callable[[StreamMsg], bool]
@@ -63,18 +62,21 @@
     AsyncWrappedHandlerCall[MsgType, T_HandlerReturn],
     SyncWrappedHandlerCall[MsgType, T_HandlerReturn],
 ]
 
 
 BrokerMiddleware: TypeAlias = Callable[[Optional[MsgType]], BaseMiddleware]
 SubscriberMiddleware: TypeAlias = Callable[
-    [Optional[DecodedMessage]],
-    AsyncContextManager[Optional[DecodedMessage]],
+    [AsyncFuncAny, MsgType],
+    MsgType,
 ]
 
 
 class PublisherMiddleware(Protocol):
     """Publisher middleware interface."""
 
     def __call__(
-        self, __msg: Any, /, **__kwargs: Any
-    ) -> AsyncContextManager[SendableMessage]: ...
+        self,
+        call_next: AsyncFunc,
+        *__args: Any,
+        **__kwargs: Any,
+    ) -> Any: ...
```

### Comparing `faststream-0.5.0rc1/faststream/broker/utils.py` & `faststream-0.5.0rc2/faststream/broker/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/core/abc.py` & `faststream-0.5.0rc2/faststream/broker/core/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/core/logging.py` & `faststream-0.5.0rc2/faststream/broker/core/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/core/usecase.py` & `faststream-0.5.0rc2/faststream/broker/core/usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from abc import abstractmethod
-from contextlib import AsyncExitStack
+from functools import partial
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Generic,
     Iterable,
     List,
@@ -38,15 +38,15 @@
     from types import TracebackType
 
     from fast_depends.dependencies import Depends
 
     from faststream.asyncapi.schema import Tag, TagDict
     from faststream.broker.publisher.proto import ProducerProto, PublisherProto
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict, LoggerProto
+    from faststream.types import AnyDict, AsyncFunc, Decorator, LoggerProto
 
 
 class BrokerUsecase(
     LoggingBroker[MsgType],
     SetupAble,
     Generic[MsgType, ConnectionType],
 ):
@@ -107,14 +107,18 @@
             bool,
             Doc("Whether to cast types using Pydantic validation."),
         ],
         _get_dependant: Annotated[
             Optional[Callable[..., Any]],
             Doc("Custom library dependant generator callback."),
         ],
+        _call_decorators: Annotated[
+            Iterable["Decorator"],
+            Doc("Any custom decorator to apply to wrapped functions."),
+        ],
         # AsyncAPI kwargs
         protocol: Annotated[
             Optional[str],
             Doc("AsyncAPI server protocol."),
         ],
         protocol_version: Annotated[
             Optional[str],
@@ -178,14 +182,15 @@
         context.set_global("logger", self.logger)
         context.set_global("broker", self)
 
         # FastDepends args
         self._is_apply_types = apply_types
         self._is_validate = validate
         self._get_dependant = _get_dependant
+        self._call_decorators = _call_decorators
 
         # AsyncAPI information
         self.url = asyncapi_url
         self.protocol = protocol
         self.protocol_version = protocol_version
         self.description = description
         self.tags = tags
@@ -232,14 +237,15 @@
             # broker options
             broker_parser=self._parser,
             broker_decoder=self._decoder,
             # dependant args
             apply_types=self._is_apply_types,
             is_validate=self._is_validate,
             _get_dependant=self._get_dependant,
+            _call_decorators=self._call_decorators,
             **self._subscriber_setup_extra,
             **kwargs,
         )
 
     def setup_publisher(
         self,
         publisher: "PublisherProto[MsgType]",
@@ -323,18 +329,14 @@
         self,
         msg: Any,
         *,
         producer: Optional["ProducerProto"],
         **kwargs: Any,
     ) -> Optional[Any]:
         """Publish message directly."""
-        assert producer, NOT_CONNECTED_YET  # nosec B101
-
-        async with AsyncExitStack() as stack:
-            for m in self._middlewares:
-                msg = await stack.enter_async_context(
-                    m(None).publish_scope(msg, **kwargs)
-                )
+        assert producer, NOT_CONNECTED_YET  # nosec B101)
 
-            return await producer.publish(msg, **kwargs)
+        publish: "AsyncFunc" = producer.publish
+        for m in self._middlewares:
+            publish = partial(m(None).publish_scope, publish)
 
-        return None
+        return await publish(msg, **kwargs)
```

### Comparing `faststream-0.5.0rc1/faststream/broker/fastapi/context.py` & `faststream-0.5.0rc2/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.0rc2/faststream/broker/fastapi/get_dependant.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/fastapi/route.py` & `faststream-0.5.0rc2/faststream/broker/fastapi/route.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/fastapi/router.py` & `faststream-0.5.0rc2/faststream/broker/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/middlewares/base.py` & `faststream-0.5.0rc2/faststream/broker/middlewares/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from contextlib import asynccontextmanager
-from typing import TYPE_CHECKING, Any, AsyncIterator, Optional, Type, cast
+from typing import TYPE_CHECKING, Any, Optional, Type
 
 from typing_extensions import Self
 
 if TYPE_CHECKING:
     from types import TracebackType
 
-    from faststream.types import DecodedMessage, SendableMessage
+    from faststream.broker.message import StreamMessage
+    from faststream.types import AsyncFunc, AsyncFuncAny
 
 
 class BaseMiddleware:
     """A base middleware class."""
 
     def __init__(self, msg: Optional[Any] = None) -> None:
         self.msg = msg
@@ -39,38 +39,43 @@
         exc_tb: Optional["TracebackType"] = None,
     ) -> Optional[bool]:
         """Exit the asynchronous context manager."""
         return await self.after_processed(exc_type, exc_val, exc_tb)
 
     async def on_consume(
         self,
-        msg: Optional["DecodedMessage"],
-    ) -> Optional["DecodedMessage"]:
+        msg: "StreamMessage[Any]",
+    ) -> "StreamMessage[Any]":
         """Asynchronously consumes a message."""
         return msg
 
     async def after_consume(self, err: Optional[Exception]) -> None:
         """A function to handle the result of consuming a resource asynchronously."""
         if err is not None:
             raise err
 
-    @asynccontextmanager
     async def consume_scope(
         self,
-        msg: Optional["DecodedMessage"],
-    ) -> AsyncIterator[Optional["DecodedMessage"]]:
+        call_next: "AsyncFuncAny",
+        msg: "StreamMessage[Any]",
+    ) -> Any:
         """Asynchronously consumes a message and returns an asynchronous iterator of decoded messages."""
         err: Optional[Exception]
         try:
-            yield await self.on_consume(msg)
+            result = await call_next(await self.on_consume(msg))
+
         except Exception as e:
             err = e
+
         else:
             err = None
-        await self.after_consume(err)
+            return result
+
+        finally:
+            await self.after_consume(err)
 
     async def on_publish(
         self,
         msg: Any,
         *args: Any,
         **kwargs: Any,
     ) -> Any:
@@ -81,24 +86,32 @@
         self,
         err: Optional[Exception],
     ) -> None:
         """Asynchronous function to handle the after publish event."""
         if err is not None:
             raise err
 
-    @asynccontextmanager
     async def publish_scope(
         self,
+        call_next: "AsyncFunc",
         msg: Any,
-        /,
         *args: Any,
         **kwargs: Any,
-    ) -> AsyncIterator["SendableMessage"]:
+    ) -> Any:
         """Publish a message and return an async iterator."""
         err: Optional[Exception]
         try:
-            yield cast("SendableMessage", await self.on_publish(msg, *args, **kwargs))
+            result = await call_next(
+                await self.on_publish(msg, *args, **kwargs),
+                *args,
+                **kwargs,
+            )
+
         except Exception as e:
             err = e
+
         else:
             err = None
-        await self.after_publish(err)
+            return result
+
+        finally:
+            await self.after_publish(err)
```

### Comparing `faststream-0.5.0rc1/faststream/broker/middlewares/logging.py` & `faststream-0.5.0rc2/faststream/broker/middlewares/logging.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from faststream.broker.middlewares.base import BaseMiddleware
 from faststream.exceptions import IgnoredException
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
     from types import TracebackType
 
-    from faststream.types import DecodedMessage, LoggerProto
+    from faststream.broker.message import StreamMessage
+    from faststream.types import LoggerProto
 
 
 class CriticalLogMiddleware(BaseMiddleware):
     """A middleware class for logging critical errors."""
 
     def __init__(
         self,
@@ -28,16 +29,16 @@
     def __call__(self, msg: Optional[Any]) -> Self:
         """Call the object with a message."""
         self.msg = msg
         return self
 
     async def on_consume(
         self,
-        msg: Optional["DecodedMessage"],
-    ) -> Optional["DecodedMessage"]:
+        msg: "StreamMessage[Any]",
+    ) -> "StreamMessage[Any]":
         if self.logger is not None:
             c = context.get_local("log_context") or {}
             self.logger.log(self.log_level, "Received", extra=c)
 
         return await super().on_consume(msg)
 
     async def after_processed(
```

### Comparing `faststream-0.5.0rc1/faststream/broker/publisher/fake.py` & `faststream-0.5.0rc2/faststream/broker/publisher/fake.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from contextlib import AsyncExitStack
+from functools import partial
 from itertools import chain
-from typing import TYPE_CHECKING, Any, Awaitable, Callable, Iterable, Optional
+from typing import TYPE_CHECKING, Any, Iterable, Optional
 
 from faststream.broker.publisher.proto import BasePublisherProto
 
 if TYPE_CHECKING:
     from faststream.broker.types import PublisherMiddleware
-    from faststream.types import AnyDict, SendableMessage
+    from faststream.types import AnyDict, AsyncFunc, SendableMessage
 
 
 class FakePublisher(BasePublisherProto):
     """Publisher Interface implementation to use as RPC or REPLY TO publisher."""
 
     def __init__(
         self,
-        method: Callable[..., Awaitable["SendableMessage"]],
+        method: "AsyncFunc",
         *,
         publish_kwargs: "AnyDict",
         middlewares: Iterable["PublisherMiddleware"] = (),
     ) -> None:
         """Initialize an object."""
         self.method = method
         self.publish_kwargs = publish_kwargs
@@ -35,12 +35,12 @@
         """Publish a message."""
         publish_kwargs = {
             "correlation_id": correlation_id,
             **self.publish_kwargs,
             **kwargs,
         }
 
-        async with AsyncExitStack() as stack:
-            for m in chain(_extra_middlewares, self.middlewares):
-                message = await stack.enter_async_context(m(message, **publish_kwargs))
+        call: "AsyncFunc" = self.method
+        for m in chain(_extra_middlewares, self.middlewares):
+            call = partial(m, call)
 
-            return await self.method(message, **publish_kwargs)
+        return await call(message, **publish_kwargs)
```

### Comparing `faststream-0.5.0rc1/faststream/broker/publisher/proto.py` & `faststream-0.5.0rc2/faststream/broker/publisher/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/publisher/usecase.py` & `faststream-0.5.0rc2/faststream/broker/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/broker/subscriber/call_item.py` & `faststream-0.5.0rc2/faststream/broker/subscriber/call_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from contextlib import AsyncExitStack
+from functools import partial
 from inspect import unwrap
 from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
@@ -25,14 +25,15 @@
     from faststream.broker.types import (
         AsyncCallable,
         AsyncFilter,
         CustomCallable,
         SubscriberMiddleware,
     )
     from faststream.broker.wrapper.call import HandlerCallWrapper
+    from faststream.types import AsyncFuncAny, Decorator
 
 
 class HandlerItem(SetupAble, Generic[MsgType]):
     """A class representing handler overloaded item."""
 
     __slots__ = (
         "handler",
@@ -49,15 +50,15 @@
     def __init__(
         self,
         *,
         handler: "HandlerCallWrapper[MsgType, ..., Any]",
         filter: "AsyncFilter[StreamMessage[MsgType]]",
         item_parser: Optional["CustomCallable"],
         item_decoder: Optional["CustomCallable"],
-        item_middlewares: Iterable["SubscriberMiddleware"],
+        item_middlewares: Iterable["SubscriberMiddleware[StreamMessage[MsgType]]"],
         dependencies: Iterable["Depends"],
     ) -> None:
         self.handler = handler
         self.filter = filter
         self.item_parser = item_parser
         self.item_decoder = item_decoder
         self.item_middlewares = item_middlewares
@@ -75,33 +76,36 @@
         *,
         parser: "AsyncCallable",
         decoder: "AsyncCallable",
         broker_dependencies: Iterable["Depends"],
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
+        _call_decorators: Iterable["Decorator"],
     ) -> None:
         if self.dependant is None:
             self.item_parser = parser
             self.item_decoder = decoder
 
             dependencies = (*broker_dependencies, *self.dependencies)
 
             dependant = self.handler.set_wrapped(
                 apply_types=apply_types,
                 is_validate=is_validate,
                 dependencies=dependencies,
                 _get_dependant=_get_dependant,
+                _call_decorators=_call_decorators,
             )
 
             if _get_dependant is None:
                 self.dependant = dependant
             else:
                 self.dependant = _get_dependant(
-                    self.handler._original_call, dependencies
+                    self.handler._original_call,
+                    dependencies,
                 )
 
     @property
     def call_name(self) -> str:
         """Returns the name of the original call."""
         if self.handler is None:
             return ""
@@ -144,30 +148,29 @@
 
         return None
 
     async def call(
         self,
         /,
         message: "StreamMessage[MsgType]",
-        _extra_middlewares: Iterable["SubscriberMiddleware"],
+        _extra_middlewares: Iterable["SubscriberMiddleware[Any]"],
     ) -> Any:
         """Execute wrapped handler with consume middlewares."""
-        async with AsyncExitStack() as consume_stack:
-            for middleware in chain(self.item_middlewares, _extra_middlewares):
-                message.decoded_body = await consume_stack.enter_async_context(
-                    middleware(message.decoded_body)
-                )
+        call: "AsyncFuncAny" = self.handler.call_wrapped
 
-            try:
-                result = await self.handler.call_wrapped(message)
+        for middleware in chain(self.item_middlewares, _extra_middlewares):
+            call = partial(middleware, call)
 
-            except (IgnoredException, SystemExit):
-                self.handler.trigger()
-                raise
-
-            except Exception as e:
-                self.handler.trigger(error=e)
-                raise e
+        try:
+            result = await call(message)
 
-            else:
-                self.handler.trigger(result=result)
-                return result
+        except (IgnoredException, SystemExit):
+            self.handler.trigger()
+            raise
+
+        except Exception as e:
+            self.handler.trigger(error=e)
+            raise e
+
+        else:
+            self.handler.trigger(result=result)
+            return result
```

### Comparing `faststream-0.5.0rc1/faststream/broker/subscriber/proto.py` & `faststream-0.5.0rc2/faststream/broker/subscriber/proto.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from faststream.broker.subscriber.call_item import HandlerItem
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
         Filter,
         SubscriberMiddleware,
     )
-    from faststream.types import AnyDict, LoggerProto
+    from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 class SubscriberProto(
     AsyncAPIProto,
     EndpointProto,
     WrapperProto[MsgType],
 ):
@@ -59,14 +59,15 @@
         broker_decoder: Optional["CustomCallable"],
         producer: Optional["ProducerProto"],
         extra_context: "AnyDict",
         # FastDepends options
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
+        _call_decorators: Iterable["Decorator"],
     ) -> None: ...
 
     @abstractmethod
     def _make_response_publisher(
         self,
         message: "StreamMessage[MsgType]",
     ) -> Iterable["BasePublisherProto"]: ...
@@ -87,10 +88,10 @@
     @abstractmethod
     def add_call(
         self,
         *,
         filter_: "Filter[Any]",
         parser_: "CustomCallable",
         decoder_: "CustomCallable",
-        middlewares_: Iterable["SubscriberMiddleware"],
+        middlewares_: Iterable["SubscriberMiddleware[Any]"],
         dependencies_: Iterable["Depends"],
     ) -> Self: ...
```

### Comparing `faststream-0.5.0rc1/faststream/broker/subscriber/usecase.py` & `faststream-0.5.0rc2/faststream/broker/subscriber/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     from faststream.broker.types import (
         AsyncCallable,
         BrokerMiddleware,
         CustomCallable,
         Filter,
         SubscriberMiddleware,
     )
-    from faststream.types import AnyDict, LoggerProto
+    from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 class _CallOptions:
     __slots__ = (
         "filter",
         "parser",
         "decoder",
@@ -61,15 +61,15 @@
 
     def __init__(
         self,
         *,
         filter: "Filter[Any]",
         parser: Optional["CustomCallable"],
         decoder: Optional["CustomCallable"],
-        middlewares: Iterable["SubscriberMiddleware"],
+        middlewares: Iterable["SubscriberMiddleware[Any]"],
         dependencies: Iterable["Depends"],
     ) -> None:
         self.filter = filter
         self.parser = parser
         self.decoder = decoder
         self.middlewares = middlewares
         self.dependencies = dependencies
@@ -142,14 +142,15 @@
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
+        _call_decorators: Iterable["Decorator"],
     ) -> None:
         self.lock = MultiLock()
 
         self._producer = producer
         self.graceful_timeout = graceful_timeout
         self.extra_context = extra_context or {}
 
@@ -172,14 +173,15 @@
 
             call.setup(
                 parser=async_parser,
                 decoder=async_decoder,
                 apply_types=apply_types,
                 is_validate=is_validate,
                 _get_dependant=_get_dependant,
+                _call_decorators=_call_decorators,
                 broker_dependencies=self._broker_dependecies,
             )
 
             call.handler.refresh(with_mock=False)
 
     @abstractmethod
     async def start(self) -> None:
@@ -198,15 +200,15 @@
 
     def add_call(
         self,
         *,
         filter_: "Filter[Any]",
         parser_: Optional["CustomCallable"],
         decoder_: Optional["CustomCallable"],
-        middlewares_: Iterable["SubscriberMiddleware"],
+        middlewares_: Iterable["SubscriberMiddleware[Any]"],
         dependencies_: Iterable["Depends"],
     ) -> Self:
         self._call_options = _CallOptions(
             filter=filter_,
             parser=parser_,
             decoder=decoder_,
             middlewares=middlewares_,
@@ -218,41 +220,41 @@
     def __call__(
         self,
         func: None = None,
         *,
         filter: Optional["Filter[Any]"] = None,
         parser: Optional["CustomCallable"] = None,
         decoder: Optional["CustomCallable"] = None,
-        middlewares: Iterable["SubscriberMiddleware"] = (),
+        middlewares: Iterable["SubscriberMiddleware[Any]"] = (),
         dependencies: Iterable["Depends"] = (),
     ) -> Callable[
         [Callable[P_HandlerParams, T_HandlerReturn]],
         "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
     ]: ...
 
     @overload
     def __call__(
         self,
         func: Callable[P_HandlerParams, T_HandlerReturn],
         *,
         filter: Optional["Filter[Any]"] = None,
         parser: Optional["CustomCallable"] = None,
         decoder: Optional["CustomCallable"] = None,
-        middlewares: Iterable["SubscriberMiddleware"] = (),
+        middlewares: Iterable["SubscriberMiddleware[Any]"] = (),
         dependencies: Iterable["Depends"] = (),
     ) -> "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]": ...
 
     def __call__(
         self,
         func: Optional[Callable[P_HandlerParams, T_HandlerReturn]] = None,
         *,
         filter: Optional["Filter[Any]"] = None,
         parser: Optional["CustomCallable"] = None,
         decoder: Optional["CustomCallable"] = None,
-        middlewares: Iterable["SubscriberMiddleware"] = (),
+        middlewares: Iterable["SubscriberMiddleware[Any]"] = (),
         dependencies: Iterable["Depends"] = (),
     ) -> Any:
         if (options := self._call_options) is None:
             raise SetupError("You can't create subscriber directly.")
 
         total_deps = (*options.dependencies, *dependencies)
         total_middlewares = (*options.middlewares, *middlewares)
```

### Comparing `faststream-0.5.0rc1/faststream/broker/wrapper/call.py` & `faststream-0.5.0rc2/faststream/broker/wrapper/call.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from faststream.utils.functions import to_async
 
 if TYPE_CHECKING:
     from fast_depends.dependencies import Depends
 
     from faststream.broker.message import StreamMessage
     from faststream.broker.publisher.proto import PublisherProto
+    from faststream.types import Decorator
 
 
 class HandlerCallWrapper(Generic[MsgType, P_HandlerParams, T_HandlerReturn]):
     """A generic class to wrap handler calls."""
 
     mock: Optional[MagicMock]
     future: Optional["asyncio.Future[Any]"]
@@ -148,16 +149,22 @@
     def set_wrapped(
         self,
         *,
         apply_types: bool,
         is_validate: bool,
         dependencies: Iterable["Depends"],
         _get_dependant: Optional[Callable[..., Any]],
+        _call_decorators: Iterable["Decorator"],
     ) -> Optional["CallModel[..., Any]"]:
-        f: Callable[..., Awaitable[Any]] = to_async(self._original_call)
+        call = self._original_call
+        for decor in _call_decorators:
+            call = decor(call)
+        self._original_call = call
+
+        f: Callable[..., Awaitable[Any]] = to_async(call)
 
         dependent: Optional["CallModel[..., Any]"] = None
         if _get_dependant is None:
             dependent = build_call_model(
                 f,
                 cast=is_validate,
                 extra_dependencies=dependencies,  # type: ignore[arg-type]
```

### Comparing `faststream-0.5.0rc1/faststream/broker/wrapper/proto.py` & `faststream-0.5.0rc2/faststream/broker/wrapper/proto.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def __call__(
         self,
         func: None = None,
         *,
         filter: Optional["Filter[Any]"] = None,
         parser: Optional["CustomCallable"] = None,
         decoder: Optional["CustomCallable"] = None,
-        middlewares: Iterable["SubscriberMiddleware"] = (),
+        middlewares: Iterable["SubscriberMiddleware[Any]"] = (),
         dependencies: Iterable["Depends"] = (),
     ) -> Callable[
         [Callable[P_HandlerParams, T_HandlerReturn]],
         "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
     ]: ...
 
     @overload
@@ -49,30 +49,30 @@
             Callable[P_HandlerParams, T_HandlerReturn],
             "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
         ],
         *,
         filter: Optional["Filter[Any]"] = None,
         parser: Optional["CustomCallable"] = None,
         decoder: Optional["CustomCallable"] = None,
-        middlewares: Iterable["SubscriberMiddleware"] = (),
+        middlewares: Iterable["SubscriberMiddleware[Any]"] = (),
         dependencies: Iterable["Depends"] = (),
     ) -> "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]": ...
 
     def __call__(
         self,
         func: Union[
             Callable[P_HandlerParams, T_HandlerReturn],
             "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
             None,
         ] = None,
         *,
         filter: Optional["Filter[Any]"] = None,
         parser: Optional["CustomCallable"] = None,
         decoder: Optional["CustomCallable"] = None,
-        middlewares: Iterable["SubscriberMiddleware"] = (),
+        middlewares: Iterable["SubscriberMiddleware[Any]"] = (),
         dependencies: Iterable["Depends"] = (),
     ) -> Union[
         "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
         Callable[
             [Callable[P_HandlerParams, T_HandlerReturn]],
             "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
         ],
```

### Comparing `faststream-0.5.0rc1/faststream/cli/main.py` & `faststream-0.5.0rc2/faststream/cli/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/cli/docs/app.py` & `faststream-0.5.0rc2/faststream/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/cli/supervisors/basereload.py` & `faststream-0.5.0rc2/faststream/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.0rc2/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/cli/supervisors/utils.py` & `faststream-0.5.0rc2/faststream/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.0rc2/faststream/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/cli/utils/imports.py` & `faststream-0.5.0rc2/faststream/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/cli/utils/logs.py` & `faststream-0.5.0rc2/faststream/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/cli/utils/parser.py` & `faststream-0.5.0rc2/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/annotations.py` & `faststream-0.5.0rc2/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/client.py` & `faststream-0.5.0rc2/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/message.py` & `faststream-0.5.0rc2/faststream/confluent/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/parser.py` & `faststream-0.5.0rc2/faststream/confluent/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/router.py` & `faststream-0.5.0rc2/faststream/confluent/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,15 @@
             Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/confluent/security.py` & `faststream-0.5.0rc2/faststream/confluent/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/testing.py` & `faststream-0.5.0rc2/faststream/confluent/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/broker/broker.py` & `faststream-0.5.0rc2/faststream/confluent/broker/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from asyncio import AbstractEventLoop
-from contextlib import AsyncExitStack
+from functools import partial
 from inspect import Parameter
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
@@ -38,15 +38,21 @@
 
     from faststream.asyncapi import schema as asyncapi
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
     )
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict, LoggerProto, SendableMessage
+    from faststream.types import (
+        AnyDict,
+        AsyncFunc,
+        Decorator,
+        LoggerProto,
+        SendableMessage,
+    )
 
 Partition = TypeVar("Partition")
 
 
 class KafkaBroker(
     KafkaRegistrator,
     KafkaLoggingBroker,
@@ -319,14 +325,18 @@
             bool,
             Doc("Whether to cast types using Pydantic validation."),
         ] = True,
         _get_dependant: Annotated[
             Optional[Callable[..., Any]],
             Doc("Custom library dependant generator callback."),
         ] = None,
+        _call_decorators: Annotated[
+            Iterable["Decorator"],
+            Doc("Any custom decorator to apply to wrapped functions."),
+        ] = (),
     ) -> None:
         if protocol is None:
             if security is not None and security.use_ssl:
                 protocol = "kafka-secure"
             else:
                 protocol = "kafka"
 
@@ -385,14 +395,15 @@
             tags=tags,
             # Logging args
             logger=logger,
             log_level=log_level,
             log_fmt=log_fmt,
             # FastDepends args
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
             apply_types=apply_types,
             validate=validate,
         )
         self.client_id = client_id
         self._producer = None
 
     async def _close(
@@ -492,33 +503,20 @@
         reply_to: str = "",
         correlation_id: Optional[str] = None,
     ) -> None:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         correlation_id = correlation_id or gen_cor_id()
 
-        async with AsyncExitStack() as stack:
-            wrapped_messages = [
-                await stack.enter_async_context(
-                    middleware(None).publish_scope(
-                        msg,
-                        topic=topic,
-                        partition=partition,
-                        timestamp_ms=timestamp_ms,
-                        headers=headers,
-                        reply_to=reply_to,
-                        correlation_id=correlation_id,
-                    )
-                )
-                for msg in msgs
-                for middleware in self._middlewares
-            ] or msgs
-
-            await self._producer.publish_batch(
-                *wrapped_messages,
-                topic=topic,
-                partition=partition,
-                timestamp_ms=timestamp_ms,
-                headers=headers,
-                reply_to=reply_to,
-                correlation_id=correlation_id,
-            )
+        call: "AsyncFunc" = self._producer.publish_batch
+        for m in self._middlewares:
+            call = partial(m(None).publish_scope, call)
+
+        await call(
+            *msgs,
+            topic=topic,
+            partition=partition,
+            timestamp_ms=timestamp_ms,
+            headers=headers,
+            reply_to=reply_to,
+            correlation_id=correlation_id,
+        )
```

### Comparing `faststream-0.5.0rc1/faststream/confluent/broker/logging.py` & `faststream-0.5.0rc2/faststream/confluent/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/broker/registrator.py` & `faststream-0.5.0rc2/faststream/confluent/broker/registrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,15 @@
             Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -599,15 +599,15 @@
             Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -891,15 +891,15 @@
             Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -1186,15 +1186,15 @@
             Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.0rc2/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.0rc2/faststream/confluent/fastapi/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,15 +653,15 @@
             Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -1068,15 +1068,15 @@
             Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -1475,15 +1475,15 @@
             Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -1893,15 +1893,15 @@
             Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.0rc2/faststream/confluent/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/publisher/producer.py` & `faststream-0.5.0rc2/faststream/confluent/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/publisher/usecase.py` & `faststream-0.5.0rc2/faststream/confluent/publisher/usecase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from contextlib import AsyncExitStack
+from functools import partial
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Tuple, Union, cast
 
 from confluent_kafka import Message
 from typing_extensions import override
 
 from faststream.broker.message import gen_cor_id
 from faststream.broker.publisher.usecase import PublisherUsecase
 from faststream.broker.types import MsgType
 from faststream.exceptions import NOT_CONNECTED_YET
 
 if TYPE_CHECKING:
     from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
     from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
-    from faststream.types import AnyDict, SendableMessage
+    from faststream.types import AnyDict, AsyncFunc, SendableMessage
 
 
 class LogicPublisher(PublisherUsecase[MsgType]):
     """A class to publish messages to a Kafka topic."""
 
     _producer: Optional["AsyncConfluentFastProducer"]
 
@@ -106,39 +106,40 @@
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         correlation_id: Optional[str] = None,
         reply_to: str = "",
         # publisher specific
         _extra_middlewares: Iterable["PublisherMiddleware"] = (),
-    ) -> None:
+    ) -> Optional[Any]:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         kwargs: "AnyDict" = {
             "key": key or self.key,
             # basic args
             "topic": topic or self.topic,
             "partition": partition or self.partition,
             "timestamp_ms": timestamp_ms,
             "headers": headers or self.headers,
             "reply_to": reply_to or self.reply_to,
             "correlation_id": correlation_id or gen_cor_id(),
         }
 
-        async with AsyncExitStack() as stack:
-            for m in chain(
-                _extra_middlewares
-                or (m(None).publish_scope for m in self._broker_middlewares),
-                self._middlewares,
-            ):
-                message = await stack.enter_async_context(m(message, **kwargs))
+        call: "AsyncFunc" = self._producer.publish
 
-            return await self._producer.publish(message=message, **kwargs)
+        for m in chain(
+            (
+                _extra_middlewares
+                or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
 
-        return None
+        return await call(message, **kwargs)
 
 
 class BatchPublisher(LogicPublisher[Tuple[Message, ...]]):
     @override
     async def publish(  # type: ignore[override]
         self,
         message: Union["SendableMessage", Iterable["SendableMessage"]],
@@ -165,21 +166,19 @@
             "partition": partition or self.partition,
             "timestamp_ms": timestamp_ms,
             "headers": headers or self.headers,
             "reply_to": reply_to or self.reply_to,
             "correlation_id": correlation_id or gen_cor_id(),
         }
 
-        async with AsyncExitStack() as stack:
-            wrapped_messages = [
-                await stack.enter_async_context(middleware(msg, **kwargs))
-                for msg in msgs
-                for middleware in chain(
-                    _extra_middlewares
-                    or (m(None).publish_scope for m in self._broker_middlewares),
-                    self._middlewares,
-                )
-            ] or msgs
+        call: "AsyncFunc" = self._producer.publish_batch
 
-            return await self._producer.publish_batch(*wrapped_messages, **kwargs)
+        for m in chain(
+            (
+                _extra_middlewares
+                or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
 
-        return None
+        await call(*msgs, **kwargs)
```

### Comparing `faststream-0.5.0rc1/faststream/confluent/schemas/params.py` & `faststream-0.5.0rc2/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.0rc2/faststream/confluent/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.0rc2/faststream/confluent/subscriber/usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     from faststream.broker.publisher.proto import ProducerProto
     from faststream.broker.types import (
         AsyncCallable,
         BrokerMiddleware,
         CustomCallable,
     )
     from faststream.confluent.client import AsyncConfluentConsumer
-    from faststream.types import AnyDict, LoggerProto
+    from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 class LogicSubscriber(ABC, SubscriberUsecase[MsgType]):
     """A class to handle logic for consuming messages from Kafka."""
 
     topics: Sequence[str]
     group_id: Optional[str]
@@ -103,28 +103,30 @@
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
+        _call_decorators: Iterable["Decorator"],
     ) -> None:
         self.client_id = client_id
         self.__connection_data = connection_data
 
         super().setup(
             logger=logger,
             producer=producer,
             graceful_timeout=graceful_timeout,
             extra_context=extra_context,
             broker_parser=broker_parser,
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
         )
 
     @override
     async def start(self) -> None:
         """Start the consumer."""
         self.consumer = consumer = self.builder(
             *self.topics,
```

### Comparing `faststream-0.5.0rc1/faststream/kafka/annotations.py` & `faststream-0.5.0rc2/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/message.py` & `faststream-0.5.0rc2/faststream/kafka/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/parser.py` & `faststream-0.5.0rc2/faststream/kafka/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/router.py` & `faststream-0.5.0rc2/faststream/kafka/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,15 @@
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/kafka/security.py` & `faststream-0.5.0rc2/faststream/kafka/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/testing.py` & `faststream-0.5.0rc2/faststream/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/broker/broker.py` & `faststream-0.5.0rc2/faststream/kafka/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from contextlib import AsyncExitStack
+from functools import partial
 from inspect import Parameter
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
@@ -25,15 +25,14 @@
 from faststream.broker.message import gen_cor_id
 from faststream.exceptions import NOT_CONNECTED_YET
 from faststream.kafka.broker.logging import KafkaLoggingBroker
 from faststream.kafka.broker.registrator import KafkaRegistrator
 from faststream.kafka.publisher.producer import AioKafkaFastProducer
 from faststream.kafka.schemas.params import ConsumerConnectionParams
 from faststream.kafka.security import parse_security
-from faststream.types import AnyDict, SendableMessage
 from faststream.utils.data import filter_by_dict
 
 Partition = TypeVar("Partition")
 
 if TYPE_CHECKING:
     from asyncio import AbstractEventLoop
     from types import TracebackType
@@ -45,15 +44,21 @@
 
     from faststream.asyncapi import schema as asyncapi
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
     )
     from faststream.security import BaseSecurity
-    from faststream.types import LoggerProto
+    from faststream.types import (
+        AnyDict,
+        AsyncFunc,
+        Decorator,
+        LoggerProto,
+        SendableMessage,
+    )
 
     class KafkaInitKwargs(TypedDict, total=False):
         request_timeout_ms: Annotated[
             int,
             Doc("Client request timeout in milliseconds."),
         ]
         retry_backoff_ms: Annotated[
@@ -451,14 +456,18 @@
             bool,
             Doc("Whether to cast types using Pydantic validation."),
         ] = True,
         _get_dependant: Annotated[
             Optional[Callable[..., Any]],
             Doc("Custom library dependant generator callback."),
         ] = None,
+        _call_decorators: Annotated[
+            Iterable["Decorator"],
+            Doc("Any custom decorator to apply to wrapped functions."),
+        ] = (),
     ) -> None:
         if protocol is None:
             if security is not None and security.use_ssl:
                 protocol = "kafka-secure"
             else:
                 protocol = "kafka"
 
@@ -517,14 +526,15 @@
             tags=tags,
             # Logging args
             logger=logger,
             log_level=log_level,
             log_fmt=log_fmt,
             # FastDepends args
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
             apply_types=apply_types,
             validate=validate,
         )
         self.client_id = client_id
         self._producer = None
 
     async def _close(
@@ -550,15 +560,18 @@
     ) -> ConsumerConnectionParams:
         """Connect to Kafka servers manually.
 
         Consumes the same with `KafkaBroker.__init__` arguments and overrides them.
         To startup subscribers too you should use `broker.start()` after/instead this method.
         """
         if bootstrap_servers is not Parameter.empty:
-            connect_kwargs: AnyDict = {**kwargs, "bootstrap_servers": bootstrap_servers}
+            connect_kwargs: "AnyDict" = {
+                **kwargs,
+                "bootstrap_servers": bootstrap_servers,
+            }
         else:
             connect_kwargs = {**kwargs}
 
         return await super().connect(**connect_kwargs)
 
     @override
     async def _connect(  # type: ignore[override]
@@ -587,15 +600,15 @@
             self._log(
                 f"`{handler.call_name}` waiting for messages",
                 extra=handler.get_log_context(None),
             )
             await handler.start()
 
     @property
-    def _subscriber_setup_extra(self) -> AnyDict:
+    def _subscriber_setup_extra(self) -> "AnyDict":
         return {
             "client_id": self.client_id,
             "connection_args": self._connection or {},
         }
 
     @override
     async def publish(  # type: ignore[override]
@@ -715,33 +728,21 @@
             ),
         ] = None,
     ) -> None:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         correlation_id = correlation_id or gen_cor_id()
 
-        async with AsyncExitStack() as stack:
-            wrapped_messages = [
-                await stack.enter_async_context(
-                    middleware(None).publish_scope(
-                        msg,
-                        topic=topic,
-                        partition=partition,
-                        timestamp_ms=timestamp_ms,
-                        headers=headers,
-                        reply_to=reply_to,
-                        correlation_id=correlation_id,
-                    )
-                )
-                for msg in msgs
-                for middleware in self._middlewares
-            ] or msgs
-
-            await self._producer.publish_batch(
-                *wrapped_messages,
-                topic=topic,
-                partition=partition,
-                timestamp_ms=timestamp_ms,
-                headers=headers,
-                reply_to=reply_to,
-                correlation_id=correlation_id,
-            )
+        call: "AsyncFunc" = self._producer.publish_batch
+
+        for m in self._middlewares:
+            call = partial(m(None).publish_scope, call)
+
+        await call(
+            *msgs,
+            topic=topic,
+            partition=partition,
+            timestamp_ms=timestamp_ms,
+            headers=headers,
+            reply_to=reply_to,
+            correlation_id=correlation_id,
+        )
```

### Comparing `faststream-0.5.0rc1/faststream/kafka/broker/logging.py` & `faststream-0.5.0rc2/faststream/kafka/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/broker/registrator.py` & `faststream-0.5.0rc2/faststream/kafka/broker/registrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -605,15 +605,15 @@
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -897,15 +897,15 @@
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -1192,15 +1192,15 @@
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.0rc2/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.0rc2/faststream/kafka/fastapi/fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -897,15 +897,15 @@
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -1347,15 +1347,15 @@
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -1797,15 +1797,15 @@
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
@@ -2250,15 +2250,15 @@
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[KafkaMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.0rc2/faststream/kafka/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/publisher/producer.py` & `faststream-0.5.0rc2/faststream/kafka/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/publisher/usecase.py` & `faststream-0.5.0rc2/faststream/kafka/publisher/usecase.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from contextlib import AsyncExitStack
+from functools import partial
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Tuple, Union, cast
 
 from aiokafka import ConsumerRecord
 from typing_extensions import Annotated, Doc, override
 
 from faststream.broker.message import gen_cor_id
 from faststream.broker.publisher.usecase import PublisherUsecase
 from faststream.broker.types import MsgType
 from faststream.exceptions import NOT_CONNECTED_YET
 
 if TYPE_CHECKING:
     from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
     from faststream.kafka.publisher.producer import AioKafkaFastProducer
-    from faststream.types import SendableMessage
+    from faststream.types import AsyncFunc, SendableMessage
 
 
 class LogicPublisher(PublisherUsecase[MsgType]):
     """A class to publish messages to a Kafka topic."""
 
     _producer: Optional["AioKafkaFastProducer"]
 
@@ -150,55 +150,45 @@
             Doc("Reply message topic name to send response."),
         ] = "",
         # publisher specific
         _extra_middlewares: Annotated[
             Iterable["PublisherMiddleware"],
             Doc("Extra middlewares to wrap publishing process."),
         ] = (),
-    ) -> None:
+    ) -> Optional[Any]:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         topic = topic or self.topic
         key = key or self.key
         partition = partition or self.partition
         headers = headers or self.headers
         reply_to = reply_to or self.reply_to
         correlation_id = correlation_id or gen_cor_id()
 
-        async with AsyncExitStack() as stack:
-            for m in chain(
+        call: "AsyncFunc" = self._producer.publish
+
+        for m in chain(
+            (
                 _extra_middlewares
-                or (m(None).publish_scope for m in self._broker_middlewares),
-                self._middlewares,
-            ):
-                message = await stack.enter_async_context(
-                    m(
-                        message,
-                        topic=topic,
-                        key=key,
-                        partition=partition,
-                        headers=headers,
-                        reply_to=reply_to,
-                        correlation_id=correlation_id,
-                        timestamp_ms=timestamp_ms,
-                    )
-                )
-
-            return await self._producer.publish(
-                message=message,
-                topic=topic,
-                key=key,
-                partition=partition,
-                headers=headers,
-                reply_to=reply_to,
-                correlation_id=correlation_id,
-                timestamp_ms=timestamp_ms,
-            )
+                or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
 
-        return None
+        return await call(
+            message,
+            topic=topic,
+            key=key,
+            partition=partition,
+            headers=headers,
+            reply_to=reply_to,
+            correlation_id=correlation_id,
+            timestamp_ms=timestamp_ms,
+        )
 
 
 class BatchPublisher(LogicPublisher[Tuple["ConsumerRecord", ...]]):
     @override
     async def publish(  # type: ignore[override]
         self,
         message: Annotated[
@@ -258,39 +248,27 @@
 
         topic = topic or self.topic
         partition = partition or self.partition
         headers = headers or self.headers
         reply_to = reply_to or self.reply_to
         correlation_id = correlation_id or gen_cor_id()
 
-        async with AsyncExitStack() as stack:
-            wrapped_messages = [
-                await stack.enter_async_context(
-                    middleware(
-                        msg,
-                        topic=topic,
-                        partition=partition,
-                        headers=headers,
-                        reply_to=reply_to,
-                        correlation_id=correlation_id,
-                        timestamp_ms=timestamp_ms,
-                    )
-                )
-                for msg in msgs
-                for middleware in chain(
-                    _extra_middlewares
-                    or (m(None).publish_scope for m in self._broker_middlewares),
-                    self._middlewares,
-                )
-            ] or msgs
-
-            return await self._producer.publish_batch(
-                *wrapped_messages,
-                topic=topic,
-                partition=partition,
-                headers=headers,
-                reply_to=reply_to,
-                correlation_id=correlation_id,
-                timestamp_ms=timestamp_ms,
-            )
+        call: "AsyncFunc" = self._producer.publish_batch
 
-        return None
+        for m in chain(
+            (
+                _extra_middlewares
+                or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
+
+        await call(
+            *msgs,
+            topic=topic,
+            partition=partition,
+            headers=headers,
+            reply_to=reply_to,
+            correlation_id=correlation_id,
+            timestamp_ms=timestamp_ms,
+        )
```

### Comparing `faststream-0.5.0rc1/faststream/kafka/schemas/params.py` & `faststream-0.5.0rc2/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/subscriber/asyncapi.py` & `faststream-0.5.0rc2/faststream/kafka/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.0rc2/faststream/kafka/subscriber/usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 if TYPE_CHECKING:
     from aiokafka import AIOKafkaConsumer, ConsumerRecord
     from fast_depends.dependencies import Depends
 
     from faststream.broker.message import StreamMessage
     from faststream.broker.publisher.proto import ProducerProto
     from faststream.kafka.schemas.params import ConsumerConnectionParams
-    from faststream.types import AnyDict, LoggerProto
+    from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 class LogicSubscriber(ABC, SubscriberUsecase[MsgType]):
     """A class to handle logic for consuming messages from Kafka."""
 
     topics: Sequence[str]
     group_id: Optional[str]
@@ -105,28 +105,30 @@
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
+        _call_decorators: Iterable["Decorator"],
     ) -> None:
         self.client_id = client_id
         self.__connection_args = connection_args
 
         super().setup(
             logger=logger,
             producer=producer,
             graceful_timeout=graceful_timeout,
             extra_context=extra_context,
             broker_parser=broker_parser,
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
         )
 
     async def start(self) -> None:
         """Start the consumer."""
         self.consumer = consumer = self.builder(
             *self.topics,
             group_id=self.group_id,
```

### Comparing `faststream-0.5.0rc1/faststream/log/formatter.py` & `faststream-0.5.0rc2/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/log/logging.py` & `faststream-0.5.0rc2/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/__init__.py` & `faststream-0.5.0rc2/faststream/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/annotations.py` & `faststream-0.5.0rc2/faststream/nats/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/helpers.py` & `faststream-0.5.0rc2/faststream/nats/helpers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/message.py` & `faststream-0.5.0rc2/faststream/nats/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/parser.py` & `faststream-0.5.0rc2/faststream/nats/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/router.py` & `faststream-0.5.0rc2/faststream/nats/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             Doc("Parser to map original **nats-py** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[NatsMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             Union[
                 "Filter[NatsMessage]",
                 "Filter[NatsBatchMessage]",
             ],
```

### Comparing `faststream-0.5.0rc1/faststream/nats/security.py` & `faststream-0.5.0rc2/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/testing.py` & `faststream-0.5.0rc2/faststream/nats/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/broker/broker.py` & `faststream-0.5.0rc2/faststream/nats/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,21 @@
     from faststream.broker.publisher.proto import ProducerProto
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
     )
     from faststream.nats.publisher.asyncapi import AsyncAPIPublisher
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict, DecodedMessage, LoggerProto, SendableMessage
+    from faststream.types import (
+        AnyDict,
+        DecodedMessage,
+        Decorator,
+        LoggerProto,
+        SendableMessage,
+    )
 
     class NatsInitKwargs(TypedDict, total=False):
         """NatsBroker.connect() method type hints."""
 
         error_cb: Annotated[
             Optional["ErrorCallback"],
             Doc("Callback to report errors."),
@@ -424,14 +430,18 @@
             bool,
             Doc("Whether to cast types using Pydantic validation."),
         ] = True,
         _get_dependant: Annotated[
             Optional[Callable[..., Any]],
             Doc("Custom library dependant generator callback."),
         ] = None,
+        _call_decorators: Annotated[
+            Iterable["Decorator"],
+            Doc("Any custom decorator to apply to wrapped functions."),
+        ] = (),
     ) -> None:
         """Initialize the NatsBroker object."""
         if tls:  # pragma: no cover
             warnings.warn(
                 (
                     "\nNATS `tls` option was deprecated and will be removed in 0.6.0"
                     "\nPlease, use `security` with `BaseSecurity` or `SASLPlaintext` instead"
@@ -518,14 +528,15 @@
             logger=logger,
             log_level=log_level,
             log_fmt=log_fmt,
             # FastDepends args
             apply_types=apply_types,
             validate=validate,
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
         )
 
         self.__is_connected = False
         self._producer = None
 
         # JS options
         self.stream = None
```

### Comparing `faststream-0.5.0rc1/faststream/nats/broker/logging.py` & `faststream-0.5.0rc2/faststream/nats/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/broker/registrator.py` & `faststream-0.5.0rc2/faststream/nats/broker/registrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             Doc("Parser to map original **nats-py** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[NatsMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             Union[
                 "Filter[NatsMessage]",
                 "Filter[NatsBatchMessage]",
             ],
```

### Comparing `faststream-0.5.0rc1/faststream/nats/fastapi/__init__.py` & `faststream-0.5.0rc2/faststream/nats/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.0rc2/faststream/nats/fastapi/fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,15 +676,15 @@
             Doc("Parser to map original **nats-py** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[NatsMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             Union[
                 "Filter[NatsMessage]",
                 "Filter[NatsBatchMessage]",
             ],
```

### Comparing `faststream-0.5.0rc1/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.0rc2/faststream/nats/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/publisher/producer.py` & `faststream-0.5.0rc2/faststream/nats/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/publisher/usecase.py` & `faststream-0.5.0rc2/faststream/nats/publisher/usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from contextlib import AsyncExitStack
+from functools import partial
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union
 
 from nats.aio.msg import Msg
 from typing_extensions import Annotated, Doc, override
 
 from faststream.broker.message import gen_cor_id
 from faststream.broker.publisher.usecase import PublisherUsecase
 from faststream.exceptions import NOT_CONNECTED_YET
 
 if TYPE_CHECKING:
     from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
     from faststream.nats.publisher.producer import NatsFastProducer, NatsJSFastProducer
     from faststream.nats.schemas import JStream
-    from faststream.types import AnyDict, DecodedMessage, SendableMessage
+    from faststream.types import AnyDict, AsyncFunc, SendableMessage
 
 
 class LogicPublisher(PublisherUsecase[Msg]):
     """A class to represent a NATS publisher."""
 
     _producer: Union["NatsFastProducer", "NatsJSFastProducer", None]
 
@@ -118,15 +118,15 @@
             ),
         ] = False,
         # publisher specific
         _extra_middlewares: Annotated[
             Iterable["PublisherMiddleware"],
             Doc("Extra middlewares to wrap publishing process."),
         ] = (),
-    ) -> Optional["DecodedMessage"]:
+    ) -> Optional[Any]:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         kwargs: "AnyDict" = {
             "subject": subject or self.subject,
             "headers": headers or self.headers,
             "reply_to": reply_to or self.reply_to,
             "correlation_id": correlation_id or gen_cor_id(),
@@ -135,21 +135,22 @@
             "rpc_timeout": rpc_timeout,
             "raise_timeout": raise_timeout,
         }
 
         if stream := stream or getattr(self.stream, "name", None):
             kwargs.update({"stream": stream, "timeout": timeout or self.timeout})
 
-        async with AsyncExitStack() as stack:
-            for m in chain(
-                _extra_middlewares
-                or (m(None).publish_scope for m in self._broker_middlewares),
-                self._middlewares,
-            ):
-                message = await stack.enter_async_context(m(message, **kwargs))
+        call: "AsyncFunc" = self._producer.publish
 
-            return await self._producer.publish(message, **kwargs)
+        for m in chain(
+            (
+                _extra_middlewares or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
+
+        return await call(message, **kwargs)
 
-        return None
 
     def add_prefix(self, prefix: str) -> None:
         self.subject = prefix + self.subject
```

### Comparing `faststream-0.5.0rc1/faststream/nats/schemas/js_stream.py` & `faststream-0.5.0rc2/faststream/nats/schemas/js_stream.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/schemas/pull_sub.py` & `faststream-0.5.0rc2/faststream/nats/schemas/pull_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.0rc2/faststream/nats/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/nats/subscriber/usecase.py` & `faststream-0.5.0rc2/faststream/nats/subscriber/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     from faststream.broker.message import StreamMessage
     from faststream.broker.publisher.proto import ProducerProto
     from faststream.broker.types import (
         AsyncCallable,
         BrokerMiddleware,
     )
     from faststream.nats.schemas import JStream, PullSub
+    from faststream.types import Decorator
 
 
 class LogicSubscriber(SubscriberUsecase[MsgType]):
     """A class to represent a NATS handler."""
 
     subscription: Union[
         None,
@@ -124,27 +125,29 @@
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
+        _call_decorators: Iterable["Decorator"],
     ) -> None:
         self._connection = connection
 
         super().setup(
             logger=logger,
             producer=producer,
             graceful_timeout=graceful_timeout,
             extra_context=extra_context,
             broker_parser=broker_parser,
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
         )
 
     async def start(self) -> None:
         """Create NATS subscription and start consume tasks."""
         assert self._connection, NOT_CONNECTED_YET  # nosec B101
         await super().start()
         await self._create_subscription(connection=self._connection)
```

### Comparing `faststream-0.5.0rc1/faststream/rabbit/__init__.py` & `faststream-0.5.0rc2/faststream/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/annotations.py` & `faststream-0.5.0rc2/faststream/rabbit/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/message.py` & `faststream-0.5.0rc2/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/parser.py` & `faststream-0.5.0rc2/faststream/rabbit/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/router.py` & `faststream-0.5.0rc2/faststream/rabbit/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[RabbitMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[RabbitMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/rabbit/security.py` & `faststream-0.5.0rc2/faststream/rabbit/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/testing.py` & `faststream-0.5.0rc2/faststream/rabbit/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/utils.py` & `faststream-0.5.0rc2/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/broker/broker.py` & `faststream-0.5.0rc2/faststream/rabbit/broker/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     from faststream.asyncapi import schema as asyncapi
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
     )
     from faststream.rabbit.types import AioPikaSendableMessage
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict, LoggerProto
+    from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 class RabbitBroker(
     RabbitRegistrator,
     RabbitLoggingBroker,
 ):
     """A class to represent a RabbitMQ broker."""
@@ -184,14 +184,18 @@
             bool,
             Doc("Whether to cast types using Pydantic validation."),
         ] = True,
         _get_dependant: Annotated[
             Optional[Callable[..., Any]],
             Doc("Custom library dependant generator callback."),
         ] = None,
+        _call_decorators: Annotated[
+            Iterable["Decorator"],
+            Doc("Any custom decorator to apply to wrapped functions."),
+        ] = (),
     ) -> None:
         security_args = parse_security(security)
 
         amqp_url = build_url(
             url,
             host=host,
             port=port,
@@ -233,14 +237,15 @@
             logger=logger,
             log_level=log_level,
             log_fmt=log_fmt,
             # FastDepends args
             apply_types=apply_types,
             validate=validate,
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
         )
 
         self._max_consumers = max_consumers
 
         self.app_id = app_id
 
         self._channel = None
```

### Comparing `faststream-0.5.0rc1/faststream/rabbit/broker/logging.py` & `faststream-0.5.0rc2/faststream/rabbit/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/broker/registrator.py` & `faststream-0.5.0rc2/faststream/rabbit/broker/registrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[RabbitMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[RabbitMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.0rc2/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/fastapi/router.py` & `faststream-0.5.0rc2/faststream/rabbit/fastapi/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,15 @@
             ),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[RabbitMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[RabbitMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.0rc2/faststream/rabbit/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/publisher/producer.py` & `faststream-0.5.0rc2/faststream/rabbit/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.0rc2/faststream/rabbit/publisher/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from contextlib import AsyncExitStack
 from copy import deepcopy
+from functools import partial
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Union
 
 from aio_pika import IncomingMessage
 from typing_extensions import Annotated, Doc, TypedDict, Unpack, override
 
 from faststream.broker.message import gen_cor_id
@@ -15,15 +15,15 @@
 if TYPE_CHECKING:
     from aio_pika.abc import DateType, HeadersType, TimeoutType
 
     from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
     from faststream.rabbit.publisher.producer import AioPikaFastProducer
     from faststream.rabbit.schemas.exchange import RabbitExchange
     from faststream.rabbit.types import AioPikaSendableMessage
-    from faststream.types import AnyDict
+    from faststream.types import AnyDict, AsyncFunc
 
 
 # should be public to use in imports
 class PublishKwargs(TypedDict, total=False):
     """Typed dict to annotate RabbitMQ publishers."""
 
     headers: Annotated[
@@ -233,24 +233,26 @@
             "rpc": rpc,
             "rpc_timeout": rpc_timeout,
             "raise_timeout": raise_timeout,
             **self.message_kwargs,
             **publish_kwargs,
         }
 
-        async with AsyncExitStack() as stack:
-            for m in chain(
+        call: "AsyncFunc" = self._producer.publish
+
+        for m in chain(
+            (
                 _extra_middlewares
-                or (m(None).publish_scope for m in self._broker_middlewares),
-                self._middlewares,
-            ):
-                message = await stack.enter_async_context(m(message, **kwargs))
+                or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
 
-            return await self._producer.publish(message, **kwargs)
+        return await call(message, **kwargs)
 
-        return None
 
     def add_prefix(self, prefix: str) -> None:
         """Include Publisher in router."""
         new_q = deepcopy(self.queue)
         new_q.name = prefix + new_q.name
         self.queue = new_q
```

### Comparing `faststream-0.5.0rc1/faststream/rabbit/schemas/constants.py` & `faststream-0.5.0rc2/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.0rc2/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/schemas/queue.py` & `faststream-0.5.0rc2/faststream/rabbit/schemas/queue.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/schemas/reply.py` & `faststream-0.5.0rc2/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/subscriber/asyncapi.py` & `faststream-0.5.0rc2/faststream/rabbit/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.0rc2/faststream/rabbit/subscriber/usecase.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from faststream.rabbit.publisher.producer import AioPikaFastProducer
     from faststream.rabbit.schemas import (
         RabbitExchange,
         RabbitQueue,
         ReplyConfig,
     )
     from faststream.rabbit.utils import RabbitDeclarer
-    from faststream.types import AnyDict, LoggerProto
+    from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 class LogicSubscriber(
     SubscriberUsecase["IncomingMessage"],
     BaseRMQInformation,
 ):
     """A class to handle logic for RabbitMQ message consumption."""
@@ -107,14 +107,15 @@
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
+        _call_decorators: Iterable["Decorator"],
     ) -> None:
         self.app_id = app_id
         self.virtual_host = virtual_host
         self.declarer = declarer
 
         super().setup(
             logger=logger,
@@ -122,14 +123,15 @@
             graceful_timeout=graceful_timeout,
             extra_context=extra_context,
             broker_parser=broker_parser,
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
         )
 
     @override
     async def start(self) -> None:
         """Starts the consumer for the RabbitMQ queue."""
         if self.declarer is None:
             raise SetupError("You should setup subscriber at first.")
```

### Comparing `faststream-0.5.0rc1/faststream/redis/__init__.py` & `faststream-0.5.0rc2/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/annotations.py` & `faststream-0.5.0rc2/faststream/redis/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/message.py` & `faststream-0.5.0rc2/faststream/redis/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/parser.py` & `faststream-0.5.0rc2/faststream/redis/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/router.py` & `faststream-0.5.0rc2/faststream/redis/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             ),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[UnifyRedisMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[UnifyRedisMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/redis/security.py` & `faststream-0.5.0rc2/faststream/redis/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/testing.py` & `faststream-0.5.0rc2/faststream/redis/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/broker/broker.py` & `faststream-0.5.0rc2/faststream/redis/broker/broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from contextlib import AsyncExitStack
+from functools import partial
 from inspect import Parameter
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Iterable,
     Mapping,
@@ -42,15 +42,22 @@
     from faststream.asyncapi import schema as asyncapi
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
     )
     from faststream.redis.message import BaseMessage
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict, DecodedMessage, LoggerProto, SendableMessage
+    from faststream.types import (
+        AnyDict,
+        AsyncFunc,
+        DecodedMessage,
+        Decorator,
+        LoggerProto,
+        SendableMessage,
+    )
 
     class RedisInitKwargs(TypedDict, total=False):
         host: Optional[str]
         port: Union[str, int, None]
         db: Union[str, int, None]
         client_name: Optional[str]
         health_check_interval: Optional[float]
@@ -178,14 +185,18 @@
             bool,
             Doc("Whether to cast types using Pydantic validation."),
         ] = True,
         _get_dependant: Annotated[
             Optional[Callable[..., Any]],
             Doc("Custom library dependant generator callback."),
         ] = None,
+        _call_decorators: Annotated[
+            Iterable["Decorator"],
+            Doc("Any custom decorator to apply to wrapped functions."),
+        ] = (),
     ) -> None:
         self.global_polling_interval = polling_interval
         self._producer = None
 
         if asyncapi_url is None:
             asyncapi_url = url
 
@@ -232,14 +243,15 @@
             logger=logger,
             log_level=log_level,
             log_fmt=log_fmt,
             # FastDepends args
             apply_types=apply_types,
             validate=validate,
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
         )
 
     @override
     async def connect(  # type: ignore[override]
         self,
         url: Union[str, None, object] = Parameter.empty,
         **kwargs: "Unpack[RedisInitKwargs]",
@@ -426,15 +438,15 @@
             rpc=rpc,
             rpc_timeout=rpc_timeout,
             raise_timeout=raise_timeout,
         )
 
     async def publish_batch(
         self,
-        *messages: Annotated[
+        *msgs: Annotated[
             "SendableMessage",
             Doc("Messages bodies to send."),
         ],
         list: Annotated[
             str,
             Doc("Redis List object name to send messages."),
         ],
@@ -447,27 +459,17 @@
         ] = None,
     ) -> None:
         """Publish multiple messages to Redis List by one request."""
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         correlation_id = correlation_id or gen_cor_id()
 
-        async with AsyncExitStack() as stack:
-            wrapped_messages = [
-                await stack.enter_async_context(
-                    middleware(None).publish_scope(
-                        msg,
-                        list=list,
-                        correlation_id=correlation_id,
-                    )
-                )
-                for msg in messages
-                for middleware in self._middlewares
-            ] or messages
-
-            return await self._producer.publish_batch(
-                *wrapped_messages,
-                list=list,
-                correlation_id=correlation_id,
-            )
+        call: "AsyncFunc" = self._producer.publish_batch
+
+        for m in self._middlewares:
+            call = partial(m(None).publish_scope, call)
 
-        return None
+        await call(
+            *msgs,
+            list=list,
+            correlation_id=correlation_id,
+        )
```

### Comparing `faststream-0.5.0rc1/faststream/redis/broker/logging.py` & `faststream-0.5.0rc2/faststream/redis/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/broker/registrator.py` & `faststream-0.5.0rc2/faststream/redis/broker/registrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             ),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[UnifyRedisMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[UnifyRedisMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/redis/fastapi/__init__.py` & `faststream-0.5.0rc2/faststream/redis/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/fastapi/fastapi.py` & `faststream-0.5.0rc2/faststream/redis/fastapi/fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
             ),
         ] = None,
         decoder: Annotated[
             Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable["SubscriberMiddleware"],
+            Iterable["SubscriberMiddleware[UnifyRedisMessage]"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             "Filter[UnifyRedisMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
```

### Comparing `faststream-0.5.0rc1/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.0rc2/faststream/redis/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/publisher/producer.py` & `faststream-0.5.0rc2/faststream/redis/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/publisher/usecase.py` & `faststream-0.5.0rc2/faststream/redis/publisher/usecase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from abc import abstractmethod
-from contextlib import AsyncExitStack
 from copy import deepcopy
+from functools import partial
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Iterable, Optional
 
 from typing_extensions import Annotated, Doc, override
 
 from faststream.broker.message import gen_cor_id
 from faststream.broker.publisher.usecase import PublisherUsecase
 from faststream.exceptions import NOT_CONNECTED_YET
 from faststream.redis.message import UnifyRedisDict
 from faststream.redis.schemas import ListSub, PubSub, StreamSub
 
 if TYPE_CHECKING:
     from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
     from faststream.redis.publisher.producer import RedisFastProducer
-    from faststream.types import AnyDict, SendableMessage
+    from faststream.types import AnyDict, AsyncFunc, SendableMessage
 
 
 class LogicPublisher(PublisherUsecase[UnifyRedisDict]):
     """A class to represent a Redis publisher."""
 
     _producer: Optional["RedisFastProducer"]
 
@@ -155,49 +155,37 @@
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         channel_sub = PubSub.validate(channel or self.channel)
         reply_to = reply_to or self.reply_to
         headers = headers or self.headers
         correlation_id = correlation_id or gen_cor_id()
 
-        async with AsyncExitStack() as stack:
-            for m in chain(
-                _extra_middlewares
-                or (m(None).publish_scope for m in self._broker_middlewares),
-                self._middlewares,
-            ):
-                message = await stack.enter_async_context(
-                    m(
-                        message,
-                        channel=channel_sub.name,
-                        # basic args
-                        reply_to=reply_to,
-                        headers=headers,
-                        correlation_id=correlation_id,
-                        # RPC args
-                        rpc=rpc,
-                        rpc_timeout=rpc_timeout,
-                        raise_timeout=raise_timeout,
-                    )
-                )
-
-            return await self._producer.publish(
-                message=message,
-                channel=channel_sub.name,
-                # basic args
-                reply_to=reply_to,
-                headers=headers,
-                correlation_id=correlation_id,
-                # RPC args
-                rpc=rpc,
-                rpc_timeout=rpc_timeout,
-                raise_timeout=raise_timeout,
-            )
+        call: "AsyncFunc" = self._producer.publish
 
-        return None
+        for m in chain(
+            (
+                _extra_middlewares
+                or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
+
+        return await call(
+            message,
+            channel=channel_sub.name,
+            # basic args
+            reply_to=reply_to,
+            headers=headers,
+            correlation_id=correlation_id,
+            # RPC args
+            rpc=rpc,
+            rpc_timeout=rpc_timeout,
+            raise_timeout=raise_timeout,
+        )
 
 
 class ListPublisher(LogicPublisher):
     def __init__(
         self,
         *,
         list: "ListSub",
@@ -293,49 +281,37 @@
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         list_sub = ListSub.validate(list or self.list)
         reply_to = reply_to or self.reply_to
         headers = headers or self.headers
         correlation_id = correlation_id or gen_cor_id()
 
-        async with AsyncExitStack() as stack:
-            for m in chain(
-                _extra_middlewares
-                or (m(None).publish_scope for m in self._broker_middlewares),
-                self._middlewares,
-            ):
-                message = await stack.enter_async_context(
-                    m(
-                        message,
-                        list=list_sub.name,
-                        # basic args
-                        reply_to=reply_to,
-                        headers=headers,
-                        correlation_id=correlation_id,
-                        # RPC args
-                        rpc=rpc,
-                        rpc_timeout=rpc_timeout,
-                        raise_timeout=raise_timeout,
-                    )
-                )
-
-            return await self._producer.publish(
-                message=message,
-                list=list_sub.name,
-                # basic args
-                reply_to=reply_to,
-                headers=headers,
-                correlation_id=correlation_id,
-                # RPC args
-                rpc=rpc,
-                rpc_timeout=rpc_timeout,
-                raise_timeout=raise_timeout,
-            )
+        call: "AsyncFunc" = self._producer.publish
 
-        return None
+        for m in chain(
+            (
+                _extra_middlewares
+                or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
+
+        return await call(
+            message,
+            list=list_sub.name,
+            # basic args
+            reply_to=reply_to,
+            headers=headers,
+            correlation_id=correlation_id,
+            # RPC args
+            rpc=rpc,
+            rpc_timeout=rpc_timeout,
+            raise_timeout=raise_timeout,
+        )
 
 
 class ListBatchPublisher(ListPublisher):
     @override
     async def publish(  # type: ignore[override]
         self,
         message: Annotated[
@@ -358,38 +334,30 @@
         ] = (),
     ) -> None:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         list_sub = ListSub.validate(list or self.list)
         correlation_id = correlation_id or gen_cor_id()
 
-        async with AsyncExitStack() as stack:
-            wrapped_messages = [
-                await stack.enter_async_context(
-                    middleware(
-                        msg,
-                        list=list_sub,
-                        correlation_id=correlation_id,
-                    )
-                )
-                for msg in message
-                for middleware in chain(
-                    _extra_middlewares
-                    or (m(None).publish_scope for m in self._broker_middlewares),
-                    self._middlewares,
-                )
-            ] or message
-
-            return await self._producer.publish_batch(
-                *wrapped_messages,
-                list=list_sub.name,
-                correlation_id=correlation_id,
-            )
+        call: "AsyncFunc" = self._producer.publish_batch
 
-        return None
+        for m in chain(
+            (
+                _extra_middlewares
+                or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
+
+        await call(
+            *message,
+            list=list_sub.name,
+            correlation_id=correlation_id,
+        )
 
 
 class StreamPublisher(LogicPublisher):
     def __init__(
         self,
         *,
         stream: "StreamSub",
@@ -489,44 +457,31 @@
 
         stream_sub = StreamSub.validate(stream or self.stream)
         maxlen = maxlen or stream_sub.maxlen
         reply_to = reply_to or self.reply_to
         headers = headers or self.headers
         correlation_id = correlation_id or gen_cor_id()
 
-        async with AsyncExitStack() as stack:
-            for m in chain(
-                _extra_middlewares
-                or (m(None).publish_scope for m in self._broker_middlewares),
-                self._middlewares,
-            ):
-                message = await stack.enter_async_context(
-                    m(
-                        message,
-                        stream=stream_sub.name,
-                        maxlen=maxlen,
-                        # basic args
-                        reply_to=reply_to,
-                        headers=headers,
-                        correlation_id=correlation_id,
-                        # RPC args
-                        rpc=rpc,
-                        rpc_timeout=rpc_timeout,
-                        raise_timeout=raise_timeout,
-                    )
-                )
-
-            return await self._producer.publish(
-                message=message,
-                stream=stream_sub.name,
-                maxlen=maxlen,
-                # basic args
-                reply_to=reply_to,
-                headers=headers,
-                correlation_id=correlation_id,
-                # RPC args
-                rpc=rpc,
-                rpc_timeout=rpc_timeout,
-                raise_timeout=raise_timeout,
-            )
+        call: "AsyncFunc" = self._producer.publish
 
-        return None
+        for m in chain(
+            (
+                _extra_middlewares
+                or (m(None).publish_scope for m in self._broker_middlewares)
+            ),
+            self._middlewares,
+        ):
+            call = partial(m, call)
+
+        return await call(
+            message,
+            stream=stream_sub.name,
+            maxlen=maxlen,
+            # basic args
+            reply_to=reply_to,
+            headers=headers,
+            correlation_id=correlation_id,
+            # RPC args
+            rpc=rpc,
+            rpc_timeout=rpc_timeout,
+            raise_timeout=raise_timeout,
+        )
```

### Comparing `faststream-0.5.0rc1/faststream/redis/schemas/list_sub.py` & `faststream-0.5.0rc2/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/schemas/proto.py` & `faststream-0.5.0rc2/faststream/redis/schemas/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.0rc2/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.0rc2/faststream/redis/schemas/stream_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/subscriber/asyncapi.py` & `faststream-0.5.0rc2/faststream/redis/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/redis/subscriber/usecase.py` & `faststream-0.5.0rc2/faststream/redis/subscriber/usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     from faststream.broker.message import StreamMessage as BrokerStreamMessage
     from faststream.broker.publisher.proto import ProducerProto
     from faststream.broker.types import (
         AsyncCallable,
         BrokerMiddleware,
         CustomCallable,
     )
-    from faststream.types import AnyDict, LoggerProto
+    from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 TopicName: TypeAlias = bytes
 Offset: TypeAlias = bytes
 
 
 class LogicSubscriber(ABC, SubscriberUsecase[UnifyRedisDict]):
@@ -107,27 +107,29 @@
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
+        _call_decorators: Iterable["Decorator"],
     ) -> None:
         self._client = connection
 
         super().setup(
             logger=logger,
             producer=producer,
             graceful_timeout=graceful_timeout,
             extra_context=extra_context,
             broker_parser=broker_parser,
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
+            _call_decorators=_call_decorators,
         )
 
     def _make_response_publisher(
         self, message: "BrokerStreamMessage[UnifyRedisDict]"
     ) -> Sequence[FakePublisher]:
         if not message.reply_to or self._producer is None:
             return ()
```

### Comparing `faststream-0.5.0rc1/faststream/testing/app.py` & `faststream-0.5.0rc2/faststream/testing/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/testing/broker.py` & `faststream-0.5.0rc2/faststream/testing/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/utils/ast.py` & `faststream-0.5.0rc2/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/utils/classes.py` & `faststream-0.5.0rc2/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/utils/data.py` & `faststream-0.5.0rc2/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/utils/functions.py` & `faststream-0.5.0rc2/faststream/utils/functions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/utils/no_cast.py` & `faststream-0.5.0rc2/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/utils/path.py` & `faststream-0.5.0rc2/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/utils/context/builders.py` & `faststream-0.5.0rc2/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/utils/context/repository.py` & `faststream-0.5.0rc2/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/faststream/utils/context/types.py` & `faststream-0.5.0rc2/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/scripts/build-docs-pre-commit.sh` & `faststream-0.5.0rc2/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/scripts/lint-pre-commit.sh` & `faststream-0.5.0rc2/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/scripts/set_variables.sh` & `faststream-0.5.0rc2/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/scripts/static-pre-commit.sh` & `faststream-0.5.0rc2/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/LICENSE` & `faststream-0.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/README.md` & `faststream-0.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc1/pyproject.toml` & `faststream-0.5.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -71,26 +71,26 @@
 
 nats = ["nats-py>=2.3.1,<=3.0.0"]
 
 redis = ["redis>=5.0.0,<6.0.0"]
 
 # dev dependencies
 devdocs = [
-    "mkdocs-material==9.5.16",
+    "mkdocs-material==9.5.17",
     "mkdocs-static-i18n==1.2.2",
     "mdx-include==1.4.2",
     "mkdocstrings[python]==0.24.1",
     "mkdocs-literate-nav==0.6.1",
     "mkdocs-git-revision-date-localized-plugin==1.2.4",
     "mike==2.0.0",                                      # versioning
     "mkdocs-minify-plugin==0.8.0",
     "mkdocs-macros-plugin==1.0.5",                      # includes with variables
     "mkdocs-glightbox==0.3.7",                          # img zoom
-    "pillow==10.2.0",                                   # required for mkdocs-glightbo
-    "cairosvg==2.7.1",                                  # required for mkdocs-glightbo
+    "pillow",                                           # required for mkdocs-glightbo
+    "cairosvg",                                         # required for mkdocs-glightbo
     "requests",                                         # using in CI, do not pin it
 ]
 
 types = [
     "faststream[rabbit,confluent,kafka,nats,redis]",
     "mypy==1.9.0",
     # mypy extensions
@@ -110,32 +110,32 @@
     "semgrep==1.67.0",
     "codespell==2.2.6",
 ]
 
 test-core = [
     "coverage[toml]==7.4.4",
     "pytest==8.1.1",
-    "pytest-asyncio==0.23.5.post1",
+    "pytest-asyncio==0.23.6",
     "dirty-equals==0.7.1.post0",
 ]
 
 testing = [
     "faststream[test-core]",
-    "fastapi==0.109.2",
+    "fastapi==0.110.1",
     "pydantic-settings>=2.0.0,<3.0.0",
     "httpx==0.27.0",
     "PyYAML==6.0.1",
     "watchfiles==0.21.0",
     "email-validator==2.1.1",
 ]
 
 dev = [
     "faststream[rabbit,kafka,confluent,nats,redis,lint,testing,devdocs]",
     "pre-commit==3.5.0; python_version < '3.9'",
-    "pre-commit==3.6.2; python_version >= '3.9'",
+    "pre-commit==3.7.0; python_version >= '3.9'",
     "detect-secrets==1.4.0",
 ]
 
 [project.urls]
 Homepage = "https://faststream.airt.ai/latest/"
 Documentation = "https://faststream.airt.ai/latest/getting-started/"
 Tracker = "https://github.com/airtai/FastStream/issues"
```

### Comparing `faststream-0.5.0rc1/PKG-INFO` & `faststream-0.5.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.0rc1
+Version: 0.5.0rc2
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
@@ -44,28 +44,28 @@
 Requires-Dist: typing-extensions>=4.8.0
 Provides-Extra: confluent
 Requires-Dist: confluent-kafka<3,>=2; extra == 'confluent'
 Provides-Extra: dev
 Requires-Dist: detect-secrets==1.4.0; extra == 'dev'
 Requires-Dist: faststream[confluent,devdocs,kafka,lint,nats,rabbit,redis,testing]; extra == 'dev'
 Requires-Dist: pre-commit==3.5.0; (python_version < '3.9') and extra == 'dev'
-Requires-Dist: pre-commit==3.6.2; (python_version >= '3.9') and extra == 'dev'
+Requires-Dist: pre-commit==3.7.0; (python_version >= '3.9') and extra == 'dev'
 Provides-Extra: devdocs
-Requires-Dist: cairosvg==2.7.1; extra == 'devdocs'
+Requires-Dist: cairosvg; extra == 'devdocs'
 Requires-Dist: mdx-include==1.4.2; extra == 'devdocs'
 Requires-Dist: mike==2.0.0; extra == 'devdocs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == 'devdocs'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'devdocs'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'devdocs'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'devdocs'
-Requires-Dist: mkdocs-material==9.5.16; extra == 'devdocs'
+Requires-Dist: mkdocs-material==9.5.17; extra == 'devdocs'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'devdocs'
 Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'devdocs'
 Requires-Dist: mkdocstrings[python]==0.24.1; extra == 'devdocs'
-Requires-Dist: pillow==10.2.0; extra == 'devdocs'
+Requires-Dist: pillow; extra == 'devdocs'
 Requires-Dist: requests; extra == 'devdocs'
 Provides-Extra: kafka
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'kafka'
 Provides-Extra: lint
 Requires-Dist: bandit==1.7.8; extra == 'lint'
 Requires-Dist: codespell==2.2.6; extra == 'lint'
 Requires-Dist: faststream[types]; extra == 'lint'
@@ -76,19 +76,19 @@
 Provides-Extra: rabbit
 Requires-Dist: aio-pika<10,>=9; extra == 'rabbit'
 Provides-Extra: redis
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'redis'
 Provides-Extra: test-core
 Requires-Dist: coverage[toml]==7.4.4; extra == 'test-core'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'test-core'
-Requires-Dist: pytest-asyncio==0.23.5.post1; extra == 'test-core'
+Requires-Dist: pytest-asyncio==0.23.6; extra == 'test-core'
 Requires-Dist: pytest==8.1.1; extra == 'test-core'
 Provides-Extra: testing
 Requires-Dist: email-validator==2.1.1; extra == 'testing'
-Requires-Dist: fastapi==0.109.2; extra == 'testing'
+Requires-Dist: fastapi==0.110.1; extra == 'testing'
 Requires-Dist: faststream[test-core]; extra == 'testing'
 Requires-Dist: httpx==0.27.0; extra == 'testing'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'testing'
 Requires-Dist: pyyaml==6.0.1; extra == 'testing'
 Requires-Dist: watchfiles==0.21.0; extra == 'testing'
 Provides-Extra: types
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'types'
```

