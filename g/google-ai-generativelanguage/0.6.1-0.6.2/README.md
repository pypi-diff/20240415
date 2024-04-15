# Comparing `tmp/google-ai-generativelanguage-0.6.1.tar.gz` & `tmp/google-ai-generativelanguage-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-ai-generativelanguage-0.6.1.tar", last modified: Wed Apr  3 01:21:39 2024, max compression
+gzip compressed data, was "google-ai-generativelanguage-0.6.2.tar", last modified: Mon Apr 15 13:58:11 2024, max compression
```

## Comparing `google-ai-generativelanguage-0.6.1.tar` & `google-ai-generativelanguage-0.6.2.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.352468 google-ai-generativelanguage-0.6.1/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5188 2024-04-03 01:21:39.352468 google-ai-generativelanguage-0.6.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3800 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.276462 google-ai-generativelanguage-0.6.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.284462 google-ai-generativelanguage-0.6.1/google/ai/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.288463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage/
--rw-rw-r--   0 root         (0)     1003     9811 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.288463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/
--rw-rw-r--   0 root         (0)     1003     2229 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3669 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.288463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.292463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    45932 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    61250 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.292463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10725 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19633 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19938 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    46100 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.292463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27020 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    43332 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003     5747 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.296463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7270 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15410 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15664 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    26746 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.296463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/
--rw-rw-r--   0 root         (0)     1003     1759 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2895 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/citation.py
--rw-rw-r--   0 root         (0)     1003     3720 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/content.py
--rw-rw-r--   0 root         (0)     1003    20134 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/generative_service.py
--rw-rw-r--   0 root         (0)     1003     4665 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/model.py
--rw-rw-r--   0 root         (0)     1003     3143 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     6161 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/safety.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.296463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/
--rw-rw-r--   0 root         (0)     1003     8304 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    21107 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.296463 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.300464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24748 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    40660 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.300464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7451 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13414 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13641 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18401 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.300464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24788 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    41498 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/client.py
--rw-rw-r--   0 root         (0)     1003     5737 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.300464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7453 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15040 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15336 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    24426 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.304464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47141 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    62455 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.304464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10886 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18398 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18725 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41119 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.304464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47264 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    62596 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003    10950 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.308464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11616 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19686 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20146 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41543 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.308464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41727 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    57530 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/client.py
--rw-rw-r--   0 root         (0)     1003     6013 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.308464 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10464 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18156 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18520 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41155 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.312465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/
--rw-rw-r--   0 root         (0)     1003      777 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    97421 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   112654 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/client.py
--rw-rw-r--   0 root         (0)     1003    16011 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.312465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20205 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33226 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    33948 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   105077 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.312465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    35868 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51394 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.312465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9013 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15599 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15899 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    28406 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.320465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     7020 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2903 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/citation.py
--rw-rw-r--   0 root         (0)     1003    17360 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/content.py
--rw-rw-r--   0 root         (0)     1003    11601 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003     3393 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/file.py
--rw-rw-r--   0 root         (0)     1003     3555 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/file_service.py
--rw-rw-r--   0 root         (0)     1003    37125 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/generative_service.py
--rw-rw-r--   0 root         (0)     1003     4669 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/model.py
--rw-rw-r--   0 root         (0)     1003     9676 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     4530 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/permission.py
--rw-rw-r--   0 root         (0)     1003     6362 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/permission_service.py
--rw-rw-r--   0 root         (0)     1003    13703 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/retriever.py
--rw-rw-r--   0 root         (0)     1003    24469 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/retriever_service.py
--rw-rw-r--   0 root         (0)     1003     8594 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/safety.py
--rw-rw-r--   0 root         (0)     1003    14378 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/text_service.py
--rw-rw-r--   0 root         (0)     1003    13772 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/tuned_model.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.320465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/
--rw-rw-r--   0 root         (0)     1003     2426 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     3627 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.320465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.320465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24701 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    40613 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.320465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7391 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13355 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13582 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18341 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.324465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    21080 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    36905 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003     5792 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.324465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7203 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12847 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13101 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    16216 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.324465 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    25037 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    40877 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.328466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7273 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13103 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13341 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17420 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.328466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     1847 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2905 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/citation.py
--rw-rw-r--   0 root         (0)     1003    11613 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003     4670 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/model.py
--rw-rw-r--   0 root         (0)     1003     3158 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     7878 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/safety.py
--rw-rw-r--   0 root         (0)     1003    10981 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.328466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/
--rw-rw-r--   0 root         (0)     1003     4188 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003     8993 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.328466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.328466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24142 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    40676 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.332466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6769 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13417 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13644 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18404 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.332466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    45130 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    62639 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003    10967 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.332466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9226 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19696 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20156 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41554 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.336466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    40149 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    57825 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/client.py
--rw-rw-r--   0 root         (0)     1003     6022 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.336466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8758 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18165 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18529 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    40318 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.336466 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    34750 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51520 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.340467 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7647 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15604 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15904 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    28412 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.340467 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/
--rw-rw-r--   0 root         (0)     1003     3416 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2905 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/citation.py
--rw-rw-r--   0 root         (0)     1003    11613 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003     4670 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/model.py
--rw-rw-r--   0 root         (0)     1003     8924 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     4460 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/permission.py
--rw-rw-r--   0 root         (0)     1003     6197 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/permission_service.py
--rw-rw-r--   0 root         (0)     1003     7974 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/safety.py
--rw-rw-r--   0 root         (0)     1003    13777 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/text_service.py
--rw-rw-r--   0 root         (0)     1003    12841 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/tuned_model.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.344467 google-ai-generativelanguage-0.6.1/google_ai_generativelanguage.egg-info/
--rw-r--r--   0 root         (0)     1003     5188 2024-04-03 01:21:39.000000 google-ai-generativelanguage-0.6.1/google_ai_generativelanguage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    15729 2024-04-03 01:21:39.000000 google-ai-generativelanguage-0.6.1/google_ai_generativelanguage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:21:39.000000 google-ai-generativelanguage-0.6.1/google_ai_generativelanguage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:21:39.000000 google-ai-generativelanguage-0.6.1/google_ai_generativelanguage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-04-03 01:21:39.000000 google-ai-generativelanguage-0.6.1/google_ai_generativelanguage.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-03 01:21:39.000000 google-ai-generativelanguage-0.6.1/google_ai_generativelanguage.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-03 01:21:39.352468 google-ai-generativelanguage-0.6.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3201 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.344467 google-ai-generativelanguage-0.6.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.344467 google-ai-generativelanguage-0.6.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.344467 google-ai-generativelanguage-0.6.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.344467 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   199891 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1/test_generative_service.py
--rw-rw-r--   0 root         (0)     1003   136179 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1/test_model_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.348467 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   113238 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003   133274 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_file_service.py
--rw-rw-r--   0 root         (0)     1003   201546 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py
--rw-rw-r--   0 root         (0)     1003   233901 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py
--rw-rw-r--   0 root         (0)     1003   208818 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py
--rw-rw-r--   0 root         (0)     1003   481948 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py
--rw-rw-r--   0 root         (0)     1003   151028 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.348467 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003   113184 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003   114125 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py
--rw-rw-r--   0 root         (0)     1003   110150 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:39.352468 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003   113246 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003   233746 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py
--rw-rw-r--   0 root         (0)     1003   209388 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py
--rw-rw-r--   0 root         (0)     1003   151575 2024-04-03 01:18:24.000000 google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.537348 google-ai-generativelanguage-0.6.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5604 2024-04-15 13:58:11.537348 google-ai-generativelanguage-0.6.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4216 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.297332 google-ai-generativelanguage-0.6.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.301332 google-ai-generativelanguage-0.6.2/google/ai/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.309333 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage/
+-rw-rw-r--   0 root         (0)     1003     9811 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.313333 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/
+-rw-rw-r--   0 root         (0)     1003     2229 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3669 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.313333 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.317333 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    45932 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    61250 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.329334 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10725 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19633 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19938 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    46280 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.333334 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27020 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43332 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5747 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.337334 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7270 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15410 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15664 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    26746 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.341335 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1759 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2895 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/citation.py
+-rw-rw-r--   0 root         (0)     1003     3720 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/content.py
+-rw-rw-r--   0 root         (0)     1003    20990 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/generative_service.py
+-rw-rw-r--   0 root         (0)     1003     4802 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/model.py
+-rw-rw-r--   0 root         (0)     1003     3143 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     6161 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/safety.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.345335 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/
+-rw-rw-r--   0 root         (0)     1003     8304 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21107 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.345335 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.349335 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24748 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40660 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.353335 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7451 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13414 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13641 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18401 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.357336 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24788 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41498 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5737 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.361336 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7453 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15040 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15336 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    24426 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.365336 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47141 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62455 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.369336 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10886 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18398 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18725 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41119 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.373337 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47264 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62596 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10950 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.377337 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11616 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19686 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20146 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41543 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.381337 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41727 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    57530 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6013 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.385338 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10464 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18156 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18520 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41155 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.393338 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/
+-rw-rw-r--   0 root         (0)     1003      777 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    97421 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   112654 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16011 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.397338 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20205 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33226 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    33948 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   105077 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.401339 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35868 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51394 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.405339 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9013 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15599 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15899 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    28406 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.421340 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     7020 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2903 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    17360 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/content.py
+-rw-rw-r--   0 root         (0)     1003    11601 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003     3393 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/file.py
+-rw-rw-r--   0 root         (0)     1003     3555 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/file_service.py
+-rw-rw-r--   0 root         (0)     1003    38481 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/generative_service.py
+-rw-rw-r--   0 root         (0)     1003     4806 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/model.py
+-rw-rw-r--   0 root         (0)     1003     9676 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     4530 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/permission.py
+-rw-rw-r--   0 root         (0)     1003     6362 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/permission_service.py
+-rw-rw-r--   0 root         (0)     1003    13703 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/retriever.py
+-rw-rw-r--   0 root         (0)     1003    24469 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/retriever_service.py
+-rw-rw-r--   0 root         (0)     1003     8594 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    14378 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/text_service.py
+-rw-rw-r--   0 root         (0)     1003    13772 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/tuned_model.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.421340 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     2426 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3627 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.425340 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.425340 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24701 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40613 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.429340 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7391 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13355 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13582 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18341 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.433341 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21080 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    36905 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5792 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.437341 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7203 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12847 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13101 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    16216 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.441341 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25037 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40877 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.445341 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7273 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13103 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13341 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17420 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.449342 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     1847 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2905 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    11613 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003     4670 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/model.py
+-rw-rw-r--   0 root         (0)     1003     3158 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     7878 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    10981 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.453342 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/
+-rw-rw-r--   0 root         (0)     1003     4188 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8993 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.453342 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.453342 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24142 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40676 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.457342 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6769 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13417 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13644 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18404 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.465343 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    45130 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62639 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10967 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.469343 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9226 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19696 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20156 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41554 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.473343 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    40149 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    57825 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6022 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.477344 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8758 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18165 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18529 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    40318 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.481344 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34750 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51520 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.485344 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7647 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15604 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15904 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    28412 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.493345 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/
+-rw-rw-r--   0 root         (0)     1003     3416 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2905 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    11613 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003     4670 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/model.py
+-rw-rw-r--   0 root         (0)     1003     8924 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     4460 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/permission.py
+-rw-rw-r--   0 root         (0)     1003     6197 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/permission_service.py
+-rw-rw-r--   0 root         (0)     1003     7974 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    13777 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/text_service.py
+-rw-rw-r--   0 root         (0)     1003    12841 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/tuned_model.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.497345 google-ai-generativelanguage-0.6.2/google_ai_generativelanguage.egg-info/
+-rw-r--r--   0 root         (0)     1003     5604 2024-04-15 13:58:11.000000 google-ai-generativelanguage-0.6.2/google_ai_generativelanguage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    15729 2024-04-15 13:58:11.000000 google-ai-generativelanguage-0.6.2/google_ai_generativelanguage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:58:11.000000 google-ai-generativelanguage-0.6.2/google_ai_generativelanguage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:58:11.000000 google-ai-generativelanguage-0.6.2/google_ai_generativelanguage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-04-15 13:58:11.000000 google-ai-generativelanguage-0.6.2/google_ai_generativelanguage.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-15 13:58:11.000000 google-ai-generativelanguage-0.6.2/google_ai_generativelanguage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-15 13:58:11.537348 google-ai-generativelanguage-0.6.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3201 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.497345 google-ai-generativelanguage-0.6.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.497345 google-ai-generativelanguage-0.6.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.497345 google-ai-generativelanguage-0.6.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.501345 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   199891 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1/test_generative_service.py
+-rw-rw-r--   0 root         (0)     1003   136179 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1/test_model_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.517346 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   113238 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003   133274 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_file_service.py
+-rw-rw-r--   0 root         (0)     1003   201546 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py
+-rw-rw-r--   0 root         (0)     1003   233901 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003   208818 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py
+-rw-rw-r--   0 root         (0)     1003   481948 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py
+-rw-rw-r--   0 root         (0)     1003   151028 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.529347 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   113184 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003   114125 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003   110150 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:11.537348 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003   113246 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003   233746 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003   209388 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py
+-rw-rw-r--   0 root         (0)     1003   151575 2024-04-15 13:54:43.000000 google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py
```

### Comparing `google-ai-generativelanguage-0.6.1/LICENSE` & `google-ai-generativelanguage-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/MANIFEST.in` & `google-ai-generativelanguage-0.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/PKG-INFO` & `google-ai-generativelanguage-0.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-generativelanguage
-Version: 0.6.1
+Version: 0.6.2
 Summary: Google Ai Generativelanguage API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ai-generativelanguage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -28,42 +28,42 @@
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 
 Python Client for Generative Language API
 =========================================
 
 |preview| |pypi| |versions|
 
-`Generative Language API`_: Generative Language API
+`Generative Language API`_: The Gemini API allows developers to build generative AI applications using Gemini models. Gemini is our most capable model, built from the ground up to be multimodal. It can generalize and seamlessly understand, operate across, and combine different types of information including language, images, audio, video, and code. You can use the Gemini API for use cases like reasoning across text and images, content generation, dialogue agents, summarization and classification systems, and more.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
-.. _Generative Language API: https://developers.generativeai.google/
+.. _Generative Language API: https://ai.google.dev/docs
 .. _Client Library Documentation: https://googleapis.dev/python/generativelanguage/latest
-.. _Product Documentation:  https://developers.generativeai.google/
+.. _Product Documentation:  https://ai.google.dev/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
 3. `Enable the Generative Language API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Generative Language API.:  https://developers.generativeai.google/
+.. _Enable the Generative Language API.:  https://ai.google.dev/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
 creates isolated Python environments. These isolated environments can have separate
@@ -129,9 +129,9 @@
 -  Read the `Client Library Documentation`_ for Generative Language API
    to see other available methods on the client.
 -  Read the `Generative Language API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Generative Language API Product documentation:  https://developers.generativeai.google/
+.. _Generative Language API Product documentation:  https://ai.google.dev/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-ai-generativelanguage-0.6.1/README.rst` & `google-ai-generativelanguage-0.6.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Python Client for Generative Language API
 =========================================
 
 |preview| |pypi| |versions|
 
-`Generative Language API`_: Generative Language API
+`Generative Language API`_: The Gemini API allows developers to build generative AI applications using Gemini models. Gemini is our most capable model, built from the ground up to be multimodal. It can generalize and seamlessly understand, operate across, and combine different types of information including language, images, audio, video, and code. You can use the Gemini API for use cases like reasoning across text and images, content generation, dialogue agents, summarization and classification systems, and more.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
-.. _Generative Language API: https://developers.generativeai.google/
+.. _Generative Language API: https://ai.google.dev/docs
 .. _Client Library Documentation: https://googleapis.dev/python/generativelanguage/latest
-.. _Product Documentation:  https://developers.generativeai.google/
+.. _Product Documentation:  https://ai.google.dev/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
 3. `Enable the Generative Language API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Generative Language API.:  https://developers.generativeai.google/
+.. _Enable the Generative Language API.:  https://ai.google.dev/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
 creates isolated Python environments. These isolated environments can have separate
@@ -100,9 +100,9 @@
 -  Read the `Client Library Documentation`_ for Generative Language API
    to see other available methods on the client.
 -  Read the `Generative Language API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Generative Language API Product documentation:  https://developers.generativeai.google/
+.. _Generative Language API Product documentation:  https://ai.google.dev/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage/gapic_version.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.1"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/gapic_metadata.json` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/gapic_version.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.1"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -735,14 +735,19 @@
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
                     "uri": "/v1/{model=models/*}:generateContent",
                     "body": "*",
                 },
+                {
+                    "method": "post",
+                    "uri": "/v1/{model=tunedModels/*}:generateContent",
+                    "body": "*",
+                },
             ]
             request, metadata = self._interceptor.pre_generate_content(
                 request, metadata
             )
             pb_request = generative_service.GenerateContentRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/services/model_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/citation.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/citation.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/content.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/content.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/generative_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/generative_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,21 +60,29 @@
             STS.
         CLASSIFICATION (4):
             Specifies that the given text will be
             classified.
         CLUSTERING (5):
             Specifies that the embeddings will be used
             for clustering.
+        QUESTION_ANSWERING (6):
+            Specifies that the given text will be used
+            for question answering.
+        FACT_VERIFICATION (7):
+            Specifies that the given text will be used
+            for fact verification.
     """
     TASK_TYPE_UNSPECIFIED = 0
     RETRIEVAL_QUERY = 1
     RETRIEVAL_DOCUMENT = 2
     SEMANTIC_SIMILARITY = 3
     CLASSIFICATION = 4
     CLUSTERING = 5
+    QUESTION_ANSWERING = 6
+    FACT_VERIFICATION = 7
 
 
 class GenerateContentRequest(proto.Message):
     r"""Request to generate a completion from the model.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
@@ -143,44 +151,43 @@
     all parameters may be configurable for every model.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         candidate_count (int):
-            Optional. Number of generated responses to return.
-
-            This value must be between [1, 8], inclusive. If unset, this
-            will default to 1.
+            Optional. Number of generated responses to
+            return.
+            Currently, this value can only be set to 1. If
+            unset, this will default to 1.
 
             This field is a member of `oneof`_ ``_candidate_count``.
         stop_sequences (MutableSequence[str]):
             Optional. The set of character sequences (up
             to 5) that will stop output generation. If
             specified, the API will stop at the first
             appearance of a stop sequence. The stop sequence
             will not be included as part of the response.
         max_output_tokens (int):
             Optional. The maximum number of tokens to include in a
             candidate.
 
-            If unset, this will default to output_token_limit specified
-            in the ``Model`` specification.
+            Note: The default value varies by model, see the
+            ``Model.output_token_limit`` attribute of the ``Model``
+            returned from the ``getModel`` function.
 
             This field is a member of `oneof`_ ``_max_output_tokens``.
         temperature (float):
-            Optional. Controls the randomness of the output. Note: The
-            default value varies by model, see the ``Model.temperature``
-            attribute of the ``Model`` returned the ``getModel``
-            function.
-
-            Values can range from [0.0,1.0], inclusive. A value closer
-            to 1.0 will produce responses that are more varied and
-            creative, while a value closer to 0.0 will typically result
-            in more straightforward responses from the model.
+            Optional. Controls the randomness of the output.
+
+            Note: The default value varies by model, see the
+            ``Model.temperature`` attribute of the ``Model`` returned
+            from the ``getModel`` function.
+
+            Values can range from [0.0, 2.0].
 
             This field is a member of `oneof`_ ``_temperature``.
         top_p (float):
             Optional. The maximum cumulative probability of tokens to
             consider when sampling.
 
             The model uses combined Top-k and nucleus sampling.
@@ -188,30 +195,32 @@
             Tokens are sorted based on their assigned probabilities so
             that only the most likely tokens are considered. Top-k
             sampling directly limits the maximum number of tokens to
             consider, while Nucleus sampling limits number of tokens
             based on the cumulative probability.
 
             Note: The default value varies by model, see the
-            ``Model.top_p`` attribute of the ``Model`` returned the
+            ``Model.top_p`` attribute of the ``Model`` returned from the
             ``getModel`` function.
 
             This field is a member of `oneof`_ ``_top_p``.
         top_k (int):
             Optional. The maximum number of tokens to consider when
             sampling.
 
-            The model uses combined Top-k and nucleus sampling.
-
-            Top-k sampling considers the set of ``top_k`` most probable
-            tokens. Defaults to 40.
+            Models use nucleus sampling or combined Top-k and nucleus
+            sampling. Top-k sampling considers the set of ``top_k`` most
+            probable tokens. Models running with nucleus sampling don't
+            allow top_k setting.
 
             Note: The default value varies by model, see the
-            ``Model.top_k`` attribute of the ``Model`` returned the
-            ``getModel`` function.
+            ``Model.top_k`` attribute of the ``Model`` returned from the
+            ``getModel`` function. Empty ``top_k`` field in ``Model``
+            indicates the model doesn't apply top-k sampling and doesn't
+            allow setting ``top_k`` on requests.
 
             This field is a member of `oneof`_ ``_top_k``.
     """
 
     candidate_count: int = proto.Field(
         proto.INT32,
         number=1,
@@ -442,14 +451,21 @@
             Optional. An optional title for the text. Only applicable
             when TaskType is ``RETRIEVAL_DOCUMENT``.
 
             Note: Specifying a ``title`` for ``RETRIEVAL_DOCUMENT``
             provides better quality embeddings for retrieval.
 
             This field is a member of `oneof`_ ``_title``.
+        output_dimensionality (int):
+            Optional. Optional reduced dimension for the output
+            embedding. If set, excessive values in the output embedding
+            are truncated from the end. Supported by
+            ``models/text-embedding-latest``.
+
+            This field is a member of `oneof`_ ``_output_dimensionality``.
     """
 
     model: str = proto.Field(
         proto.STRING,
         number=1,
     )
     content: gag_content.Content = proto.Field(
@@ -464,14 +480,19 @@
         enum="TaskType",
     )
     title: str = proto.Field(
         proto.STRING,
         number=4,
         optional=True,
     )
+    output_dimensionality: int = proto.Field(
+        proto.INT32,
+        number=5,
+        optional=True,
+    )
 
 
 class ContentEmbedding(proto.Message):
     r"""A list of floats representing an embedding.
 
     Attributes:
         values (MutableSequence[float]):
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/model.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.ai.generativelanguage.v1",
+    package="google.ai.generativelanguage.v1beta2",
     manifest={
         "Model",
     },
 )
 
 
 class Model(proto.Message):
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/model_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1/types/safety.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/safety.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,20 +38,20 @@
     Values:
         HARM_CATEGORY_UNSPECIFIED (0):
             Category is unspecified.
         HARM_CATEGORY_DEROGATORY (1):
             Negative or harmful comments targeting
             identity and/or protected attribute.
         HARM_CATEGORY_TOXICITY (2):
-            Content that is rude, disrepspectful, or
+            Content that is rude, disrespectful, or
             profane.
         HARM_CATEGORY_VIOLENCE (3):
-            Describes scenarios depictng violence against
-            an individual or group, or general descriptions
-            of gore.
+            Describes scenarios depicting violence
+            against an individual or group, or general
+            descriptions of gore.
         HARM_CATEGORY_SEXUAL (4):
             Contains references to sexual acts or other
             lewd content.
         HARM_CATEGORY_MEDICAL (5):
             Promotes unchecked medical advice.
         HARM_CATEGORY_DANGEROUS (6):
             Dangerous content that promotes, facilitates,
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/gapic_metadata.json` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/gapic_version.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.1"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/__init__.py` & `google-ai-generativelanguage-0.6.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/pagers.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/file_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/file_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/citation.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/citation.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/content.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/content.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/discuss_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/file.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/file.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/file_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/file_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/generative_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/generative_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,21 +65,29 @@
             STS.
         CLASSIFICATION (4):
             Specifies that the given text will be
             classified.
         CLUSTERING (5):
             Specifies that the embeddings will be used
             for clustering.
+        QUESTION_ANSWERING (6):
+            Specifies that the given text will be used
+            for question answering.
+        FACT_VERIFICATION (7):
+            Specifies that the given text will be used
+            for fact verification.
     """
     TASK_TYPE_UNSPECIFIED = 0
     RETRIEVAL_QUERY = 1
     RETRIEVAL_DOCUMENT = 2
     SEMANTIC_SIMILARITY = 3
     CLASSIFICATION = 4
     CLUSTERING = 5
+    QUESTION_ANSWERING = 6
+    FACT_VERIFICATION = 7
 
 
 class GenerateContentRequest(proto.Message):
     r"""Request to generate a completion from the model.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
@@ -208,15 +216,15 @@
         temperature (float):
             Optional. Controls the randomness of the output.
 
             Note: The default value varies by model, see the
             ``Model.temperature`` attribute of the ``Model`` returned
             from the ``getModel`` function.
 
-            Values can range from [0.0, infinity).
+            Values can range from [0.0, 2.0].
 
             This field is a member of `oneof`_ ``_temperature``.
         top_p (float):
             Optional. The maximum cumulative probability of tokens to
             consider when sampling.
 
             The model uses combined Top-k and nucleus sampling.
@@ -232,24 +240,31 @@
             ``getModel`` function.
 
             This field is a member of `oneof`_ ``_top_p``.
         top_k (int):
             Optional. The maximum number of tokens to consider when
             sampling.
 
-            The model uses combined Top-k and nucleus sampling.
-
-            Top-k sampling considers the set of ``top_k`` most probable
-            tokens.
+            Models use nucleus sampling or combined Top-k and nucleus
+            sampling. Top-k sampling considers the set of ``top_k`` most
+            probable tokens. Models running with nucleus sampling don't
+            allow top_k setting.
 
             Note: The default value varies by model, see the
             ``Model.top_k`` attribute of the ``Model`` returned from the
-            ``getModel`` function.
+            ``getModel`` function. Empty ``top_k`` field in ``Model``
+            indicates the model doesn't apply top-k sampling and doesn't
+            allow setting ``top_k`` on requests.
 
             This field is a member of `oneof`_ ``_top_k``.
+        response_mime_type (str):
+            Optional. Output response mimetype of the generated
+            candidate text. Supported mimetype: ``text/plain``:
+            (default) Text output. ``application/json``: JSON response
+            in the candidates.
     """
 
     candidate_count: int = proto.Field(
         proto.INT32,
         number=1,
         optional=True,
     )
@@ -273,14 +288,18 @@
         optional=True,
     )
     top_k: int = proto.Field(
         proto.INT32,
         number=7,
         optional=True,
     )
+    response_mime_type: str = proto.Field(
+        proto.STRING,
+        number=13,
+    )
 
 
 class SemanticRetrieverConfig(proto.Message):
     r"""Configuration for retrieving grounding content from a ``Corpus`` or
     ``Document`` created using the Semantic Retriever API.
 
 
@@ -892,14 +911,21 @@
             Optional. An optional title for the text. Only applicable
             when TaskType is ``RETRIEVAL_DOCUMENT``.
 
             Note: Specifying a ``title`` for ``RETRIEVAL_DOCUMENT``
             provides better quality embeddings for retrieval.
 
             This field is a member of `oneof`_ ``_title``.
+        output_dimensionality (int):
+            Optional. Optional reduced dimension for the output
+            embedding. If set, excessive values in the output embedding
+            are truncated from the end. Supported by
+            ``models/text-embedding-latest``.
+
+            This field is a member of `oneof`_ ``_output_dimensionality``.
     """
 
     model: str = proto.Field(
         proto.STRING,
         number=1,
     )
     content: gag_content.Content = proto.Field(
@@ -914,14 +940,19 @@
         enum="TaskType",
     )
     title: str = proto.Field(
         proto.STRING,
         number=4,
         optional=True,
     )
+    output_dimensionality: int = proto.Field(
+        proto.INT32,
+        number=5,
+        optional=True,
+    )
 
 
 class ContentEmbedding(proto.Message):
     r"""A list of floats representing an embedding.
 
     Attributes:
         values (MutableSequence[float]):
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/model.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.ai.generativelanguage.v1beta",
+    package="google.ai.generativelanguage.v1beta3",
     manifest={
         "Model",
     },
 )
 
 
 class Model(proto.Message):
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/model_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/permission.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/permission.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/permission_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/permission_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/retriever.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/retriever.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/retriever_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/retriever_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/safety.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/safety.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/text_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta/types/tuned_model.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/tuned_model.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/gapic_metadata.json` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/gapic_version.py` & `google-ai-generativelanguage-0.6.2/tests/unit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.1"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/__init__.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/citation.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/citation.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/discuss_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/model.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1/types/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.ai.generativelanguage.v1beta2",
+    package="google.ai.generativelanguage.v1",
     manifest={
         "Model",
     },
 )
 
 
 class Model(proto.Message):
@@ -94,15 +94,17 @@
 
             This field is a member of `oneof`_ ``_top_p``.
         top_k (int):
             For Top-k sampling.
 
             Top-k sampling considers the set of ``top_k`` most probable
             tokens. This value specifies default to be used by the
-            backend while making the call to the model.
+            backend while making the call to the model. If empty,
+            indicates the model doesn't use top-k sampling, and
+            ``top_k`` isn't allowed as a generation parameter.
 
             This field is a member of `oneof`_ ``_top_k``.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/model_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/safety.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/safety.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta2/types/text_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta2/types/text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/gapic_metadata.json` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/gapic_version.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.1"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/__init__.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/client.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/__init__.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/citation.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/citation.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/discuss_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/model.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta/types/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.ai.generativelanguage.v1beta3",
+    package="google.ai.generativelanguage.v1beta",
     manifest={
         "Model",
     },
 )
 
 
 class Model(proto.Message):
@@ -94,15 +94,17 @@
 
             This field is a member of `oneof`_ ``_top_p``.
         top_k (int):
             For Top-k sampling.
 
             Top-k sampling considers the set of ``top_k`` most probable
             tokens. This value specifies default to be used by the
-            backend while making the call to the model.
+            backend while making the call to the model. If empty,
+            indicates the model doesn't use top-k sampling, and
+            ``top_k`` isn't allowed as a generation parameter.
 
             This field is a member of `oneof`_ ``_top_k``.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/model_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/permission.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/permission.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/permission_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/permission_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/safety.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/safety.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/text_service.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google/ai/generativelanguage_v1beta3/types/tuned_model.py` & `google-ai-generativelanguage-0.6.2/google/ai/generativelanguage_v1beta3/types/tuned_model.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/google_ai_generativelanguage.egg-info/PKG-INFO` & `google-ai-generativelanguage-0.6.2/google_ai_generativelanguage.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-generativelanguage
-Version: 0.6.1
+Version: 0.6.2
 Summary: Google Ai Generativelanguage API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ai-generativelanguage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -28,42 +28,42 @@
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 
 Python Client for Generative Language API
 =========================================
 
 |preview| |pypi| |versions|
 
-`Generative Language API`_: Generative Language API
+`Generative Language API`_: The Gemini API allows developers to build generative AI applications using Gemini models. Gemini is our most capable model, built from the ground up to be multimodal. It can generalize and seamlessly understand, operate across, and combine different types of information including language, images, audio, video, and code. You can use the Gemini API for use cases like reasoning across text and images, content generation, dialogue agents, summarization and classification systems, and more.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-ai-generativelanguage.svg
    :target: https://pypi.org/project/google-ai-generativelanguage/
-.. _Generative Language API: https://developers.generativeai.google/
+.. _Generative Language API: https://ai.google.dev/docs
 .. _Client Library Documentation: https://googleapis.dev/python/generativelanguage/latest
-.. _Product Documentation:  https://developers.generativeai.google/
+.. _Product Documentation:  https://ai.google.dev/docs
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
 3. `Enable the Generative Language API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Generative Language API.:  https://developers.generativeai.google/
+.. _Enable the Generative Language API.:  https://ai.google.dev/docs
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
 creates isolated Python environments. These isolated environments can have separate
@@ -129,9 +129,9 @@
 -  Read the `Client Library Documentation`_ for Generative Language API
    to see other available methods on the client.
 -  Read the `Generative Language API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Generative Language API Product documentation:  https://developers.generativeai.google/
+.. _Generative Language API Product documentation:  https://ai.google.dev/docs
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-ai-generativelanguage-0.6.1/google_ai_generativelanguage.egg-info/SOURCES.txt` & `google-ai-generativelanguage-0.6.2/google_ai_generativelanguage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/setup.py` & `google-ai-generativelanguage-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/__init__.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/__init__.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1/test_generative_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1/test_generative_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1/test_model_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1/test_model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_file_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_file_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.1/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py` & `google-ai-generativelanguage-0.6.2/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py`

 * *Files identical despite different names*

