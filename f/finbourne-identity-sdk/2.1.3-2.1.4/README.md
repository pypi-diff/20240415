# Comparing `tmp/finbourne_identity_sdk-2.1.3.tar.gz` & `tmp/finbourne_identity_sdk-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_identity_sdk-2.1.3.tar", max compression
+gzip compressed data, was "finbourne_identity_sdk-2.1.4.tar", max compression
```

## Comparing `finbourne_identity_sdk-2.1.3.tar` & `finbourne_identity_sdk-2.1.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    16101 2024-04-12 16:51:19.526524 finbourne_identity_sdk-2.1.3/README.md
--rw-r--r--   0        0        0     7317 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/__init__.py
--rw-r--r--   0        0        0      882 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/__init__.py
--rw-r--r--   0        0        0     7558 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/application_metadata_api.py
--rw-r--r--   0        0        0    36614 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/applications_api.py
--rw-r--r--   0        0        0    53741 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/authentication_api.py
--rw-r--r--   0        0        0    15656 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/identity_provider_api.py
--rw-r--r--   0        0        0    14855 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/me_api.py
--rw-r--r--   0        0        0    21850 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/personal_authentication_tokens_api.py
--rw-r--r--   0        0        0    57682 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/roles_api.py
--rw-r--r--   0        0        0     6897 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/tokens_api.py
--rw-r--r--   0        0        0    95611 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/api/users_api.py
--rw-r--r--   0        0        0    30821 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/api_client.py
--rw-r--r--   0        0        0      852 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/api_response.py
--rw-r--r--   0        0        0    14468 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/configuration.py
--rw-r--r--   0        0        0     5347 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/exceptions.py
--rw-r--r--   0        0        0      599 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/__init__.py
--rw-r--r--   0        0        0    30692 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/api_client.py
--rw-r--r--   0        0        0     9902 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8117 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/api_configuration.py
--rw-r--r--   0        0        0     6812 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12711 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/rest.py
--rw-r--r--   0        0        0    11577 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3890 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     5374 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-12 16:51:19.519524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/access_controlled_action.py
--rw-r--r--   0        0        0     4866 2024-04-12 16:51:19.519524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2078 2024-04-12 16:51:19.519524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/action_id.py
--rw-r--r--   0        0        0     2436 2024-04-12 16:51:19.519524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/add_scim_response.py
--rw-r--r--   0        0        0     3349 2024-04-12 16:51:19.519524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/api_key.py
--rw-r--r--   0        0        0     5239 2024-04-12 16:51:19.519524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/authentication_information.py
--rw-r--r--   0        0        0     2784 2024-04-12 16:51:19.519524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/create_api_key.py
--rw-r--r--   0        0        0     4489 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/create_application_request.py
--rw-r--r--   0        0        0     3118 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/create_role_request.py
--rw-r--r--   0        0        0     5261 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/create_user_request.py
--rw-r--r--   0        0        0     3526 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/created_api_key.py
--rw-r--r--   0        0        0     3521 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/current_user_response.py
--rw-r--r--   0        0        0     2776 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/error_detail.py
--rw-r--r--   0        0        0     3192 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/id_selector_definition.py
--rw-r--r--   0        0        0     3117 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2270 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/link.py
--rw-r--r--   0        0        0     4744 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/list_users_response.py
--rw-r--r--   0        0        0     3865 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4701 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     2990 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/o_auth_application.py
--rw-r--r--   0        0        0     2302 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response.py
--rw-r--r--   0        0        0     2311 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response_age.py
--rw-r--r--   0        0        0     2577 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response_complexity.py
--rw-r--r--   0        0        0     3282 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response_conditions.py
--rw-r--r--   0        0        0     2104 2024-04-12 16:51:19.520524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response_lockout.py
--rw-r--r--   0        0        0     4271 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     1922 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/role_id.py
--rw-r--r--   0        0        0     3430 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/role_response.py
--rw-r--r--   0        0        0     1912 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/set_password.py
--rw-r--r--   0        0        0     2770 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/set_password_response.py
--rw-r--r--   0        0        0     1993 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_access_expiry.py
--rw-r--r--   0        0        0     2388 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_access_expiry_with_role.py
--rw-r--r--   0        0        0     3923 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_access_request.py
--rw-r--r--   0        0        0     5257 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_access_response.py
--rw-r--r--   0        0        0     3186 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_role.py
--rw-r--r--   0        0        0     2681 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_roles_response.py
--rw-r--r--   0        0        0     1933 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/temporary_password.py
--rw-r--r--   0        0        0     2363 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request.py
--rw-r--r--   0        0        0     2437 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request_age.py
--rw-r--r--   0        0        0     2638 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request_complexity.py
--rw-r--r--   0        0        0     3380 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request_conditions.py
--rw-r--r--   0        0        0     2188 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request_lockout.py
--rw-r--r--   0        0        0     2557 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_role_request.py
--rw-r--r--   0        0        0     4752 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_user_request.py
--rw-r--r--   0        0        0     5148 2024-04-12 16:51:19.521524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/user_response.py
--rw-r--r--   0        0        0     4920 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/models/user_summary.py
--rw-r--r--   0        0        0        0 2024-04-12 16:51:19.522524 finbourne_identity_sdk-2.1.3/finbourne_identity/py.typed
--rw-r--r--   0        0        0    10172 2024-04-12 16:51:19.523524 finbourne_identity_sdk-2.1.3/finbourne_identity/rest.py
--rw-r--r--   0        0        0      897 2024-04-12 16:51:19.526524 finbourne_identity_sdk-2.1.3/pyproject.toml
--rw-r--r--   0        0        0    17190 1970-01-01 00:00:00.000000 finbourne_identity_sdk-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0    15621 2024-04-15 13:27:23.116445 finbourne_identity_sdk-2.1.4/README.md
+-rw-r--r--   0        0        0     7317 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/__init__.py
+-rw-r--r--   0        0        0      882 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/__init__.py
+-rw-r--r--   0        0        0     7528 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/application_metadata_api.py
+-rw-r--r--   0        0        0    36614 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/applications_api.py
+-rw-r--r--   0        0        0    53621 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/authentication_api.py
+-rw-r--r--   0        0        0    15596 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/identity_provider_api.py
+-rw-r--r--   0        0        0    14825 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/me_api.py
+-rw-r--r--   0        0        0    21760 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/personal_authentication_tokens_api.py
+-rw-r--r--   0        0        0    57442 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/roles_api.py
+-rw-r--r--   0        0        0     6867 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/tokens_api.py
+-rw-r--r--   0        0        0    95281 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/api/users_api.py
+-rw-r--r--   0        0        0    30821 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/api_response.py
+-rw-r--r--   0        0        0    14468 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/configuration.py
+-rw-r--r--   0        0        0     5347 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/exceptions.py
+-rw-r--r--   0        0        0      599 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/__init__.py
+-rw-r--r--   0        0        0    30692 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/api_client.py
+-rw-r--r--   0        0        0     9902 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8117 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6812 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12711 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/rest.py
+-rw-r--r--   0        0        0    11577 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3890 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     5374 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-15 13:27:23.109445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4866 2024-04-15 13:27:23.109445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2078 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/action_id.py
+-rw-r--r--   0        0        0     2436 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/add_scim_response.py
+-rw-r--r--   0        0        0     3349 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/api_key.py
+-rw-r--r--   0        0        0     5239 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/authentication_information.py
+-rw-r--r--   0        0        0     2784 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/create_api_key.py
+-rw-r--r--   0        0        0     4489 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/create_application_request.py
+-rw-r--r--   0        0        0     3118 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/create_role_request.py
+-rw-r--r--   0        0        0     5261 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/create_user_request.py
+-rw-r--r--   0        0        0     3526 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/created_api_key.py
+-rw-r--r--   0        0        0     3521 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/current_user_response.py
+-rw-r--r--   0        0        0     2776 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/error_detail.py
+-rw-r--r--   0        0        0     3192 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3117 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2270 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/link.py
+-rw-r--r--   0        0        0     4744 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/list_users_response.py
+-rw-r--r--   0        0        0     3865 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4701 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     2990 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/o_auth_application.py
+-rw-r--r--   0        0        0     2302 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response.py
+-rw-r--r--   0        0        0     2311 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response_age.py
+-rw-r--r--   0        0        0     2577 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response_complexity.py
+-rw-r--r--   0        0        0     3282 2024-04-15 13:27:23.110445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response_conditions.py
+-rw-r--r--   0        0        0     2104 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response_lockout.py
+-rw-r--r--   0        0        0     4271 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     1922 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/role_id.py
+-rw-r--r--   0        0        0     3430 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/role_response.py
+-rw-r--r--   0        0        0     1912 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/set_password.py
+-rw-r--r--   0        0        0     2770 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/set_password_response.py
+-rw-r--r--   0        0        0     1993 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_access_expiry.py
+-rw-r--r--   0        0        0     2388 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_access_expiry_with_role.py
+-rw-r--r--   0        0        0     3923 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_access_request.py
+-rw-r--r--   0        0        0     5257 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_access_response.py
+-rw-r--r--   0        0        0     3186 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_role.py
+-rw-r--r--   0        0        0     2681 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_roles_response.py
+-rw-r--r--   0        0        0     1933 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/temporary_password.py
+-rw-r--r--   0        0        0     2363 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request.py
+-rw-r--r--   0        0        0     2437 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request_age.py
+-rw-r--r--   0        0        0     2638 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request_complexity.py
+-rw-r--r--   0        0        0     3380 2024-04-15 13:27:23.111445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request_conditions.py
+-rw-r--r--   0        0        0     2188 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request_lockout.py
+-rw-r--r--   0        0        0     2557 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_role_request.py
+-rw-r--r--   0        0        0     4752 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_user_request.py
+-rw-r--r--   0        0        0     5148 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/user_response.py
+-rw-r--r--   0        0        0     4920 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/models/user_summary.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:27:23.112445 finbourne_identity_sdk-2.1.4/finbourne_identity/py.typed
+-rw-r--r--   0        0        0    10172 2024-04-15 13:27:23.113445 finbourne_identity_sdk-2.1.4/finbourne_identity/rest.py
+-rw-r--r--   0        0        0      897 2024-04-15 13:27:23.116445 finbourne_identity_sdk-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0    16710 1970-01-01 00:00:00.000000 finbourne_identity_sdk-2.1.4/PKG-INFO
```

### Comparing `finbourne_identity_sdk-2.1.3/README.md` & `finbourne_identity_sdk-2.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,40 @@
+Metadata-Version: 2.1
+Name: finbourne-identity-sdk
+Version: 2.1.4
+Summary: FINBOURNE Identity Service API
+Home-page: https://github.com/finbourne/finbourne-identity-sdk-python
+License: MIT
+Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Identity Service API,finbourne-identity-sdk
+Author: FINBOURNE Technology
+Author-email: info@finbourne.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aenum (>=3.1.11,<4.0.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: pydantic (>=2.6.3,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2,<3)
+Requires-Dist: urllib3 (>=1.25.3,<2.0.0)
+Project-URL: Repository, https://github.com/finbourne/finbourne-identity-sdk-python
+Description-Content-Type: text/markdown
+
 # finbourne-identity-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.2862
-- Package version: 2.1.3
+- API version: 0.0.2866
+- Package version: 2.1.4
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -169,71 +195,71 @@
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
     api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
-        # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
+        # ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling ApplicationMetadataApi->list_access_controlled_resources: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/identity*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
+*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | ListAccessControlledResources: Get resources available for access control
 *ApplicationsApi* | [**create_application**](docs/ApplicationsApi.md#create_application) | **POST** /api/applications | [EARLY ACCESS] CreateApplication: Create Application
 *ApplicationsApi* | [**delete_application**](docs/ApplicationsApi.md#delete_application) | **DELETE** /api/applications/{id} | [EARLY ACCESS] DeleteApplication: Delete Application
 *ApplicationsApi* | [**get_application**](docs/ApplicationsApi.md#get_application) | **GET** /api/applications/{id} | [EARLY ACCESS] GetApplication: Get Application
 *ApplicationsApi* | [**list_applications**](docs/ApplicationsApi.md#list_applications) | **GET** /api/applications | [EARLY ACCESS] ListApplications: List Applications
 *ApplicationsApi* | [**rotate_application_secrets**](docs/ApplicationsApi.md#rotate_application_secrets) | **POST** /api/applications/{id}/lifecycle/$newsecret | [EARLY ACCESS] RotateApplicationSecrets: Rotate Application Secrets
 *AuthenticationApi* | [**get_authentication_information**](docs/AuthenticationApi.md#get_authentication_information) | **GET** /api/authentication/information | GetAuthenticationInformation: Gets AuthenticationInformation
 *AuthenticationApi* | [**get_password_policy**](docs/AuthenticationApi.md#get_password_policy) | **GET** /api/authentication/password-policy/{userType} | [EXPERIMENTAL] GetPasswordPolicy: Gets password policy for a user type
-*AuthenticationApi* | [**get_support_access_history**](docs/AuthenticationApi.md#get_support_access_history) | **GET** /api/authentication/support | [EARLY ACCESS] GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination
-*AuthenticationApi* | [**get_support_roles**](docs/AuthenticationApi.md#get_support_roles) | **GET** /api/authentication/support-roles | [EARLY ACCESS] GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation
-*AuthenticationApi* | [**grant_support_access**](docs/AuthenticationApi.md#grant_support_access) | **POST** /api/authentication/support | [EARLY ACCESS] GrantSupportAccess: Grants FINBOURNE support access to your account
-*AuthenticationApi* | [**invalidate_support_access**](docs/AuthenticationApi.md#invalidate_support_access) | **DELETE** /api/authentication/support | [EARLY ACCESS] InvalidateSupportAccess: Revoke any FINBOURNE support access to your account
+*AuthenticationApi* | [**get_support_access_history**](docs/AuthenticationApi.md#get_support_access_history) | **GET** /api/authentication/support | GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination
+*AuthenticationApi* | [**get_support_roles**](docs/AuthenticationApi.md#get_support_roles) | **GET** /api/authentication/support-roles | GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation
+*AuthenticationApi* | [**grant_support_access**](docs/AuthenticationApi.md#grant_support_access) | **POST** /api/authentication/support | GrantSupportAccess: Grants FINBOURNE support access to your account
+*AuthenticationApi* | [**invalidate_support_access**](docs/AuthenticationApi.md#invalidate_support_access) | **DELETE** /api/authentication/support | InvalidateSupportAccess: Revoke any FINBOURNE support access to your account
 *AuthenticationApi* | [**update_password_policy**](docs/AuthenticationApi.md#update_password_policy) | **PUT** /api/authentication/password-policy/{userType} | [EXPERIMENTAL] UpdatePasswordPolicy: Updates password policy for a user type
-*IdentityProviderApi* | [**add_scim**](docs/IdentityProviderApi.md#add_scim) | **PUT** /api/identityprovider/scim | [EARLY ACCESS] AddScim: Add SCIM
-*IdentityProviderApi* | [**remove_scim**](docs/IdentityProviderApi.md#remove_scim) | **DELETE** /api/identityprovider/scim | [EARLY ACCESS] RemoveScim: Remove SCIM
-*MeApi* | [**get_user_info**](docs/MeApi.md#get_user_info) | **GET** /api/me | [EARLY ACCESS] GetUserInfo: Get User Info
+*IdentityProviderApi* | [**add_scim**](docs/IdentityProviderApi.md#add_scim) | **PUT** /api/identityprovider/scim | AddScim: Add SCIM
+*IdentityProviderApi* | [**remove_scim**](docs/IdentityProviderApi.md#remove_scim) | **DELETE** /api/identityprovider/scim | RemoveScim: Remove SCIM
+*MeApi* | [**get_user_info**](docs/MeApi.md#get_user_info) | **GET** /api/me | GetUserInfo: Get User Info
 *MeApi* | [**set_password**](docs/MeApi.md#set_password) | **PUT** /api/me/password | SetPassword: Set password of current user
-*PersonalAuthenticationTokensApi* | [**create_api_key**](docs/PersonalAuthenticationTokensApi.md#create_api_key) | **POST** /api/keys | [EARLY ACCESS] CreateApiKey: Create a Personal Access Token
-*PersonalAuthenticationTokensApi* | [**delete_api_key**](docs/PersonalAuthenticationTokensApi.md#delete_api_key) | **DELETE** /api/keys/{id} | [EARLY ACCESS] DeleteApiKey: Invalidate a Personal Access Token
-*PersonalAuthenticationTokensApi* | [**list_own_api_keys**](docs/PersonalAuthenticationTokensApi.md#list_own_api_keys) | **GET** /api/keys | [EARLY ACCESS] ListOwnApiKeys: Gets the meta data for all of the user&#39;s existing Personal Access Tokens.
-*RolesApi* | [**add_user_to_role**](docs/RolesApi.md#add_user_to_role) | **PUT** /api/roles/{id}/users/{userId} | [EARLY ACCESS] AddUserToRole: Add User to Role
-*RolesApi* | [**create_role**](docs/RolesApi.md#create_role) | **POST** /api/roles | [EARLY ACCESS] CreateRole: Create Role
-*RolesApi* | [**delete_role**](docs/RolesApi.md#delete_role) | **DELETE** /api/roles/{id} | [EARLY ACCESS] DeleteRole: Delete Role
-*RolesApi* | [**get_role**](docs/RolesApi.md#get_role) | **GET** /api/roles/{id} | [EARLY ACCESS] GetRole: Get Role
-*RolesApi* | [**list_roles**](docs/RolesApi.md#list_roles) | **GET** /api/roles | [EARLY ACCESS] ListRoles: List Roles
-*RolesApi* | [**list_users_in_role**](docs/RolesApi.md#list_users_in_role) | **GET** /api/roles/{id}/users | [EARLY ACCESS] ListUsersInRole: Get the users in the specified role.
-*RolesApi* | [**remove_user_from_role**](docs/RolesApi.md#remove_user_from_role) | **DELETE** /api/roles/{id}/users/{userId} | [EARLY ACCESS] RemoveUserFromRole: Remove User from Role
-*RolesApi* | [**update_role**](docs/RolesApi.md#update_role) | **PUT** /api/roles/{id} | [EARLY ACCESS] UpdateRole: Update Role
-*TokensApi* | [**invalidate_token**](docs/TokensApi.md#invalidate_token) | **DELETE** /api/tokens | [EARLY ACCESS] InvalidateToken: Invalidate current JWT token (sign out)
-*UsersApi* | [**create_user**](docs/UsersApi.md#create_user) | **POST** /api/users | [EARLY ACCESS] CreateUser: Create User
-*UsersApi* | [**delete_user**](docs/UsersApi.md#delete_user) | **DELETE** /api/users/{id} | [EARLY ACCESS] DeleteUser: Delete User
-*UsersApi* | [**expire_password**](docs/UsersApi.md#expire_password) | **POST** /api/users/{id}/lifecycle/$expirepassword | [EARLY ACCESS] ExpirePassword: Reset the user&#39;s password to a temporary one
-*UsersApi* | [**find_users_by_id**](docs/UsersApi.md#find_users_by_id) | **GET** /api/directory | [EARLY ACCESS] FindUsersById: Find users by id endpoint
-*UsersApi* | [**get_user**](docs/UsersApi.md#get_user) | **GET** /api/users/{id} | [EARLY ACCESS] GetUser: Get User
+*PersonalAuthenticationTokensApi* | [**create_api_key**](docs/PersonalAuthenticationTokensApi.md#create_api_key) | **POST** /api/keys | CreateApiKey: Create a Personal Access Token
+*PersonalAuthenticationTokensApi* | [**delete_api_key**](docs/PersonalAuthenticationTokensApi.md#delete_api_key) | **DELETE** /api/keys/{id} | DeleteApiKey: Invalidate a Personal Access Token
+*PersonalAuthenticationTokensApi* | [**list_own_api_keys**](docs/PersonalAuthenticationTokensApi.md#list_own_api_keys) | **GET** /api/keys | ListOwnApiKeys: Gets the meta data for all of the user&#39;s existing Personal Access Tokens.
+*RolesApi* | [**add_user_to_role**](docs/RolesApi.md#add_user_to_role) | **PUT** /api/roles/{id}/users/{userId} | AddUserToRole: Add User to Role
+*RolesApi* | [**create_role**](docs/RolesApi.md#create_role) | **POST** /api/roles | CreateRole: Create Role
+*RolesApi* | [**delete_role**](docs/RolesApi.md#delete_role) | **DELETE** /api/roles/{id} | DeleteRole: Delete Role
+*RolesApi* | [**get_role**](docs/RolesApi.md#get_role) | **GET** /api/roles/{id} | GetRole: Get Role
+*RolesApi* | [**list_roles**](docs/RolesApi.md#list_roles) | **GET** /api/roles | ListRoles: List Roles
+*RolesApi* | [**list_users_in_role**](docs/RolesApi.md#list_users_in_role) | **GET** /api/roles/{id}/users | ListUsersInRole: Get the users in the specified role.
+*RolesApi* | [**remove_user_from_role**](docs/RolesApi.md#remove_user_from_role) | **DELETE** /api/roles/{id}/users/{userId} | RemoveUserFromRole: Remove User from Role
+*RolesApi* | [**update_role**](docs/RolesApi.md#update_role) | **PUT** /api/roles/{id} | UpdateRole: Update Role
+*TokensApi* | [**invalidate_token**](docs/TokensApi.md#invalidate_token) | **DELETE** /api/tokens | InvalidateToken: Invalidate current JWT token (sign out)
+*UsersApi* | [**create_user**](docs/UsersApi.md#create_user) | **POST** /api/users | CreateUser: Create User
+*UsersApi* | [**delete_user**](docs/UsersApi.md#delete_user) | **DELETE** /api/users/{id} | DeleteUser: Delete User
+*UsersApi* | [**expire_password**](docs/UsersApi.md#expire_password) | **POST** /api/users/{id}/lifecycle/$expirepassword | ExpirePassword: Reset the user&#39;s password to a temporary one
+*UsersApi* | [**find_users_by_id**](docs/UsersApi.md#find_users_by_id) | **GET** /api/directory | FindUsersById: Find users by id endpoint
+*UsersApi* | [**get_user**](docs/UsersApi.md#get_user) | **GET** /api/users/{id} | GetUser: Get User
 *UsersApi* | [**list_runnable_users**](docs/UsersApi.md#list_runnable_users) | **GET** /api/users/$runnable | [EARLY ACCESS] ListRunnableUsers: List Runable Users
-*UsersApi* | [**list_users**](docs/UsersApi.md#list_users) | **GET** /api/users | [EARLY ACCESS] ListUsers: List Users
-*UsersApi* | [**reset_factors**](docs/UsersApi.md#reset_factors) | **POST** /api/users/{id}/lifecycle/$resetfactors | [EARLY ACCESS] ResetFactors: Reset MFA factors
-*UsersApi* | [**reset_password**](docs/UsersApi.md#reset_password) | **POST** /api/users/{id}/lifecycle/$resetpassword | [EARLY ACCESS] ResetPassword: Reset Password
-*UsersApi* | [**send_activation_email**](docs/UsersApi.md#send_activation_email) | **POST** /api/users/{id}/lifecycle/$activate | [EARLY ACCESS] SendActivationEmail: Sends an activation email to the User
-*UsersApi* | [**unlock_user**](docs/UsersApi.md#unlock_user) | **POST** /api/users/{id}/lifecycle/$unlock | [EARLY ACCESS] UnlockUser: Unlock User
+*UsersApi* | [**list_users**](docs/UsersApi.md#list_users) | **GET** /api/users | ListUsers: List Users
+*UsersApi* | [**reset_factors**](docs/UsersApi.md#reset_factors) | **POST** /api/users/{id}/lifecycle/$resetfactors | ResetFactors: Reset MFA factors
+*UsersApi* | [**reset_password**](docs/UsersApi.md#reset_password) | **POST** /api/users/{id}/lifecycle/$resetpassword | ResetPassword: Reset Password
+*UsersApi* | [**send_activation_email**](docs/UsersApi.md#send_activation_email) | **POST** /api/users/{id}/lifecycle/$activate | SendActivationEmail: Sends an activation email to the User
+*UsersApi* | [**unlock_user**](docs/UsersApi.md#unlock_user) | **POST** /api/users/{id}/lifecycle/$unlock | UnlockUser: Unlock User
 *UsersApi* | [**unsuspend_user**](docs/UsersApi.md#unsuspend_user) | **POST** /api/users/{id}/lifecycle/$unsuspend | [EXPERIMENTAL] UnsuspendUser: Unsuspend user
-*UsersApi* | [**update_user**](docs/UsersApi.md#update_user) | **PUT** /api/users/{id} | [EARLY ACCESS] UpdateUser: Update User
+*UsersApi* | [**update_user**](docs/UsersApi.md#update_user) | **PUT** /api/users/{id} | UpdateUser: Update User
 
 
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
@@ -297,7 +323,8 @@
 
 
 ## Author
 
 info@finbourne.com
 
 
+
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/__init__.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/__init__.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/application_metadata_api.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     @overload
     def list_access_controlled_resources(self, async_req: Optional[bool]=True, **kwargs) -> ResourceListOfAccessControlledResource:  # noqa: E501
         ...
 
     @validate_arguments
     def list_access_controlled_resources(self, async_req: Optional[bool]=None, **kwargs) -> Union[ResourceListOfAccessControlledResource, Awaitable[ResourceListOfAccessControlledResource]]:  # noqa: E501
-        """[EARLY ACCESS] ListAccessControlledResources: Get resources available for access control  # noqa: E501
+        """ListAccessControlledResources: Get resources available for access control  # noqa: E501
 
         Get the comprehensive set of resources that are available for access control  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_access_controlled_resources(async_req=True)
         >>> result = thread.get()
@@ -77,15 +77,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_access_controlled_resources_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def list_access_controlled_resources_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListAccessControlledResources: Get resources available for access control  # noqa: E501
+        """ListAccessControlledResources: Get resources available for access control  # noqa: E501
 
         Get the comprehensive set of resources that are available for access control  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_access_controlled_resources_with_http_info(async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/applications_api.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/applications_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/authentication_api.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
 
     @overload
     def get_support_access_history(self, start : Annotated[Optional[datetime], Field(description="The start expiry date to query support access requests from")] = None, end : Annotated[Optional[datetime], Field(description="The end expiry date to query support access requests to")] = None, async_req: Optional[bool]=True, **kwargs) -> List[SupportAccessResponse]:  # noqa: E501
         ...
 
     @validate_arguments
     def get_support_access_history(self, start : Annotated[Optional[datetime], Field(description="The start expiry date to query support access requests from")] = None, end : Annotated[Optional[datetime], Field(description="The end expiry date to query support access requests to")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[List[SupportAccessResponse], Awaitable[List[SupportAccessResponse]]]:  # noqa: E501
-        """[EARLY ACCESS] GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination  # noqa: E501
+        """GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination  # noqa: E501
 
         The active and inactive support requests will be returned, inactive support requests will have information pertaining to their termination  including obfuscated userIds of those who created and terminated the request  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_support_access_history(start, end, async_req=True)
         >>> result = thread.get()
@@ -386,15 +386,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_support_access_history_with_http_info(start, end, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_support_access_history_with_http_info(self, start : Annotated[Optional[datetime], Field(description="The start expiry date to query support access requests from")] = None, end : Annotated[Optional[datetime], Field(description="The end expiry date to query support access requests to")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination  # noqa: E501
+        """GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination  # noqa: E501
 
         The active and inactive support requests will be returned, inactive support requests will have information pertaining to their termination  including obfuscated userIds of those who created and terminated the request  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_support_access_history_with_http_info(start, end, async_req=True)
         >>> result = thread.get()
@@ -517,15 +517,15 @@
 
     @overload
     def get_support_roles(self, async_req: Optional[bool]=True, **kwargs) -> SupportRolesResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def get_support_roles(self, async_req: Optional[bool]=None, **kwargs) -> Union[SupportRolesResponse, Awaitable[SupportRolesResponse]]:  # noqa: E501
-        """[EARLY ACCESS] GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
+        """GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
 
         Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_support_roles(async_req=True)
         >>> result = thread.get()
@@ -547,15 +547,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_support_roles_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def get_support_roles_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
+        """GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
 
         Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_support_roles_with_http_info(async_req=True)
         >>> result = thread.get()
@@ -659,15 +659,15 @@
 
     @overload
     def grant_support_access(self, support_access_request : Annotated[SupportAccessRequest, Field(..., description="Request detailing the duration and reasons for supplying support access")], async_req: Optional[bool]=True, **kwargs) -> SupportAccessResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def grant_support_access(self, support_access_request : Annotated[SupportAccessRequest, Field(..., description="Request detailing the duration and reasons for supplying support access")], async_req: Optional[bool]=None, **kwargs) -> Union[SupportAccessResponse, Awaitable[SupportAccessResponse]]:  # noqa: E501
-        """[EARLY ACCESS] GrantSupportAccess: Grants FINBOURNE support access to your account  # noqa: E501
+        """GrantSupportAccess: Grants FINBOURNE support access to your account  # noqa: E501
 
         Granting support access will allow FINBOURNE employees full access to your data with the express intent to investigate support issues  You can revoke this (and all) access at any time using the InvalidateSupportAccess endpoint.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.grant_support_access(support_access_request, async_req=True)
         >>> result = thread.get()
@@ -691,15 +691,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.grant_support_access_with_http_info(support_access_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def grant_support_access_with_http_info(self, support_access_request : Annotated[SupportAccessRequest, Field(..., description="Request detailing the duration and reasons for supplying support access")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GrantSupportAccess: Grants FINBOURNE support access to your account  # noqa: E501
+        """GrantSupportAccess: Grants FINBOURNE support access to your account  # noqa: E501
 
         Granting support access will allow FINBOURNE employees full access to your data with the express intent to investigate support issues  You can revoke this (and all) access at any time using the InvalidateSupportAccess endpoint.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.grant_support_access_with_http_info(support_access_request, async_req=True)
         >>> result = thread.get()
@@ -817,15 +817,15 @@
 
     @overload
     def invalidate_support_access(self, async_req: Optional[bool]=True, **kwargs) -> List[SupportAccessResponse]:  # noqa: E501
         ...
 
     @validate_arguments
     def invalidate_support_access(self, async_req: Optional[bool]=None, **kwargs) -> Union[List[SupportAccessResponse], Awaitable[List[SupportAccessResponse]]]:  # noqa: E501
-        """[EARLY ACCESS] InvalidateSupportAccess: Revoke any FINBOURNE support access to your account  # noqa: E501
+        """InvalidateSupportAccess: Revoke any FINBOURNE support access to your account  # noqa: E501
 
         This will result in a loss of access to your data for all FINBOURNE support agents  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.invalidate_support_access(async_req=True)
         >>> result = thread.get()
@@ -847,15 +847,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.invalidate_support_access_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def invalidate_support_access_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] InvalidateSupportAccess: Revoke any FINBOURNE support access to your account  # noqa: E501
+        """InvalidateSupportAccess: Revoke any FINBOURNE support access to your account  # noqa: E501
 
         This will result in a loss of access to your data for all FINBOURNE support agents  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.invalidate_support_access_with_http_info(async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/identity_provider_api.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/identity_provider_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     @overload
     def add_scim(self, api_token_action : Annotated[Optional[StrictStr], Field(description="The action to take. For the API token. Defaults to \"ensure\"")] = None, old_api_token_deactivation : Annotated[Optional[datetime], Field(description="Optional deactivation date for the old API token. Only used if apiTokenAction is \"regenerate\"")] = None, async_req: Optional[bool]=True, **kwargs) -> AddScimResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def add_scim(self, api_token_action : Annotated[Optional[StrictStr], Field(description="The action to take. For the API token. Defaults to \"ensure\"")] = None, old_api_token_deactivation : Annotated[Optional[datetime], Field(description="Optional deactivation date for the old API token. Only used if apiTokenAction is \"regenerate\"")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[AddScimResponse, Awaitable[AddScimResponse]]:  # noqa: E501
-        """[EARLY ACCESS] AddScim: Add SCIM  # noqa: E501
+        """AddScim: Add SCIM  # noqa: E501
 
         Generates an API token to be used for SCIM  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_scim(api_token_action, old_api_token_deactivation, async_req=True)
         >>> result = thread.get()
@@ -88,15 +88,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.add_scim_with_http_info(api_token_action, old_api_token_deactivation, **kwargs)  # noqa: E501
 
     @validate_arguments
     def add_scim_with_http_info(self, api_token_action : Annotated[Optional[StrictStr], Field(description="The action to take. For the API token. Defaults to \"ensure\"")] = None, old_api_token_deactivation : Annotated[Optional[datetime], Field(description="Optional deactivation date for the old API token. Only used if apiTokenAction is \"regenerate\"")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] AddScim: Add SCIM  # noqa: E501
+        """AddScim: Add SCIM  # noqa: E501
 
         Generates an API token to be used for SCIM  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_scim_with_http_info(api_token_action, old_api_token_deactivation, async_req=True)
         >>> result = thread.get()
@@ -216,15 +216,15 @@
 
     @overload
     def remove_scim(self, async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def remove_scim(self, async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] RemoveScim: Remove SCIM  # noqa: E501
+        """RemoveScim: Remove SCIM  # noqa: E501
 
         Deactivates any existing SCIM API token  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_scim(async_req=True)
         >>> result = thread.get()
@@ -246,15 +246,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.remove_scim_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def remove_scim_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] RemoveScim: Remove SCIM  # noqa: E501
+        """RemoveScim: Remove SCIM  # noqa: E501
 
         Deactivates any existing SCIM API token  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_scim_with_http_info(async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/me_api.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/me_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     @overload
     def get_user_info(self, async_req: Optional[bool]=True, **kwargs) -> CurrentUserResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def get_user_info(self, async_req: Optional[bool]=None, **kwargs) -> Union[CurrentUserResponse, Awaitable[CurrentUserResponse]]:  # noqa: E501
-        """[EARLY ACCESS] GetUserInfo: Get User Info  # noqa: E501
+        """GetUserInfo: Get User Info  # noqa: E501
 
         Get the requesting user's basic info  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_user_info(async_req=True)
         >>> result = thread.get()
@@ -82,15 +82,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_user_info_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def get_user_info_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetUserInfo: Get User Info  # noqa: E501
+        """GetUserInfo: Get User Info  # noqa: E501
 
         Get the requesting user's basic info  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_user_info_with_http_info(async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/personal_authentication_tokens_api.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/personal_authentication_tokens_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     @overload
     def create_api_key(self, create_api_key : Annotated[CreateApiKey, Field(..., description="The request to create a new Personal Access Token")], async_req: Optional[bool]=True, **kwargs) -> CreatedApiKey:  # noqa: E501
         ...
 
     @validate_arguments
     def create_api_key(self, create_api_key : Annotated[CreateApiKey, Field(..., description="The request to create a new Personal Access Token")], async_req: Optional[bool]=None, **kwargs) -> Union[CreatedApiKey, Awaitable[CreatedApiKey]]:  # noqa: E501
-        """[EARLY ACCESS] CreateApiKey: Create a Personal Access Token  # noqa: E501
+        """CreateApiKey: Create a Personal Access Token  # noqa: E501
 
         Generates a Personal Access Token and returns the new key and its associated metadata.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_api_key(create_api_key, async_req=True)
         >>> result = thread.get()
@@ -86,15 +86,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.create_api_key_with_http_info(create_api_key, **kwargs)  # noqa: E501
 
     @validate_arguments
     def create_api_key_with_http_info(self, create_api_key : Annotated[CreateApiKey, Field(..., description="The request to create a new Personal Access Token")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] CreateApiKey: Create a Personal Access Token  # noqa: E501
+        """CreateApiKey: Create a Personal Access Token  # noqa: E501
 
         Generates a Personal Access Token and returns the new key and its associated metadata.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_api_key_with_http_info(create_api_key, async_req=True)
         >>> result = thread.get()
@@ -212,15 +212,15 @@
 
     @overload
     def delete_api_key(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The id of the Personal Access Token to delete")], async_req: Optional[bool]=True, **kwargs) -> ApiKey:  # noqa: E501
         ...
 
     @validate_arguments
     def delete_api_key(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The id of the Personal Access Token to delete")], async_req: Optional[bool]=None, **kwargs) -> Union[ApiKey, Awaitable[ApiKey]]:  # noqa: E501
-        """[EARLY ACCESS] DeleteApiKey: Invalidate a Personal Access Token  # noqa: E501
+        """DeleteApiKey: Invalidate a Personal Access Token  # noqa: E501
 
         Immediately invalidates the specified Personal Access Token  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_api_key(id, async_req=True)
         >>> result = thread.get()
@@ -244,15 +244,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.delete_api_key_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_api_key_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The id of the Personal Access Token to delete")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] DeleteApiKey: Invalidate a Personal Access Token  # noqa: E501
+        """DeleteApiKey: Invalidate a Personal Access Token  # noqa: E501
 
         Immediately invalidates the specified Personal Access Token  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_api_key_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -363,15 +363,15 @@
 
     @overload
     def list_own_api_keys(self, async_req: Optional[bool]=True, **kwargs) -> List[ApiKey]:  # noqa: E501
         ...
 
     @validate_arguments
     def list_own_api_keys(self, async_req: Optional[bool]=None, **kwargs) -> Union[List[ApiKey], Awaitable[List[ApiKey]]]:  # noqa: E501
-        """[EARLY ACCESS] ListOwnApiKeys: Gets the meta data for all of the user's existing Personal Access Tokens.  # noqa: E501
+        """ListOwnApiKeys: Gets the meta data for all of the user's existing Personal Access Tokens.  # noqa: E501
 
         Gets the meta data for all of the user's Personal Access Tokens that have not been deleted. They may be  invalid due to the deactivation date having passed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_own_api_keys(async_req=True)
         >>> result = thread.get()
@@ -393,15 +393,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_own_api_keys_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def list_own_api_keys_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListOwnApiKeys: Gets the meta data for all of the user's existing Personal Access Tokens.  # noqa: E501
+        """ListOwnApiKeys: Gets the meta data for all of the user's existing Personal Access Tokens.  # noqa: E501
 
         Gets the meta data for all of the user's Personal Access Tokens that have not been deleted. They may be  invalid due to the deactivation date having passed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_own_api_keys_with_http_info(async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/roles_api.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/roles_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     @overload
     def add_user_to_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the Role")], user_id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def add_user_to_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the Role")], user_id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] AddUserToRole: Add User to Role  # noqa: E501
+        """AddUserToRole: Add User to Role  # noqa: E501
 
         Adds the User to the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_user_to_role(id, user_id, async_req=True)
         >>> result = thread.get()
@@ -89,15 +89,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.add_user_to_role_with_http_info(id, user_id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def add_user_to_role_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the Role")], user_id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] AddUserToRole: Add User to Role  # noqa: E501
+        """AddUserToRole: Add User to Role  # noqa: E501
 
         Adds the User to the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_user_to_role_with_http_info(id, user_id, async_req=True)
         >>> result = thread.get()
@@ -211,15 +211,15 @@
 
     @overload
     def create_role(self, create_role_request : Annotated[CreateRoleRequest, Field(..., description="Details of the role to be created")], async_req: Optional[bool]=True, **kwargs) -> RoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def create_role(self, create_role_request : Annotated[CreateRoleRequest, Field(..., description="Details of the role to be created")], async_req: Optional[bool]=None, **kwargs) -> Union[RoleResponse, Awaitable[RoleResponse]]:  # noqa: E501
-        """[EARLY ACCESS] CreateRole: Create Role  # noqa: E501
+        """CreateRole: Create Role  # noqa: E501
 
         Creates a new Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_role(create_role_request, async_req=True)
         >>> result = thread.get()
@@ -243,15 +243,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.create_role_with_http_info(create_role_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def create_role_with_http_info(self, create_role_request : Annotated[CreateRoleRequest, Field(..., description="Details of the role to be created")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] CreateRole: Create Role  # noqa: E501
+        """CreateRole: Create Role  # noqa: E501
 
         Creates a new Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_role_with_http_info(create_role_request, async_req=True)
         >>> result = thread.get()
@@ -370,15 +370,15 @@
 
     @overload
     def delete_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the role")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def delete_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the role")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] DeleteRole: Delete Role  # noqa: E501
+        """DeleteRole: Delete Role  # noqa: E501
 
         Delete the specified role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_role(id, async_req=True)
         >>> result = thread.get()
@@ -402,15 +402,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.delete_role_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_role_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the role")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] DeleteRole: Delete Role  # noqa: E501
+        """DeleteRole: Delete Role  # noqa: E501
 
         Delete the specified role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_role_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -518,15 +518,15 @@
 
     @overload
     def get_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the role")], async_req: Optional[bool]=True, **kwargs) -> RoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def get_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the role")], async_req: Optional[bool]=None, **kwargs) -> Union[RoleResponse, Awaitable[RoleResponse]]:  # noqa: E501
-        """[EARLY ACCESS] GetRole: Get Role  # noqa: E501
+        """GetRole: Get Role  # noqa: E501
 
         Get the specified role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_role(id, async_req=True)
         >>> result = thread.get()
@@ -550,15 +550,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_role_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_role_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the role")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetRole: Get Role  # noqa: E501
+        """GetRole: Get Role  # noqa: E501
 
         Get the specified role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_role_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -670,15 +670,15 @@
 
     @overload
     def list_roles(self, async_req: Optional[bool]=True, **kwargs) -> List[RoleResponse]:  # noqa: E501
         ...
 
     @validate_arguments
     def list_roles(self, async_req: Optional[bool]=None, **kwargs) -> Union[List[RoleResponse], Awaitable[List[RoleResponse]]]:  # noqa: E501
-        """[EARLY ACCESS] ListRoles: List Roles  # noqa: E501
+        """ListRoles: List Roles  # noqa: E501
 
         List the available Roles  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_roles(async_req=True)
         >>> result = thread.get()
@@ -700,15 +700,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_roles_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def list_roles_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListRoles: List Roles  # noqa: E501
+        """ListRoles: List Roles  # noqa: E501
 
         List the available Roles  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_roles_with_http_info(async_req=True)
         >>> result = thread.get()
@@ -812,15 +812,15 @@
 
     @overload
     def list_users_in_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the Role")], async_req: Optional[bool]=True, **kwargs) -> List[UserResponse]:  # noqa: E501
         ...
 
     @validate_arguments
     def list_users_in_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the Role")], async_req: Optional[bool]=None, **kwargs) -> Union[List[UserResponse], Awaitable[List[UserResponse]]]:  # noqa: E501
-        """[EARLY ACCESS] ListUsersInRole: Get the users in the specified role.  # noqa: E501
+        """ListUsersInRole: Get the users in the specified role.  # noqa: E501
 
         List all Users in the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_users_in_role(id, async_req=True)
         >>> result = thread.get()
@@ -844,15 +844,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_users_in_role_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def list_users_in_role_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the Role")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListUsersInRole: Get the users in the specified role.  # noqa: E501
+        """ListUsersInRole: Get the users in the specified role.  # noqa: E501
 
         List all Users in the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_users_in_role_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -963,15 +963,15 @@
 
     @overload
     def remove_user_from_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the Role")], user_id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def remove_user_from_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the Role")], user_id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] RemoveUserFromRole: Remove User from Role  # noqa: E501
+        """RemoveUserFromRole: Remove User from Role  # noqa: E501
 
         Removes the User from the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_user_from_role(id, user_id, async_req=True)
         >>> result = thread.get()
@@ -997,15 +997,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.remove_user_from_role_with_http_info(id, user_id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def remove_user_from_role_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the Role")], user_id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] RemoveUserFromRole: Remove User from Role  # noqa: E501
+        """RemoveUserFromRole: Remove User from Role  # noqa: E501
 
         Removes the User from the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_user_from_role_with_http_info(id, user_id, async_req=True)
         >>> result = thread.get()
@@ -1119,15 +1119,15 @@
 
     @overload
     def update_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the role to be updated")], update_role_request : Annotated[Optional[UpdateRoleRequest], Field(description="The new definition of the role")] = None, async_req: Optional[bool]=True, **kwargs) -> RoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def update_role(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the role to be updated")], update_role_request : Annotated[Optional[UpdateRoleRequest], Field(description="The new definition of the role")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[RoleResponse, Awaitable[RoleResponse]]:  # noqa: E501
-        """[EARLY ACCESS] UpdateRole: Update Role  # noqa: E501
+        """UpdateRole: Update Role  # noqa: E501
 
         Update the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_role(id, update_role_request, async_req=True)
         >>> result = thread.get()
@@ -1153,15 +1153,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.update_role_with_http_info(id, update_role_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def update_role_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the role to be updated")], update_role_request : Annotated[Optional[UpdateRoleRequest], Field(description="The new definition of the role")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] UpdateRole: Update Role  # noqa: E501
+        """UpdateRole: Update Role  # noqa: E501
 
         Update the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_role_with_http_info(id, update_role_request, async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/tokens_api.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/tokens_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     @overload
     def invalidate_token(self, async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def invalidate_token(self, async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] InvalidateToken: Invalidate current JWT token (sign out)  # noqa: E501
+        """InvalidateToken: Invalidate current JWT token (sign out)  # noqa: E501
 
         Log the current user out of all Finbourne platforms by invalidating the current token  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.invalidate_token(async_req=True)
         >>> result = thread.get()
@@ -76,15 +76,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.invalidate_token_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def invalidate_token_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] InvalidateToken: Invalidate current JWT token (sign out)  # noqa: E501
+        """InvalidateToken: Invalidate current JWT token (sign out)  # noqa: E501
 
         Log the current user out of all Finbourne platforms by invalidating the current token  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.invalidate_token_with_http_info(async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api/users_api.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api/users_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     @overload
     def create_user(self, create_user_request : Annotated[CreateUserRequest, Field(..., description="Details of the User to be created")], wait_for_reindex : Annotated[Optional[StrictBool], Field(description="Should the request wait until the newly created User is indexed (available in List) before returning")] = None, async_req: Optional[bool]=True, **kwargs) -> UserResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def create_user(self, create_user_request : Annotated[CreateUserRequest, Field(..., description="Details of the User to be created")], wait_for_reindex : Annotated[Optional[StrictBool], Field(description="Should the request wait until the newly created User is indexed (available in List) before returning")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[UserResponse, Awaitable[UserResponse]]:  # noqa: E501
-        """[EARLY ACCESS] CreateUser: Create User  # noqa: E501
+        """CreateUser: Create User  # noqa: E501
 
         Create a new User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_user(create_user_request, wait_for_reindex, async_req=True)
         >>> result = thread.get()
@@ -90,15 +90,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.create_user_with_http_info(create_user_request, wait_for_reindex, **kwargs)  # noqa: E501
 
     @validate_arguments
     def create_user_with_http_info(self, create_user_request : Annotated[CreateUserRequest, Field(..., description="Details of the User to be created")], wait_for_reindex : Annotated[Optional[StrictBool], Field(description="Should the request wait until the newly created User is indexed (available in List) before returning")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] CreateUser: Create User  # noqa: E501
+        """CreateUser: Create User  # noqa: E501
 
         Create a new User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_user_with_http_info(create_user_request, wait_for_reindex, async_req=True)
         >>> result = thread.get()
@@ -222,15 +222,15 @@
 
     @overload
     def delete_user(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the user")], purge : Annotated[Optional[StrictBool], Field(description="Whether to purge any trace of the user from the identity provider (will affect audit)")] = None, async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def delete_user(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the user")], purge : Annotated[Optional[StrictBool], Field(description="Whether to purge any trace of the user from the identity provider (will affect audit)")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] DeleteUser: Delete User  # noqa: E501
+        """DeleteUser: Delete User  # noqa: E501
 
         By default the user will be de-provisioned and inactive, however their record will remain in the identity  provider for audit purposes. If this is not desirable and removal of all trace of the user is required,  the purge parameter can be specified to indicate the details should be purged completely.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_user(id, purge, async_req=True)
         >>> result = thread.get()
@@ -256,15 +256,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.delete_user_with_http_info(id, purge, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_user_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the user")], purge : Annotated[Optional[StrictBool], Field(description="Whether to purge any trace of the user from the identity provider (will affect audit)")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] DeleteUser: Delete User  # noqa: E501
+        """DeleteUser: Delete User  # noqa: E501
 
         By default the user will be de-provisioned and inactive, however their record will remain in the identity  provider for audit purposes. If this is not desirable and removal of all trace of the user is required,  the purge parameter can be specified to indicate the details should be purged completely.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_user_with_http_info(id, purge, async_req=True)
         >>> result = thread.get()
@@ -378,15 +378,15 @@
 
     @overload
     def expire_password(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User having its password reset")], async_req: Optional[bool]=True, **kwargs) -> TemporaryPassword:  # noqa: E501
         ...
 
     @validate_arguments
     def expire_password(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User having its password reset")], async_req: Optional[bool]=None, **kwargs) -> Union[TemporaryPassword, Awaitable[TemporaryPassword]]:  # noqa: E501
-        """[EARLY ACCESS] ExpirePassword: Reset the user's password to a temporary one  # noqa: E501
+        """ExpirePassword: Reset the user's password to a temporary one  # noqa: E501
 
         Resets the user's password to a temporary one which is then expired  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.expire_password(id, async_req=True)
         >>> result = thread.get()
@@ -410,15 +410,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.expire_password_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def expire_password_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User having its password reset")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ExpirePassword: Reset the user's password to a temporary one  # noqa: E501
+        """ExpirePassword: Reset the user's password to a temporary one  # noqa: E501
 
         Resets the user's password to a temporary one which is then expired  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.expire_password_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -529,15 +529,15 @@
 
     @overload
     def find_users_by_id(self, id : Annotated[conlist(StrictStr), Field(..., description="A list of unique identifiers for the users")], async_req: Optional[bool]=True, **kwargs) -> ListUsersResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def find_users_by_id(self, id : Annotated[conlist(StrictStr), Field(..., description="A list of unique identifiers for the users")], async_req: Optional[bool]=None, **kwargs) -> Union[ListUsersResponse, Awaitable[ListUsersResponse]]:  # noqa: E501
-        """[EARLY ACCESS] FindUsersById: Find users by id endpoint  # noqa: E501
+        """FindUsersById: Find users by id endpoint  # noqa: E501
 
         Finds a maximum of 50 users by ID  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.find_users_by_id(id, async_req=True)
         >>> result = thread.get()
@@ -561,15 +561,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.find_users_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def find_users_by_id_with_http_info(self, id : Annotated[conlist(StrictStr), Field(..., description="A list of unique identifiers for the users")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] FindUsersById: Find users by id endpoint  # noqa: E501
+        """FindUsersById: Find users by id endpoint  # noqa: E501
 
         Finds a maximum of 50 users by ID  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.find_users_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -681,15 +681,15 @@
 
     @overload
     def get_user(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User")], include_roles : Annotated[Optional[StrictBool], Field(description="Flag indicating that the users roles should be included in the response")] = None, async_req: Optional[bool]=True, **kwargs) -> UserResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def get_user(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User")], include_roles : Annotated[Optional[StrictBool], Field(description="Flag indicating that the users roles should be included in the response")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[UserResponse, Awaitable[UserResponse]]:  # noqa: E501
-        """[EARLY ACCESS] GetUser: Get User  # noqa: E501
+        """GetUser: Get User  # noqa: E501
 
         Get the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_user(id, include_roles, async_req=True)
         >>> result = thread.get()
@@ -715,15 +715,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_user_with_http_info(id, include_roles, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_user_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User")], include_roles : Annotated[Optional[StrictBool], Field(description="Flag indicating that the users roles should be included in the response")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetUser: Get User  # noqa: E501
+        """GetUser: Get User  # noqa: E501
 
         Get the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_user_with_http_info(id, include_roles, async_req=True)
         >>> result = thread.get()
@@ -982,15 +982,15 @@
 
     @overload
     def list_users(self, include_roles : Annotated[Optional[StrictBool], Field(description="Flag indicating that the users roles should be included in the response")] = None, include_deactivated : Annotated[Optional[StrictBool], Field(description="Include previously deleted (not purged) users")] = None, async_req: Optional[bool]=True, **kwargs) -> List[UserResponse]:  # noqa: E501
         ...
 
     @validate_arguments
     def list_users(self, include_roles : Annotated[Optional[StrictBool], Field(description="Flag indicating that the users roles should be included in the response")] = None, include_deactivated : Annotated[Optional[StrictBool], Field(description="Include previously deleted (not purged) users")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[List[UserResponse], Awaitable[List[UserResponse]]]:  # noqa: E501
-        """[EARLY ACCESS] ListUsers: List Users  # noqa: E501
+        """ListUsers: List Users  # noqa: E501
 
         List the available Users  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_users(include_roles, include_deactivated, async_req=True)
         >>> result = thread.get()
@@ -1016,15 +1016,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_users_with_http_info(include_roles, include_deactivated, **kwargs)  # noqa: E501
 
     @validate_arguments
     def list_users_with_http_info(self, include_roles : Annotated[Optional[StrictBool], Field(description="Flag indicating that the users roles should be included in the response")] = None, include_deactivated : Annotated[Optional[StrictBool], Field(description="Include previously deleted (not purged) users")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListUsers: List Users  # noqa: E501
+        """ListUsers: List Users  # noqa: E501
 
         List the available Users  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_users_with_http_info(include_roles, include_deactivated, async_req=True)
         >>> result = thread.get()
@@ -1141,15 +1141,15 @@
 
     @overload
     def reset_factors(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User having their MFA factors reset")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def reset_factors(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User having their MFA factors reset")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] ResetFactors: Reset MFA factors  # noqa: E501
+        """ResetFactors: Reset MFA factors  # noqa: E501
 
         Resets the MFA factors of the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.reset_factors(id, async_req=True)
         >>> result = thread.get()
@@ -1173,15 +1173,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.reset_factors_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def reset_factors_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User having their MFA factors reset")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ResetFactors: Reset MFA factors  # noqa: E501
+        """ResetFactors: Reset MFA factors  # noqa: E501
 
         Resets the MFA factors of the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.reset_factors_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -1289,15 +1289,15 @@
 
     @overload
     def reset_password(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User having their password reset")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def reset_password(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User having their password reset")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] ResetPassword: Reset Password  # noqa: E501
+        """ResetPassword: Reset Password  # noqa: E501
 
         Resets the password of the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.reset_password(id, async_req=True)
         >>> result = thread.get()
@@ -1321,15 +1321,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.reset_password_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def reset_password_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User having their password reset")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ResetPassword: Reset Password  # noqa: E501
+        """ResetPassword: Reset Password  # noqa: E501
 
         Resets the password of the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.reset_password_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -1437,15 +1437,15 @@
 
     @overload
     def send_activation_email(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User to be activated")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def send_activation_email(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User to be activated")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] SendActivationEmail: Sends an activation email to the User  # noqa: E501
+        """SendActivationEmail: Sends an activation email to the User  # noqa: E501
 
         Sends an activation email to the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.send_activation_email(id, async_req=True)
         >>> result = thread.get()
@@ -1469,15 +1469,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.send_activation_email_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def send_activation_email_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User to be activated")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] SendActivationEmail: Sends an activation email to the User  # noqa: E501
+        """SendActivationEmail: Sends an activation email to the User  # noqa: E501
 
         Sends an activation email to the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.send_activation_email_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -1585,15 +1585,15 @@
 
     @overload
     def unlock_user(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User to be unlocked")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def unlock_user(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User to be unlocked")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] UnlockUser: Unlock User  # noqa: E501
+        """UnlockUser: Unlock User  # noqa: E501
 
         Unlocks the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.unlock_user(id, async_req=True)
         >>> result = thread.get()
@@ -1617,15 +1617,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.unlock_user_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def unlock_user_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User to be unlocked")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] UnlockUser: Unlock User  # noqa: E501
+        """UnlockUser: Unlock User  # noqa: E501
 
         Unlocks the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.unlock_user_with_http_info(id, async_req=True)
         >>> result = thread.get()
@@ -1881,15 +1881,15 @@
 
     @overload
     def update_user(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User to be updated")], update_user_request : Annotated[UpdateUserRequest, Field(..., description="The new definition of the User")], async_req: Optional[bool]=True, **kwargs) -> UserResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def update_user(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User to be updated")], update_user_request : Annotated[UpdateUserRequest, Field(..., description="The new definition of the User")], async_req: Optional[bool]=None, **kwargs) -> Union[UserResponse, Awaitable[UserResponse]]:  # noqa: E501
-        """[EARLY ACCESS] UpdateUser: Update User  # noqa: E501
+        """UpdateUser: Update User  # noqa: E501
 
         Updates the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_user(id, update_user_request, async_req=True)
         >>> result = thread.get()
@@ -1915,15 +1915,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.update_user_with_http_info(id, update_user_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def update_user_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the User to be updated")], update_user_request : Annotated[UpdateUserRequest, Field(..., description="The new definition of the User")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] UpdateUser: Update User  # noqa: E501
+        """UpdateUser: Update User  # noqa: E501
 
         Updates the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_user_with_http_info(id, update_user_request, async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api_client.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/api_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/configuration.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_identity-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.2862\n"\
+               "Version of the API: 0.0.2866\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/exceptions.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/__init__.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/api_client.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/api_client_factory.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/api_configuration.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/configuration_loaders.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/proxy_config.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/refreshing_token.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/rest.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/retry.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/socket_keep_alive.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/extensions/tcp_keep_alive_connector.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/__init__.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/access_controlled_action.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/access_controlled_resource.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/action_id.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/action_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/add_scim_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/add_scim_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/api_key.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/api_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/authentication_information.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/authentication_information.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/create_api_key.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/create_api_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/create_application_request.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/create_application_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/create_role_request.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/create_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/create_user_request.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/created_api_key.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/created_api_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/current_user_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/current_user_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/error_detail.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/id_selector_definition.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/identifier_part_schema.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/link.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/list_users_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/list_users_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/lusid_problem_details.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/lusid_validation_problem_details.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/o_auth_application.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/o_auth_application.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response_age.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response_age.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response_complexity.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response_complexity.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response_conditions.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response_conditions.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/password_policy_response_lockout.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/password_policy_response_lockout.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/resource_list_of_access_controlled_resource.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/role_id.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/role_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/role_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/set_password.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/set_password.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/set_password_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/set_password_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_access_expiry.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_access_expiry.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_access_expiry_with_role.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_access_expiry_with_role.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_access_request.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_access_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_access_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_access_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_role.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_role.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/support_roles_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/support_roles_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/temporary_password.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/temporary_password.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request_age.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request_age.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request_complexity.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request_complexity.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request_conditions.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request_conditions.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_password_policy_request_lockout.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_password_policy_request_lockout.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_role_request.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/update_user_request.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/user_response.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/user_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/models/user_summary.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/models/user_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/finbourne_identity/rest.py` & `finbourne_identity_sdk-2.1.4/finbourne_identity/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.3/PKG-INFO` & `finbourne_identity_sdk-2.1.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,14 @@
-Metadata-Version: 2.1
-Name: finbourne-identity-sdk
-Version: 2.1.3
-Summary: FINBOURNE Identity Service API
-Home-page: https://github.com/finbourne/finbourne-identity-sdk-python
-License: MIT
-Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Identity Service API,finbourne-identity-sdk
-Author: FINBOURNE Technology
-Author-email: info@finbourne.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aenum (>=3.1.11,<4.0.0)
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: pydantic (>=2.6.3,<3.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: requests (>=2,<3)
-Requires-Dist: urllib3 (>=1.25.3,<2.0.0)
-Project-URL: Repository, https://github.com/finbourne/finbourne-identity-sdk-python
-Description-Content-Type: text/markdown
-
 # finbourne-identity-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.2862
-- Package version: 2.1.3
+- API version: 0.0.2866
+- Package version: 2.1.4
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -195,71 +169,71 @@
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
     api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
-        # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
+        # ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling ApplicationMetadataApi->list_access_controlled_resources: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/identity*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
+*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | ListAccessControlledResources: Get resources available for access control
 *ApplicationsApi* | [**create_application**](docs/ApplicationsApi.md#create_application) | **POST** /api/applications | [EARLY ACCESS] CreateApplication: Create Application
 *ApplicationsApi* | [**delete_application**](docs/ApplicationsApi.md#delete_application) | **DELETE** /api/applications/{id} | [EARLY ACCESS] DeleteApplication: Delete Application
 *ApplicationsApi* | [**get_application**](docs/ApplicationsApi.md#get_application) | **GET** /api/applications/{id} | [EARLY ACCESS] GetApplication: Get Application
 *ApplicationsApi* | [**list_applications**](docs/ApplicationsApi.md#list_applications) | **GET** /api/applications | [EARLY ACCESS] ListApplications: List Applications
 *ApplicationsApi* | [**rotate_application_secrets**](docs/ApplicationsApi.md#rotate_application_secrets) | **POST** /api/applications/{id}/lifecycle/$newsecret | [EARLY ACCESS] RotateApplicationSecrets: Rotate Application Secrets
 *AuthenticationApi* | [**get_authentication_information**](docs/AuthenticationApi.md#get_authentication_information) | **GET** /api/authentication/information | GetAuthenticationInformation: Gets AuthenticationInformation
 *AuthenticationApi* | [**get_password_policy**](docs/AuthenticationApi.md#get_password_policy) | **GET** /api/authentication/password-policy/{userType} | [EXPERIMENTAL] GetPasswordPolicy: Gets password policy for a user type
-*AuthenticationApi* | [**get_support_access_history**](docs/AuthenticationApi.md#get_support_access_history) | **GET** /api/authentication/support | [EARLY ACCESS] GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination
-*AuthenticationApi* | [**get_support_roles**](docs/AuthenticationApi.md#get_support_roles) | **GET** /api/authentication/support-roles | [EARLY ACCESS] GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation
-*AuthenticationApi* | [**grant_support_access**](docs/AuthenticationApi.md#grant_support_access) | **POST** /api/authentication/support | [EARLY ACCESS] GrantSupportAccess: Grants FINBOURNE support access to your account
-*AuthenticationApi* | [**invalidate_support_access**](docs/AuthenticationApi.md#invalidate_support_access) | **DELETE** /api/authentication/support | [EARLY ACCESS] InvalidateSupportAccess: Revoke any FINBOURNE support access to your account
+*AuthenticationApi* | [**get_support_access_history**](docs/AuthenticationApi.md#get_support_access_history) | **GET** /api/authentication/support | GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination
+*AuthenticationApi* | [**get_support_roles**](docs/AuthenticationApi.md#get_support_roles) | **GET** /api/authentication/support-roles | GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation
+*AuthenticationApi* | [**grant_support_access**](docs/AuthenticationApi.md#grant_support_access) | **POST** /api/authentication/support | GrantSupportAccess: Grants FINBOURNE support access to your account
+*AuthenticationApi* | [**invalidate_support_access**](docs/AuthenticationApi.md#invalidate_support_access) | **DELETE** /api/authentication/support | InvalidateSupportAccess: Revoke any FINBOURNE support access to your account
 *AuthenticationApi* | [**update_password_policy**](docs/AuthenticationApi.md#update_password_policy) | **PUT** /api/authentication/password-policy/{userType} | [EXPERIMENTAL] UpdatePasswordPolicy: Updates password policy for a user type
-*IdentityProviderApi* | [**add_scim**](docs/IdentityProviderApi.md#add_scim) | **PUT** /api/identityprovider/scim | [EARLY ACCESS] AddScim: Add SCIM
-*IdentityProviderApi* | [**remove_scim**](docs/IdentityProviderApi.md#remove_scim) | **DELETE** /api/identityprovider/scim | [EARLY ACCESS] RemoveScim: Remove SCIM
-*MeApi* | [**get_user_info**](docs/MeApi.md#get_user_info) | **GET** /api/me | [EARLY ACCESS] GetUserInfo: Get User Info
+*IdentityProviderApi* | [**add_scim**](docs/IdentityProviderApi.md#add_scim) | **PUT** /api/identityprovider/scim | AddScim: Add SCIM
+*IdentityProviderApi* | [**remove_scim**](docs/IdentityProviderApi.md#remove_scim) | **DELETE** /api/identityprovider/scim | RemoveScim: Remove SCIM
+*MeApi* | [**get_user_info**](docs/MeApi.md#get_user_info) | **GET** /api/me | GetUserInfo: Get User Info
 *MeApi* | [**set_password**](docs/MeApi.md#set_password) | **PUT** /api/me/password | SetPassword: Set password of current user
-*PersonalAuthenticationTokensApi* | [**create_api_key**](docs/PersonalAuthenticationTokensApi.md#create_api_key) | **POST** /api/keys | [EARLY ACCESS] CreateApiKey: Create a Personal Access Token
-*PersonalAuthenticationTokensApi* | [**delete_api_key**](docs/PersonalAuthenticationTokensApi.md#delete_api_key) | **DELETE** /api/keys/{id} | [EARLY ACCESS] DeleteApiKey: Invalidate a Personal Access Token
-*PersonalAuthenticationTokensApi* | [**list_own_api_keys**](docs/PersonalAuthenticationTokensApi.md#list_own_api_keys) | **GET** /api/keys | [EARLY ACCESS] ListOwnApiKeys: Gets the meta data for all of the user&#39;s existing Personal Access Tokens.
-*RolesApi* | [**add_user_to_role**](docs/RolesApi.md#add_user_to_role) | **PUT** /api/roles/{id}/users/{userId} | [EARLY ACCESS] AddUserToRole: Add User to Role
-*RolesApi* | [**create_role**](docs/RolesApi.md#create_role) | **POST** /api/roles | [EARLY ACCESS] CreateRole: Create Role
-*RolesApi* | [**delete_role**](docs/RolesApi.md#delete_role) | **DELETE** /api/roles/{id} | [EARLY ACCESS] DeleteRole: Delete Role
-*RolesApi* | [**get_role**](docs/RolesApi.md#get_role) | **GET** /api/roles/{id} | [EARLY ACCESS] GetRole: Get Role
-*RolesApi* | [**list_roles**](docs/RolesApi.md#list_roles) | **GET** /api/roles | [EARLY ACCESS] ListRoles: List Roles
-*RolesApi* | [**list_users_in_role**](docs/RolesApi.md#list_users_in_role) | **GET** /api/roles/{id}/users | [EARLY ACCESS] ListUsersInRole: Get the users in the specified role.
-*RolesApi* | [**remove_user_from_role**](docs/RolesApi.md#remove_user_from_role) | **DELETE** /api/roles/{id}/users/{userId} | [EARLY ACCESS] RemoveUserFromRole: Remove User from Role
-*RolesApi* | [**update_role**](docs/RolesApi.md#update_role) | **PUT** /api/roles/{id} | [EARLY ACCESS] UpdateRole: Update Role
-*TokensApi* | [**invalidate_token**](docs/TokensApi.md#invalidate_token) | **DELETE** /api/tokens | [EARLY ACCESS] InvalidateToken: Invalidate current JWT token (sign out)
-*UsersApi* | [**create_user**](docs/UsersApi.md#create_user) | **POST** /api/users | [EARLY ACCESS] CreateUser: Create User
-*UsersApi* | [**delete_user**](docs/UsersApi.md#delete_user) | **DELETE** /api/users/{id} | [EARLY ACCESS] DeleteUser: Delete User
-*UsersApi* | [**expire_password**](docs/UsersApi.md#expire_password) | **POST** /api/users/{id}/lifecycle/$expirepassword | [EARLY ACCESS] ExpirePassword: Reset the user&#39;s password to a temporary one
-*UsersApi* | [**find_users_by_id**](docs/UsersApi.md#find_users_by_id) | **GET** /api/directory | [EARLY ACCESS] FindUsersById: Find users by id endpoint
-*UsersApi* | [**get_user**](docs/UsersApi.md#get_user) | **GET** /api/users/{id} | [EARLY ACCESS] GetUser: Get User
+*PersonalAuthenticationTokensApi* | [**create_api_key**](docs/PersonalAuthenticationTokensApi.md#create_api_key) | **POST** /api/keys | CreateApiKey: Create a Personal Access Token
+*PersonalAuthenticationTokensApi* | [**delete_api_key**](docs/PersonalAuthenticationTokensApi.md#delete_api_key) | **DELETE** /api/keys/{id} | DeleteApiKey: Invalidate a Personal Access Token
+*PersonalAuthenticationTokensApi* | [**list_own_api_keys**](docs/PersonalAuthenticationTokensApi.md#list_own_api_keys) | **GET** /api/keys | ListOwnApiKeys: Gets the meta data for all of the user&#39;s existing Personal Access Tokens.
+*RolesApi* | [**add_user_to_role**](docs/RolesApi.md#add_user_to_role) | **PUT** /api/roles/{id}/users/{userId} | AddUserToRole: Add User to Role
+*RolesApi* | [**create_role**](docs/RolesApi.md#create_role) | **POST** /api/roles | CreateRole: Create Role
+*RolesApi* | [**delete_role**](docs/RolesApi.md#delete_role) | **DELETE** /api/roles/{id} | DeleteRole: Delete Role
+*RolesApi* | [**get_role**](docs/RolesApi.md#get_role) | **GET** /api/roles/{id} | GetRole: Get Role
+*RolesApi* | [**list_roles**](docs/RolesApi.md#list_roles) | **GET** /api/roles | ListRoles: List Roles
+*RolesApi* | [**list_users_in_role**](docs/RolesApi.md#list_users_in_role) | **GET** /api/roles/{id}/users | ListUsersInRole: Get the users in the specified role.
+*RolesApi* | [**remove_user_from_role**](docs/RolesApi.md#remove_user_from_role) | **DELETE** /api/roles/{id}/users/{userId} | RemoveUserFromRole: Remove User from Role
+*RolesApi* | [**update_role**](docs/RolesApi.md#update_role) | **PUT** /api/roles/{id} | UpdateRole: Update Role
+*TokensApi* | [**invalidate_token**](docs/TokensApi.md#invalidate_token) | **DELETE** /api/tokens | InvalidateToken: Invalidate current JWT token (sign out)
+*UsersApi* | [**create_user**](docs/UsersApi.md#create_user) | **POST** /api/users | CreateUser: Create User
+*UsersApi* | [**delete_user**](docs/UsersApi.md#delete_user) | **DELETE** /api/users/{id} | DeleteUser: Delete User
+*UsersApi* | [**expire_password**](docs/UsersApi.md#expire_password) | **POST** /api/users/{id}/lifecycle/$expirepassword | ExpirePassword: Reset the user&#39;s password to a temporary one
+*UsersApi* | [**find_users_by_id**](docs/UsersApi.md#find_users_by_id) | **GET** /api/directory | FindUsersById: Find users by id endpoint
+*UsersApi* | [**get_user**](docs/UsersApi.md#get_user) | **GET** /api/users/{id} | GetUser: Get User
 *UsersApi* | [**list_runnable_users**](docs/UsersApi.md#list_runnable_users) | **GET** /api/users/$runnable | [EARLY ACCESS] ListRunnableUsers: List Runable Users
-*UsersApi* | [**list_users**](docs/UsersApi.md#list_users) | **GET** /api/users | [EARLY ACCESS] ListUsers: List Users
-*UsersApi* | [**reset_factors**](docs/UsersApi.md#reset_factors) | **POST** /api/users/{id}/lifecycle/$resetfactors | [EARLY ACCESS] ResetFactors: Reset MFA factors
-*UsersApi* | [**reset_password**](docs/UsersApi.md#reset_password) | **POST** /api/users/{id}/lifecycle/$resetpassword | [EARLY ACCESS] ResetPassword: Reset Password
-*UsersApi* | [**send_activation_email**](docs/UsersApi.md#send_activation_email) | **POST** /api/users/{id}/lifecycle/$activate | [EARLY ACCESS] SendActivationEmail: Sends an activation email to the User
-*UsersApi* | [**unlock_user**](docs/UsersApi.md#unlock_user) | **POST** /api/users/{id}/lifecycle/$unlock | [EARLY ACCESS] UnlockUser: Unlock User
+*UsersApi* | [**list_users**](docs/UsersApi.md#list_users) | **GET** /api/users | ListUsers: List Users
+*UsersApi* | [**reset_factors**](docs/UsersApi.md#reset_factors) | **POST** /api/users/{id}/lifecycle/$resetfactors | ResetFactors: Reset MFA factors
+*UsersApi* | [**reset_password**](docs/UsersApi.md#reset_password) | **POST** /api/users/{id}/lifecycle/$resetpassword | ResetPassword: Reset Password
+*UsersApi* | [**send_activation_email**](docs/UsersApi.md#send_activation_email) | **POST** /api/users/{id}/lifecycle/$activate | SendActivationEmail: Sends an activation email to the User
+*UsersApi* | [**unlock_user**](docs/UsersApi.md#unlock_user) | **POST** /api/users/{id}/lifecycle/$unlock | UnlockUser: Unlock User
 *UsersApi* | [**unsuspend_user**](docs/UsersApi.md#unsuspend_user) | **POST** /api/users/{id}/lifecycle/$unsuspend | [EXPERIMENTAL] UnsuspendUser: Unsuspend user
-*UsersApi* | [**update_user**](docs/UsersApi.md#update_user) | **PUT** /api/users/{id} | [EARLY ACCESS] UpdateUser: Update User
+*UsersApi* | [**update_user**](docs/UsersApi.md#update_user) | **PUT** /api/users/{id} | UpdateUser: Update User
 
 
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
@@ -323,8 +297,7 @@
 
 
 ## Author
 
 info@finbourne.com
 
 
-
```

