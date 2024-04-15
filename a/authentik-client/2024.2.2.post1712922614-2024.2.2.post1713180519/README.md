# Comparing `tmp/authentik_client-2024.2.2.post1712922614.tar.gz` & `tmp/authentik_client-2024.2.2.post1713180519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.2.2.post1712922614.tar", max compression
+gzip compressed data, was "authentik_client-2024.2.2.post1713180519.tar", max compression
```

## Comparing `authentik_client-2024.2.2.post1712922614.tar` & `authentik_client-2024.2.2.post1713180519.tar`

### file list

```diff
@@ -1,583 +1,582 @@
--rw-r--r--   0        0        0   140456 2024-04-12 11:50:27.891247 authentik_client-2024.2.2.post1712922614/README.md
--rw-r--r--   0        0        0    47475 2024-04-12 11:50:27.903247 authentik_client-2024.2.2.post1712922614/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-04-12 11:50:27.907247 authentik_client-2024.2.2.post1712922614/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-04-12 11:50:27.627245 authentik_client-2024.2.2.post1712922614/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-04-12 11:50:27.651245 authentik_client-2024.2.2.post1712922614/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   699928 2024-04-12 11:50:27.671245 authentik_client-2024.2.2.post1712922614/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-04-12 11:50:27.683246 authentik_client-2024.2.2.post1712922614/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-04-12 11:50:27.691246 authentik_client-2024.2.2.post1712922614/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-04-12 11:50:27.699246 authentik_client-2024.2.2.post1712922614/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-04-12 11:50:27.711246 authentik_client-2024.2.2.post1712922614/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-04-12 11:50:27.719246 authentik_client-2024.2.2.post1712922614/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-04-12 11:50:27.735246 authentik_client-2024.2.2.post1712922614/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413301 2024-04-12 11:50:27.747246 authentik_client-2024.2.2.post1712922614/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725201 2024-04-12 11:50:27.759246 authentik_client-2024.2.2.post1712922614/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   552586 2024-04-12 11:50:27.775246 authentik_client-2024.2.2.post1712922614/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0   718066 2024-04-12 11:50:27.799246 authentik_client-2024.2.2.post1712922614/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-04-12 11:50:27.815246 authentik_client-2024.2.2.post1712922614/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-04-12 11:50:27.823246 authentik_client-2024.2.2.post1712922614/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-04-12 11:50:27.831246 authentik_client-2024.2.2.post1712922614/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-04-12 11:50:27.835246 authentik_client-2024.2.2.post1712922614/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0   802117 2024-04-12 11:50:27.847246 authentik_client-2024.2.2.post1712922614/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1945986 2024-04-12 11:50:27.871246 authentik_client-2024.2.2.post1712922614/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-04-12 11:50:27.883247 authentik_client-2024.2.2.post1712922614/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-04-12 11:50:27.907247 authentik_client-2024.2.2.post1712922614/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-04-12 11:50:27.911247 authentik_client-2024.2.2.post1712922614/authentik_client/api_response.py
--rw-r--r--   0        0        0    14724 2024-04-12 11:50:27.903247 authentik_client-2024.2.2.post1712922614/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-04-12 11:50:27.907247 authentik_client-2024.2.2.post1712922614/authentik_client/exceptions.py
--rw-r--r--   0        0        0    45777 2024-04-12 11:50:27.903247 authentik_client-2024.2.2.post1712922614/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-04-12 11:50:24.575224 authentik_client-2024.2.2.post1712922614/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0     2482 2024-04-12 11:50:24.591224 authentik_client-2024.2.2.post1712922614/authentik_client/models/app.py
--rw-r--r--   0        0        0     4168 2024-04-12 11:50:24.599224 authentik_client-2024.2.2.post1712922614/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-04-12 11:50:24.615224 authentik_client-2024.2.2.post1712922614/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-04-12 11:50:24.627225 authentik_client-2024.2.2.post1712922614/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-04-12 11:50:24.639225 authentik_client-2024.2.2.post1712922614/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-04-12 11:50:24.651225 authentik_client-2024.2.2.post1712922614/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-04-12 11:50:24.659225 authentik_client-2024.2.2.post1712922614/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-04-12 11:50:24.663225 authentik_client-2024.2.2.post1712922614/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     5195 2024-04-12 11:50:24.671225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-04-12 11:50:24.679225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-04-12 11:50:24.691225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-04-12 11:50:24.699225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-04-12 11:50:24.707225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-04-12 11:50:24.715225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-04-12 11:50:24.727225 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-04-12 11:50:24.731226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-04-12 11:50:24.735226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-04-12 11:50:24.747226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-04-12 11:50:24.755226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-04-12 11:50:24.767226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-04-12 11:50:24.775226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-04-12 11:50:24.783226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-04-12 11:50:24.791226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-12 11:50:24.799226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-04-12 11:50:24.807226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-04-12 11:50:24.811226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-04-12 11:50:24.819226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-04-12 11:50:24.827226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-04-12 11:50:24.835226 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-04-12 11:50:24.839227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-04-12 11:50:24.843227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-04-12 11:50:24.851227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-04-12 11:50:24.855227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-04-12 11:50:24.859227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-04-12 11:50:24.867227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     6722 2024-04-12 11:50:24.875227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4893 2024-04-12 11:50:24.879227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-04-12 11:50:24.887227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-04-12 11:50:24.895227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-04-12 11:50:24.903227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-04-12 11:50:24.907227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     7081 2024-04-12 11:50:24.911227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_stage.py
--rw-r--r--   0        0        0     5302 2024-04-12 11:50:24.919227 authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     2718 2024-04-12 11:50:24.923227 authentik_client-2024.2.2.post1712922614/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-04-12 11:50:24.927227 authentik_client-2024.2.2.post1712922614/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-04-12 11:50:24.931228 authentik_client-2024.2.2.post1712922614/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-04-12 11:50:24.935227 authentik_client-2024.2.2.post1712922614/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-04-12 11:50:24.939227 authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-04-12 11:50:24.947228 authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-04-12 11:50:24.955228 authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-04-12 11:50:24.963228 authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-04-12 11:50:24.967228 authentik_client-2024.2.2.post1712922614/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-04-12 11:50:24.971228 authentik_client-2024.2.2.post1712922614/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-04-12 11:50:24.975228 authentik_client-2024.2.2.post1712922614/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-04-12 11:50:24.979228 authentik_client-2024.2.2.post1712922614/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-04-12 11:50:24.983228 authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-04-12 11:50:24.987228 authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-04-12 11:50:24.991228 authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-04-12 11:50:24.995228 authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-04-12 11:50:24.999228 authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2861 2024-04-12 11:50:25.007228 authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-04-12 11:50:25.011228 authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-04-12 11:50:25.015228 authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-04-12 11:50:25.019228 authentik_client-2024.2.2.post1712922614/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-04-12 11:50:25.027228 authentik_client-2024.2.2.post1712922614/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-04-12 11:50:25.031228 authentik_client-2024.2.2.post1712922614/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-04-12 11:50:25.035229 authentik_client-2024.2.2.post1712922614/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-04-12 11:50:25.039229 authentik_client-2024.2.2.post1712922614/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-04-12 11:50:25.043228 authentik_client-2024.2.2.post1712922614/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-04-12 11:50:25.047229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-04-12 11:50:25.055229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-04-12 11:50:25.063229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-04-12 11:50:25.075229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-04-12 11:50:25.079229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-04-12 11:50:25.083229 authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-04-12 11:50:25.091229 authentik_client-2024.2.2.post1712922614/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-04-12 11:50:25.095229 authentik_client-2024.2.2.post1712922614/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-04-12 11:50:25.103229 authentik_client-2024.2.2.post1712922614/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-04-12 11:50:25.111229 authentik_client-2024.2.2.post1712922614/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-04-12 11:50:25.115229 authentik_client-2024.2.2.post1712922614/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-04-12 11:50:25.123229 authentik_client-2024.2.2.post1712922614/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-04-12 11:50:25.131229 authentik_client-2024.2.2.post1712922614/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-04-12 11:50:25.139229 authentik_client-2024.2.2.post1712922614/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-04-12 11:50:25.147230 authentik_client-2024.2.2.post1712922614/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-04-12 11:50:25.155230 authentik_client-2024.2.2.post1712922614/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-04-12 11:50:25.159230 authentik_client-2024.2.2.post1712922614/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-04-12 11:50:25.163230 authentik_client-2024.2.2.post1712922614/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-04-12 11:50:25.163230 authentik_client-2024.2.2.post1712922614/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-04-12 11:50:25.171230 authentik_client-2024.2.2.post1712922614/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-04-12 11:50:25.179230 authentik_client-2024.2.2.post1712922614/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-04-12 11:50:25.187230 authentik_client-2024.2.2.post1712922614/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-04-12 11:50:25.199230 authentik_client-2024.2.2.post1712922614/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-04-12 11:50:25.207230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-04-12 11:50:25.215230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-04-12 11:50:25.219230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-04-12 11:50:25.227230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-04-12 11:50:25.235231 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-04-12 11:50:25.243230 authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-04-12 11:50:25.247231 authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-04-12 11:50:25.255231 authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-04-12 11:50:25.263231 authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-04-12 11:50:25.263231 authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-04-12 11:50:25.271231 authentik_client-2024.2.2.post1712922614/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-04-12 11:50:25.279231 authentik_client-2024.2.2.post1712922614/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-04-12 11:50:25.287231 authentik_client-2024.2.2.post1712922614/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-04-12 11:50:25.295231 authentik_client-2024.2.2.post1712922614/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-04-12 11:50:25.299231 authentik_client-2024.2.2.post1712922614/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-04-12 11:50:25.307231 authentik_client-2024.2.2.post1712922614/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-04-12 11:50:25.315231 authentik_client-2024.2.2.post1712922614/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-04-12 11:50:25.323231 authentik_client-2024.2.2.post1712922614/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-04-12 11:50:25.331231 authentik_client-2024.2.2.post1712922614/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-04-12 11:50:25.335231 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-04-12 11:50:25.339231 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-04-12 11:50:25.347231 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-04-12 11:50:25.351232 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-04-12 11:50:25.359232 authentik_client-2024.2.2.post1712922614/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3926 2024-04-12 11:50:25.367232 authentik_client-2024.2.2.post1712922614/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-04-12 11:50:25.375232 authentik_client-2024.2.2.post1712922614/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-04-12 11:50:25.383232 authentik_client-2024.2.2.post1712922614/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-04-12 11:50:25.391232 authentik_client-2024.2.2.post1712922614/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-04-12 11:50:25.395232 authentik_client-2024.2.2.post1712922614/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-04-12 11:50:25.403232 authentik_client-2024.2.2.post1712922614/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-04-12 11:50:25.411232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-04-12 11:50:25.419232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-04-12 11:50:25.423232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-04-12 11:50:25.427232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-04-12 11:50:25.439232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-04-12 11:50:25.443232 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-04-12 11:50:25.451233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-04-12 11:50:25.459233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-04-12 11:50:25.463233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-04-12 11:50:25.471233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-04-12 11:50:25.479233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-04-12 11:50:25.483233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-04-12 11:50:25.487233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-04-12 11:50:25.487233 authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-04-12 11:50:25.491233 authentik_client-2024.2.2.post1712922614/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-04-12 11:50:25.495233 authentik_client-2024.2.2.post1712922614/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-04-12 11:50:25.499233 authentik_client-2024.2.2.post1712922614/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     5216 2024-04-12 11:50:25.499233 authentik_client-2024.2.2.post1712922614/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-04-12 11:50:25.507233 authentik_client-2024.2.2.post1712922614/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-04-12 11:50:25.511233 authentik_client-2024.2.2.post1712922614/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-04-12 11:50:25.515233 authentik_client-2024.2.2.post1712922614/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-04-12 11:50:25.519233 authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-04-12 11:50:25.523233 authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-04-12 11:50:25.527233 authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-04-12 11:50:25.531233 authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-04-12 11:50:25.535233 authentik_client-2024.2.2.post1712922614/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-04-12 11:50:25.535233 authentik_client-2024.2.2.post1712922614/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-04-12 11:50:25.539234 authentik_client-2024.2.2.post1712922614/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4878 2024-04-12 11:50:25.543233 authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3895 2024-04-12 11:50:25.547233 authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-04-12 11:50:25.551234 authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-04-12 11:50:25.555234 authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-04-12 11:50:25.555234 authentik_client-2024.2.2.post1712922614/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-04-12 11:50:25.559234 authentik_client-2024.2.2.post1712922614/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-04-12 11:50:25.563234 authentik_client-2024.2.2.post1712922614/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-04-12 11:50:25.567234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-04-12 11:50:25.571234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-04-12 11:50:25.575234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-04-12 11:50:25.579234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-04-12 11:50:25.583234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-04-12 11:50:25.587234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11791 2024-04-12 11:50:25.591234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-04-12 11:50:25.595234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0     3129 2024-04-12 11:50:25.599234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_sync_status.py
--rw-r--r--   0        0        0      726 2024-04-12 11:50:25.563234 authentik_client-2024.2.2.post1712922614/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-04-12 11:50:25.603234 authentik_client-2024.2.2.post1712922614/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-04-12 11:50:25.607234 authentik_client-2024.2.2.post1712922614/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-04-12 11:50:25.611234 authentik_client-2024.2.2.post1712922614/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-04-12 11:50:25.615234 authentik_client-2024.2.2.post1712922614/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-04-12 11:50:25.619234 authentik_client-2024.2.2.post1712922614/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-04-12 11:50:25.623234 authentik_client-2024.2.2.post1712922614/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-04-12 11:50:25.627234 authentik_client-2024.2.2.post1712922614/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-04-12 11:50:25.631234 authentik_client-2024.2.2.post1712922614/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-04-12 11:50:25.635234 authentik_client-2024.2.2.post1712922614/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-04-12 11:50:25.639234 authentik_client-2024.2.2.post1712922614/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-04-12 11:50:25.643234 authentik_client-2024.2.2.post1712922614/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     7524 2024-04-12 11:50:25.647235 authentik_client-2024.2.2.post1712922614/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0     9828 2024-04-12 11:50:25.651234 authentik_client-2024.2.2.post1712922614/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-04-12 11:50:25.655235 authentik_client-2024.2.2.post1712922614/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-04-12 11:50:25.659235 authentik_client-2024.2.2.post1712922614/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-04-12 11:50:25.663235 authentik_client-2024.2.2.post1712922614/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-04-12 11:50:25.663235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-04-12 11:50:25.671235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-04-12 11:50:25.675235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-04-12 11:50:25.679235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-04-12 11:50:25.683235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-04-12 11:50:25.687235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-04-12 11:50:25.691235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-04-12 11:50:25.695235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-04-12 11:50:25.699235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-04-12 11:50:25.703235 authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-04-12 11:50:25.707235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-04-12 11:50:25.711235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-04-12 11:50:25.715235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-04-12 11:50:25.719235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-04-12 11:50:25.719235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-04-12 11:50:25.727235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-04-12 11:50:25.731235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10563 2024-04-12 11:50:25.735235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8013 2024-04-12 11:50:25.739235 authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-04-12 11:50:25.743235 authentik_client-2024.2.2.post1712922614/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0     5545 2024-04-12 11:50:25.747235 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-04-12 11:50:25.751236 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     3755 2024-04-12 11:50:25.755236 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-04-12 11:50:25.755236 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-04-12 11:50:25.759236 authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-04-12 11:50:25.763236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3395 2024-04-12 11:50:25.767236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-04-12 11:50:25.771236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-04-12 11:50:25.775236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-04-12 11:50:25.779236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-04-12 11:50:25.783236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-04-12 11:50:25.783236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3445 2024-04-12 11:50:25.787236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
--rw-r--r--   0        0        0     3371 2024-04-12 11:50:25.791236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-04-12 11:50:25.795236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.799236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-04-12 11:50:25.799236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-04-12 11:50:25.803236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.807236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-12 11:50:25.811236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-04-12 11:50:25.811236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-04-12 11:50:25.815236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-04-12 11:50:25.819236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.823236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-04-12 11:50:25.823236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.827236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-04-12 11:50:25.831236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-04-12 11:50:25.835236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-04-12 11:50:25.835236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-04-12 11:50:25.839236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-04-12 11:50:25.843236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-04-12 11:50:25.847236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-04-12 11:50:25.847236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-12 11:50:25.851236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-04-12 11:50:25.855236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3274 2024-04-12 11:50:25.859236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-04-12 11:50:25.867236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-12 11:50:25.871236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-04-12 11:50:25.871236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-04-12 11:50:25.875236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-04-12 11:50:25.879236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-04-12 11:50:25.883236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.883236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.887236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-12 11:50:25.891236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3330 2024-04-12 11:50:25.895236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-04-12 11:50:25.895236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-04-12 11:50:25.899237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-04-12 11:50:25.903236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-04-12 11:50:25.907236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-04-12 11:50:25.907236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-04-12 11:50:25.911236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-04-12 11:50:25.915237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-04-12 11:50:25.919237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-04-12 11:50:25.923236 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-04-12 11:50:25.927237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-04-12 11:50:25.931237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.935237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-04-12 11:50:25.939237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-04-12 11:50:25.943237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-04-12 11:50:25.943237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-04-12 11:50:25.947237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-04-12 11:50:25.951237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-04-12 11:50:25.955237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-12 11:50:25.959237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-04-12 11:50:25.963237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-04-12 11:50:25.967237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-04-12 11:50:25.971237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-04-12 11:50:25.971237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-04-12 11:50:25.975237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-04-12 11:50:25.979237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-04-12 11:50:25.979237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-04-12 11:50:25.983237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-04-12 11:50:25.987237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-04-12 11:50:25.987237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.991237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-04-12 11:50:25.995237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-12 11:50:25.995237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-04-12 11:50:25.999237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3331 2024-04-12 11:50:26.003237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-04-12 11:50:26.007237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-04-12 11:50:26.003237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-04-12 11:50:26.011237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-04-12 11:50:26.011237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-04-12 11:50:26.015237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-04-12 11:50:26.019237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-04-12 11:50:26.023237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-04-12 11:50:26.027237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-04-12 11:50:26.031237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-04-12 11:50:26.035237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-04-12 11:50:26.023237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-04-12 11:50:26.035237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-04-12 11:50:26.039237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-04-12 11:50:26.043237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-04-12 11:50:26.043237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-04-12 11:50:26.051237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-04-12 11:50:26.051237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-04-12 11:50:26.055237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-04-12 11:50:26.059237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-04-12 11:50:26.059237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-04-12 11:50:26.063237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-04-12 11:50:26.067237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3381 2024-04-12 11:50:26.071237 authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_web_authn_device_type_list.py
--rw-r--r--   0        0        0     3076 2024-04-12 11:50:26.075237 authentik_client-2024.2.2.post1712922614/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-04-12 11:50:26.079237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-04-12 11:50:26.079237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-04-12 11:50:26.083237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-04-12 11:50:26.087237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-04-12 11:50:26.087237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-04-12 11:50:26.091237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-04-12 11:50:26.095237 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-04-12 11:50:26.099238 authentik_client-2024.2.2.post1712922614/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-04-12 11:50:26.099238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     4833 2024-04-12 11:50:26.103237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-04-12 11:50:26.107237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-04-12 11:50:26.111237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-04-12 11:50:26.111237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4931 2024-04-12 11:50:26.115238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5340 2024-04-12 11:50:26.119238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     3246 2024-04-12 11:50:26.123237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-04-12 11:50:26.123237 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-04-12 11:50:26.127238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-04-12 11:50:26.131238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-04-12 11:50:26.131238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-04-12 11:50:26.135238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-04-12 11:50:26.139238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-04-12 11:50:26.139238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-04-12 11:50:26.143238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-04-12 11:50:26.147238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-04-12 11:50:26.147238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-04-12 11:50:26.151238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-04-12 11:50:26.155238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-04-12 11:50:26.159238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-04-12 11:50:26.163238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-04-12 11:50:26.167238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-04-12 11:50:26.171238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-04-12 11:50:26.175238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-04-12 11:50:26.179238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     3385 2024-04-12 11:50:26.183238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-04-12 11:50:26.187238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3985 2024-04-12 11:50:26.191238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-04-12 11:50:26.195238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-04-12 11:50:26.195238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-04-12 11:50:26.199238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-04-12 11:50:26.203238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-04-12 11:50:26.211238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-04-12 11:50:26.215238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2879 2024-04-12 11:50:26.219238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-04-12 11:50:26.223238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-04-12 11:50:26.223238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-04-12 11:50:26.227238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-04-12 11:50:26.231238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8185 2024-04-12 11:50:26.231238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-04-12 11:50:26.235238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-04-12 11:50:26.239238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-04-12 11:50:26.243238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-04-12 11:50:26.243238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-04-12 11:50:26.247238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-04-12 11:50:26.251238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-04-12 11:50:26.255238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-04-12 11:50:26.263238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-04-12 11:50:26.267238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-04-12 11:50:26.267238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-04-12 11:50:26.271238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-04-12 11:50:26.275238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-04-12 11:50:26.275238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-04-12 11:50:26.279238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-04-12 11:50:26.283238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-04-12 11:50:26.283238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-04-12 11:50:26.287238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-04-12 11:50:26.291238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-04-12 11:50:26.291238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-04-12 11:50:26.295238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-04-12 11:50:26.299239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3819 2024-04-12 11:50:26.303238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     5079 2024-04-12 11:50:26.307238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-04-12 11:50:26.299239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-04-12 11:50:26.311239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-04-12 11:50:26.311239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-04-12 11:50:26.319239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4419 2024-04-12 11:50:26.323238 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-04-12 11:50:26.315239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-04-12 11:50:26.327239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-04-12 11:50:26.331239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-04-12 11:50:26.339239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-04-12 11:50:26.339239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-04-12 11:50:26.347239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-04-12 11:50:26.351239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-04-12 11:50:26.355239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-04-12 11:50:26.355239 authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-04-12 11:50:26.359239 authentik_client-2024.2.2.post1712922614/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-04-12 11:50:26.359239 authentik_client-2024.2.2.post1712922614/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-04-12 11:50:26.363239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-04-12 11:50:26.367239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7752 2024-04-12 11:50:26.371239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-04-12 11:50:26.371239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-04-12 11:50:26.375239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-04-12 11:50:26.379239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-04-12 11:50:26.379239 authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-04-12 11:50:26.383239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-04-12 11:50:26.387239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-04-12 11:50:26.387239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-04-12 11:50:26.391239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-04-12 11:50:26.391239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-04-12 11:50:26.395239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-04-12 11:50:26.395239 authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-04-12 11:50:26.399239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-04-12 11:50:26.403239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-04-12 11:50:26.407239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-04-12 11:50:26.407239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-04-12 11:50:26.411239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-04-12 11:50:26.415239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-04-12 11:50:26.415239 authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-04-12 11:50:26.419239 authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-04-12 11:50:26.419239 authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2744 2024-04-12 11:50:26.423239 authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-04-12 11:50:26.427239 authentik_client-2024.2.2.post1712922614/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-04-12 11:50:26.427239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-04-12 11:50:26.431239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1314 2024-04-12 11:50:26.431239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-04-12 11:50:26.435239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-04-12 11:50:26.435239 authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-04-12 11:50:26.435239 authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-04-12 11:50:26.439239 authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-04-12 11:50:26.439239 authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-04-12 11:50:26.443239 authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-04-12 11:50:26.447239 authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-04-12 11:50:26.447239 authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-04-12 11:50:26.451239 authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-04-12 11:50:26.451239 authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-04-12 11:50:26.455239 authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-04-12 11:50:26.455239 authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-04-12 11:50:26.459239 authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-04-12 11:50:26.463239 authentik_client-2024.2.2.post1712922614/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-04-12 11:50:26.463239 authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-04-12 11:50:26.467239 authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-04-12 11:50:26.467239 authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-04-12 11:50:26.471239 authentik_client-2024.2.2.post1712922614/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-04-12 11:50:26.471239 authentik_client-2024.2.2.post1712922614/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-04-12 11:50:26.475239 authentik_client-2024.2.2.post1712922614/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-04-12 11:50:26.475239 authentik_client-2024.2.2.post1712922614/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-04-12 11:50:26.479239 authentik_client-2024.2.2.post1712922614/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-04-12 11:50:26.479239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-04-12 11:50:26.483240 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-04-12 11:50:26.483240 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-04-12 11:50:26.487239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-04-12 11:50:26.491239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10563 2024-04-12 11:50:26.491239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-04-12 11:50:26.495239 authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-04-12 11:50:26.495239 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-04-12 11:50:26.499240 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-04-12 11:50:26.503239 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-04-12 11:50:26.503239 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     3131 2024-04-12 11:50:26.507239 authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_sync_status.py
--rw-r--r--   0        0        0     4629 2024-04-12 11:50:26.515240 authentik_client-2024.2.2.post1712922614/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-04-12 11:50:26.519240 authentik_client-2024.2.2.post1712922614/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-04-12 11:50:26.523240 authentik_client-2024.2.2.post1712922614/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-04-12 11:50:26.527240 authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-04-12 11:50:26.527240 authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-04-12 11:50:26.531240 authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-04-12 11:50:26.535240 authentik_client-2024.2.2.post1712922614/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4931 2024-04-12 11:50:26.539240 authentik_client-2024.2.2.post1712922614/authentik_client/models/settings.py
--rw-r--r--   0        0        0     5058 2024-04-12 11:50:26.539240 authentik_client-2024.2.2.post1712922614/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-04-12 11:50:26.543240 authentik_client-2024.2.2.post1712922614/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-04-12 11:50:26.543240 authentik_client-2024.2.2.post1712922614/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     1492 2024-04-12 11:50:26.543240 authentik_client-2024.2.2.post1712922614/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-04-12 11:50:26.511240 authentik_client-2024.2.2.post1712922614/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-04-12 11:50:26.515240 authentik_client-2024.2.2.post1712922614/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-04-12 11:50:26.547240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-04-12 11:50:26.551240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-04-12 11:50:26.551240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-04-12 11:50:26.555240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-04-12 11:50:26.555240 authentik_client-2024.2.2.post1712922614/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-04-12 11:50:26.559240 authentik_client-2024.2.2.post1712922614/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-04-12 11:50:26.559240 authentik_client-2024.2.2.post1712922614/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-04-12 11:50:26.563240 authentik_client-2024.2.2.post1712922614/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-04-12 11:50:26.563240 authentik_client-2024.2.2.post1712922614/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-04-12 11:50:26.567240 authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-04-12 11:50:26.567240 authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-04-12 11:50:26.571240 authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-04-12 11:50:26.571240 authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-04-12 11:50:26.575240 authentik_client-2024.2.2.post1712922614/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     4463 2024-04-12 11:50:26.575240 authentik_client-2024.2.2.post1712922614/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     2934 2024-04-12 11:50:26.575240 authentik_client-2024.2.2.post1712922614/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4286 2024-04-12 11:50:26.579240 authentik_client-2024.2.2.post1712922614/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-04-12 11:50:26.579240 authentik_client-2024.2.2.post1712922614/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-04-12 11:50:26.587240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-04-12 11:50:26.591240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-04-12 11:50:26.591240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-04-12 11:50:26.595240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-04-12 11:50:26.595240 authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4802 2024-04-12 11:50:26.599240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token.py
--rw-r--r--   0        0        0     4198 2024-04-12 11:50:26.603240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4329 2024-04-12 11:50:26.607240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-04-12 11:50:26.607240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-04-12 11:50:26.611240 authentik_client-2024.2.2.post1712922614/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-04-12 11:50:26.583240 authentik_client-2024.2.2.post1712922614/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-04-12 11:50:26.583240 authentik_client-2024.2.2.post1712922614/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-04-12 11:50:26.615240 authentik_client-2024.2.2.post1712922614/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-04-12 11:50:26.619240 authentik_client-2024.2.2.post1712922614/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     2936 2024-04-12 11:50:26.619240 authentik_client-2024.2.2.post1712922614/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-04-12 11:50:26.623240 authentik_client-2024.2.2.post1712922614/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-04-12 11:50:26.623240 authentik_client-2024.2.2.post1712922614/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-04-12 11:50:26.627240 authentik_client-2024.2.2.post1712922614/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5226 2024-04-12 11:50:26.627240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-04-12 11:50:26.631240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-04-12 11:50:26.635240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3828 2024-04-12 11:50:26.635240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-04-12 11:50:26.639240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-04-12 11:50:26.639240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-04-12 11:50:26.643240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-04-12 11:50:26.647240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-04-12 11:50:26.647240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     3193 2024-04-12 11:50:26.651240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_group_request.py
--rw-r--r--   0        0        0     4334 2024-04-12 11:50:26.655240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-04-12 11:50:26.659240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-04-12 11:50:26.659240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-04-12 11:50:26.663240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-04-12 11:50:26.663240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-04-12 11:50:26.667240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-04-12 11:50:26.667240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-04-12 11:50:26.671240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-04-12 11:50:26.675240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-04-12 11:50:26.675240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-04-12 11:50:26.679240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-04-12 11:50:26.683241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-04-12 11:50:26.683241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-04-12 11:50:26.687240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-04-12 11:50:26.687240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-04-12 11:50:26.691240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-04-12 11:50:26.695240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-04-12 11:50:26.699241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-04-12 11:50:26.699241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-04-12 11:50:26.703240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-04-12 11:50:26.703240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-04-12 11:50:26.707240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-04-12 11:50:26.707240 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-04-12 11:50:26.711241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-04-12 11:50:26.715241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-04-12 11:50:26.715241 authentik_client-2024.2.2.post1712922614/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-04-12 11:50:26.719241 authentik_client-2024.2.2.post1712922614/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-04-12 11:50:26.723241 authentik_client-2024.2.2.post1712922614/authentik_client/models/version.py
--rw-r--r--   0        0        0     3630 2024-04-12 11:50:26.727241 authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-04-12 11:50:26.727241 authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2562 2024-04-12 11:50:26.731241 authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_type.py
--rw-r--r--   0        0        0     2669 2024-04-12 11:50:26.735241 authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_type_request.py
--rw-r--r--   0        0        0     2410 2024-04-12 11:50:26.735241 authentik_client-2024.2.2.post1712922614/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-04-12 11:50:27.899247 authentik_client-2024.2.2.post1712922614/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-04-12 11:50:27.911247 authentik_client-2024.2.2.post1712922614/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-04-12 11:50:27.899247 authentik_client-2024.2.2.post1712922614/pyproject.toml
--rw-r--r--   0        0        0   141408 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1712922614/PKG-INFO
+-rw-r--r--   0        0        0   140408 2024-04-15 11:28:51.673251 authentik_client-2024.2.2.post1713180519/README.md
+-rw-r--r--   0        0        0    47403 2024-04-15 11:28:51.685251 authentik_client-2024.2.2.post1713180519/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-04-15 11:28:51.685251 authentik_client-2024.2.2.post1713180519/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-04-15 11:28:51.381248 authentik_client-2024.2.2.post1713180519/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-04-15 11:28:51.405248 authentik_client-2024.2.2.post1713180519/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   701197 2024-04-15 11:28:51.425248 authentik_client-2024.2.2.post1713180519/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-04-15 11:28:51.437248 authentik_client-2024.2.2.post1713180519/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-04-15 11:28:51.445248 authentik_client-2024.2.2.post1713180519/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-04-15 11:28:51.457248 authentik_client-2024.2.2.post1713180519/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-04-15 11:28:51.469248 authentik_client-2024.2.2.post1713180519/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-04-15 11:28:51.477249 authentik_client-2024.2.2.post1713180519/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-04-15 11:28:51.485249 authentik_client-2024.2.2.post1713180519/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413301 2024-04-15 11:28:51.497249 authentik_client-2024.2.2.post1713180519/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725201 2024-04-15 11:28:51.513249 authentik_client-2024.2.2.post1713180519/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   552586 2024-04-15 11:28:51.529249 authentik_client-2024.2.2.post1713180519/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0   718066 2024-04-15 11:28:51.553249 authentik_client-2024.2.2.post1713180519/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-04-15 11:28:51.565249 authentik_client-2024.2.2.post1713180519/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-04-15 11:28:51.577249 authentik_client-2024.2.2.post1713180519/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-04-15 11:28:51.581250 authentik_client-2024.2.2.post1713180519/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-04-15 11:28:51.589250 authentik_client-2024.2.2.post1713180519/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0   802117 2024-04-15 11:28:51.605250 authentik_client-2024.2.2.post1713180519/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945986 2024-04-15 11:28:51.649250 authentik_client-2024.2.2.post1713180519/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-04-15 11:28:51.665250 authentik_client-2024.2.2.post1713180519/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-04-15 11:28:51.689251 authentik_client-2024.2.2.post1713180519/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-15 11:28:51.689251 authentik_client-2024.2.2.post1713180519/authentik_client/api_response.py
+-rw-r--r--   0        0        0    14724 2024-04-15 11:28:51.681250 authentik_client-2024.2.2.post1713180519/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-04-15 11:28:51.685251 authentik_client-2024.2.2.post1713180519/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    45705 2024-04-15 11:28:51.685251 authentik_client-2024.2.2.post1713180519/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-04-15 11:28:48.585221 authentik_client-2024.2.2.post1713180519/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0     2482 2024-04-15 11:28:48.597221 authentik_client-2024.2.2.post1713180519/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4168 2024-04-15 11:28:48.605221 authentik_client-2024.2.2.post1713180519/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-04-15 11:28:48.617221 authentik_client-2024.2.2.post1713180519/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-04-15 11:28:48.625221 authentik_client-2024.2.2.post1713180519/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-04-15 11:28:48.637221 authentik_client-2024.2.2.post1713180519/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-04-15 11:28:48.645221 authentik_client-2024.2.2.post1713180519/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-04-15 11:28:48.649221 authentik_client-2024.2.2.post1713180519/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-04-15 11:28:48.649221 authentik_client-2024.2.2.post1713180519/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     5195 2024-04-15 11:28:48.657221 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-04-15 11:28:48.665221 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-04-15 11:28:48.669221 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-04-15 11:28:48.677221 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-04-15 11:28:48.681221 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-04-15 11:28:48.689221 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-04-15 11:28:48.693221 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-04-15 11:28:48.697222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-04-15 11:28:48.701222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-04-15 11:28:48.705222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-04-15 11:28:48.713222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-04-15 11:28:48.717222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-04-15 11:28:48.725222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-04-15 11:28:48.729222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-04-15 11:28:48.733222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-15 11:28:48.741222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-04-15 11:28:48.745222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-04-15 11:28:48.749222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-04-15 11:28:48.757222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-04-15 11:28:48.761222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-04-15 11:28:48.765222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-04-15 11:28:48.769222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-04-15 11:28:48.773222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-04-15 11:28:48.781222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-04-15 11:28:48.781222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-04-15 11:28:48.785222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-04-15 11:28:48.789222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     6722 2024-04-15 11:28:48.797222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4893 2024-04-15 11:28:48.801222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-04-15 11:28:48.805222 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-04-15 11:28:48.813223 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-04-15 11:28:48.817223 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-04-15 11:28:48.829223 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-04-15 11:28:48.837223 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-04-15 11:28:48.837223 authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-04-15 11:28:48.841223 authentik_client-2024.2.2.post1713180519/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-04-15 11:28:48.845223 authentik_client-2024.2.2.post1713180519/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-04-15 11:28:48.849223 authentik_client-2024.2.2.post1713180519/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-04-15 11:28:48.853223 authentik_client-2024.2.2.post1713180519/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-04-15 11:28:48.857223 authentik_client-2024.2.2.post1713180519/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-04-15 11:28:48.861223 authentik_client-2024.2.2.post1713180519/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-04-15 11:28:48.865223 authentik_client-2024.2.2.post1713180519/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-04-15 11:28:48.865223 authentik_client-2024.2.2.post1713180519/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-04-15 11:28:48.869223 authentik_client-2024.2.2.post1713180519/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-04-15 11:28:48.873223 authentik_client-2024.2.2.post1713180519/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-04-15 11:28:48.877223 authentik_client-2024.2.2.post1713180519/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-04-15 11:28:48.881223 authentik_client-2024.2.2.post1713180519/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-04-15 11:28:48.885223 authentik_client-2024.2.2.post1713180519/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-04-15 11:28:48.889223 authentik_client-2024.2.2.post1713180519/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-04-15 11:28:48.893223 authentik_client-2024.2.2.post1713180519/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-04-15 11:28:48.897223 authentik_client-2024.2.2.post1713180519/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-04-15 11:28:48.901223 authentik_client-2024.2.2.post1713180519/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2861 2024-04-15 11:28:48.905223 authentik_client-2024.2.2.post1713180519/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-04-15 11:28:48.909223 authentik_client-2024.2.2.post1713180519/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-04-15 11:28:48.909223 authentik_client-2024.2.2.post1713180519/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-04-15 11:28:48.913223 authentik_client-2024.2.2.post1713180519/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-04-15 11:28:48.921223 authentik_client-2024.2.2.post1713180519/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-04-15 11:28:48.925223 authentik_client-2024.2.2.post1713180519/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-04-15 11:28:48.929223 authentik_client-2024.2.2.post1713180519/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-04-15 11:28:48.933224 authentik_client-2024.2.2.post1713180519/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-04-15 11:28:48.937224 authentik_client-2024.2.2.post1713180519/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-04-15 11:28:48.941224 authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-04-15 11:28:48.945224 authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-04-15 11:28:48.949224 authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-04-15 11:28:48.953224 authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-04-15 11:28:48.953224 authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-04-15 11:28:48.957224 authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-04-15 11:28:48.961224 authentik_client-2024.2.2.post1713180519/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-04-15 11:28:48.969224 authentik_client-2024.2.2.post1713180519/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-04-15 11:28:48.969224 authentik_client-2024.2.2.post1713180519/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-04-15 11:28:48.973224 authentik_client-2024.2.2.post1713180519/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-04-15 11:28:48.977224 authentik_client-2024.2.2.post1713180519/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-04-15 11:28:48.981224 authentik_client-2024.2.2.post1713180519/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-04-15 11:28:48.985224 authentik_client-2024.2.2.post1713180519/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-04-15 11:28:48.989224 authentik_client-2024.2.2.post1713180519/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-04-15 11:28:48.993224 authentik_client-2024.2.2.post1713180519/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-04-15 11:28:49.001224 authentik_client-2024.2.2.post1713180519/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-04-15 11:28:49.001224 authentik_client-2024.2.2.post1713180519/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-04-15 11:28:49.005224 authentik_client-2024.2.2.post1713180519/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-04-15 11:28:49.009224 authentik_client-2024.2.2.post1713180519/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-04-15 11:28:49.009224 authentik_client-2024.2.2.post1713180519/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-04-15 11:28:49.013224 authentik_client-2024.2.2.post1713180519/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-04-15 11:28:49.021224 authentik_client-2024.2.2.post1713180519/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-04-15 11:28:49.021224 authentik_client-2024.2.2.post1713180519/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-04-15 11:28:49.025224 authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-04-15 11:28:49.029224 authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-04-15 11:28:49.033224 authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-04-15 11:28:49.037224 authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-04-15 11:28:49.041224 authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-04-15 11:28:49.045225 authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-04-15 11:28:49.049224 authentik_client-2024.2.2.post1713180519/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-04-15 11:28:49.053224 authentik_client-2024.2.2.post1713180519/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-04-15 11:28:49.057225 authentik_client-2024.2.2.post1713180519/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-04-15 11:28:49.057225 authentik_client-2024.2.2.post1713180519/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-04-15 11:28:49.061225 authentik_client-2024.2.2.post1713180519/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-04-15 11:28:49.065225 authentik_client-2024.2.2.post1713180519/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-04-15 11:28:49.069225 authentik_client-2024.2.2.post1713180519/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-04-15 11:28:49.073225 authentik_client-2024.2.2.post1713180519/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-04-15 11:28:49.081225 authentik_client-2024.2.2.post1713180519/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-04-15 11:28:49.085225 authentik_client-2024.2.2.post1713180519/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-04-15 11:28:49.089225 authentik_client-2024.2.2.post1713180519/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-04-15 11:28:49.093225 authentik_client-2024.2.2.post1713180519/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-04-15 11:28:49.101225 authentik_client-2024.2.2.post1713180519/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-04-15 11:28:49.109225 authentik_client-2024.2.2.post1713180519/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-04-15 11:28:49.113225 authentik_client-2024.2.2.post1713180519/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-04-15 11:28:49.117225 authentik_client-2024.2.2.post1713180519/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-04-15 11:28:49.125225 authentik_client-2024.2.2.post1713180519/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-04-15 11:28:49.129225 authentik_client-2024.2.2.post1713180519/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3926 2024-04-15 11:28:49.133225 authentik_client-2024.2.2.post1713180519/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-04-15 11:28:49.137225 authentik_client-2024.2.2.post1713180519/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-04-15 11:28:49.141225 authentik_client-2024.2.2.post1713180519/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-04-15 11:28:49.145225 authentik_client-2024.2.2.post1713180519/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-04-15 11:28:49.153225 authentik_client-2024.2.2.post1713180519/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-04-15 11:28:49.157225 authentik_client-2024.2.2.post1713180519/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-04-15 11:28:49.165225 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-04-15 11:28:49.173225 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-04-15 11:28:49.177225 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-04-15 11:28:49.181226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-04-15 11:28:49.189226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-04-15 11:28:49.197226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-04-15 11:28:49.201226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-04-15 11:28:49.209226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-04-15 11:28:49.213226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-04-15 11:28:49.217226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-04-15 11:28:49.225226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-04-15 11:28:49.229226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-04-15 11:28:49.237226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-04-15 11:28:49.245226 authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-04-15 11:28:49.253226 authentik_client-2024.2.2.post1713180519/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-04-15 11:28:49.257226 authentik_client-2024.2.2.post1713180519/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-04-15 11:28:49.261226 authentik_client-2024.2.2.post1713180519/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     5216 2024-04-15 11:28:49.265226 authentik_client-2024.2.2.post1713180519/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-04-15 11:28:49.273227 authentik_client-2024.2.2.post1713180519/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-04-15 11:28:49.277227 authentik_client-2024.2.2.post1713180519/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-04-15 11:28:49.285227 authentik_client-2024.2.2.post1713180519/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-04-15 11:28:49.289227 authentik_client-2024.2.2.post1713180519/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-04-15 11:28:49.297227 authentik_client-2024.2.2.post1713180519/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-04-15 11:28:49.305227 authentik_client-2024.2.2.post1713180519/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-04-15 11:28:49.309227 authentik_client-2024.2.2.post1713180519/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-04-15 11:28:49.317227 authentik_client-2024.2.2.post1713180519/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-04-15 11:28:49.321227 authentik_client-2024.2.2.post1713180519/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-04-15 11:28:49.325227 authentik_client-2024.2.2.post1713180519/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4878 2024-04-15 11:28:49.329227 authentik_client-2024.2.2.post1713180519/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3895 2024-04-15 11:28:49.337227 authentik_client-2024.2.2.post1713180519/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-04-15 11:28:49.341227 authentik_client-2024.2.2.post1713180519/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-04-15 11:28:49.345227 authentik_client-2024.2.2.post1713180519/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-04-15 11:28:49.349227 authentik_client-2024.2.2.post1713180519/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-04-15 11:28:49.353227 authentik_client-2024.2.2.post1713180519/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-04-15 11:28:49.361227 authentik_client-2024.2.2.post1713180519/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-04-15 11:28:49.369228 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-04-15 11:28:49.373227 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-04-15 11:28:49.381228 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-04-15 11:28:49.385228 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-04-15 11:28:49.389228 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-04-15 11:28:49.397228 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11791 2024-04-15 11:28:49.401228 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-04-15 11:28:49.409228 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0     3129 2024-04-15 11:28:49.413228 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_sync_status.py
+-rw-r--r--   0        0        0      726 2024-04-15 11:28:49.361227 authentik_client-2024.2.2.post1713180519/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-04-15 11:28:49.417228 authentik_client-2024.2.2.post1713180519/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-04-15 11:28:49.421228 authentik_client-2024.2.2.post1713180519/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-04-15 11:28:49.421228 authentik_client-2024.2.2.post1713180519/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-04-15 11:28:49.425228 authentik_client-2024.2.2.post1713180519/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-04-15 11:28:49.429228 authentik_client-2024.2.2.post1713180519/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-04-15 11:28:49.433228 authentik_client-2024.2.2.post1713180519/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-04-15 11:28:49.437228 authentik_client-2024.2.2.post1713180519/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-04-15 11:28:49.441228 authentik_client-2024.2.2.post1713180519/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-04-15 11:28:49.441228 authentik_client-2024.2.2.post1713180519/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-04-15 11:28:49.445228 authentik_client-2024.2.2.post1713180519/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-04-15 11:28:49.449228 authentik_client-2024.2.2.post1713180519/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     7524 2024-04-15 11:28:49.449228 authentik_client-2024.2.2.post1713180519/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0     9828 2024-04-15 11:28:49.453228 authentik_client-2024.2.2.post1713180519/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-04-15 11:28:49.457228 authentik_client-2024.2.2.post1713180519/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-04-15 11:28:49.457228 authentik_client-2024.2.2.post1713180519/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-04-15 11:28:49.461228 authentik_client-2024.2.2.post1713180519/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-04-15 11:28:49.461228 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-04-15 11:28:49.465228 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-04-15 11:28:49.469228 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-04-15 11:28:49.473229 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-04-15 11:28:49.473229 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-04-15 11:28:49.477228 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-04-15 11:28:49.481229 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-04-15 11:28:49.485229 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-04-15 11:28:49.485229 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-04-15 11:28:49.489229 authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-04-15 11:28:49.493229 authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-04-15 11:28:49.497229 authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-04-15 11:28:49.497229 authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-04-15 11:28:49.501229 authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-04-15 11:28:49.505229 authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-04-15 11:28:49.509229 authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-04-15 11:28:49.513229 authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10563 2024-04-15 11:28:49.513229 authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8013 2024-04-15 11:28:49.517229 authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-04-15 11:28:49.521229 authentik_client-2024.2.2.post1713180519/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0     5545 2024-04-15 11:28:49.525229 authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-04-15 11:28:49.529229 authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     3755 2024-04-15 11:28:49.529229 authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-04-15 11:28:49.533229 authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-04-15 11:28:49.537229 authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-04-15 11:28:49.537229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-04-15 11:28:49.541229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-04-15 11:28:49.545229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-04-15 11:28:49.549229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-04-15 11:28:49.553229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-04-15 11:28:49.557229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-04-15 11:28:49.561229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-04-15 11:28:49.565230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-04-15 11:28:49.569229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-04-15 11:28:49.573229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-04-15 11:28:49.573229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-04-15 11:28:49.577230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-04-15 11:28:49.581230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-04-15 11:28:49.585229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-15 11:28:49.585229 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-04-15 11:28:49.589230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-04-15 11:28:49.593230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-04-15 11:28:49.593230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-04-15 11:28:49.597230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-04-15 11:28:49.601230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-15 11:28:49.605230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-04-15 11:28:49.609230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-04-15 11:28:49.609230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-04-15 11:28:49.613230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-04-15 11:28:49.617230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-04-15 11:28:49.617230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-04-15 11:28:49.621230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-04-15 11:28:49.625230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-15 11:28:49.629230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-04-15 11:28:49.629230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3274 2024-04-15 11:28:49.633230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-04-15 11:28:49.637230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-15 11:28:49.641230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-04-15 11:28:49.645230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-04-15 11:28:49.649230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-04-15 11:28:49.653230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-04-15 11:28:49.657230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-15 11:28:49.657230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-15 11:28:49.661230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-15 11:28:49.665230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3330 2024-04-15 11:28:49.665230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-04-15 11:28:49.669231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-04-15 11:28:49.673231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-04-15 11:28:49.677230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-04-15 11:28:49.677230 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-04-15 11:28:49.681231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-04-15 11:28:49.685231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-04-15 11:28:49.689231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-04-15 11:28:49.693231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-04-15 11:28:49.693231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-04-15 11:28:49.697231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-04-15 11:28:49.701231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-04-15 11:28:49.701231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-04-15 11:28:49.705231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-04-15 11:28:49.709231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-04-15 11:28:49.709231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-04-15 11:28:49.713231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-04-15 11:28:49.713231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-04-15 11:28:49.717231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-15 11:28:49.721231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-04-15 11:28:49.721231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-04-15 11:28:49.725231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-04-15 11:28:49.729231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-04-15 11:28:49.733231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-04-15 11:28:49.733231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-04-15 11:28:49.737231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-04-15 11:28:49.741231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-04-15 11:28:49.741231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-04-15 11:28:49.745231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-04-15 11:28:49.749231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-15 11:28:49.749231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-04-15 11:28:49.753231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-15 11:28:49.757231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-04-15 11:28:49.757231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3331 2024-04-15 11:28:49.765231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-04-15 11:28:49.765231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-04-15 11:28:49.761231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-04-15 11:28:49.769231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-04-15 11:28:49.773231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-04-15 11:28:49.773231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-04-15 11:28:49.777232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-04-15 11:28:49.781231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-04-15 11:28:49.785232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-04-15 11:28:49.789232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-04-15 11:28:49.789232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-04-15 11:28:49.781231 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-04-15 11:28:49.793232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-04-15 11:28:49.797232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-04-15 11:28:49.797232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-04-15 11:28:49.801232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-04-15 11:28:49.805232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-04-15 11:28:49.805232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-04-15 11:28:49.809232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-04-15 11:28:49.813232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-04-15 11:28:49.813232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-04-15 11:28:49.817232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-04-15 11:28:49.821232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-04-15 11:28:49.821232 authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-04-15 11:28:49.825232 authentik_client-2024.2.2.post1713180519/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-04-15 11:28:49.829232 authentik_client-2024.2.2.post1713180519/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-04-15 11:28:49.829232 authentik_client-2024.2.2.post1713180519/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-04-15 11:28:49.833232 authentik_client-2024.2.2.post1713180519/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-04-15 11:28:49.837232 authentik_client-2024.2.2.post1713180519/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-04-15 11:28:49.837232 authentik_client-2024.2.2.post1713180519/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-04-15 11:28:49.841232 authentik_client-2024.2.2.post1713180519/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-04-15 11:28:49.845232 authentik_client-2024.2.2.post1713180519/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-04-15 11:28:49.845232 authentik_client-2024.2.2.post1713180519/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-04-15 11:28:49.849232 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-04-15 11:28:49.853232 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-04-15 11:28:49.857232 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-04-15 11:28:49.857232 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-04-15 11:28:49.861232 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4931 2024-04-15 11:28:49.865232 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-04-15 11:28:49.869233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-04-15 11:28:49.873232 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-04-15 11:28:49.873232 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-04-15 11:28:49.877232 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-04-15 11:28:49.881233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-04-15 11:28:49.881233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-04-15 11:28:49.885233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-04-15 11:28:49.885233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-04-15 11:28:49.889233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-04-15 11:28:49.889233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-04-15 11:28:49.893233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-04-15 11:28:49.893233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-04-15 11:28:49.897233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-04-15 11:28:49.901233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-04-15 11:28:49.901233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-04-15 11:28:49.905233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-04-15 11:28:49.909233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-04-15 11:28:49.909233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-04-15 11:28:49.913233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-04-15 11:28:49.917233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     3385 2024-04-15 11:28:49.921233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-04-15 11:28:49.925233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3985 2024-04-15 11:28:49.929233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-04-15 11:28:49.933233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-04-15 11:28:49.933233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-04-15 11:28:49.937233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-04-15 11:28:49.941233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-04-15 11:28:49.945233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-04-15 11:28:49.949233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     2879 2024-04-15 11:28:49.949233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-04-15 11:28:49.953233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-04-15 11:28:49.957233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-04-15 11:28:49.957233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-04-15 11:28:49.961233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8185 2024-04-15 11:28:49.965233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-04-15 11:28:49.969233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-04-15 11:28:49.969233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-04-15 11:28:49.973234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-04-15 11:28:49.977234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-04-15 11:28:49.981233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-04-15 11:28:49.981233 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-04-15 11:28:49.985234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-04-15 11:28:49.989234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-04-15 11:28:49.993234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-04-15 11:28:49.997234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-04-15 11:28:50.001234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-04-15 11:28:50.005234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-04-15 11:28:50.005234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-04-15 11:28:50.009234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-04-15 11:28:50.013234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-04-15 11:28:50.013234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-04-15 11:28:50.017234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-04-15 11:28:50.017234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-04-15 11:28:50.021234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-04-15 11:28:50.025234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-04-15 11:28:50.025234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3819 2024-04-15 11:28:50.033234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     5079 2024-04-15 11:28:50.037234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-04-15 11:28:50.029234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-04-15 11:28:50.037234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-04-15 11:28:50.041234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-04-15 11:28:50.049234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4419 2024-04-15 11:28:50.049234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-04-15 11:28:50.045234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-04-15 11:28:50.053234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-04-15 11:28:50.057234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-04-15 11:28:50.057234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-04-15 11:28:50.061234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-04-15 11:28:50.061234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-04-15 11:28:50.065234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-04-15 11:28:50.069234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-04-15 11:28:50.073234 authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-04-15 11:28:50.077235 authentik_client-2024.2.2.post1713180519/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-04-15 11:28:50.077235 authentik_client-2024.2.2.post1713180519/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-04-15 11:28:50.081235 authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-04-15 11:28:50.085234 authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7752 2024-04-15 11:28:50.089235 authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-04-15 11:28:50.093235 authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-04-15 11:28:50.093235 authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-04-15 11:28:50.097235 authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-04-15 11:28:50.097235 authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-04-15 11:28:50.101235 authentik_client-2024.2.2.post1713180519/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-04-15 11:28:50.101235 authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-04-15 11:28:50.105235 authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-04-15 11:28:50.109235 authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-04-15 11:28:50.109235 authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-04-15 11:28:50.113235 authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-04-15 11:28:50.117235 authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-04-15 11:28:50.121235 authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-04-15 11:28:50.125235 authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-04-15 11:28:50.125235 authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-04-15 11:28:50.129235 authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-04-15 11:28:50.133235 authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-04-15 11:28:50.137235 authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-04-15 11:28:50.137235 authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-04-15 11:28:50.141235 authentik_client-2024.2.2.post1713180519/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-04-15 11:28:50.145235 authentik_client-2024.2.2.post1713180519/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2744 2024-04-15 11:28:50.145235 authentik_client-2024.2.2.post1713180519/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-04-15 11:28:50.149235 authentik_client-2024.2.2.post1713180519/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-04-15 11:28:50.149235 authentik_client-2024.2.2.post1713180519/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-04-15 11:28:50.153235 authentik_client-2024.2.2.post1713180519/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1314 2024-04-15 11:28:50.157235 authentik_client-2024.2.2.post1713180519/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-04-15 11:28:50.157235 authentik_client-2024.2.2.post1713180519/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-04-15 11:28:50.157235 authentik_client-2024.2.2.post1713180519/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-04-15 11:28:50.161235 authentik_client-2024.2.2.post1713180519/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-04-15 11:28:50.161235 authentik_client-2024.2.2.post1713180519/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-04-15 11:28:50.165235 authentik_client-2024.2.2.post1713180519/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-04-15 11:28:50.165235 authentik_client-2024.2.2.post1713180519/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-04-15 11:28:50.169235 authentik_client-2024.2.2.post1713180519/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-04-15 11:28:50.169235 authentik_client-2024.2.2.post1713180519/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-04-15 11:28:50.173236 authentik_client-2024.2.2.post1713180519/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-04-15 11:28:50.173236 authentik_client-2024.2.2.post1713180519/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-04-15 11:28:50.177235 authentik_client-2024.2.2.post1713180519/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-04-15 11:28:50.181236 authentik_client-2024.2.2.post1713180519/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-04-15 11:28:50.181236 authentik_client-2024.2.2.post1713180519/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-04-15 11:28:50.185236 authentik_client-2024.2.2.post1713180519/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-04-15 11:28:50.185236 authentik_client-2024.2.2.post1713180519/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-04-15 11:28:50.189236 authentik_client-2024.2.2.post1713180519/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-04-15 11:28:50.189236 authentik_client-2024.2.2.post1713180519/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-04-15 11:28:50.189236 authentik_client-2024.2.2.post1713180519/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-04-15 11:28:50.193236 authentik_client-2024.2.2.post1713180519/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-04-15 11:28:50.193236 authentik_client-2024.2.2.post1713180519/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-04-15 11:28:50.197236 authentik_client-2024.2.2.post1713180519/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-04-15 11:28:50.197236 authentik_client-2024.2.2.post1713180519/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-04-15 11:28:50.201236 authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-04-15 11:28:50.205236 authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-04-15 11:28:50.205236 authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-04-15 11:28:50.209236 authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-04-15 11:28:50.213236 authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10563 2024-04-15 11:28:50.217236 authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-04-15 11:28:50.217236 authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-04-15 11:28:50.221236 authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-04-15 11:28:50.225236 authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-04-15 11:28:50.229236 authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-04-15 11:28:50.229236 authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     3131 2024-04-15 11:28:50.233236 authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_sync_status.py
+-rw-r--r--   0        0        0     4629 2024-04-15 11:28:50.241236 authentik_client-2024.2.2.post1713180519/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-04-15 11:28:50.245236 authentik_client-2024.2.2.post1713180519/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-04-15 11:28:50.249236 authentik_client-2024.2.2.post1713180519/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-04-15 11:28:50.249236 authentik_client-2024.2.2.post1713180519/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-04-15 11:28:50.253236 authentik_client-2024.2.2.post1713180519/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-04-15 11:28:50.257236 authentik_client-2024.2.2.post1713180519/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-04-15 11:28:50.257236 authentik_client-2024.2.2.post1713180519/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4931 2024-04-15 11:28:50.261236 authentik_client-2024.2.2.post1713180519/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     5058 2024-04-15 11:28:50.265236 authentik_client-2024.2.2.post1713180519/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-04-15 11:28:50.265236 authentik_client-2024.2.2.post1713180519/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-04-15 11:28:50.269236 authentik_client-2024.2.2.post1713180519/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     1492 2024-04-15 11:28:50.273236 authentik_client-2024.2.2.post1713180519/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-04-15 11:28:50.237236 authentik_client-2024.2.2.post1713180519/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-04-15 11:28:50.237236 authentik_client-2024.2.2.post1713180519/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-04-15 11:28:50.277237 authentik_client-2024.2.2.post1713180519/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-04-15 11:28:50.281237 authentik_client-2024.2.2.post1713180519/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-04-15 11:28:50.285237 authentik_client-2024.2.2.post1713180519/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-04-15 11:28:50.289237 authentik_client-2024.2.2.post1713180519/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-04-15 11:28:50.293237 authentik_client-2024.2.2.post1713180519/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-04-15 11:28:50.297237 authentik_client-2024.2.2.post1713180519/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-04-15 11:28:50.297237 authentik_client-2024.2.2.post1713180519/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-04-15 11:28:50.301237 authentik_client-2024.2.2.post1713180519/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-04-15 11:28:50.305237 authentik_client-2024.2.2.post1713180519/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-04-15 11:28:50.309237 authentik_client-2024.2.2.post1713180519/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-04-15 11:28:50.313237 authentik_client-2024.2.2.post1713180519/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-04-15 11:28:50.317237 authentik_client-2024.2.2.post1713180519/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-04-15 11:28:50.321237 authentik_client-2024.2.2.post1713180519/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-04-15 11:28:50.321237 authentik_client-2024.2.2.post1713180519/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     4463 2024-04-15 11:28:50.325237 authentik_client-2024.2.2.post1713180519/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     2934 2024-04-15 11:28:50.325237 authentik_client-2024.2.2.post1713180519/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4286 2024-04-15 11:28:50.329237 authentik_client-2024.2.2.post1713180519/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-04-15 11:28:50.329237 authentik_client-2024.2.2.post1713180519/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-04-15 11:28:50.337237 authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-04-15 11:28:50.341237 authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-04-15 11:28:50.341237 authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-04-15 11:28:50.345237 authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-04-15 11:28:50.349237 authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4802 2024-04-15 11:28:50.349237 authentik_client-2024.2.2.post1713180519/authentik_client/models/token.py
+-rw-r--r--   0        0        0     4198 2024-04-15 11:28:50.353237 authentik_client-2024.2.2.post1713180519/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4329 2024-04-15 11:28:50.357237 authentik_client-2024.2.2.post1713180519/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-04-15 11:28:50.361237 authentik_client-2024.2.2.post1713180519/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-04-15 11:28:50.361237 authentik_client-2024.2.2.post1713180519/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-04-15 11:28:50.333237 authentik_client-2024.2.2.post1713180519/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-04-15 11:28:50.337237 authentik_client-2024.2.2.post1713180519/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-04-15 11:28:50.365237 authentik_client-2024.2.2.post1713180519/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-04-15 11:28:50.369238 authentik_client-2024.2.2.post1713180519/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     2936 2024-04-15 11:28:50.369238 authentik_client-2024.2.2.post1713180519/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-04-15 11:28:50.373237 authentik_client-2024.2.2.post1713180519/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-04-15 11:28:50.373237 authentik_client-2024.2.2.post1713180519/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-04-15 11:28:50.377237 authentik_client-2024.2.2.post1713180519/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5226 2024-04-15 11:28:50.377237 authentik_client-2024.2.2.post1713180519/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-04-15 11:28:50.381238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-04-15 11:28:50.385238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3828 2024-04-15 11:28:50.389238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-04-15 11:28:50.389238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-04-15 11:28:50.393238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-15 11:28:50.397238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-04-15 11:28:50.397238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-04-15 11:28:50.401238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     4334 2024-04-15 11:28:50.405238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-04-15 11:28:50.409238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-04-15 11:28:50.413238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-04-15 11:28:50.413238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-04-15 11:28:50.417238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-04-15 11:28:50.421238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-04-15 11:28:50.425238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-04-15 11:28:50.425238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-04-15 11:28:50.429238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-04-15 11:28:50.433238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-04-15 11:28:50.437238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-04-15 11:28:50.437238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-04-15 11:28:50.441238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-04-15 11:28:50.445238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-04-15 11:28:50.449238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-04-15 11:28:50.453238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-04-15 11:28:50.457238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-04-15 11:28:50.457238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-04-15 11:28:50.461238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-04-15 11:28:50.465238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-04-15 11:28:50.465238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-04-15 11:28:50.469238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-04-15 11:28:50.469238 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-04-15 11:28:50.473239 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-04-15 11:28:50.473239 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-04-15 11:28:50.477239 authentik_client-2024.2.2.post1713180519/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-04-15 11:28:50.481238 authentik_client-2024.2.2.post1713180519/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-04-15 11:28:50.481238 authentik_client-2024.2.2.post1713180519/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3630 2024-04-15 11:28:50.485239 authentik_client-2024.2.2.post1713180519/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-04-15 11:28:50.485239 authentik_client-2024.2.2.post1713180519/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-04-15 11:28:50.489239 authentik_client-2024.2.2.post1713180519/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-04-15 11:28:50.493239 authentik_client-2024.2.2.post1713180519/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-04-15 11:28:50.493239 authentik_client-2024.2.2.post1713180519/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-04-15 11:28:51.681250 authentik_client-2024.2.2.post1713180519/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-04-15 11:28:51.689251 authentik_client-2024.2.2.post1713180519/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-04-15 11:28:51.681250 authentik_client-2024.2.2.post1713180519/pyproject.toml
+-rw-r--r--   0        0        0   141360 1970-01-01 00:00:00.000000 authentik_client-2024.2.2.post1713180519/PKG-INFO
```

### Comparing `authentik_client-2024.2.2.post1712922614/README.md` & `authentik_client-2024.2.2.post1713180519/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1712922614
+- Package version: 2024.2.2-1713180519
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -1330,15 +1330,14 @@
  - [UserAssignedObjectPermission](docs/UserAssignedObjectPermission.md)
  - [UserConsent](docs/UserConsent.md)
  - [UserCreationModeEnum](docs/UserCreationModeEnum.md)
  - [UserDeleteStage](docs/UserDeleteStage.md)
  - [UserDeleteStageRequest](docs/UserDeleteStageRequest.md)
  - [UserFieldsEnum](docs/UserFieldsEnum.md)
  - [UserGroup](docs/UserGroup.md)
- - [UserGroupRequest](docs/UserGroupRequest.md)
  - [UserLoginChallenge](docs/UserLoginChallenge.md)
  - [UserLoginChallengeResponseRequest](docs/UserLoginChallengeResponseRequest.md)
  - [UserLoginStage](docs/UserLoginStage.md)
  - [UserLoginStageRequest](docs/UserLoginStageRequest.md)
  - [UserLogoutStage](docs/UserLogoutStage.md)
  - [UserLogoutStageRequest](docs/UserLogoutStageRequest.md)
  - [UserMatchingModeEnum](docs/UserMatchingModeEnum.md)
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/__init__.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.2.2-1712922614"
+__version__ = "2024.2.2-1713180519"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
@@ -564,15 +564,14 @@
 from authentik_client.models.user_assigned_object_permission import UserAssignedObjectPermission
 from authentik_client.models.user_consent import UserConsent
 from authentik_client.models.user_creation_mode_enum import UserCreationModeEnum
 from authentik_client.models.user_delete_stage import UserDeleteStage
 from authentik_client.models.user_delete_stage_request import UserDeleteStageRequest
 from authentik_client.models.user_fields_enum import UserFieldsEnum
 from authentik_client.models.user_group import UserGroup
-from authentik_client.models.user_group_request import UserGroupRequest
 from authentik_client.models.user_login_challenge import UserLoginChallenge
 from authentik_client.models.user_login_challenge_response_request import UserLoginChallengeResponseRequest
 from authentik_client.models.user_login_stage import UserLoginStage
 from authentik_client.models.user_login_stage_request import UserLoginStageRequest
 from authentik_client.models.user_logout_stage import UserLogoutStage
 from authentik_client.models.user_logout_stage_request import UserLogoutStageRequest
 from authentik_client.models.user_matching_mode_enum import UserMatchingModeEnum
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/__init__.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/admin_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/authenticators_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/authenticators_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/core_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/core_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -7767,14 +7767,15 @@
 
 
 
     @validate_call
     def core_groups_list(
         self,
         attributes: Annotated[Optional[StrictStr], Field(description="Attributes")] = None,
+        include_users: Optional[StrictBool] = None,
         is_superuser: Optional[StrictBool] = None,
         members_by_pk: Optional[List[StrictInt]] = None,
         members_by_username: Annotated[Optional[List[StrictStr]], Field(description="Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.")] = None,
         name: Optional[StrictStr] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
@@ -7794,14 +7795,16 @@
     ) -> PaginatedGroupList:
         """core_groups_list
 
         Group Viewset
 
         :param attributes: Attributes
         :type attributes: str
+        :param include_users:
+        :type include_users: bool
         :param is_superuser:
         :type is_superuser: bool
         :param members_by_pk:
         :type members_by_pk: List[int]
         :param members_by_username: Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.
         :type members_by_username: List[str]
         :param name:
@@ -7834,14 +7837,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._core_groups_list_serialize(
             attributes=attributes,
+            include_users=include_users,
             is_superuser=is_superuser,
             members_by_pk=members_by_pk,
             members_by_username=members_by_username,
             name=name,
             ordering=ordering,
             page=page,
             page_size=page_size,
@@ -7868,14 +7872,15 @@
         ).data
 
 
     @validate_call
     def core_groups_list_with_http_info(
         self,
         attributes: Annotated[Optional[StrictStr], Field(description="Attributes")] = None,
+        include_users: Optional[StrictBool] = None,
         is_superuser: Optional[StrictBool] = None,
         members_by_pk: Optional[List[StrictInt]] = None,
         members_by_username: Annotated[Optional[List[StrictStr]], Field(description="Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.")] = None,
         name: Optional[StrictStr] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
@@ -7895,14 +7900,16 @@
     ) -> ApiResponse[PaginatedGroupList]:
         """core_groups_list
 
         Group Viewset
 
         :param attributes: Attributes
         :type attributes: str
+        :param include_users:
+        :type include_users: bool
         :param is_superuser:
         :type is_superuser: bool
         :param members_by_pk:
         :type members_by_pk: List[int]
         :param members_by_username: Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.
         :type members_by_username: List[str]
         :param name:
@@ -7935,14 +7942,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._core_groups_list_serialize(
             attributes=attributes,
+            include_users=include_users,
             is_superuser=is_superuser,
             members_by_pk=members_by_pk,
             members_by_username=members_by_username,
             name=name,
             ordering=ordering,
             page=page,
             page_size=page_size,
@@ -7969,14 +7977,15 @@
         )
 
 
     @validate_call
     def core_groups_list_without_preload_content(
         self,
         attributes: Annotated[Optional[StrictStr], Field(description="Attributes")] = None,
+        include_users: Optional[StrictBool] = None,
         is_superuser: Optional[StrictBool] = None,
         members_by_pk: Optional[List[StrictInt]] = None,
         members_by_username: Annotated[Optional[List[StrictStr]], Field(description="Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.")] = None,
         name: Optional[StrictStr] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
@@ -7996,14 +8005,16 @@
     ) -> RESTResponseType:
         """core_groups_list
 
         Group Viewset
 
         :param attributes: Attributes
         :type attributes: str
+        :param include_users:
+        :type include_users: bool
         :param is_superuser:
         :type is_superuser: bool
         :param members_by_pk:
         :type members_by_pk: List[int]
         :param members_by_username: Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.
         :type members_by_username: List[str]
         :param name:
@@ -8036,14 +8047,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._core_groups_list_serialize(
             attributes=attributes,
+            include_users=include_users,
             is_superuser=is_superuser,
             members_by_pk=members_by_pk,
             members_by_username=members_by_username,
             name=name,
             ordering=ordering,
             page=page,
             page_size=page_size,
@@ -8065,14 +8077,15 @@
         )
         return response_data.response
 
 
     def _core_groups_list_serialize(
         self,
         attributes,
+        include_users,
         is_superuser,
         members_by_pk,
         members_by_username,
         name,
         ordering,
         page,
         page_size,
@@ -8099,14 +8112,18 @@
 
         # process the path parameters
         # process the query parameters
         if attributes is not None:
             
             _query_params.append(('attributes', attributes))
             
+        if include_users is not None:
+            
+            _query_params.append(('include_users', include_users))
+            
         if is_superuser is not None:
             
             _query_params.append(('is_superuser', is_superuser))
             
         if members_by_pk is not None:
             
             _query_params.append(('members_by_pk', members_by_pk))
@@ -14718,14 +14735,15 @@
     @validate_call
     def core_users_list(
         self,
         attributes: Annotated[Optional[StrictStr], Field(description="Attributes")] = None,
         email: Optional[StrictStr] = None,
         groups_by_name: Optional[List[StrictStr]] = None,
         groups_by_pk: Optional[List[StrictStr]] = None,
+        include_groups: Optional[StrictBool] = None,
         is_active: Optional[StrictBool] = None,
         is_superuser: Optional[StrictBool] = None,
         name: Optional[StrictStr] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         path: Optional[StrictStr] = None,
@@ -14755,14 +14773,16 @@
         :type attributes: str
         :param email:
         :type email: str
         :param groups_by_name:
         :type groups_by_name: List[str]
         :param groups_by_pk:
         :type groups_by_pk: List[str]
+        :param include_groups:
+        :type include_groups: bool
         :param is_active:
         :type is_active: bool
         :param is_superuser:
         :type is_superuser: bool
         :param name:
         :type name: str
         :param ordering: Which field to use when ordering the results.
@@ -14806,14 +14826,15 @@
         """ # noqa: E501
 
         _param = self._core_users_list_serialize(
             attributes=attributes,
             email=email,
             groups_by_name=groups_by_name,
             groups_by_pk=groups_by_pk,
+            include_groups=include_groups,
             is_active=is_active,
             is_superuser=is_superuser,
             name=name,
             ordering=ordering,
             page=page,
             page_size=page_size,
             path=path,
@@ -14847,14 +14868,15 @@
     @validate_call
     def core_users_list_with_http_info(
         self,
         attributes: Annotated[Optional[StrictStr], Field(description="Attributes")] = None,
         email: Optional[StrictStr] = None,
         groups_by_name: Optional[List[StrictStr]] = None,
         groups_by_pk: Optional[List[StrictStr]] = None,
+        include_groups: Optional[StrictBool] = None,
         is_active: Optional[StrictBool] = None,
         is_superuser: Optional[StrictBool] = None,
         name: Optional[StrictStr] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         path: Optional[StrictStr] = None,
@@ -14884,14 +14906,16 @@
         :type attributes: str
         :param email:
         :type email: str
         :param groups_by_name:
         :type groups_by_name: List[str]
         :param groups_by_pk:
         :type groups_by_pk: List[str]
+        :param include_groups:
+        :type include_groups: bool
         :param is_active:
         :type is_active: bool
         :param is_superuser:
         :type is_superuser: bool
         :param name:
         :type name: str
         :param ordering: Which field to use when ordering the results.
@@ -14935,14 +14959,15 @@
         """ # noqa: E501
 
         _param = self._core_users_list_serialize(
             attributes=attributes,
             email=email,
             groups_by_name=groups_by_name,
             groups_by_pk=groups_by_pk,
+            include_groups=include_groups,
             is_active=is_active,
             is_superuser=is_superuser,
             name=name,
             ordering=ordering,
             page=page,
             page_size=page_size,
             path=path,
@@ -14976,14 +15001,15 @@
     @validate_call
     def core_users_list_without_preload_content(
         self,
         attributes: Annotated[Optional[StrictStr], Field(description="Attributes")] = None,
         email: Optional[StrictStr] = None,
         groups_by_name: Optional[List[StrictStr]] = None,
         groups_by_pk: Optional[List[StrictStr]] = None,
+        include_groups: Optional[StrictBool] = None,
         is_active: Optional[StrictBool] = None,
         is_superuser: Optional[StrictBool] = None,
         name: Optional[StrictStr] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         path: Optional[StrictStr] = None,
@@ -15013,14 +15039,16 @@
         :type attributes: str
         :param email:
         :type email: str
         :param groups_by_name:
         :type groups_by_name: List[str]
         :param groups_by_pk:
         :type groups_by_pk: List[str]
+        :param include_groups:
+        :type include_groups: bool
         :param is_active:
         :type is_active: bool
         :param is_superuser:
         :type is_superuser: bool
         :param name:
         :type name: str
         :param ordering: Which field to use when ordering the results.
@@ -15064,14 +15092,15 @@
         """ # noqa: E501
 
         _param = self._core_users_list_serialize(
             attributes=attributes,
             email=email,
             groups_by_name=groups_by_name,
             groups_by_pk=groups_by_pk,
+            include_groups=include_groups,
             is_active=is_active,
             is_superuser=is_superuser,
             name=name,
             ordering=ordering,
             page=page,
             page_size=page_size,
             path=path,
@@ -15100,14 +15129,15 @@
 
     def _core_users_list_serialize(
         self,
         attributes,
         email,
         groups_by_name,
         groups_by_pk,
+        include_groups,
         is_active,
         is_superuser,
         name,
         ordering,
         page,
         page_size,
         path,
@@ -15151,14 +15181,18 @@
             
             _query_params.append(('groups_by_name', groups_by_name))
             
         if groups_by_pk is not None:
             
             _query_params.append(('groups_by_pk', groups_by_pk))
             
+        if include_groups is not None:
+            
+            _query_params.append(('include_groups', include_groups))
+            
         if is_active is not None:
             
             _query_params.append(('is_active', is_active))
             
         if is_superuser is not None:
             
             _query_params.append(('is_superuser', is_superuser))
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/crypto_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/crypto_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/enterprise_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/enterprise_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/events_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/flows_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/flows_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/managed_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/managed_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/oauth2_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/oauth2_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/outposts_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/outposts_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/policies_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/propertymappings_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/providers_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/providers_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/rac_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/rac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/rbac_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/rbac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/root_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/root_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/schema_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/sources_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/stages_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/stages_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api/tenants_api.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api/tenants_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api_client.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.2.2-1712922614/python'
+        self.user_agent = 'OpenAPI-Generator/2024.2.2-1713180519/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/api_response.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/configuration.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2024.2.2\n"\
-               "SDK Package Version: 2024.2.2-1712922614".\
+               "SDK Package Version: 2024.2.2-1713180519".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/exceptions.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/__init__.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,15 +528,14 @@
 from authentik_client.models.user_assigned_object_permission import UserAssignedObjectPermission
 from authentik_client.models.user_consent import UserConsent
 from authentik_client.models.user_creation_mode_enum import UserCreationModeEnum
 from authentik_client.models.user_delete_stage import UserDeleteStage
 from authentik_client.models.user_delete_stage_request import UserDeleteStageRequest
 from authentik_client.models.user_fields_enum import UserFieldsEnum
 from authentik_client.models.user_group import UserGroup
-from authentik_client.models.user_group_request import UserGroupRequest
 from authentik_client.models.user_login_challenge import UserLoginChallenge
 from authentik_client.models.user_login_challenge_response_request import UserLoginChallengeResponseRequest
 from authentik_client.models.user_login_stage import UserLoginStage
 from authentik_client.models.user_login_stage_request import UserLoginStageRequest
 from authentik_client.models.user_logout_stage import UserLogoutStage
 from authentik_client.models.user_logout_stage_request import UserLogoutStageRequest
 from authentik_client.models.user_matching_mode_enum import UserMatchingModeEnum
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/access_denied_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/app.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/app.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/app_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/app_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/apple_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/apple_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/application.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/application.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/application_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/auth_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/auth_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_asn.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authentication_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authentication_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_attachment_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_sms_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_sms_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_static_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_static_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_totp_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_totp_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_validate_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_validation_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_web_authn_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/autosubmit_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/backends_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/backends_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/binding_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_file.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/blueprint_file.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/blueprint_instance.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/brand.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/brand_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/cache.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/cache.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/capabilities_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/captcha_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/captcha_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/captcha_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_data.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/certificate_data.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/certificate_generation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/certificate_key_pair.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/challenge_choices.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/challenge_choices.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/challenge_types.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/client_type_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/client_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/config.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/connection_token.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/connection_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/connection_token_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_permission.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_stage_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/contextual_flow_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/coordinate.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/coordinate.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/current_brand.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/current_brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/denied_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/deny_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/deny_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/device.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/device_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/device_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/device_challenge_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/device_classes_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/digest_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/digits_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/digits_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/docker_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/domain.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/domain.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/domain_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_policy.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/duo_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/duo_device_enrollment_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/duo_response_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/email_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/email_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/email_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/email_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/email_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/email_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/endpoint.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/endpoint_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/error_detail.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/error_reporting_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/event.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_actions.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/event_actions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/event_matcher_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/event_top_per_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/expiring_base_grant_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/expression_policy.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/expression_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/extra_role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/extra_user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/file_path_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/file_path_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_designation_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_diagram.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_diagram.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_error_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_import_result.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_import_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_inspection.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_inspection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_inspector_plan.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_set.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_set.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_set_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_stage_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/footer_link.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/footer_link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/generic_error.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/generic_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/geoip_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/group.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/group_member.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/group_member_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/group_member_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/group_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/identification_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/identification_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/identification_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/install_id.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/install_id.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/intent_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/intent_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/invalid_response_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/invitation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/invitation_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/issuer_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/kubernetes_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_debug.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_debug.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_provider.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_source.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldap_sync_status.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldap_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ldapapi_access_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/license.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/license.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/license_forecast.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/license_forecast.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/license_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/license_summary.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/license_summary.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/link.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/log_event.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/log_event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/log_level_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/log_level_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/login_challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/login_metrics.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/login_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/login_source.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/login_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/metadata.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/model_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/model_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/model_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/name_id_policy_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/network_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/not_configured_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_rule.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_rule.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_transport.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_transport_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_transport_test.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_webhook_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth2_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_source.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/open_id_connect_configuration.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost_default_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_health.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost_health.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/outpost_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_authenticator_web_authn_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_brand_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_connection_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_consent_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_deny_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_domain_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_duo_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_email_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_endpoint_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_event_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_expression_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_flow_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_identification_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_invitation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_ldap_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_license_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_notification_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_notification_rule_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_notification_transport_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_outpost_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_password_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_password_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_plex_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_policy_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_prompt_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_rac_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_radius_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_reputation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_role_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_saml_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_saml_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_scim_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_sms_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_source_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_static_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_system_task_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_tenant_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_token_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_totp_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_consent_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/paginated_web_authn_device_type_list.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/pagination.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/pagination.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/password_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/password_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/password_expiry_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_policy.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/password_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/password_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/password_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_application_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_authenticator_web_authn_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_event_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_group_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_license_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_license_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_role_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_token_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/patched_web_authn_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/permission.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_authentication_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_source_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/plex_token_redeem_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_binding.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_engine_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_test_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_test_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/policy_test_result.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/policy_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/prompt_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/property_mapping_preview.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/property_mapping_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/protocol_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/protocol_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/provider_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/provider_model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/provider_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_mode.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/proxy_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/proxy_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_provider.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/proxy_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/rac_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_provider.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/rac_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/radius_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_provider.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/radius_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/redirect_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/reputation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation_policy.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/reputation_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/resident_key_requirement_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/role.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/role.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/role_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/role_object_permission.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/role_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_metadata.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_provider.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_source.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/saml_source_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_mapping.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_provider.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/scim_sync_status.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/scim_sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/scope_mapping.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/scope_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/selectable_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/selectable_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/service_connection_state.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/service_connection_state.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/session_user.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/session_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/settings.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/settings.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/settings_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/severity_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/severity_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/shell_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/shell_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/signature_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/sms_device.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/sms_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/sms_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/source.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/source_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/source_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/source_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/source_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/source_type.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/sp_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/stage_prompt.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/stage_prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/static_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_token.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/static_device_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/static_device_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/sub_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/system_info.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/system_info_runtime.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/system_task.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/system_task.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/system_task_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant_recovery_key_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/tenant_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/token.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/token_model.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/token_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/token_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/token_set_key_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/token_view.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/token_view.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/totp_device.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/totp_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/totp_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/transaction_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/transaction_application_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/type_create.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/type_create.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/ui_theme_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/used_by.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/used_by.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/used_by_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_account_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_account_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_consent.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_consent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_creation_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_delete_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_fields_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_group.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_group_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_service_account_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
+from datetime import datetime
+from pydantic import BaseModel, ConfigDict, Field, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserGroupRequest(BaseModel):
+class UserServiceAccountRequest(BaseModel):
     """
-    Simplified Group Serializer for user's groups
+    UserServiceAccountRequest
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True, max_length=80)]
-    is_superuser: Optional[StrictBool] = Field(default=None, description="Users added to this group will be superusers.")
-    parent: Optional[StrictStr] = None
-    attributes: Optional[Dict[str, Any]] = None
-    __properties: ClassVar[List[str]] = ["name", "is_superuser", "parent", "attributes"]
+    name: Annotated[str, Field(min_length=1, strict=True)]
+    create_group: Optional[StrictBool] = False
+    expiring: Optional[StrictBool] = True
+    expires: Optional[datetime] = Field(default=None, description="If not provided, valid for 360 days")
+    __properties: ClassVar[List[str]] = ["name", "create_group", "expiring", "expires"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -48,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserGroupRequest from a JSON string"""
+        """Create an instance of UserServiceAccountRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,32 +70,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if parent (nullable) is None
-        # and model_fields_set contains the field
-        if self.parent is None and "parent" in self.model_fields_set:
-            _dict['parent'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserGroupRequest from a dict"""
+        """Create an instance of UserServiceAccountRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
-            "is_superuser": obj.get("is_superuser"),
-            "parent": obj.get("parent"),
-            "attributes": obj.get("attributes")
+            "create_group": obj.get("create_group") if obj.get("create_group") is not None else False,
+            "expiring": obj.get("expiring") if obj.get("expiring") is not None else True,
+            "expires": obj.get("expires")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_login_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_login_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_logout_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_matching_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_metrics.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_o_auth_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_object_permission.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_password_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_path.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_path.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_saml_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_self.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_self.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_self_groups.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_self_groups.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/web_authn_device_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,30 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, ConfigDict, Field, StrictBool
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, Field
+from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserServiceAccountRequest(BaseModel):
+class WebAuthnDeviceRequest(BaseModel):
     """
-    UserServiceAccountRequest
+    Serializer for WebAuthn authenticator devices
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True)]
-    create_group: Optional[StrictBool] = False
-    expiring: Optional[StrictBool] = True
-    expires: Optional[datetime] = Field(default=None, description="If not provided, valid for 360 days")
-    __properties: ClassVar[List[str]] = ["name", "create_group", "expiring", "expires"]
+    name: Annotated[str, Field(min_length=1, strict=True, max_length=200)]
+    __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserServiceAccountRequest from a JSON string"""
+        """Create an instance of WebAuthnDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,23 +70,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserServiceAccountRequest from a dict"""
+        """Create an instance of WebAuthnDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "create_group": obj.get("create_group") if obj.get("create_group") is not None else False,
-            "expiring": obj.get("expiring") if obj.get("expiring") is not None else True,
-            "expires": obj.get("expires")
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_service_account_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_setting.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_setting.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_source_connection.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_type_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_verification_enum.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_verification_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_write_stage.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_write_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/user_write_stage_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/validation_error.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/version.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/version.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/web_authn_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/web_authn_device_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class WebAuthnDeviceRequest(BaseModel):
+class WebAuthnDeviceType(BaseModel):
     """
-    Serializer for WebAuthn authenticator devices
+    WebAuthnDeviceType Serializer
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True, max_length=200)]
-    __properties: ClassVar[List[str]] = ["name"]
+    aaguid: StrictStr
+    description: StrictStr
+    __properties: ClassVar[List[str]] = ["aaguid", "description"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceRequest from a JSON string"""
+        """Create an instance of WebAuthnDeviceType from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceRequest from a dict"""
+        """Create an instance of WebAuthnDeviceType from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name")
+            "aaguid": obj.get("aaguid"),
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_type.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/web_authn_device_type_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class WebAuthnDeviceType(BaseModel):
+class WebAuthnDeviceTypeRequest(BaseModel):
     """
     WebAuthnDeviceType Serializer
     """ # noqa: E501
     aaguid: StrictStr
-    description: StrictStr
+    description: Annotated[str, Field(min_length=1, strict=True)]
     __properties: ClassVar[List[str]] = ["aaguid", "description"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -45,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceType from a JSON string"""
+        """Create an instance of WebAuthnDeviceTypeRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +71,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceType from a dict"""
+        """Create an instance of WebAuthnDeviceTypeRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/models/web_authn_device_type_request.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/models/workers.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
-from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class WebAuthnDeviceTypeRequest(BaseModel):
+class Workers(BaseModel):
     """
-    WebAuthnDeviceType Serializer
+    Workers
     """ # noqa: E501
-    aaguid: StrictStr
-    description: Annotated[str, Field(min_length=1, strict=True)]
-    __properties: ClassVar[List[str]] = ["aaguid", "description"]
+    count: StrictInt
+    __properties: ClassVar[List[str]] = ["count"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceTypeRequest from a JSON string"""
+        """Create an instance of Workers from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of WebAuthnDeviceTypeRequest from a dict"""
+        """Create an instance of Workers from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "aaguid": obj.get("aaguid"),
-            "description": obj.get("description")
+            "count": obj.get("count")
         })
         return _obj
```

### Comparing `authentik_client-2024.2.2.post1712922614/authentik_client/rest.py` & `authentik_client-2024.2.2.post1713180519/authentik_client/rest.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.2.2.post1712922614/pyproject.toml` & `authentik_client-2024.2.2.post1713180519/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.2.2-1712922614"
+version = "2024.2.2-1713180519"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.2.2.post1712922614/PKG-INFO` & `authentik_client-2024.2.2.post1713180519/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.2.2.post1712922614
+Version: 2024.2.2.post1713180519
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -25,15 +25,15 @@
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.2.2
-- Package version: 2024.2.2-1712922614
+- Package version: 2024.2.2-1713180519
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -1355,15 +1355,14 @@
  - [UserAssignedObjectPermission](docs/UserAssignedObjectPermission.md)
  - [UserConsent](docs/UserConsent.md)
  - [UserCreationModeEnum](docs/UserCreationModeEnum.md)
  - [UserDeleteStage](docs/UserDeleteStage.md)
  - [UserDeleteStageRequest](docs/UserDeleteStageRequest.md)
  - [UserFieldsEnum](docs/UserFieldsEnum.md)
  - [UserGroup](docs/UserGroup.md)
- - [UserGroupRequest](docs/UserGroupRequest.md)
  - [UserLoginChallenge](docs/UserLoginChallenge.md)
  - [UserLoginChallengeResponseRequest](docs/UserLoginChallengeResponseRequest.md)
  - [UserLoginStage](docs/UserLoginStage.md)
  - [UserLoginStageRequest](docs/UserLoginStageRequest.md)
  - [UserLogoutStage](docs/UserLogoutStage.md)
  - [UserLogoutStageRequest](docs/UserLogoutStageRequest.md)
  - [UserMatchingModeEnum](docs/UserMatchingModeEnum.md)
```

