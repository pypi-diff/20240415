# Comparing `tmp/aliyun-python-sdk-core-2.9.4.tar.gz` & `tmp/aliyun-python-sdk-core-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-core-2.9.4.tar", last modified: Sun Sep 30 04:07:06 2018, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-core-2.9.5.tar", last modified: Sun Sep 30 04:30:53 2018, max compression
```

## Comparing `aliyun-python-sdk-core-2.9.4.tar` & `aliyun-python-sdk-core-2.9.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/
--rw-r--r--   0 haowei.yao (55176) users      (100)    18690 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/request.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/
--rw-r--r--   0 haowei.yao (55176) users      (100)       26 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1013 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/error_type.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1501 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/error_code.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     2153 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/error_msg.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     2712 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/exceptions.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/
--rw-r--r--   0 haowei.yao (55176) users      (100)        1 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1430 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/region_provider.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/
--rw-r--r--   0 haowei.yao (55176) users      (100)        1 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)      177 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)      573 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/user_config_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)      360 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/request_domain_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1290 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/location_service_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)      776 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/local_regional_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)      613 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/local_global_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)        1 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)    25958 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/endpoint_profile.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1495 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/endpoint_resolver.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/algorithm/
--rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/algorithm/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1232 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/algorithm/sha_hmac1.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1827 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/algorithm/sha_hmac256.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/composer/
--rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/composer/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     3097 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/composer/rpc_signature_composer.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     4183 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/composer/oss_signature_composer.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     5776 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/composer/roa_signature_composer.py
--rw-r--r--   0 haowei.yao (55176) users      (100)       26 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/__init__.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/
--rw-r--r--   0 haowei.yao (55176) users      (100)     5619 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/rsa_key_pair_signer.py
--rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     3437 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/signer_factory.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1274 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/access_key_signer.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     2656 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/ecs_ram_role_singer.py
--rw-r--r--   0 haowei.yao (55176) users      (100)      976 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/signer.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     3862 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/ram_role_arn_signer.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1498 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/sts_token_signer.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/utils/
--rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/utils/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1095 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/utils/md5_tool.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1510 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/utils/url_encoder.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1079 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/credentials.py
--rw-r--r--   0 haowei.yao (55176) users      (100)       48 2018-09-30 04:06:10.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/__init__.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/
--rw-r--r--   0 haowei.yao (55176) users      (100)     1741 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/format_type.py
--rw-r--r--   0 haowei.yao (55176) users      (100)       26 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     3237 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/http_request.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     7140 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/http_response.py
--rw-r--r--   0 haowei.yao (55176) users      (100)      921 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/method_type.py
--rw-r--r--   0 haowei.yao (55176) users      (100)      861 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/protocol_type.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     9901 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/client.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/utils/
--rw-r--r--   0 haowei.yao (55176) users      (100)       26 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/utils/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1837 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/utils/parameter_helper.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/
--rw-r--r--   0 haowei.yao (55176) users      (100)      871 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)    30812 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/endpoints.json
--rw-r--r--   0 haowei.yao (55176) users      (100)     1927 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/local_config_global_endpoint_resolver.py
-drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/location/
--rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/location/__init__.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1415 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/location/DescribeEndpointsRequest.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     2052 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/default_endpoint_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     4047 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/local_config_regional_endpoint_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1707 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/endpoint_resolver_base.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1418 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/resolver_endpoint_request.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     5494 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/location_service_endpoint_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1761 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/user_customized_endpoint_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     2945 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/chained_endpoint_resolver.py
--rw-r--r--   0 haowei.yao (55176) users      (100)     1300 2018-09-30 04:07:06.000000 aliyun-python-sdk-core-2.9.4/PKG-INFO
--rw-r--r--   0 haowei.yao (55176) users      (100)     2504 2018-09-30 04:04:29.000000 aliyun-python-sdk-core-2.9.4/setup.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/
+-rw-r--r--   0 haowei.yao (55176) users      (100)    18690 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/request.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/
+-rw-r--r--   0 haowei.yao (55176) users      (100)       26 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1013 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/error_type.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1501 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/error_code.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     2153 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/error_msg.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     2712 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/exceptions.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/
+-rw-r--r--   0 haowei.yao (55176) users      (100)        1 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1430 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/region_provider.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/
+-rw-r--r--   0 haowei.yao (55176) users      (100)        1 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)      177 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)      573 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/user_config_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)      360 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/request_domain_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1290 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/location_service_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)      776 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/local_regional_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)      613 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/local_global_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)        1 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)    25958 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/endpoint_profile.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1495 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/endpoint_resolver.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/algorithm/
+-rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/algorithm/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1232 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/algorithm/sha_hmac1.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1827 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/algorithm/sha_hmac256.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/composer/
+-rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/composer/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     3097 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/composer/rpc_signature_composer.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     4183 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/composer/oss_signature_composer.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     5776 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/composer/roa_signature_composer.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)       26 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/__init__.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/
+-rw-r--r--   0 haowei.yao (55176) users      (100)     5619 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/rsa_key_pair_signer.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     3437 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/signer_factory.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1274 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/access_key_signer.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     2656 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/ecs_ram_role_singer.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)      976 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/signer.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     3862 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/ram_role_arn_signer.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1498 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/sts_token_signer.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/utils/
+-rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/utils/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1095 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/utils/md5_tool.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1510 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/utils/url_encoder.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1079 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/credentials.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)       48 2018-09-30 04:30:37.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/__init__.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1741 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/format_type.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)       26 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     3237 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/http_request.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     7140 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/http_response.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)      921 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/method_type.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)      861 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/protocol_type.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     9901 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/client.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/utils/
+-rw-r--r--   0 haowei.yao (55176) users      (100)       26 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/utils/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1837 2018-09-12 13:19:03.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/utils/parameter_helper.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/
+-rw-r--r--   0 haowei.yao (55176) users      (100)      871 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)    30812 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/endpoints.json
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1927 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/local_config_global_endpoint_resolver.py
+drwxr-xr-x   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/location/
+-rw-r--r--   0 haowei.yao (55176) users      (100)        0 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/location/__init__.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1415 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/location/DescribeEndpointsRequest.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     2052 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/default_endpoint_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     4047 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/local_config_regional_endpoint_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1707 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/endpoint_resolver_base.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1418 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/resolver_endpoint_request.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     5494 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/location_service_endpoint_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1761 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/user_customized_endpoint_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     2945 2018-09-30 04:03:27.000000 aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/chained_endpoint_resolver.py
+-rw-r--r--   0 haowei.yao (55176) users      (100)     1324 2018-09-30 04:30:53.000000 aliyun-python-sdk-core-2.9.5/PKG-INFO
+-rw-r--r--   0 haowei.yao (55176) users      (100)     2839 2018-09-30 04:29:12.000000 aliyun-python-sdk-core-2.9.5/setup.py
```

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/request.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/request.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/error_type.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/error_type.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/error_code.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/error_code.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/error_msg.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/error_msg.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/acs_exception/exceptions.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/acs_exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/region_provider.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/region_provider.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/user_config_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/user_config_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/location_service_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/location_service_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/local_regional_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/local_regional_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/resolvers/local_global_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/resolvers/local_global_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/endpoint_profile.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/endpoint_profile.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/profile/endpoint/endpoint_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/profile/endpoint/endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/algorithm/sha_hmac1.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/algorithm/sha_hmac1.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/algorithm/sha_hmac256.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/algorithm/sha_hmac256.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/composer/rpc_signature_composer.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/composer/rpc_signature_composer.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/composer/oss_signature_composer.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/composer/oss_signature_composer.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/composer/roa_signature_composer.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/composer/roa_signature_composer.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/rsa_key_pair_signer.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/rsa_key_pair_signer.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/signer_factory.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/signer_factory.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/access_key_signer.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/access_key_signer.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/ecs_ram_role_singer.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/ecs_ram_role_singer.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/signer.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/signer.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/ram_role_arn_signer.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/ram_role_arn_signer.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/signers/sts_token_signer.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/signers/sts_token_signer.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/utils/md5_tool.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/utils/md5_tool.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/utils/url_encoder.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/utils/url_encoder.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/auth/credentials.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/format_type.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/format_type.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/http_request.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/http_request.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/http_response.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/http_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/method_type.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/method_type.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/http/protocol_type.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/http/protocol_type.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/client.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/client.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/utils/parameter_helper.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/utils/parameter_helper.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/__init__.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/endpoints.json` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/endpoints.json`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/local_config_global_endpoint_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/local_config_global_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/location/DescribeEndpointsRequest.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/location/DescribeEndpointsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/default_endpoint_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/default_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/local_config_regional_endpoint_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/local_config_regional_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/endpoint_resolver_base.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/endpoint_resolver_base.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/resolver_endpoint_request.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/resolver_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/location_service_endpoint_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/location_service_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/user_customized_endpoint_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/user_customized_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/aliyunsdkcore/endpoint/chained_endpoint_resolver.py` & `aliyun-python-sdk-core-2.9.5/aliyunsdkcore/endpoint/chained_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-core-2.9.4/PKG-INFO` & `aliyun-python-sdk-core-2.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-core
-Version: 2.9.4
+Version: 2.9.5
 Summary: The core module of Aliyun Python SDK.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
-Description: ======================
+Description: 
+        ======================
         aliyun-python-sdk-core
         ======================
         
         
         This is the core module of Aliyun Python SDK.
         
         Aliyun Python SDK is the official software development kit. It makes things easy to integrate your Python application,
         library, or script with Aliyun services.
         
         This module works on Python versions:
         
            * 2.6.5 and greater
         
         
-        Documentation:
+           Documentation:
+        
+           Please visit http://develop.aliyun.com/sdk/python
         
-        Please visit http://develop.aliyun.com/sdk/python
 Keywords: aliyun,sdk,core
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
```

### Comparing `aliyun-python-sdk-core-2.9.4/setup.py` & `aliyun-python-sdk-core-2.9.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,19 +36,34 @@
 AUTHOR = "Aliyun"
 AUTHOR_EMAIL = "aliyun-developers-efficiency@list.alibaba-inc.com"
 URL = "http://develop.aliyun.com/sdk/python"
 
 TOPDIR = os.path.dirname(__file__) or "."
 VERSION = __import__(PACKAGE).__version__
 
-desc_file = open("README.rst")
-try:
-    LONG_DESCRIPTION = desc_file.read()
-finally:
-    desc_file.close()
+LONG_DESCRIPTION = """
+======================
+aliyun-python-sdk-core
+======================
+
+
+This is the core module of Aliyun Python SDK.
+
+Aliyun Python SDK is the official software development kit. It makes things easy to integrate your Python application,
+library, or script with Aliyun services.
+
+This module works on Python versions:
+
+   * 2.6.5 and greater
+
+
+   Documentation:
+
+   Please visit http://develop.aliyun.com/sdk/python
+"""
 
 requires = []
 if platform.system() != "Windows":
     requires.append("pycryptodome>=3.4.7")
 else:
     logging.warning(
         "auth type [publicKeyId] is disabled because 'pycrypto' not support windows, we will resolve this soon")
```

