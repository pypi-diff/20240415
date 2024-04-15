# Comparing `tmp/refinitiv-data-1.6.0.tar.gz` & `tmp/refinitiv-data-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refinitiv-data-1.6.0.tar", last modified: Wed Feb  7 12:31:00 2024, max compression
+gzip compressed data, was "refinitiv-data-1.6.1.tar", last modified: Thu Apr 11 09:08:52 2024, max compression
```

## Comparing `refinitiv-data-1.6.0.tar` & `refinitiv-data-1.6.1.tar`

### file list

```diff
@@ -1,1066 +1,1066 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.736445 refinitiv-data-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)    21080 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11358 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10325 2024-02-07 12:31:00.736445 refinitiv-data-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9061 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.480445 refinitiv-data-1.6.0/changes/
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/changes/template.jinja
--rw-rw-rw-   0 root         (0) root         (0)    22005 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.480445 refinitiv-data-1.6.0/refinitiv/
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.484445 refinitiv-data-1.6.0/refinitiv/data/
--rw-rw-rw-   0 root         (0) root         (0)     1508 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.488445 refinitiv-data-1.6.0/refinitiv/data/_access_layer/
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5249 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_containers.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_data_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    12207 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4849 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_history_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_history_df_builder_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1500 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_intervals_consts.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_mixed_streams.py
--rw-rw-rw-   0 root         (0) root         (0)     5066 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_ohlc_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    12101 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_pricing_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)     5290 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_recording_control.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/_stream_update_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.492445 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2982 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_adc_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_adc_rdp_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1979 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_adc_udf_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_context.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_context_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_cust_inst_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_cust_inst_rdp_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_cust_inst_udf_context.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_hp_and_cust_inst_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_hp_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.492445 refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2483 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_add_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     2504 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_count_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     3622 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_date_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)     4581 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_holidays.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_is_working_day.py
--rw-rw-rw-   0 root         (0) root         (0)     4948 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/get_data_func.py
--rw-rw-rw-   0 root         (0) root         (0)     9025 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/get_history_func.py
--rw-rw-rw-   0 root         (0) root         (0)     3658 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/get_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.492445 refinitiv-data-1.6.0/refinitiv/data/_access_layer/news/
--rw-rw-rw-   0 root         (0) root         (0)      280 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/news/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/news/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     3577 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_access_layer/session.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)    16652 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_config_defaults.py
--rw-rw-rw-   0 root         (0) root         (0)    15985 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_configure.py
--rw-rw-rw-   0 root         (0) root         (0)     3968 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_content_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.492445 refinitiv-data-1.6.0/refinitiv/data/_core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 12:30:11.000000 refinitiv-data-1.6.0/refinitiv/data/_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/log_reporter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.500445 refinitiv-data-1.6.0/refinitiv/data/_core/session/
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      245 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_dacs_params.py
--rw-rw-rw-   0 root         (0) root         (0)     3967 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_default_session_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5854 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_desktop_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_listeners.py
--rw-rw-rw-   0 root         (0) root         (0)    12061 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_platform_session.py
--rw-rw-rw-   0 root         (0) root         (0)    11845 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_retry_transport.py
--rw-rw-rw-   0 root         (0) root         (0)    16872 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_session_cxn_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_session_cxn_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2472 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_session_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    10238 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_session_provider.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_session_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/_user_uuid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.504445 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/
--rw-rw-rw-   0 root         (0) root         (0)      360 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3309 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_access_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)    10920 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_auth_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_auth_manager_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_grant.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_grant_client_credentials.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_grant_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1956 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_grant_password.py
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_null_grant.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_ping_access_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_ping_auth_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_ping_refresh_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_ping_token_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3911 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_refresh_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_sts_access_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_sts_auth_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      373 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_sts_refresh_token_updater.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_sts_token_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_token_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3990 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_updater.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/revoke_token.py
--rw-rw-rw-   0 root         (0) root         (0)    10876 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/connection.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/event.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/event_code.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/global_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    13648 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/http_service.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/null_session.py
--rw-rw-rw-   0 root         (0) root         (0)     4110 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/proxy_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1214 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_core/session/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.504445 refinitiv-data-1.6.0/refinitiv/data/_external_libraries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 12:30:11.000000 refinitiv-data-1.6.0/refinitiv/data/_external_libraries/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.504445 refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    26229 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11913 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     7238 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/configuration_set.py
--rw-rw-rw-   0 root         (0) root         (0)     5845 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_listener.py
--rw-rw-rw-   0 root         (0) root         (0)    13060 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_log.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_open_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.512445 refinitiv-data-1.6.0/refinitiv/data/_tools/
--rw-rw-rw-   0 root         (0) root         (0)     5386 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13809 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_common.py
--rw-rw-rw-   0 root         (0) root         (0)     1281 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     6337 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_dataframe.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_datetime.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_debug.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_delays.py
--rw-rw-rw-   0 root         (0) root         (0)     6678 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_lazy_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_params.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_patterns.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_repr.py
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_specification.py
--rw-rw-rw-   0 root         (0) root         (0)     2600 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5236 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_tools/templates.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/_types.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-02-07 12:30:59.000000 refinitiv-data-1.6.0/refinitiv/data/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.516445 refinitiv-data-1.6.0/refinitiv/data/content/
--rw-rw-rw-   0 root         (0) root         (0)     2433 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_content_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1195 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_content_data_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_content_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4170 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_content_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_content_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_df_build_type.py
--rw-rw-rw-   0 root         (0) root         (0)    18779 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     8645 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_df_builder_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    18438 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_entire_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_error_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_events.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_get_adc_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_historical_content_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     6441 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_historical_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     7267 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_historical_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_historical_raw_transf.py
--rw-rw-rw-   0 root         (0) root         (0)     3244 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_historical_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3064 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_intervals.py
--rw-rw-rw-   0 root         (0) root         (0)     6076 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     3945 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_states.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_universe_content_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_universe_stream.py
--rw-rw-rw-   0 root         (0) root         (0)    20880 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/_universe_streams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.524445 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14624 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2178 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_events.py
--rw-rw-rw-   0 root         (0) root         (0)     6121 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_instrument_class.py
--rw-rw-rw-   0 root         (0) root         (0)    12895 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py
--rw-rw-rw-   0 root         (0) root         (0)     6208 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_manage.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_search.py
--rw-rw-rw-   0 root         (0) root         (0)     8399 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_stream_facade.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_summaries.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/events.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/manage.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/search.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/summaries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.524445 refinitiv-data-1.6.0/refinitiv/data/content/esg/
--rw-rw-rw-   0 root         (0) root         (0)      295 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1470 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/_base_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/_basic_overview_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1152 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/_esg_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/_full_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/_full_scores_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/_standard_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1652 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/_standard_scores_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/_universe_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/basic_overview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.528445 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3850 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)     9731 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_db_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1805 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7363 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_file_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3243 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_package_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_package_manager_facade.py
--rw-rw-rw-   0 root         (0) root         (0)     2552 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/full_measures.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/full_scores.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/standard_measures.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/standard_scores.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/esg/universe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.528445 refinitiv-data-1.6.0/refinitiv/data/content/estimates/
--rw-rw-rw-   0 root         (0) root         (0)     1093 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/_enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.528445 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2163 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals/annual.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals/interim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.532445 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals_kpi/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals_kpi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1777 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1781 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals_kpi/annual.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals_kpi/interim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.536445 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2134 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2287 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2302 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2293 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2138 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2178 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/annual.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_non_periodic_measures.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_annual.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_interim.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/historical_snapshots_recommendations.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/interim.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/non_periodic_measures.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/recommendations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.536445 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1759 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/annual.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/historical_snapshots_kpi.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/interim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.540445 refinitiv-data-1.6.0/refinitiv/data/content/filings/
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/_feed_name.py
--rw-rw-rw-   0 root         (0) root         (0)     4876 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/_filing_query.py
--rw-rw-rw-   0 root         (0) root         (0)    20068 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/_retrieval_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/_retrieval_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8227 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/_search_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4699 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/_search_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/_search_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/retrieval.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/filings/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.540445 refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4031 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_content_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2041 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py
--rw-rw-rw-   0 root         (0) root         (0)      821 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    11008 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2693 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_response_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.544445 refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3077 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     3067 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_events_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3628 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3593 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_summaries_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/events.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/summaries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.544445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10741 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_content_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)     1416 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_content_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.544445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 12:30:11.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.544445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.548445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py
--rw-rw-rw-   0 root         (0) root         (0)    11538 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    28231 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2919 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.556445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_basis_spline_smooth_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calendar_adjustment.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calibration_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py
--rw-rw-rw-   0 root         (0) root         (0)     8933 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_issuer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_price_side.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating_scale_source.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_reference_entity_type.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_seniority.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.556445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.560445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4482 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     5158 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.560445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_risk_type.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_constituent_override_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_type.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_unit.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py
--rw-rw-rw-   0 root         (0) root         (0)     5472 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5868 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2470 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)     3907 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     3908 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     3719 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     7749 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3908 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     6759 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     4464 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py
--rw-rw-rw-   0 root         (0) root         (0)      483 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.564445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      799 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1236 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py
--rw-rw-rw-   0 root         (0) root         (0)     3593 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.568445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3767 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.568445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.568445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_quotation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_standard_turn_period.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py
--rw-rw-rw-   0 root         (0) root         (0)     2176 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py
--rw-rw-rw-   0 root         (0) root         (0)     2171 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py
--rw-rw-rw-   0 root         (0) root         (0)     3621 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2568 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.568445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7044 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2871 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.568445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8798 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.568445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.572445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_risk_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.572445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3353 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.588445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/
--rw-rw-rw-   0 root         (0) root         (0)     3302 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_adjust_interest_to_payment_date.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_american_monte_carlo_method.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_amortization_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_amortization_type.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_average_type.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_axis.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_barrier_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_barrier_style.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_barrier_type.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_benchmark_yield_selection_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_business_day_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_buy_sell.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_calibration_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_call_put.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_cds_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_credit_spread_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_date_moving_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_dates_calendars_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_day_count_basis.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_day_of_week.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_direction.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_discounting_type.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_dividend_extrapolation.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_dividend_type.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_doc_clause.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_double_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_end_of_month_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_equity_dividend_type.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_eti_input_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_exercise_schedule_type.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_exercise_style.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_extrapolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_fixing_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_format.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_forward_compute_method.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_forward_extrapolation.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_funding_spread_method.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_fx_binary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_fx_cross_type.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_fx_leg_type.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_fx_volatility_model.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_holiday_outupts.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_implied_deposit_date_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_in_or_out.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_index_average_method.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_index_compounding_method.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_integration_method.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_method.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_type.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_index_observation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_index_reset_type.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_index_spread_compounding_method.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_inflation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_input_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_interest_calculation_convention.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_interest_type.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_interpolation_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_local_volatility_method.py
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_method.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_notional_exchange.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_numeraire_type.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_option_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_period_type.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_premium_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_price_side.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_pricing_model_type.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_projected_index_calculation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_redemption_date_type.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_repo_curve_type.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_risk_type.py
--rw-rw-rw-   0 root         (0) root         (0)      308 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_rounding.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_rounding_type.py
--rw-rw-rw-   0 root         (0) root         (0)      741 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_seniority.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_stub_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_swaption_settlement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_swaption_type.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_swaption_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_tenor_reference_date.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_time_stamp.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_underlying_type.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_up_or_down.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_vol_type.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_volatility_adjustment_type.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_volatility_model.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_volatility_term_structure_type.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_volatility_type.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_yield_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.592445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/
--rw-rw-rw-   0 root         (0) root         (0)      614 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_amortization_item.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_barrier_definition_element.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_basket_item.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_bid_ask_mid.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_day_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     1098 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_fx_point.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_input_flow.py
--rw-rw-rw-   0 root         (0) root         (0)     1170 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_interpolation_weight.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_numerical_method.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_payout_scaling.py
--rw-rw-rw-   0 root         (0) root         (0)      761 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_pde_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     4761 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_object_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1342 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_param_item.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/_serializable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.592445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.592445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_bond_curves/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_bond_curves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.592445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2740 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.596445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_arg_enums.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_base_data_class.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_request_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.596445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.596445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/
--rw-rw-rw-   0 root         (0) root         (0)     2037 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7353 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    11268 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py
--rw-rw-rw-   0 root         (0) root         (0)     4933 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/manage.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.596445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5917 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2936 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/search.py
--rw-rw-rw-   0 root         (0) root         (0)    21252 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_curves_builder_df.py
--rw-rw-rw-   0 root         (0) root         (0)    10724 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_curves_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.600445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_calendar_adjustment.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_compounding_type.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_constituent_override_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_forward_curves_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_instrument_type.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_main_constituent_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_market_data_access_denied_fallback.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_swap_price_side.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_zc_curves_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      600 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_zc_interpolation_mode.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.604445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_constituents.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_convexity.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_curve.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_curve_point.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     7236 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_interest_rate_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_par_rate_shift.py
--rw-rw-rw-   0 root         (0) root         (0)     1330 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_shift_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_step.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_turn.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_valuation_time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.604445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/
--rw-rw-rw-   0 root         (0) root         (0)     1005 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6572 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_forward_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1979 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_forward_curve_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)     5452 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_swap_zc_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    10427 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_swap_zc_curve_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.604445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      178 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5209 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4807 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_zc_curve_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_zc_curve_definition_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.608445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/
--rw-rw-rw-   0 root         (0) root         (0)     1307 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     6765 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    10381 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_request_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.608445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1443 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/_response_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.608445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2066 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     9999 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.608445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8258 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     1845 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.608445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6926 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.612445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7249 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py
--rw-rw-rw-   0 root         (0) root         (0)     3424 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.612445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6908 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.616445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_base_financial_contracts_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_base_option_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8306 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     3863 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_events.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1222 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     3267 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.616445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/bond/
--rw-rw-rw-   0 root         (0) root         (0)     1524 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7306 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    45147 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    15065 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.620445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/
--rw-rw-rw-   0 root         (0) root         (0)     1152 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7607 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4443 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    12843 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.620445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/
--rw-rw-rw-   0 root         (0) root         (0)      678 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3091 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     7423 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     6225 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4659 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.620445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6659 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3966 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     6013 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.624445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/
--rw-rw-rw-   0 root         (0) root         (0)     1379 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1144 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_cbbc_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     6096 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_double_barriers_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4118 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_eti_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_fixing_info.py
--rw-rw-rw-   0 root         (0) root         (0)     9038 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_underlying_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.628445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/
--rw-rw-rw-   0 root         (0) root         (0)     1894 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_average_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2153 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8350 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1376 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_barrier_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_barrier_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2087 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_binary_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_dual_currency_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_forward_start.py
--rw-rw-rw-   0 root         (0) root         (0)     5203 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_fx_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8176 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      589 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_underlying_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.632445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/
--rw-rw-rw-   0 root         (0) root         (0)     2131 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10119 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_eti_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1736 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4838 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    14985 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_underlying_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.632445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6187 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2728 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2059 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py
--rw-rw-rw-   0 root         (0) root         (0)     2939 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.632445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    18947 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5508 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.636445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/
--rw-rw-rw-   0 root         (0) root         (0)     1361 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.636445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/
--rw-rw-rw-   0 root         (0) root         (0)      375 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7572 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2803 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.640445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/
--rw-rw-rw-   0 root         (0) root         (0)      362 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      739 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.640445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_enums/
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_enums/_calibration_type.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_enums/_moneyness_type.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_enums/_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_enums/_strike_type.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_enums/_volatility_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.644445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/
--rw-rw-rw-   0 root         (0) root         (0)      379 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_maturity_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_moneyness_weight.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_strike_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_strike_filter_range.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_surface.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_surface_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     3361 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_surface_output.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_surface_point.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_volatility_surface_point.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_surface_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11035 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_surfaces_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.644445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/
--rw-rw-rw-   0 root         (0) root         (0)      703 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/_cap_surface_request_item.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/_i_ir_vol_model_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5576 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/_i_ir_vol_model_pricing_parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.648445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2870 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1812 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5106 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_request_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.648445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2921 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_fx_statistics_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7238 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_request_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.652445 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/
--rw-rw-rw-   0 root         (0) root         (0)      794 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3636 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     7968 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/_swaption_calculation_params.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/_swaption_surface_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1243 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/_swaption_surface_request_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.652445 refinitiv-data-1.6.0/refinitiv/data/content/news/
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/_news_data_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)     2425 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/_urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.656445 refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3248 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4959 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/_sort_order.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.656445 refinitiv-data-1.6.0/refinitiv/data/content/news/images/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/images/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3503 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/images/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1383 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/images/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2821 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/images/_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.656445 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_image_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1267 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.660445 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/hierarchy/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/hierarchy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/hierarchy/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/hierarchy/_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.660445 refinitiv-data-1.6.0/refinitiv/data/content/news/story/
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/story/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/story/_data.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/story/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/story/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/story/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/story/_response.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/story/_response_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.664445 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/_top_news_headline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.664445 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1290 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/_subcategory.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/_top_news_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.664445 refinitiv-data-1.6.0/refinitiv/data/content/ownership/
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/_org_info_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3955 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/_ownership_data_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.668445 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2420 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2117 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_investors_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3273 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/breakdown.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/concentration.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/investors.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/recent_activity.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/shareholders_history_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/shareholders_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/top_n_concentration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.672445 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_breakdown_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1759 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_holdings_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_investors_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_recent_activity_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3185 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1933 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/breakdown.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/concentration.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/holdings.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/investors.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/recent_activity.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/shareholders_history_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/shareholders_report.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/top_n_concentration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.676445 refinitiv-data-1.6.0/refinitiv/data/content/ownership/insider/
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/insider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3226 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/insider/_transaction_report_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/insider/shareholders_report.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/insider/transaction_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.676445 refinitiv-data-1.6.0/refinitiv/data/content/ownership/investor/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/investor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/investor/_holdings_definition.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/investor/holdings.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/ownership/org_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.676445 refinitiv-data-1.6.0/refinitiv/data/content/pricing/
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3412 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5253 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/_pricing_content_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    17614 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.680445 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8116 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_chain_record.py
--rw-rw-rw-   0 root         (0) root         (0)     1756 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_chains_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4119 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    55563 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_display_template.py
--rw-rw-rw-   0 root         (0) root         (0)     1451 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_events.py
--rw-rw-rw-   0 root         (0) root         (0)     2862 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     8874 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     4193 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.680445 refinitiv-data-1.6.0/refinitiv/data/content/search/
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11894 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/search/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4241 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/search/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2021 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/search/_lookup_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/search/_metadata_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/search/_views.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/search/lookup.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/search/metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.684445 refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/
--rw-rw-rw-   0 root         (0) root         (0)      483 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2824 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_asset_class.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_asset_state.py
--rw-rw-rw-   0 root         (0) root         (0)     4444 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_country_code.py
--rw-rw-rw-   0 root         (0) root         (0)     7531 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_symbol_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.684445 refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/
--rw-rw-rw-   0 root         (0) root         (0)      453 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3723 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_events.py
--rw-rw-rw-   0 root         (0) root         (0)     2382 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     3839 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)    10744 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_stream_facade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.688445 refinitiv-data-1.6.0/refinitiv/data/delivery/
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.692445 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_api_type.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_data_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3236 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    26471 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_data_provider_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     6943 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_data_provider_layer.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_data_type.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_endpoint_data.py
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_endpoint_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     5668 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_endpoint_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2091 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_parsed_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_raw_data_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5910 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_request_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2584 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_response_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3617 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_validators.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_dictionary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.704445 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/
--rw-rw-rw-   0 root         (0) root         (0)     1011 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6337 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_basestream.py
--rw-rw-rw-   0 root         (0) root         (0)     5340 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_contrib_funcs.py
--rw-rw-rw-   0 root         (0) root         (0)     2740 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_contrib_response.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_contrib_type.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_dictionary_stream.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_off_stream_contrib_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     3532 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_offstream.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_omm_stream.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_protocol_type.py
--rw-rw-rw-   0 root         (0) root         (0)     4253 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_rdp_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     4490 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)    10072 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream_cxn_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5051 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11954 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     9279 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_validator_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.708445 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/
--rw-rw-rw-   0 root         (0) root         (0)      715 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_cxn_events.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_cxn_listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     3991 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_events.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_events_type.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_offstream_cxn_listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     6954 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_omm_cxn_listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_rdp_cxn_listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     6005 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_stream_events.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/message_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.708445 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      494 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14672 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_dictionary_type.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_field_description.py
--rw-rw-rw-   0 root         (0) root         (0)     6746 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     9811 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    16057 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/omm_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     8053 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/omm_stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2649 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/omm_stream_definition.py
--rw-rw-rw-   0 root         (0) root         (0)    10626 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rdp_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     3504 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rdp_stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2374 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rdp_stream_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.712445 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rwf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 12:30:11.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rwf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rwf/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     5310 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rwf/ema.py
--rw-rw-rw-   0 root         (0) root         (0)     9550 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rwf/socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.712445 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/states/
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/states/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3673 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/states/_basestream_states.py
--rw-rw-rw-   0 root         (0) root         (0)     3706 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/states/_omm_states.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/states/_stream_states.py
--rw-rw-rw-   0 root         (0) root         (0)     4075 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/stream_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    17098 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/stream_connection.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/stream_cxn_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.712445 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/ws/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 12:30:11.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/ws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/ws/ws_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.716445 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/
--rw-rw-rw-   0 root         (0) root         (0)      824 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3105 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_buckets_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     3480 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_cfs_data_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_data_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_data_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1204 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_file_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1353 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_file_downloader_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_file_downloader_facade.py
--rw-rw-rw-   0 root         (0) root         (0)     3893 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_file_sets_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     2442 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_files_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4205 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_iter_object.py
--rw-rw-rw-   0 root         (0) root         (0)     2829 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_packages_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_unpacker.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/buckets.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/file_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1035 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/file_sets.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/files.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/packages.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/endpoint_request.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/omm_stream.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/delivery/rdp_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.716445 refinitiv-data-1.6.0/refinitiv/data/discovery/
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2473 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_convert_symbols.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.720445 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/
--rw-rw-rw-   0 root         (0) root         (0)       94 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_buckets_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3509 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_df_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_navigator.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3610 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_property.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_property_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3409 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_search_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)     8754 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.724445 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12659 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8133 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/embedded.py
--rw-rw-rw-   0 root         (0) root         (0)     5265 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/manage.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/search.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.724445 refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/_customers.py
--rw-rw-rw-   0 root         (0) root         (0)     4911 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/_fetch_data.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/_relationship_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1360 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/_stakeholders.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/_suppliers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.728445 refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3907 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/_chain.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/_peers.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/_screener.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/_universe_expander.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.728445 refinitiv-data-1.6.0/refinitiv/data/early_access/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/early_access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.728445 refinitiv-data-1.6.0/refinitiv/data/early_access/content/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/early_access/content/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.728445 refinitiv-data-1.6.0/refinitiv/data/early_access/content/ipa/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/early_access/content/ipa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.728445 refinitiv-data-1.6.0/refinitiv/data/early_access/content/ipa/curves/
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/early_access/content/ipa/curves/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/early_access/content/ipa/curves/cross_currency_curves.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.728445 refinitiv-data-1.6.0/refinitiv/data/early_access/discovery/
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/early_access/discovery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.732445 refinitiv-data-1.6.0/refinitiv/data/eikon/
--rw-rw-rw-   0 root         (0) root         (0)      764 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/eikon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9549 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/eikon/_data_grid.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/eikon/_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8917 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/eikon/_json_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     7371 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/eikon/_news_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/eikon/_streaming_prices.py
--rw-rw-rw-   0 root         (0) root         (0)     5234 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/eikon/_symbology.py
--rw-rw-rw-   0 root         (0) root         (0)    13648 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/eikon/_time_series.py
--rw-rw-rw-   0 root         (0) root         (0)     5695 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/eikon/_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.732445 refinitiv-data-1.6.0/refinitiv/data/session/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/session/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1832 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/session/desktop.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/session/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.732445 refinitiv-data-1.6.0/refinitiv/data/usage_collection/
--rw-rw-rw-   0 root         (0) root         (0)      359 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/usage_collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/usage_collection/_abstract_logger.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/usage_collection/_filter_types.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/usage_collection/_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/usage_collection/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-07 12:30:10.000000 refinitiv-data-1.6.0/refinitiv/data/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 12:31:00.736445 refinitiv-data-1.6.0/refinitiv_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10325 2024-02-07 12:31:00.000000 refinitiv-data-1.6.0/refinitiv_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    56999 2024-02-07 12:31:00.000000 refinitiv-data-1.6.0/refinitiv_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 12:31:00.000000 refinitiv-data-1.6.0/refinitiv_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      307 2024-02-07 12:31:00.000000 refinitiv-data-1.6.0/refinitiv_data.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-07 12:31:00.000000 refinitiv-data-1.6.0/refinitiv_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-07 12:31:00.736445 refinitiv-data-1.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.565691 refinitiv-data-1.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)    21587 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10325 2024-04-11 09:08:52.565691 refinitiv-data-1.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9061 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.309687 refinitiv-data-1.6.1/changes/
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/changes/template.jinja
+-rw-rw-rw-   0 root         (0) root         (0)    22005 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.309687 refinitiv-data-1.6.1/refinitiv/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.313688 refinitiv-data-1.6.1/refinitiv/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.317688 refinitiv-data-1.6.1/refinitiv/data/_access_layer/
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5249 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_data_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4849 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_history_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_history_df_builder_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_intervals_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_mixed_streams.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_ohlc_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12101 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_pricing_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5290 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_recording_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/_stream_update_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.321688 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2982 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_adc_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_adc_rdp_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_adc_udf_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_context_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_cust_inst_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_cust_inst_rdp_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_cust_inst_udf_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_hp_and_cust_inst_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_hp_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.325688 refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2483 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_add_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_count_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     3622 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_date_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_holidays.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_is_working_day.py
+-rw-rw-rw-   0 root         (0) root         (0)     4948 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/get_data_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     9025 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/get_history_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     3658 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/get_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.325688 refinitiv-data-1.6.1/refinitiv/data/_access_layer/news/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/news/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/news/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     3577 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_access_layer/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)    16652 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_config_defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)    15985 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3968 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_content_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.325688 refinitiv-data-1.6.1/refinitiv/data/_core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 09:08:18.000000 refinitiv-data-1.6.1/refinitiv/data/_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/log_reporter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.329688 refinitiv-data-1.6.1/refinitiv/data/_core/session/
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      245 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_dacs_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     3967 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_default_session_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5854 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_desktop_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)    12107 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_platform_session.py
+-rw-rw-rw-   0 root         (0) root         (0)    11845 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_retry_transport.py
+-rw-rw-rw-   0 root         (0) root         (0)    16872 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_session_cxn_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_session_cxn_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_session_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    10238 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_session_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_session_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/_user_uuid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.337688 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3309 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_access_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)    10920 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_auth_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_auth_manager_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_grant.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_grant_client_credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_grant_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_grant_password.py
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_null_grant.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_ping_access_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_ping_auth_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_ping_refresh_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_ping_token_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3911 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_refresh_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_sts_access_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_sts_auth_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      373 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_sts_refresh_token_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_sts_token_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_token_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3990 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_updater.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/revoke_token.py
+-rw-rw-rw-   0 root         (0) root         (0)    10458 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/event_code.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/global_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    13648 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/http_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/null_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4110 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/proxy_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_core/session/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.337688 refinitiv-data-1.6.1/refinitiv/data/_external_libraries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 09:08:18.000000 refinitiv-data-1.6.1/refinitiv/data/_external_libraries/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.337688 refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    26229 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11913 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     7238 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/configuration_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     5845 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)    13060 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_log.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_open_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.341688 refinitiv-data-1.6.1/refinitiv/data/_tools/
+-rw-rw-rw-   0 root         (0) root         (0)     5386 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13809 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6337 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_dataframe.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_debug.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_delays.py
+-rw-rw-rw-   0 root         (0) root         (0)     6678 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_lazy_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_patterns.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_repr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_specification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5236 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_tools/templates.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/_types.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-11 09:08:51.000000 refinitiv-data-1.6.1/refinitiv/data/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.349688 refinitiv-data-1.6.1/refinitiv/data/content/
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_content_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_content_data_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_content_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4170 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_content_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_content_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_df_build_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    18779 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8645 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_df_builder_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    18438 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_entire_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_error_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_get_adc_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_historical_content_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6441 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_historical_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_historical_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_historical_raw_transf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_historical_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3064 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_intervals.py
+-rw-rw-rw-   0 root         (0) root         (0)     6076 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     3945 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_states.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_universe_content_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_universe_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    20880 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/_universe_streams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.353688 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14624 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2178 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     6121 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_instrument_class.py
+-rw-rw-rw-   0 root         (0) root         (0)    12895 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)     6208 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     8399 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_stream_facade.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_summaries.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/search.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/summaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.357688 refinitiv-data-1.6.1/refinitiv/data/content/esg/
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1470 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/_base_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/_basic_overview_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/_esg_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/_full_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/_full_scores_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/_standard_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1652 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/_standard_scores_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/_universe_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/basic_overview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.357688 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3850 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9731 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_db_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1805 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7363 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_file_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_package_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_package_manager_facade.py
+-rw-rw-rw-   0 root         (0) root         (0)     2552 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/full_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/full_scores.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/standard_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/standard_scores.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/esg/universe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.357688 refinitiv-data-1.6.1/refinitiv/data/content/estimates/
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/_enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.361688 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2163 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals/interim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.361688 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals_kpi/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals_kpi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals_kpi/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals_kpi/interim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.365688 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2302 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2138 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2178 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/historical_snapshots_non_periodic_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_annual.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/historical_snapshots_periodic_measures_interim.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/historical_snapshots_recommendations.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/interim.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/non_periodic_measures.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/recommendations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.365688 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/annual.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/historical_snapshots_kpi.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/interim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.369688 refinitiv-data-1.6.1/refinitiv/data/content/filings/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/_feed_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4876 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/_filing_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    20068 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/_retrieval_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/_retrieval_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8227 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/_search_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4699 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/_search_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/_search_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/retrieval.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/filings/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.369688 refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4031 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_content_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      821 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    11008 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2693 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_response_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.373688 refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3077 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     3067 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_events_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3628 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3593 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_summaries_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/summaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.373688 refinitiv-data-1.6.1/refinitiv/data/content/ipa/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10741 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_content_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_content_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.373688 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 09:08:18.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.373688 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.377689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py
+-rw-rw-rw-   0 root         (0) root         (0)    11538 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    28231 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.381688 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_basis_spline_smooth_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calendar_adjustment.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_calibration_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py
+-rw-rw-rw-   0 root         (0) root         (0)     8933 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_issuer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_price_side.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating_scale_source.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_reference_entity_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_seniority.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.381688 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.389689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4482 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.389689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_array_risk_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_constituent_override_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_enums/_shift_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py
+-rw-rw-rw-   0 root         (0) root         (0)     5472 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     3719 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     7749 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     6759 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)      483 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.397689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     3593 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.397689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3767 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.397689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.397689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_quotation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_enums/_standard_turn_period.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2568 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.397689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7044 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2871 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.401689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8798 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.401689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.401689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_enums/_risk_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.401689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.425689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_adjust_interest_to_payment_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_american_monte_carlo_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_amortization_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_amortization_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_average_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_axis.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_barrier_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_barrier_style.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_barrier_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_benchmark_yield_selection_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_business_day_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_buy_sell.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_calibration_strategy.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_call_put.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_cds_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_credit_spread_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_date_moving_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_dates_calendars_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_day_count_basis.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_day_of_week.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_direction.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_discounting_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_dividend_extrapolation.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_dividend_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_doc_clause.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_double_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_end_of_month_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_equity_dividend_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_eti_input_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_exercise_schedule_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_exercise_style.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_extrapolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_fixing_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_format.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_forward_compute_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_forward_extrapolation.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_funding_spread_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_fx_binary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_fx_cross_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_fx_leg_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_fx_volatility_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_holiday_outupts.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_implied_deposit_date_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_in_or_out.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_index_average_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_index_compounding_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_integration_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_index_convexity_adjustment_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_index_observation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_index_reset_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_index_spread_compounding_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_inflation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_input_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_interest_calculation_convention.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_interest_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_interpolation_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_local_volatility_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_notional_exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_numeraire_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_option_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_period_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_premium_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_price_side.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_pricing_model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_projected_index_calculation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_redemption_date_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_repo_curve_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_risk_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      308 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_rounding.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_rounding_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      741 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_seniority.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_stub_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_swaption_settlement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_swaption_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_swaption_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_tenor_reference_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_time_stamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_underlying_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_up_or_down.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_vol_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_volatility_adjustment_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_volatility_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_volatility_term_structure_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_volatility_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_yield_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.429689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_amortization_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_barrier_definition_element.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_basket_item.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_bid_ask_mid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_day_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_fx_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_input_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1170 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_interpolation_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_numerical_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_payout_scaling.py
+-rw-rw-rw-   0 root         (0) root         (0)      761 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_pde_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4761 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_object_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1342 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_param_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/_serializable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.429689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.429689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_bond_curves/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_bond_curves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.429689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.429689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/_arg_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/_base_data_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/_request_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.429689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.433689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7353 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11268 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4933 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.433689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5917 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/search.py
+-rw-rw-rw-   0 root         (0) root         (0)    21252 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_curves_builder_df.py
+-rw-rw-rw-   0 root         (0) root         (0)    10724 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_curves_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.437689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_calendar_adjustment.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_compounding_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_constituent_override_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_forward_curves_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_instrument_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_main_constituent_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_market_data_access_denied_fallback.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_swap_price_side.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_zc_curves_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      600 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_zc_interpolation_mode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.437689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_constituents.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_convexity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_curve.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_curve_point.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     7236 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_interest_rate_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_par_rate_shift.py
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_shift_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_turn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_valuation_time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.441689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6572 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_forward_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_forward_curve_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     5452 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_swap_zc_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_swap_zc_curve_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.441689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5209 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4807 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/_zc_curve_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/_zc_curve_definition_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.445689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     6765 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10381 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_request_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.445689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1443 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/_response_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.445689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     9999 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.445689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8258 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     1845 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.445689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6926 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.449689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7249 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.449689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6908 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.453689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_base_financial_contracts_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_base_option_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8306 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3267 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.453689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/bond/
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7306 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    45147 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    15065 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.453689 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7607 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4443 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    12843 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.457690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/
+-rw-rw-rw-   0 root         (0) root         (0)      678 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4232 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     7423 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.457690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6659 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3966 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     6013 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.461690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/
+-rw-rw-rw-   0 root         (0) root         (0)     1379 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_cbbc_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     6096 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_double_barriers_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4118 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_eti_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_fixing_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     9038 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_underlying_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.465690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_average_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2153 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8350 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_barrier_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_barrier_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_binary_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_dual_currency_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_forward_start.py
+-rw-rw-rw-   0 root         (0) root         (0)     5203 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_fx_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8176 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_underlying_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.465690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10119 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_eti_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4838 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    14985 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      262 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_underlying_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.469690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6187 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.469690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    18947 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5508 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.473690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.473690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/
+-rw-rw-rw-   0 root         (0) root         (0)      375 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7572 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2803 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.473690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      362 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      739 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.477690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_enums/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_enums/_calibration_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_enums/_moneyness_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_enums/_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_enums/_strike_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_enums/_volatility_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.477690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/
+-rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_maturity_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_moneyness_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_strike_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_strike_filter_range.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_surface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_surface_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3361 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_surface_output.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_surface_point.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_volatility_surface_point.py
+-rw-rw-rw-   0 root         (0) root         (0)      809 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_surface_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11035 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_surfaces_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.477690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/_cap_surface_request_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/_i_ir_vol_model_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5576 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/_i_ir_vol_model_pricing_parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.481690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2870 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5106 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_request_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.481690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2921 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_fx_statistics_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7238 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_request_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.485690 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/
+-rw-rw-rw-   0 root         (0) root         (0)      794 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7968 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/_swaption_calculation_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/_swaption_surface_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/_swaption_surface_request_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.485690 refinitiv-data-1.6.1/refinitiv/data/content/news/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/_news_data_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/_urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.489690 refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4959 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/_sort_order.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.489690 refinitiv-data-1.6.1/refinitiv/data/content/news/images/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/images/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3503 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/images/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1383 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/images/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/images/_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.489690 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_image_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.493690 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/hierarchy/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/hierarchy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/hierarchy/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/hierarchy/_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.493690 refinitiv-data-1.6.1/refinitiv/data/content/news/story/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/story/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/story/_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/story/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/story/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/story/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/story/_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/story/_response_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.497690 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/_top_news_headline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.497690 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/_subcategory.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/_top_news_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.497690 refinitiv-data-1.6.1/refinitiv/data/content/ownership/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/_org_info_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/_ownership_data_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.501690 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2420 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_investors_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3273 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/breakdown.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/concentration.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/investors.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/recent_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/shareholders_history_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/shareholders_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/top_n_concentration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.505690 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_breakdown_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_holdings_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_investors_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_recent_activity_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3185 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1933 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/breakdown.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/concentration.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/holdings.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/investors.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/recent_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/shareholders_history_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/shareholders_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/top_n_concentration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.509690 refinitiv-data-1.6.1/refinitiv/data/content/ownership/insider/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/insider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3226 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/insider/_transaction_report_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/insider/shareholders_report.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/insider/transaction_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.509690 refinitiv-data-1.6.1/refinitiv/data/content/ownership/investor/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/investor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/investor/_holdings_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/investor/holdings.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/ownership/org_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.509690 refinitiv-data-1.6.1/refinitiv/data/content/pricing/
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3412 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5253 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/_pricing_content_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    17614 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.513690 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8116 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_chain_record.py
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_chains_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4119 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    55563 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_display_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     2862 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     8874 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     4193 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.517690 refinitiv-data-1.6.1/refinitiv/data/content/search/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11894 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/search/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4241 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/search/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/search/_lookup_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/search/_metadata_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/search/_views.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/search/lookup.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/search/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.517690 refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/
+-rw-rw-rw-   0 root         (0) root         (0)      483 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_asset_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_asset_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     4444 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_country_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     7531 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_symbol_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.517690 refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     2382 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     3839 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    10744 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_stream_facade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.521690 refinitiv-data-1.6.1/refinitiv/data/delivery/
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.525690 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_api_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_data_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3236 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    26471 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_data_provider_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6943 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_data_provider_layer.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_data_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_endpoint_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_endpoint_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     5668 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_endpoint_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_parsed_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_raw_data_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5910 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_request_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2584 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_response_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_validators.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_dictionary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.533691 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6337 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_basestream.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_contrib_funcs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_contrib_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_contrib_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_dictionary_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_off_stream_contrib_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3532 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_offstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_omm_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_protocol_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     4253 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_rdp_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     4490 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    10072 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream_cxn_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5051 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11954 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     9279 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_validator_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.537690 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_cxn_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_cxn_listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     3991 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_events_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_offstream_cxn_listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     6954 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_omm_cxn_listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_rdp_cxn_listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     6005 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_stream_events.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/message_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.537690 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14672 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_dictionary_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_field_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     6746 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     9811 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    16057 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/omm_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     8053 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/omm_stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2649 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/omm_stream_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)    10626 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rdp_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3504 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rdp_stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2374 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rdp_stream_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.541691 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rwf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 09:08:18.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rwf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rwf/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     5310 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rwf/ema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9434 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rwf/socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.541691 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/states/
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/states/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/states/_basestream_states.py
+-rw-rw-rw-   0 root         (0) root         (0)     3706 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/states/_omm_states.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/states/_stream_states.py
+-rw-rw-rw-   0 root         (0) root         (0)     4075 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/stream_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    17098 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/stream_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/stream_cxn_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.541691 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/ws/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 09:08:18.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/ws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/ws/ws_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.545691 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_buckets_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_cfs_data_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_data_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_file_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_file_downloader_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_file_downloader_facade.py
+-rw-rw-rw-   0 root         (0) root         (0)     3893 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_file_sets_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2442 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_files_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4205 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_iter_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     2829 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_packages_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_unpacker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/buckets.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/file_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/file_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/files.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/packages.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/endpoint_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/omm_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/delivery/rdp_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.549691 refinitiv-data-1.6.1/refinitiv/data/discovery/
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_convert_symbols.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.549691 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_buckets_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3509 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_df_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_navigator.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3610 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_property.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_property_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3409 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_search_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)     8754 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.553691 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12659 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8133 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/embedded.py
+-rw-rw-rw-   0 root         (0) root         (0)     5265 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/search.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.553691 refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/_customers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/_fetch_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/_relationship_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1360 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/_stakeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/_suppliers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.553691 refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/_chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/_peers.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/_screener.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/_universe_expander.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.553691 refinitiv-data-1.6.1/refinitiv/data/early_access/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/early_access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.557691 refinitiv-data-1.6.1/refinitiv/data/early_access/content/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/early_access/content/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.557691 refinitiv-data-1.6.1/refinitiv/data/early_access/content/ipa/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/early_access/content/ipa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.557691 refinitiv-data-1.6.1/refinitiv/data/early_access/content/ipa/curves/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/early_access/content/ipa/curves/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/early_access/content/ipa/curves/cross_currency_curves.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.557691 refinitiv-data-1.6.1/refinitiv/data/early_access/discovery/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/early_access/discovery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.557691 refinitiv-data-1.6.1/refinitiv/data/eikon/
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/eikon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9549 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/eikon/_data_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/eikon/_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8917 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/eikon/_json_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     7371 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/eikon/_news_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/eikon/_streaming_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)     5234 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/eikon/_symbology.py
+-rw-rw-rw-   0 root         (0) root         (0)    13648 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/eikon/_time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     5695 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/eikon/_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.561691 refinitiv-data-1.6.1/refinitiv/data/session/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/session/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/session/desktop.py
+-rw-rw-rw-   0 root         (0) root         (0)     5277 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/session/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.561691 refinitiv-data-1.6.1/refinitiv/data/usage_collection/
+-rw-rw-rw-   0 root         (0) root         (0)      359 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/usage_collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/usage_collection/_abstract_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/usage_collection/_filter_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/usage_collection/_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/usage_collection/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-11 09:08:17.000000 refinitiv-data-1.6.1/refinitiv/data/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:08:52.565691 refinitiv-data-1.6.1/refinitiv_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10325 2024-04-11 09:08:51.000000 refinitiv-data-1.6.1/refinitiv_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    56999 2024-04-11 09:08:52.000000 refinitiv-data-1.6.1/refinitiv_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 09:08:51.000000 refinitiv-data-1.6.1/refinitiv_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      307 2024-04-11 09:08:51.000000 refinitiv-data-1.6.1/refinitiv_data.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-11 09:08:51.000000 refinitiv-data-1.6.1/refinitiv_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 09:08:52.565691 refinitiv-data-1.6.1/setup.cfg
```

### Comparing `refinitiv-data-1.6.0/CHANGELOG.md` & `refinitiv-data-1.6.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!-- towncrier release notes start -->
 
+## [1.6.1] - 2024-04-11
+
+### Fixed
+
+- rssl issue on reconnect after long timeout ([DME-5395](https://jira.refinitiv.com/browse/DME-5395))
+- rssl issue not being able to load ema library with python versions linked with openssl3.0  ([DME-7679](https://jira.refinitiv.com/browse/DME-7679))
+- rssl issue sending partial updates incorrectly ([DME-10284](https://jira.refinitiv.com/browse/DME-10284))
+- wrong authorization header for deployed session ([DME-13414](https://jira.refinitiv.com/browse/DME-13414))
+
+
 ## [1.6.0] - 2024-02-07
 
 ### Added
 
 - `app_name` parameter in session object and user config to define Application Client ID Header. ([eapi-6117](https://jira.refinitiv.com/browse/eapi-6117))
 - Proxies for asynchronous requests usage. ([eapi-6279](https://jira.refinitiv.com/browse/eapi-6279))
```

### Comparing `refinitiv-data-1.6.0/LICENSE` & `refinitiv-data-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/PKG-INFO` & `refinitiv-data-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refinitiv-data
-Version: 1.6.0
+Version: 1.6.1
 Summary: Client for Refinitiv Data Platform API's
 Author: REFINITIV
 License: Apache 2.0
 Project-URL: Homepage, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python
 Project-URL: Documentation, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python/documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `refinitiv-data-1.6.0/README.md` & `refinitiv-data-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/pyproject.toml` & `refinitiv-data-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_containers.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_containers.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_data_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_data_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_history_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_history_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_history_df_builder_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_history_df_builder_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_intervals_consts.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_intervals_consts.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_mixed_streams.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_mixed_streams.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_ohlc_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_ohlc_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_pricing_recorder.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_pricing_recorder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_recording_control.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_recording_control.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/_stream_update_handler.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/_stream_update_handler.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_adc_context.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_adc_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_adc_rdp_context.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_adc_rdp_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_adc_udf_context.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_adc_udf_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_context.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_context_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_context_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_cust_inst_context.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_cust_inst_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_cust_inst_rdp_context.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_cust_inst_rdp_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_cust_inst_udf_context.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_cust_inst_udf_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_hp_and_cust_inst_context.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_hp_and_cust_inst_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/context_collection/_hp_context.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/context_collection/_hp_context.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_add_periods.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_add_periods.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_count_periods.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_count_periods.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_date_schedule.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_date_schedule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_holidays.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_holidays.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/dates_and_calendars/_is_working_day.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/dates_and_calendars/_is_working_day.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/get_data_func.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/get_data_func.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/get_history_func.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/get_history_func.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/get_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/get_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/news/_news.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/news/_news.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_access_layer/session.py` & `refinitiv-data-1.6.1/refinitiv/data/_access_layer/session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_config_defaults.py` & `refinitiv-data-1.6.1/refinitiv/data/_config_defaults.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_configure.py` & `refinitiv-data-1.6.1/refinitiv/data/_configure.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_content_type.py` & `refinitiv-data-1.6.1/refinitiv/data/_content_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/log_reporter.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/log_reporter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_default_session_manager.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_default_session_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_desktop_session.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_desktop_session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_listeners.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_listeners.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_platform_session.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_platform_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     @cached_property
     def _connection(self) -> "PlatformConnection":
         from ._session_cxn_factory import get_session_cxn
 
         cxn_type = self._get_session_cxn_type()
         cxn = get_session_cxn(cxn_type, self)
 
-        if cxn_type is SessionCxnType.REFINITIV_DATA:
+        if cxn_type in [SessionCxnType.REFINITIV_DATA, SessionCxnType.REFINITIV_DATA_AND_DEPLOYED]:
             from .event import UpdateEvent
 
             auth_mgr = cxn.auth_manager
             auth_mgr.on(UpdateEvent.AUTHENTICATION_SUCCESS, self._on_authentication_success)
             auth_mgr.on(
                 UpdateEvent.AUTHENTICATION_FAILED,
                 lambda message: self._call_on_event(EventCode.SessionAuthenticationFailed, message),
```

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_retry_transport.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_retry_transport.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_session.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_session_cxn_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_session_cxn_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_session_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_session_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_session_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_session_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/_user_uuid.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/_user_uuid.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_access_token_updater.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_access_token_updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_auth_manager.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_auth_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_auth_manager_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_auth_manager_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_grant_client_credentials.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_grant_client_credentials.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_grant_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_grant_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_grant_password.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_grant_password.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_ping_token_info.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_ping_token_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_refresh_token_updater.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_refresh_token_updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_sts_access_token_updater.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_sts_access_token_updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_sts_auth_manager.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_sts_auth_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_sts_token_info.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_sts_token_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_token_info.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_token_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/_updater.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/_updater.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/auth/revoke_token.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/auth/revoke_token.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/connection.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,67 +176,65 @@
         except ConnectionError as e:
             is_debug and self.debug(f"Connexion Error on checking proxy {url} : {e!r}")
         except Exception as e:
             is_debug and self.debug(f"Error on checking proxy url {url} : {e!r}")
         return False
 
     def handshake(self, url, timeout=None):
-        #   set default timeout
         timeout = timeout if timeout is not None else self.get_timeout()
+
         is_debug = self.is_debug()
         is_debug and self.debug(f"Try to handshake on url {url}...")
 
         try:
             # DAPI for E4 - API Proxy - Handshake
-            _body = {
+            json = {
                 "AppKey": self.app_key,
                 "AppScope": "trapi",
                 "ApiVersion": "1",
                 "LibraryName": "RDP Python Library",
                 "LibraryVersion": __version__,
             }
 
             if self._uuid:
                 # add uuid for DP-PROXY multi user mode
-                _body.update({"Uuid": self._uuid})
-
-            _headers = {"Content-Type": "application/json"}
+                json.update({"Uuid": self._uuid})
 
-            response = None
-            try:
-                request = Request(
+            response = self._session.http_request(
+                Request(
                     url=url,
                     method=RequestMethod.POST,
-                    headers=_headers,
-                    json=_body,
+                    headers={"Content-Type": "application/json"},
+                    json=json,
                     timeout=timeout,
                 )
-                response = self._session.http_request(request)
+            )
+
+            status_code = response.status_code
+
+            if status_code == httpx.codes.OK:
+                self._session._access_token = response.json().get("access_token", None)
+
+            else:
+                text = response.text
+
+                if status_code == httpx.codes.BAD_REQUEST:
+                    self.error(f"Status code {status_code}: Bad request on handshake url {url} : {text}")
+                    message = f"Status code {status_code}: App key is incorrect"
 
-                is_debug and self.debug(f"Response : {response.status_code} - {response.text}")
-            except Exception as e:
-                is_debug and self.debug(f"HTTP request failed: {e!r}")
-
-            if response:
-                if response.status_code == httpx.codes.OK:
-                    result = response.json()
-                    self._session._access_token = result.get("access_token", None)
-
-                elif response.status_code == httpx.codes.BAD_REQUEST:
-                    self.error(
-                        f"Status code {response.status_code}: Bad request on handshake url {url} : {response.text}"
-                    )
-                    key_is_incorrect_msg = f"Status code {response.status_code}: App key is incorrect"
-                    self._session._call_on_event(EventCode.SessionAuthenticationFailed, key_is_incorrect_msg)
-                    raise DesktopSessionError(1, key_is_incorrect_msg)
                 else:
-                    is_debug and self.debug(f"Response {response.status_code} on handshake url {url} : {response.text}")
+                    message = f"Response {status_code} on handshake url {url} : {text}"
+                    self.error(message)
+
+                self._session._call_on_event(EventCode.SessionAuthenticationFailed, message)
+                raise DesktopSessionError(1, message)
 
         except (socket.timeout, httpx.ConnectTimeout):
             raise DesktopSessionError(1, f"Timeout on handshake url {url}")
+
         except Exception as e:
             raise DesktopSessionError(1, f"Error on handshake url {url} : {e!r}")
 
 
 # --------------------------------------------------------------------------------------
 #   RefinitivData
 # --------------------------------------------------------------------------------------
```

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/event.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/event.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/event_code.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/event_code.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/http_service.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/http_service.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/null_session.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/null_session.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/proxy_info.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/proxy_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_core/session/tools.py` & `refinitiv-data-1.6.1/refinitiv/data/_core/session/tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_errors.py` & `refinitiv-data-1.6.1/refinitiv/data/_errors.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/LICENSE` & `refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/LICENSE`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/configuration.py` & `refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/configuration_set.py` & `refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/configuration_set.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_external_libraries/python_configuration/helpers.py` & `refinitiv-data-1.6.1/refinitiv/data/_external_libraries/python_configuration/helpers.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_listener.py` & `refinitiv-data-1.6.1/refinitiv/data/_listener.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_log.py` & `refinitiv-data-1.6.1/refinitiv/data/_log.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_common.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_common.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_converter.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_converter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_dataframe.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_dataframe.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_datetime.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_datetime.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_delays.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_delays.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_lazy_loader.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_lazy_loader.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_params.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_params.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_patterns.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_patterns.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_repr.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_repr.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_specification.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_specification.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/_utils.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/_utils.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_tools/templates.py` & `refinitiv-data-1.6.1/refinitiv/data/_tools/templates.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/_types.py` & `refinitiv-data-1.6.1/refinitiv/data/_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_content_data_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_content_data_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_content_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_content_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_content_provider_layer.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_content_provider_layer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_content_response_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_content_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_df_builder_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_df_builder_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_entire_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_entire_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_error_parser.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_error_parser.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_events.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_get_adc_data.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_get_adc_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_historical_content_validator.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_historical_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_historical_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_historical_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_historical_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_historical_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_historical_raw_transf.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_historical_raw_transf.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_historical_response_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_historical_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_intervals.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_intervals.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_listeners.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_listeners.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_states.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_states.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_universe_content_validator.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_universe_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_universe_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_universe_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/_universe_streams.py` & `refinitiv-data-1.6.1/refinitiv/data/content/_universe_streams.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_custom_instruments_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_enums.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_enums.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_events.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_instrument_class.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_instrument_class.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_instrument_prop_classes.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_manage.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_search.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_stream_facade.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/_summaries.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/_summaries.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/custom_instruments/manage.py` & `refinitiv-data-1.6.1/refinitiv/data/content/custom_instruments/manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/_base_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/_base_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/_basic_overview_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/_basic_overview_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/_esg_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/_esg_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/_full_measures_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/_full_measures_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/_full_scores_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/_full_scores_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/_standard_measures_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/_standard_measures_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/_standard_scores_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/_standard_scores_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/_universe_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/_universe_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_actions.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_actions.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_db_manager.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_db_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_file_manager.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_file_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_package_manager.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_package_manager.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_package_manager_facade.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_package_manager_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/esg/bulk/_tools.py` & `refinitiv-data-1.6.1/refinitiv/data/content/esg/bulk/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals/_annual_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals/_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals/_interim_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals/_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals_kpi/_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_actuals_kpi/_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_annual_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_non_periodic_measures_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_periodic_measures_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_historical_snapshots_recommendations_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_interim_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_non_periodic_measures_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary/_recommendations_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/_annual_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/_historical_snapshots_kpi_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/estimates/view_summary_kpi/_interim_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/filings/_filing_query.py` & `refinitiv-data-1.6.1/refinitiv/data/content/filings/_filing_query.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/filings/_retrieval_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/filings/_retrieval_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/filings/_retrieval_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/filings/_retrieval_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/filings/_search_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/filings/_search_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/filings/_search_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/filings/_search_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/filings/_search_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/content/filings/_search_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_content_validator.py` & `refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py` & `refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_data_grid_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_request_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/fundamental_and_reference/_response_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/fundamental_and_reference/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_enums.py` & `refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_enums.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_events_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_events_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_historical_pricing_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_historical_pricing_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/historical_pricing/_summaries_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/historical_pricing/_summaries_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_content_provider_layer.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_content_provider_layer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_content_validator.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_content_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_constituents.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_credit_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_curves/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_business_sector.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_curve_sub_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_economic_sector.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_industry_group.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interest_calculation_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_interpolation_mode.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_bond_curves/_enums/_rating.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_butterfly_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_combined_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_curve_definition_pricing.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_flattening_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_constituents.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_forward_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_fx_shift_scenario.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_long_end_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_parallel_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_shift_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_short_end_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_time_bucket_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_curves/_twist_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_base_definition_mixin.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_bid_ask_fields_formula_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_constituents_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_curve_definition_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_create/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_delete/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_field_formula_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_formula_parameter_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_instrument_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_forward_turn_fields.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_fx_spot_instrument_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_curve_definition_keys.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_get/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instrument_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_instruments_segment.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_mixin_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_bid_ask_fields.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_override_fx_forward_turn.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_search/_curve_get_definition_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_turn_adjustment.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_curve_update_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_definitions/_update/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_curves/_cross_currency_curves/_triangulate_definitions/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_business_day_convention.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_business_day_convention.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_date_moving_convention.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_date_moving_convention.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_date_rolling_convention.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_day_count_basis.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_day_count_basis.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_day_of_week.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_day_of_week.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_exercise_style.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_exercise_style.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_frequency.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_frequency.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_fx_binary_type.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_fx_binary_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_fx_swap_calculation_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_holiday_outupts.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_holiday_outupts.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_index_compounding_method.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_index_compounding_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_period_type.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_period_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_quote_fallback_logic.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_redemption_date_type.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_redemption_date_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_seniority.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_seniority.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_stub_rule.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_stub_rule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_enums/_yield_type.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_enums/_yield_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_american_monte_carlo_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_amortization_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_amortization_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_barrier_definition_element.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_barrier_definition_element.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_bid_ask_mid.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_bid_ask_mid.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_bond_rounding_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_fx_point.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_fx_point.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_input_flow.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_input_flow.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_interpolation_weight.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_interpolation_weight.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_numerical_method.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_numerical_method.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_payout_scaling.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_payout_scaling.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_models/_pde_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_models/_pde_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_object_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_object_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_param_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_param_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_request_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/_serializable.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/_serializable.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_bond_curves/curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/_request_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_data_classes.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/definitions/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_cross_currency_curves/triangulate_definitions/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_curves_builder_df.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_curves_builder_df.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_curves_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_curves_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_instrument_type.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_instrument_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_enums/_zc_interpolation_mode.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_enums/_zc_interpolation_mode.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_convexity.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_convexity.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_curve.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_curve.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_interest_rate_curve_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_interest_rate_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_par_rate_shift.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_par_rate_shift.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_shift_scenario.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_shift_scenario.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_step.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_step.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_turn.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_turn.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/_models/_valuation_time.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/_models/_valuation_time.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_forward_curve_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_forward_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_forward_curve_request_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_forward_curve_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_swap_zc_curve_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_swap_zc_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/forward_curves/_swap_zc_curve_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/forward_curves/_swap_zc_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_zc_curve_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/_zc_curve_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curve_definitions/_zc_curve_definition_request.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curve_definitions/_zc_curve_definition_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_definitions.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_definitions.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_request_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/curves/zc_curves/_zc_curve_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/_base_request_items.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/_content_data_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/_response_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_add_periods_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/add_periods/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/count_periods/_count_periods_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/date_schedule/_date_schedule_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/holidays/_holidays_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/dates_and_calendars/is_working_day/_is_working_day_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_base_financial_contracts_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_base_financial_contracts_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_base_option_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_base_option_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_events.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_listeners.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_listeners.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_quantitative_data_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/bond/_bond_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/bond/_bond_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/bond/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_cap_floor_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cap_floor/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_cds_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_cds_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_premium_leg_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cds/_protection_leg_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_leg_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/cross/_fx_cross_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_barrier_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_barrier_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_binary_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_binary_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_cbbc_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_cbbc_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_double_barriers_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_double_barriers_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_eti_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_eti_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_fixing_info.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_fixing_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/eti_option/_underlying_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/eti_option/_underlying_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_average_info.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_average_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_barrier_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_barrier_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_binary_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_binary_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_barrier_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_barrier_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_barrier_info.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_barrier_info.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_binary_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_double_binary_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_dual_currency_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_dual_currency_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_forward_start.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_forward_start.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_fx_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_fx_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/fx_option/_underlying_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/fx_option/_underlying_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_eti_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_eti_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_option_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_option_instrument_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/option/_option_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_contract.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/repo/_repo_underlying_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_leg_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swap/_swap_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_bermudan_swaption_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_market_data_rule.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/swaption/_swaption_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/financial_contracts/term_deposit/_term_deposit_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_maturity_filter.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_maturity_filter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_moneyness_weight.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_moneyness_weight.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_strike_filter.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_strike_filter.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_strike_filter_range.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_strike_filter_range.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_surface.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_surface.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_surface_filters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_surface_filters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_surface_output.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_surface_output.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_models/_volatility_surface_point.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_models/_volatility_surface_point.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_surface_request_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/_surfaces_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/_surfaces_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/_cap_surface_request_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/_cap_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/_i_ir_vol_model_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/_i_ir_vol_model_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/cap/_i_ir_vol_model_pricing_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/cap/_i_ir_vol_model_pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_request_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/eti/_eti_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_fx_statistics_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_fx_statistics_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_parameters.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_parameters.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_request_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/fx/_fx_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/_swaption_calculation_params.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/_swaption_calculation_params.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/_swaption_surface_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/_swaption_surface_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ipa/surfaces/swaption/_swaption_surface_request_item.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ipa/surfaces/swaption/_swaption_surface_request_item.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/_news_data_provider_layer.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/_news_data_provider_layer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/_tools.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/_data.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/headlines/_request_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/headlines/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/images/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/images/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/images/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/images/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/images/_image.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/images/_image.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_image_data.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_image_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/_report.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/_report.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/hierarchy/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/hierarchy/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/hierarchy/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/online_reports/hierarchy/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/story/_data.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/story/_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/story/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/story/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/story/_request_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/story/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/story/_response_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/story/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/_top_news_headline.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/_top_news_headline.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/content/news/top_news/hierarchy/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/_org_info_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/_org_info_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/_ownership_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/_ownership_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_breakdown_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_concentration_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_concentration_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_investors_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_investors_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_recent_activity_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_shareholders_history_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_shareholders_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/consolidated/_top_n_concentration_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_breakdown_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_breakdown_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_concentration_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_concentration_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_holdings_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_holdings_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_investors_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_investors_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_recent_activity_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_recent_activity_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_shareholders_history_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_shareholders_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/fund/_top_n_concentration_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/insider/_shareholders_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/insider/_transaction_report_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/insider/_transaction_report_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/ownership/investor/_holdings_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/ownership/investor/_holdings_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/_pricing_content_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/_pricing_content_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/_stream_facade.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_chain_record.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_chain_record.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_chains_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_chains_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_display_template.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_display_template.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_events.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_listeners.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_listeners.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/pricing/chain/_stream_facade.py` & `refinitiv-data-1.6.1/refinitiv/data/content/pricing/chain/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/search/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/content/search/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/search/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/search/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/search/_lookup_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/search/_lookup_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/search/_metadata_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/search/_metadata_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/search/_views.py` & `refinitiv-data-1.6.1/refinitiv/data/content/search/_views.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_asset_class.py` & `refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_asset_class.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_asset_state.py` & `refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_asset_state.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_country_code.py` & `refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_country_code.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/symbol_conversion/_symbol_type.py` & `refinitiv-data-1.6.1/refinitiv/data/content/symbol_conversion/_symbol_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_events.py` & `refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_listeners.py` & `refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_listeners.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/content/trade_data_service/_stream_facade.py` & `refinitiv-data-1.6.1/refinitiv/data/content/trade_data_service/_stream_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_api_type.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_api_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_connection.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_data_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_data_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_data_provider_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_data_provider_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_data_provider_layer.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_data_provider_layer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_endpoint_data.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_endpoint_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_endpoint_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_endpoint_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_endpoint_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_endpoint_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_parsed_data.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_parsed_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_raw_data_parser.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_raw_data_parser.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_request.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_request_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_request_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_response.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_response.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_response_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_response_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_data/_validators.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_data/_validators.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_basestream.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_basestream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_contrib_funcs.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_contrib_funcs.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_contrib_response.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_contrib_response.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_offstream.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_offstream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_omm_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_omm_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_rdp_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_rdp_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream_cxn_cache.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream_cxn_cache.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream_cxn_config_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream_cxn_config_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/_stream_factory.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/_stream_factory.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/event.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/event.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_cxn_events.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_cxn_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_cxn_listeners.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_cxn_listeners.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_events.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_events_type.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_events_type.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_offstream_cxn_listeners.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_offstream_cxn_listeners.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_omm_cxn_listeners.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_omm_cxn_listeners.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_rdp_cxn_listeners.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_rdp_cxn_listeners.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/events/_stream_events.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/events/_stream_events.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_dictionary.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_dictionary.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_enum_type_entry.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_field_description.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_field_description.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_types.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/metadata/_validator.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/metadata/_validator.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/omm_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/omm_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/omm_stream_connection.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/omm_stream_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/omm_stream_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/omm_stream_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rdp_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rdp_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rdp_stream_connection.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rdp_stream_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rdp_stream_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rdp_stream_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rwf/conversion.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rwf/conversion.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rwf/ema.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rwf/ema.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/rwf/socket.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/rwf/socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,22 @@
 try:
     from ema import __version__ as _ema_version
 
     _ema_version = _get_version(_ema_version)
 except ImportError as e:
     _ema_version = (0, 0, 0)
 
-_EMA_VERSION_MIN = (0, 5, 0)
-_EMA_VERSION_MAX = (0, 6, 0)
+_EMA_VERSION_MIN = (0, 6, 0)
+_EMA_VERSION_MAX = (0, 7, 0)
 
 try:
     from ema import (
         OmmConsumer,
         OmmConsumerConfig,
         AppClient,
-        CustomLoggerClient,
         LoggerSeverity,
         Msg,
         OmmConsumerEvent,
         RefreshMsg,
         LoginRefresh,
         EmaOmmInvalidHandleException,
         EmaOmmInvalidUsageException,
@@ -48,18 +47,15 @@
     _exc_info = e
 else:
     from .conversion import json_marketprice_msg_to_ema
     from .ema import ema_login_message, create_programmatic_cfg, generate_login_msg
 
 if EMA_INSTALLED:
 
-    class EmaPythonLogger(CustomLoggerClient):
-        def __init__(self):
-            super().__init__(EmaPythonLogger.log)
-
+    class EmaPythonLogger:
         severity_logging_map: dict = {
             LoggerSeverity.NoLogMsg: 1000,  # higher than critical to avoid logging
             LoggerSeverity.Error: logging.ERROR,
             LoggerSeverity.Warning: logging.WARNING,
             LoggerSeverity.Success: logging.INFO,
             LoggerSeverity.Verbose: logging.DEBUG,
         }
@@ -127,15 +123,15 @@
 
         self.login_client = AppClient(
             on_refresh_msg=self.__refresh_msg_cb,
             on_update_msg=self.__nothing_callback,
             on_status_msg=self.__msg_cb,
         )
         if python_logger:
-            self.ema_logger = EmaPythonLogger()
+            self.ema_logger = EmaPythonLogger.log
         else:
             self.ema_logger = None  # Will use internal OmmLoggerClient
 
     def __refresh_msg_cb(self, msg: "RefreshMsg", event: "OmmConsumerEvent"):
         self._reissue_handle = event.get_handle()
         tmp_refresh = LoginRefresh(msg)
         if tmp_refresh.has_authentication_tt_reissue():
@@ -221,16 +217,16 @@
         return reissue_success
 
     def _handle_consumer(self, msg):
         self.info("Creating consumer")
         self._init_consumer(msg)
         if len(self.handles) > 0:
             self.info("Re-registering all streams")
-            for msg_id, msg in self.handles.copy().values():
-                self._send_message(msg, msg_id)
+            for msg_id, handle in self.handles.copy().items():
+                self._send_message(handle.msg, msg_id)
 
     def _send_message(self, msg: dict, msg_id=None):
         msg_id = msg.pop("ID", msg_id)
 
         if msg_id is None:
             raise ValueError("Message ID is not set")
```

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/states/_basestream_states.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/states/_basestream_states.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/states/_omm_states.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/states/_omm_states.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/states/_stream_states.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/states/_stream_states.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/stream_cache.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/stream_cache.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/stream_connection.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/stream_connection.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/_stream/ws/ws_client.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/_stream/ws/ws_client.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_buckets_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_buckets_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_cfs_data_provider.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_cfs_data_provider.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_data_class.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_data_class.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_data_types.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_data_types.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_file_downloader.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_file_downloader.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_file_downloader_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_file_downloader_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_file_downloader_facade.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_file_downloader_facade.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_file_sets_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_file_sets_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_files_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_files_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_iter_object.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_iter_object.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_packages_definition.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_packages_definition.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_tools.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/_unpacker.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/_unpacker.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/buckets.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/buckets.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/cfs/file_sets.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/cfs/file_sets.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/delivery/omm_stream.py` & `refinitiv-data-1.6.1/refinitiv/data/delivery/omm_stream.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_convert_symbols.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_convert_symbols.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_buckets_data.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_buckets_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_df_builder.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_df_builder.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_property.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_property.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_search_explorer.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_search_explorer.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_explorer/_search_explorer_response.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/base.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/base.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/embedded.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/embedded.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/manage.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/manage.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/namespaces.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/namespaces.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/search.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/search.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_search_templates/utils.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_search_templates/utils.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/_fetch_data.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/_fetch_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/_stakeholder_data.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_stakeholders/_stakeholders.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_stakeholders/_stakeholders.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/_chain.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/_chain.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/_discovery_universe.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/discovery/_universe_expanders/_screener.py` & `refinitiv-data-1.6.1/refinitiv/data/discovery/_universe_expanders/_screener.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/early_access/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/early_access/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/eikon/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/eikon/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/eikon/_data_grid.py` & `refinitiv-data-1.6.1/refinitiv/data/eikon/_data_grid.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/eikon/_json_requests.py` & `refinitiv-data-1.6.1/refinitiv/data/eikon/_json_requests.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/eikon/_news_request.py` & `refinitiv-data-1.6.1/refinitiv/data/eikon/_news_request.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/eikon/_streaming_prices.py` & `refinitiv-data-1.6.1/refinitiv/data/eikon/_streaming_prices.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/eikon/_symbology.py` & `refinitiv-data-1.6.1/refinitiv/data/eikon/_symbology.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/eikon/_time_series.py` & `refinitiv-data-1.6.1/refinitiv/data/eikon/_time_series.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/eikon/_tools.py` & `refinitiv-data-1.6.1/refinitiv/data/eikon/_tools.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/errors.py` & `refinitiv-data-1.6.1/refinitiv/data/errors.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/session/__init__.py` & `refinitiv-data-1.6.1/refinitiv/data/session/__init__.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/session/desktop.py` & `refinitiv-data-1.6.1/refinitiv/data/session/desktop.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/session/platform.py` & `refinitiv-data-1.6.1/refinitiv/data/session/platform.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/usage_collection/_logger.py` & `refinitiv-data-1.6.1/refinitiv/data/usage_collection/_logger.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv/data/usage_collection/_utils.py` & `refinitiv-data-1.6.1/refinitiv/data/usage_collection/_utils.py`

 * *Files identical despite different names*

### Comparing `refinitiv-data-1.6.0/refinitiv_data.egg-info/PKG-INFO` & `refinitiv-data-1.6.1/refinitiv_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refinitiv-data
-Version: 1.6.0
+Version: 1.6.1
 Summary: Client for Refinitiv Data Platform API's
 Author: REFINITIV
 License: Apache 2.0
 Project-URL: Homepage, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python
 Project-URL: Documentation, https://developers.refinitiv.com/en/api-catalog/refinitiv-data-platform/refinitiv-data-library-for-python/documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `refinitiv-data-1.6.0/refinitiv_data.egg-info/SOURCES.txt` & `refinitiv-data-1.6.1/refinitiv_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

