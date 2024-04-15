# Comparing `tmp/empire-platform-api-public-client-3.0.6.tar.gz` & `tmp/empire-platform-api-public-client-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empire-platform-api-public-client-3.0.6.tar", last modified: Mon Mar 11 12:43:53 2024, max compression
+gzip compressed data, was "empire-platform-api-public-client-3.0.7.tar", last modified: Mon Apr 15 08:50:43 2024, max compression
```

## Comparing `empire-platform-api-public-client-3.0.6.tar` & `empire-platform-api-public-client-3.0.7.tar`

### file list

```diff
@@ -1,762 +1,762 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:43:53.317522 empire-platform-api-public-client-3.0.6/
--rw-r--r--   0 root         (0) root         (0)      568 2024-03-11 12:43:53.317522 empire-platform-api-public-client-3.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    55385 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:43:53.257523 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/
--rw-r--r--   0 root         (0) root         (0)    43655 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:43:53.257523 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/
--rw-r--r--   0 root         (0) root         (0)     2285 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26235 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/allocated_auction_api.py
--rw-r--r--   0 root         (0) root         (0)    10436 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/attachment_api.py
--rw-r--r--   0 root         (0) root         (0)   126206 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/auction_api.py
--rw-r--r--   0 root         (0) root         (0)    19476 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/audit_log_api.py
--rw-r--r--   0 root         (0) root         (0)    15523 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/bidding_configuration_api.py
--rw-r--r--   0 root         (0) root         (0)    17494 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/buy_now_offers_api.py
--rw-r--r--   0 root         (0) root         (0)    73532 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/default_bid_api.py
--rw-r--r--   0 root         (0) root         (0)    48329 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/default_nomination_api.py
--rw-r--r--   0 root         (0) root         (0)    47142 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/finance_api.py
--rw-r--r--   0 root         (0) root         (0)     8015 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/finance_information_api.py
--rw-r--r--   0 root         (0) root         (0)    24382 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/manual_file_upload_api.py
--rw-r--r--   0 root         (0) root         (0)    30817 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/messages_api.py
--rw-r--r--   0 root         (0) root         (0)     6792 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    51180 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/nomination_api.py
--rw-r--r--   0 root         (0) root         (0)    20162 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/organisation_api.py
--rw-r--r--   0 root         (0) root         (0)    35765 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/organisation_document_api.py
--rw-r--r--   0 root         (0) root         (0)    71824 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/participant_dashboard_api.py
--rw-r--r--   0 root         (0) root         (0)     8059 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/participant_overview_api.py
--rw-r--r--   0 root         (0) root         (0)    55942 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/profile_api.py
--rw-r--r--   0 root         (0) root         (0)    22948 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/public_allocated_auction_api.py
--rw-r--r--   0 root         (0) root         (0)    69040 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/public_auction_api.py
--rw-r--r--   0 root         (0) root         (0)     8795 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/public_nominations_api.py
--rw-r--r--   0 root         (0) root         (0)   142505 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/reporting_api.py
--rw-r--r--   0 root         (0) root         (0)   214379 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/secondary_market_api.py
--rw-r--r--   0 root         (0) root         (0)    11195 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/transmission_right_api.py
--rw-r--r--   0 root         (0) root         (0)    49549 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/user_api.py
--rw-r--r--   0 root         (0) root         (0)    30604 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api_client.py
--rw-r--r--   0 root         (0) root         (0)      852 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api_response.py
--rw-r--r--   0 root         (0) root         (0)    15731 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5598 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:43:53.287523 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/
--rw-r--r--   0 root         (0) root         (0)    40703 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2518 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/address.py
--rw-r--r--   0 root         (0) root         (0)     5328 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_allocated_auction.py
--rw-r--r--   0 root         (0) root         (0)     3148 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     2439 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nomination_options_nominee_participants.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nomination_type.py
--rw-r--r--   0 root         (0) root         (0)     3172 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2914 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb.py
--rw-r--r--   0 root         (0) root         (0)     3990 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2704 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_mtu_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_mtu_value.py
--rw-r--r--   0 root         (0) root         (0)     2852 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_nl.py
--rw-r--r--   0 root         (0) root         (0)     4568 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2635 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_eprogram_values.py
--rw-r--r--   0 root         (0) root         (0)     4003 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_pre_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     2539 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_pre_nomination_options_timescale.py
--rw-r--r--   0 root         (0) root         (0)     5292 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/allocated_auction.py
--rw-r--r--   0 root         (0) root         (0)     2864 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/allocated_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/allocated_auction_participant_status.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/allocated_auction_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2645 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/api_key.py
--rw-r--r--   0 root         (0) root         (0)     2985 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/attachment.py
--rw-r--r--   0 root         (0) root         (0)     5832 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_allocation_resolution.py
--rw-r--r--   0 root         (0) root         (0)     2818 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     2239 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_bid_participant.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     3086 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_bidding_configuration.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_bidding_mode.py
--rw-r--r--   0 root         (0) root         (0)     1270 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_filter_status.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_intra_day_product_type.py
--rw-r--r--   0 root         (0) root         (0)     6529 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_process_steps_absolute.py
--rw-r--r--   0 root         (0) root         (0)     1714 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_product_type.py
--rw-r--r--   0 root         (0) root         (0)     2965 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_reduction_period.py
--rw-r--r--   0 root         (0) root         (0)     3136 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_result_congestion_rent.py
--rw-r--r--   0 root         (0) root         (0)     2401 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_result_participant.py
--rw-r--r--   0 root         (0) root         (0)     1532 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1317 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_status.py
--rw-r--r--   0 root         (0) root         (0)     1354 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_timescale.py
--rw-r--r--   0 root         (0) root         (0)     4663 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2709 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_api_key.py
--rw-r--r--   0 root         (0) root         (0)     2789 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_batch.py
--rw-r--r--   0 root         (0) root         (0)     1945 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_domain.py
--rw-r--r--   0 root         (0) root         (0)     2377 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_payload.py
--rw-r--r--   0 root         (0) root         (0)      963 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      933 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_status.py
--rw-r--r--   0 root         (0) root         (0)     8159 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_type.py
--rw-r--r--   0 root         (0) root         (0)     2817 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_user.py
--rw-r--r--   0 root         (0) root         (0)     2263 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     2427 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bid_value.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bidding_configuration.py
--rw-r--r--   0 root         (0) root         (0)     3112 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bidding_configuration_per_direction.py
--rw-r--r--   0 root         (0) root         (0)     2541 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bidding_configuration_secondary_market_notices.py
--rw-r--r--   0 root         (0) root         (0)     2788 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bidding_configuration_values.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/border_direction.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/border_direction_with_both.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/border_direction_with_both_and_none.py
--rw-r--r--   0 root         (0) root         (0)     1244 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/buy_now_day_ahead_offer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     5687 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/buy_now_offer.py
--rw-r--r--   0 root         (0) root         (0)     2747 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/buy_now_offer_mtus.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/buy_now_offer_status.py
--rw-r--r--   0 root         (0) root         (0)     2089 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_api_key_request.py
--rw-r--r--   0 root         (0) root         (0)     5997 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2946 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids.py
--rw-r--r--   0 root         (0) root         (0)     3000 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_mtus.py
--rw-r--r--   0 root         (0) root         (0)     3752 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_default_nomination_request.py
--rw-r--r--   0 root         (0) root         (0)     5761 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_long_term_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2427 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_organisation_document_request.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     3600 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     3924 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py
--rw-r--r--   0 root         (0) root         (0)     4215 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     3492 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     3383 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_long_term_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2844 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_return_request.py
--rw-r--r--   0 root         (0) root         (0)     2257 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_api_key.py
--rw-r--r--   0 root         (0) root         (0)     2129 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2185 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_default_nomination.py
--rw-r--r--   0 root         (0) root         (0)     2209 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_organisation_document.py
--rw-r--r--   0 root         (0) root         (0)     2441 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2465 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2433 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2385 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2353 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_long_term_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2353 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_return_request_identifier.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/credit_cover_type.py
--rw-r--r--   0 root         (0) root         (0)     4011 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/dashboard_next_nomination_gate.py
--rw-r--r--   0 root         (0) root         (0)     3120 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/dashboard_next_nomination_gate_window.py
--rw-r--r--   0 root         (0) root         (0)     1042 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/dashboard_next_nomination_window_status.py
--rw-r--r--   0 root         (0) root         (0)     2538 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/date_period.py
--rw-r--r--   0 root         (0) root         (0)     3085 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/date_time_period.py
--rw-r--r--   0 root         (0) root         (0)     6273 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_auction.py
--rw-r--r--   0 root         (0) root         (0)     3193 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group.py
--rw-r--r--   0 root         (0) root         (0)     3235 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids.py
--rw-r--r--   0 root         (0) root         (0)     3834 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_bid.py
--rw-r--r--   0 root         (0) root         (0)     2861 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_bid_results.py
--rw-r--r--   0 root         (0) root         (0)     3522 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_batch.py
--rw-r--r--   0 root         (0) root         (0)     3308 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_bids.py
--rw-r--r--   0 root         (0) root         (0)     3334 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_bids_bid.py
--rw-r--r--   0 root         (0) root         (0)     4297 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2824 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results_bids.py
--rw-r--r--   0 root         (0) root         (0)     2920 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results.py
--rw-r--r--   0 root         (0) root         (0)     3381 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2966 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_value.py
--rw-r--r--   0 root         (0) root         (0)     4161 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     4819 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results_mtu.py
--rw-r--r--   0 root         (0) root         (0)     5984 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2788 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid_bids.py
--rw-r--r--   0 root         (0) root         (0)     2896 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid_bids_mtus.py
--rw-r--r--   0 root         (0) root         (0)     5195 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2792 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid_batch.py
--rw-r--r--   0 root         (0) root         (0)     2692 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid_options.py
--rw-r--r--   0 root         (0) root         (0)     1587 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      941 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination.py
--rw-r--r--   0 root         (0) root         (0)     2876 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_batch.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_declaration_type.py
--rw-r--r--   0 root         (0) root         (0)     3849 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_details.py
--rw-r--r--   0 root         (0) root         (0)     2847 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2710 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     1342 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      976 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_status.py
--rw-r--r--   0 root         (0) root         (0)     9640 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/error_code.py
--rw-r--r--   0 root         (0) root         (0)     3278 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/error_response.py
--rw-r--r--   0 root         (0) root         (0)     5470 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information.py
--rw-r--r--   0 root         (0) root         (0)     2712 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_bank_deposits.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_letter_of_credits.py
--rw-r--r--   0 root         (0) root         (0)     2489 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_lockable_amount.py
--rw-r--r--   0 root         (0) root         (0)     2431 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_lockable_date.py
--rw-r--r--   0 root         (0) root         (0)     3549 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_lockable_period.py
--rw-r--r--   0 root         (0) root         (0)     2590 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_market_vat_details.py
--rw-r--r--   0 root         (0) root         (0)     2344 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_sage_settings.py
--rw-r--r--   0 root         (0) root         (0)     6273 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/intra_day_auction.py
--rw-r--r--   0 root         (0) root         (0)     4687 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice.py
--rw-r--r--   0 root         (0) root         (0)     1028 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_action_type.py
--rw-r--r--   0 root         (0) root         (0)     2755 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_batch.py
--rw-r--r--   0 root         (0) root         (0)     8176 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_details.py
--rw-r--r--   0 root         (0) root         (0)     3168 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_history.py
--rw-r--r--   0 root         (0) root         (0)     4486 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_line_item.py
--rw-r--r--   0 root         (0) root         (0)     2289 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_participant_details.py
--rw-r--r--   0 root         (0) root         (0)      960 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_status.py
--rw-r--r--   0 root         (0) root         (0)     3964 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_summary.py
--rw-r--r--   0 root         (0) root         (0)     2504 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_vat_rate.py
--rw-r--r--   0 root         (0) root         (0)     6429 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction.py
--rw-r--r--   0 root         (0) root         (0)     3947 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid.py
--rw-r--r--   0 root         (0) root         (0)     3797 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid_result.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid_result_batch.py
--rw-r--r--   0 root         (0) root         (0)     2685 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid_results.py
--rw-r--r--   0 root         (0) root         (0)     1079 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     5319 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     3394 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_results_allocated_capacity.py
--rw-r--r--   0 root         (0) root         (0)     2946 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_results_bids.py
--rw-r--r--   0 root         (0) root         (0)     5802 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2837 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_offered_capacity.py
--rw-r--r--   0 root         (0) root         (0)     2902 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_reserve_price.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_reserve_price_steps.py
--rw-r--r--   0 root         (0) root         (0)     2241 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/manual_file_upload_request.py
--rw-r--r--   0 root         (0) root         (0)      873 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/market.py
--rw-r--r--   0 root         (0) root         (0)     4125 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message.py
--rw-r--r--   0 root         (0) root         (0)     2755 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_batch.py
--rw-r--r--   0 root         (0) root         (0)      978 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_category.py
--rw-r--r--   0 root         (0) root         (0)      918 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_sender.py
--rw-r--r--   0 root         (0) root         (0)      996 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_severity.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1446 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_type.py
--rw-r--r--   0 root         (0) root         (0)     3453 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/mtu_period.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/mtu_size.py
--rw-r--r--   0 root         (0) root         (0)     2517 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/mtu_size_per_auction_product_type.py
--rw-r--r--   0 root         (0) root         (0)     2370 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/mtu_size_per_timescale.py
--rw-r--r--   0 root         (0) root         (0)     2276 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/nested_error.py
--rw-r--r--   0 root         (0) root         (0)     1067 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/nomination_capacity_resolution.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/nomination_restriction_type.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/noticeboard_entry_type.py
--rw-r--r--   0 root         (0) root         (0)     1007 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/noticeboard_entry_type_with_both.py
--rw-r--r--   0 root         (0) root         (0)     2119 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/notification_preference.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/notification_preference_with_sms.py
--rw-r--r--   0 root         (0) root         (0)     3498 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/ntc_overview_mtu_data.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/offered_capacity_setup.py
--rw-r--r--   0 root         (0) root         (0)     2969 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_auth_method.py
--rw-r--r--   0 root         (0) root         (0)     2292 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_contact.py
--rw-r--r--   0 root         (0) root         (0)     3339 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_contact_information.py
--rw-r--r--   0 root         (0) root         (0)     4298 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_batch.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_file_type.py
--rw-r--r--   0 root         (0) root         (0)     3068 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_options.py
--rw-r--r--   0 root         (0) root         (0)     2966 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1333 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      995 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_status.py
--rw-r--r--   0 root         (0) root         (0)     2934 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_uploaded_by_user.py
--rw-r--r--   0 root         (0) root         (0)     2439 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_uploaded_by_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     2263 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_user.py
--rw-r--r--   0 root         (0) root         (0)     2326 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_file_settings.py
--rw-r--r--   0 root         (0) root         (0)     3600 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_market_settings.py
--rw-r--r--   0 root         (0) root         (0)     2995 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_market_settings_gb_nomination_settings.py
--rw-r--r--   0 root         (0) root         (0)     2791 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_market_settings_nl_nomination_settings.py
--rw-r--r--   0 root         (0) root         (0)      959 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_status.py
--rw-r--r--   0 root         (0) root         (0)      959 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_type.py
--rw-r--r--   0 root         (0) root         (0)     4266 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_user.py
--rw-r--r--   0 root         (0) root         (0)     2864 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_user_batch.py
--rw-r--r--   0 root         (0) root         (0)     1173 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2184 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/other_party.py
--rw-r--r--   0 root         (0) root         (0)     2159 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant.py
--rw-r--r--   0 root         (0) root         (0)     2601 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_default_bids_and_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     3816 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_finance_overview_data.py
--rw-r--r--   0 root         (0) root         (0)     3598 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_finance_overview_invoice.py
--rw-r--r--   0 root         (0) root         (0)     3143 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data.py
--rw-r--r--   0 root         (0) root         (0)     3598 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2891 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     3014 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data.py
--rw-r--r--   0 root         (0) root         (0)     4434 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     3207 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_messages.py
--rw-r--r--   0 root         (0) root         (0)     3070 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     4504 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2787 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_aggregated_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2751 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     4903 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_next_auction.py
--rw-r--r--   0 root         (0) root         (0)     4442 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_next_auctions_and_nomination_gates.py
--rw-r--r--   0 root         (0) root         (0)     3252 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     3720 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     4041 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     2966 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_values_nomination_restriction.py
--rw-r--r--   0 root         (0) root         (0)     3136 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data.py
--rw-r--r--   0 root         (0) root         (0)     3781 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     3166 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     4429 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_organisation_details.py
--rw-r--r--   0 root         (0) root         (0)     5035 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_overview_data.py
--rw-r--r--   0 root         (0) root         (0)     3427 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_overview_data_contact_information.py
--rw-r--r--   0 root         (0) root         (0)     3085 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_overview_data_finance_overview.py
--rw-r--r--   0 root         (0) root         (0)     2659 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_overview_data_organisation_members.py
--rw-r--r--   0 root         (0) root         (0)     6843 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/permission.py
--rw-r--r--   0 root         (0) root         (0)     1153 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/platform_appearance.py
--rw-r--r--   0 root         (0) root         (0)     3142 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/profile.py
--rw-r--r--   0 root         (0) root         (0)     3081 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/profile_details.py
--rw-r--r--   0 root         (0) root         (0)     2915 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/profile_user.py
--rw-r--r--   0 root         (0) root         (0)     2493 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/profile_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     3115 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     4304 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2767 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2982 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_allocated_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     4460 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction.py
--rw-r--r--   0 root         (0) root         (0)     2828 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     1220 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction_filter_status.py
--rw-r--r--   0 root         (0) root         (0)     1246 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction_status.py
--rw-r--r--   0 root         (0) root         (0)     5423 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_day_ahead_auction.py
--rw-r--r--   0 root         (0) root         (0)     2897 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results.py
--rw-r--r--   0 root         (0) root         (0)     3117 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results_bids.py
--rw-r--r--   0 root         (0) root         (0)     3628 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     5423 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_intra_day_auction.py
--rw-r--r--   0 root         (0) root         (0)     5877 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_long_term_auction.py
--rw-r--r--   0 root         (0) root         (0)     4169 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_long_term_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     3013 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_long_term_auction_results_bids.py
--rw-r--r--   0 root         (0) root         (0)     2255 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/purchased_by_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1238 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/reserve_price_publish_type.py
--rw-r--r--   0 root         (0) root         (0)     3108 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/return_auction.py
--rw-r--r--   0 root         (0) root         (0)     5215 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/sage_code.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_capacity_price_mtu.py
--rw-r--r--   0 root         (0) root         (0)     4592 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     4594 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py
--rw-r--r--   0 root         (0) root         (0)     4952 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py
--rw-r--r--   0 root         (0) root         (0)     4120 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py
--rw-r--r--   0 root         (0) root         (0)     3538 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus.py
--rw-r--r--   0 root         (0) root         (0)     3139 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_options.py
--rw-r--r--   0 root         (0) root         (0)     3203 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py
--rw-r--r--   0 root         (0) root         (0)     6549 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     3142 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py
--rw-r--r--   0 root         (0) root         (0)     3236 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options.py
--rw-r--r--   0 root         (0) root         (0)     3282 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus.py
--rw-r--r--   0 root         (0) root         (0)     3560 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     4309 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_details.py
--rw-r--r--   0 root         (0) root         (0)     3881 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_response.py
--rw-r--r--   0 root         (0) root         (0)     2526 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_options.py
--rw-r--r--   0 root         (0) root         (0)     2590 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_response_options.py
--rw-r--r--   0 root         (0) root         (0)     2506 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_transfer_request_options.py
--rw-r--r--   0 root         (0) root         (0)     5332 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     3046 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_batch.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_status.py
--rw-r--r--   0 root         (0) root         (0)     4441 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_return_request.py
--rw-r--r--   0 root         (0) root         (0)     3010 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_return_request_batch.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_return_request_status.py
--rw-r--r--   0 root         (0) root         (0)     6453 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     3034 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_request_batch.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_request_status.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_request_type.py
--rw-r--r--   0 root         (0) root         (0)     3214 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_transmission_rights_mtu.py
--rw-r--r--   0 root         (0) root         (0)     3120 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement_item.py
--rw-r--r--   0 root         (0) root         (0)     3350 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement_per_source.py
--rw-r--r--   0 root         (0) root         (0)     1037 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement_source_type.py
--rw-r--r--   0 root         (0) root         (0)     2222 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement_sub_source_type.py
--rw-r--r--   0 root         (0) root         (0)     3715 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/source_auction.py
--rw-r--r--   0 root         (0) root         (0)     2348 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/source_auction_display_data.py
--rw-r--r--   0 root         (0) root         (0)     2684 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/source_auction_result.py
--rw-r--r--   0 root         (0) root         (0)     2914 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request.py
--rw-r--r--   0 root         (0) root         (0)     3750 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups.py
--rw-r--r--   0 root         (0) root         (0)     3205 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_bids.py
--rw-r--r--   0 root         (0) root         (0)     2701 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_long_term_bids_request.py
--rw-r--r--   0 root         (0) root         (0)     3285 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_long_term_bids_request_bids.py
--rw-r--r--   0 root         (0) root         (0)     2837 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_nominations_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_timescale_nominations_request.py
--rw-r--r--   0 root         (0) root         (0)      976 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/system_message_category.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_mtu_status.py
--rw-r--r--   0 root         (0) root         (0)     3262 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     3150 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_options_window_timing.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_status.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_type.py
--rw-r--r--   0 root         (0) root         (0)     1044 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_window_status.py
--rw-r--r--   0 root         (0) root         (0)     3111 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nominations.py
--rw-r--r--   0 root         (0) root         (0)     5019 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nominations_mtus.py
--rw-r--r--   0 root         (0) root         (0)     3512 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nominations_mtus_current_nomination.py
--rw-r--r--   0 root         (0) root         (0)     2711 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/transmission_rights_overview.py
--rw-r--r--   0 root         (0) root         (0)     3356 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/transmission_rights_overview_mtus.py
--rw-r--r--   0 root         (0) root         (0)     3817 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/transmission_rights_overview_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     2668 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/transmission_rights_overview_mtus_values_timescales.py
--rw-r--r--   0 root         (0) root         (0)     2355 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/uiosi_not_resold.py
--rw-r--r--   0 root         (0) root         (0)     2740 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/uiosi_overview.py
--rw-r--r--   0 root         (0) root         (0)     4015 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/uiosi_overview_per_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2841 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/uiosi_resold.py
--rw-r--r--   0 root         (0) root         (0)     2206 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/unread_messages_response.py
--rw-r--r--   0 root         (0) root         (0)     5311 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2946 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request_bids.py
--rw-r--r--   0 root         (0) root         (0)     3000 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request_bids_mtus.py
--rw-r--r--   0 root         (0) root         (0)     3318 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_default_nomination_request.py
--rw-r--r--   0 root         (0) root         (0)     5075 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_long_term_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2463 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_profile_details_request.py
--rw-r--r--   0 root         (0) root         (0)     2532 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     3284 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user.py
--rw-r--r--   0 root         (0) root         (0)     2199 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     3545 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_preferences.py
--rw-r--r--   0 root         (0) root         (0)     3806 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_preferences_general_notifications.py
--rw-r--r--   0 root         (0) root         (0)     3409 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_preferences_subscription_notifications.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_role.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_status.py
--rw-r--r--   0 root         (0) root         (0)     1264 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/vat_rate_type.py
--rw-r--r--   0 root         (0) root         (0)     2129 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/version.py
--rw-r--r--   0 root         (0) root         (0)     2133 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/zendesk_chat_token_response.py
--rw-r--r--   0 root         (0) root         (0)    13115 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:43:53.257523 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      568 2024-03-11 12:43:53.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    45898 2024-03-11 12:43:53.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 12:43:53.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-11 12:43:53.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-03-11 12:43:53.000000 empire-platform-api-public-client-3.0.6/empire_platform_api_public_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       69 2024-03-11 12:43:53.317522 empire-platform-api-public-client-3.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1646 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:43:53.317522 empire-platform-api-public-client-3.0.6/test/
--rw-r--r--   0 root         (0) root         (0)     1793 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_address.py
--rw-r--r--   0 root         (0) root         (0)     3037 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_allocated_auction.py
--rw-r--r--   0 root         (0) root         (0)     2165 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nomination_options_nominee_participants.py
--rw-r--r--   0 root         (0) root         (0)     1004 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nomination_type.py
--rw-r--r--   0 root         (0) root         (0)     8340 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations.py
--rw-r--r--   0 root         (0) root         (0)     3449 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_mns_or_gb.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_mns_or_gb_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2043 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_mtu_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     1900 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_mtu_value.py
--rw-r--r--   0 root         (0) root         (0)     3897 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_nl.py
--rw-r--r--   0 root         (0) root         (0)     3320 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_nl_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2042 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_nl_mtus_eprogram_values.py
--rw-r--r--   0 root         (0) root         (0)     3594 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_pre_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     2059 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_aggregated_pre_nomination_options_timescale.py
--rw-r--r--   0 root         (0) root         (0)     2952 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_allocated_auction.py
--rw-r--r--   0 root         (0) root         (0)     1166 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_allocated_auction_api.py
--rw-r--r--   0 root         (0) root         (0)     3807 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_allocated_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     1068 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_allocated_auction_participant_status.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_allocated_auction_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_api_key.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_attachment.py
--rw-r--r--   0 root         (0) root         (0)      977 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_attachment_api.py
--rw-r--r--   0 root         (0) root         (0)     3259 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_allocation_resolution.py
--rw-r--r--   0 root         (0) root         (0)     3220 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_auction_api.py
--rw-r--r--   0 root         (0) root         (0)     4094 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_bid_participant.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     2067 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_bidding_configuration.py
--rw-r--r--   0 root         (0) root         (0)      962 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_bidding_mode.py
--rw-r--r--   0 root         (0) root         (0)      969 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_filter_status.py
--rw-r--r--   0 root         (0) root         (0)     1020 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_intra_day_product_type.py
--rw-r--r--   0 root         (0) root         (0)     2583 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_process_steps_absolute.py
--rw-r--r--   0 root         (0) root         (0)      962 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_product_type.py
--rw-r--r--   0 root         (0) root         (0)     2227 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_reduction_period.py
--rw-r--r--   0 root         (0) root         (0)     1978 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_result_congestion_rent.py
--rw-r--r--   0 root         (0) root         (0)     1979 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_result_participant.py
--rw-r--r--   0 root         (0) root         (0)      927 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_status.py
--rw-r--r--   0 root         (0) root         (0)      947 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_auction_timescale.py
--rw-r--r--   0 root         (0) root         (0)     3772 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_api.py
--rw-r--r--   0 root         (0) root         (0)     1866 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_api_key.py
--rw-r--r--   0 root         (0) root         (0)     5146 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_batch.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-03-11 12:43:48.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_domain.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_payload.py
--rw-r--r--   0 root         (0) root         (0)      935 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_status.py
--rw-r--r--   0 root         (0) root         (0)      920 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_type.py
--rw-r--r--   0 root         (0) root         (0)     2273 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_user.py
--rw-r--r--   0 root         (0) root         (0)     1886 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_audit_log_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1640 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_bid_value.py
--rw-r--r--   0 root         (0) root         (0)     3326 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_bidding_configuration.py
--rw-r--r--   0 root         (0) root         (0)     1182 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_bidding_configuration_api.py
--rw-r--r--   0 root         (0) root         (0)     1935 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_bidding_configuration_per_direction.py
--rw-r--r--   0 root         (0) root         (0)     2131 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_bidding_configuration_secondary_market_notices.py
--rw-r--r--   0 root         (0) root         (0)     2385 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_bidding_configuration_values.py
--rw-r--r--   0 root         (0) root         (0)      940 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_border_direction.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_border_direction_with_both.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_border_direction_with_both_and_none.py
--rw-r--r--   0 root         (0) root         (0)     1015 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_buy_now_day_ahead_offer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     3342 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_buy_now_offer.py
--rw-r--r--   0 root         (0) root         (0)     1738 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_buy_now_offer_mtus.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_buy_now_offer_status.py
--rw-r--r--   0 root         (0) root         (0)     1117 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_buy_now_offers_api.py
--rw-r--r--   0 root         (0) root         (0)     1704 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_api_key_request.py
--rw-r--r--   0 root         (0) root         (0)     4021 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_day_ahead_or_intra_day_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2862 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_day_ahead_or_intra_day_default_bid_request_bids.py
--rw-r--r--   0 root         (0) root         (0)     2238 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2724 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_default_nomination_request.py
--rw-r--r--   0 root         (0) root         (0)     2884 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_long_term_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2030 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_organisation_document_request.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     7234 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     3186 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2251 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2540 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     6649 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_long_term_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_long_term_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2211 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_return_request.py
--rw-r--r--   0 root         (0) root         (0)     1809 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_api_key.py
--rw-r--r--   0 root         (0) root         (0)     1747 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     1831 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_default_nomination.py
--rw-r--r--   0 root         (0) root         (0)     1867 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_organisation_document.py
--rw-r--r--   0 root         (0) root         (0)     2222 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2258 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2210 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2099 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2135 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_long_term_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2087 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_long_term_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2086 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_return_request_identifier.py
--rw-r--r--   0 root         (0) root         (0)      941 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_credit_cover_type.py
--rw-r--r--   0 root         (0) root         (0)     2942 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_dashboard_next_nomination_gate.py
--rw-r--r--   0 root         (0) root         (0)     2013 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_dashboard_next_nomination_gate_window.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_dashboard_next_nomination_window_status.py
--rw-r--r--   0 root         (0) root         (0)     1760 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_date_period.py
--rw-r--r--   0 root         (0) root         (0)     1765 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_date_time_period.py
--rw-r--r--   0 root         (0) root         (0)     5396 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_auction.py
--rw-r--r--   0 root         (0) root         (0)     4056 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group.py
--rw-r--r--   0 root         (0) root         (0)     2675 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_bids.py
--rw-r--r--   0 root         (0) root         (0)     2684 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_bids_bid.py
--rw-r--r--   0 root         (0) root         (0)     2155 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_bids_bid_results.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_result.py
--rw-r--r--   0 root         (0) root         (0)     4730 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_result_batch.py
--rw-r--r--   0 root         (0) root         (0)     2478 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_result_bids.py
--rw-r--r--   0 root         (0) root         (0)     2437 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_result_bids_bid.py
--rw-r--r--   0 root         (0) root         (0)     1985 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2820 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_mtu_results.py
--rw-r--r--   0 root         (0) root         (0)     2342 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_mtu_results_bids.py
--rw-r--r--   0 root         (0) root         (0)     3072 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_participant_results.py
--rw-r--r--   0 root         (0) root         (0)     2349 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_participant_results_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2206 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_value.py
--rw-r--r--   0 root         (0) root         (0)     3831 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     2406 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_results_mtu.py
--rw-r--r--   0 root         (0) root         (0)     3873 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2648 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_default_bid_bids.py
--rw-r--r--   0 root         (0) root         (0)     2080 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_default_bid_bids_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2316 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_default_bid_api.py
--rw-r--r--   0 root         (0) root         (0)     2979 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_bid_batch.py
--rw-r--r--   0 root         (0) root         (0)     2237 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_bid_options.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_bid_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     2200 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_nomination.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_default_nomination_api.py
--rw-r--r--   0 root         (0) root         (0)     2807 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_nomination_batch.py
--rw-r--r--   0 root         (0) root         (0)     1061 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_nomination_declaration_type.py
--rw-r--r--   0 root         (0) root         (0)     2773 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_nomination_details.py
--rw-r--r--   0 root         (0) root         (0)     1827 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_nomination_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2229 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_nomination_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_default_nomination_status.py
--rw-r--r--   0 root         (0) root         (0)      898 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_error_code.py
--rw-r--r--   0 root         (0) root         (0)     2130 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)     1512 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_finance_api.py
--rw-r--r--   0 root         (0) root         (0)     9777 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_finance_information.py
--rw-r--r--   0 root         (0) root         (0)     1030 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_finance_information_api.py
--rw-r--r--   0 root         (0) root         (0)     3624 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_finance_information_bank_deposits.py
--rw-r--r--   0 root         (0) root         (0)     3727 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_finance_information_letter_of_credits.py
--rw-r--r--   0 root         (0) root         (0)     1932 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_finance_information_lockable_amount.py
--rw-r--r--   0 root         (0) root         (0)     1962 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_finance_information_lockable_date.py
--rw-r--r--   0 root         (0) root         (0)     3172 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_finance_information_lockable_period.py
--rw-r--r--   0 root         (0) root         (0)     2045 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_finance_information_market_vat_details.py
--rw-r--r--   0 root         (0) root         (0)     1918 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_finance_information_sage_settings.py
--rw-r--r--   0 root         (0) root         (0)     5396 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_intra_day_auction.py
--rw-r--r--   0 root         (0) root         (0)     2836 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_invoice.py
--rw-r--r--   0 root         (0) root         (0)      955 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_invoice_action_type.py
--rw-r--r--   0 root         (0) root         (0)     3858 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_invoice_batch.py
--rw-r--r--   0 root         (0) root         (0)     7263 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_invoice_details.py
--rw-r--r--   0 root         (0) root         (0)     1985 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_invoice_history.py
--rw-r--r--   0 root         (0) root         (0)     2338 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_invoice_line_item.py
--rw-r--r--   0 root         (0) root         (0)     1897 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_invoice_participant_details.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_invoice_status.py
--rw-r--r--   0 root         (0) root         (0)     1993 2024-03-11 12:43:49.000000 empire-platform-api-public-client-3.0.6/test/test_invoice_summary.py
--rw-r--r--   0 root         (0) root         (0)     1723 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_invoice_vat_rate.py
--rw-r--r--   0 root         (0) root         (0)     5863 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_auction.py
--rw-r--r--   0 root         (0) root         (0)     2518 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid.py
--rw-r--r--   0 root         (0) root         (0)     2446 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid_result.py
--rw-r--r--   0 root         (0) root         (0)     3392 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid_result_batch.py
--rw-r--r--   0 root         (0) root         (0)     1885 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid_results.py
--rw-r--r--   0 root         (0) root         (0)     1007 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     4405 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     2557 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_auction_results_allocated_capacity.py
--rw-r--r--   0 root         (0) root         (0)     2182 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_auction_results_bids.py
--rw-r--r--   0 root         (0) root         (0)     2848 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     1868 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_offered_capacity.py
--rw-r--r--   0 root         (0) root         (0)     2348 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_reserve_price.py
--rw-r--r--   0 root         (0) root         (0)     1913 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_long_term_reserve_price_steps.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_manual_file_upload_api.py
--rw-r--r--   0 root         (0) root         (0)     1842 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_manual_file_upload_request.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_market.py
--rw-r--r--   0 root         (0) root         (0)     2502 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_message.py
--rw-r--r--   0 root         (0) root         (0)     3530 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_message_batch.py
--rw-r--r--   0 root         (0) root         (0)      940 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_message_category.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_message_sender.py
--rw-r--r--   0 root         (0) root         (0)      940 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_message_severity.py
--rw-r--r--   0 root         (0) root         (0)      927 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_message_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      912 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_message_type.py
--rw-r--r--   0 root         (0) root         (0)     1245 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_messages_api.py
--rw-r--r--   0 root         (0) root         (0)      955 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)     1736 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_mtu_period.py
--rw-r--r--   0 root         (0) root         (0)      884 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_mtu_size.py
--rw-r--r--   0 root         (0) root         (0)     1978 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_mtu_size_per_auction_product_type.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_mtu_size_per_timescale.py
--rw-r--r--   0 root         (0) root         (0)     1669 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_nested_error.py
--rw-r--r--   0 root         (0) root         (0)     1715 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_nomination_api.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_nomination_capacity_resolution.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_nomination_restriction_type.py
--rw-r--r--   0 root         (0) root         (0)      976 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_noticeboard_entry_type.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_noticeboard_entry_type_with_both.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_notification_preference.py
--rw-r--r--   0 root         (0) root         (0)     1886 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_notification_preference_with_sms.py
--rw-r--r--   0 root         (0) root         (0)     1851 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_ntc_overview_mtu_data.py
--rw-r--r--   0 root         (0) root         (0)      976 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_offered_capacity_setup.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1247 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_api.py
--rw-r--r--   0 root         (0) root         (0)      990 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_auth_method.py
--rw-r--r--   0 root         (0) root         (0)     5954 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_contact.py
--rw-r--r--   0 root         (0) root         (0)    11039 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_contact_information.py
--rw-r--r--   0 root         (0) root         (0)     3480 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_api.py
--rw-r--r--   0 root         (0) root         (0)     4509 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_batch.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_file_type.py
--rw-r--r--   0 root         (0) root         (0)     3119 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_options.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1019 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1018 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_status.py
--rw-r--r--   0 root         (0) root         (0)     2555 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_uploaded_by_user.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_uploaded_by_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1885 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_document_user.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_file_settings.py
--rw-r--r--   0 root         (0) root         (0)     3355 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_market_settings.py
--rw-r--r--   0 root         (0) root         (0)     2221 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_market_settings_gb_nomination_settings.py
--rw-r--r--   0 root         (0) root         (0)     2172 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_market_settings_nl_nomination_settings.py
--rw-r--r--   0 root         (0) root         (0)      961 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_status.py
--rw-r--r--   0 root         (0) root         (0)      947 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_type.py
--rw-r--r--   0 root         (0) root         (0)     6297 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_user.py
--rw-r--r--   0 root         (0) root         (0)     7009 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_user_batch.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_organisation_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_other_party.py
--rw-r--r--   0 root         (0) root         (0)     1727 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant.py
--rw-r--r--   0 root         (0) root         (0)     2770 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_api.py
--rw-r--r--   0 root         (0) root         (0)     2199 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_default_bids_and_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     3833 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_finance_overview_data.py
--rw-r--r--   0 root         (0) root         (0)     2607 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_finance_overview_invoice.py
--rw-r--r--   0 root         (0) root         (0)     3943 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_data.py
--rw-r--r--   0 root         (0) root         (0)     3306 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2723 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_data_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     4008 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_graph_data.py
--rw-r--r--   0 root         (0) root         (0)     3447 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2419 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2284 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     5565 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_messages.py
--rw-r--r--   0 root         (0) root         (0)     3943 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_netted_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     3340 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_netted_nominations_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2348 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_netted_nominations_data_mtus_aggregated_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2298 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_netted_nominations_data_mtus_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2951 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_next_auction.py
--rw-r--r--   0 root         (0) root         (0)     7431 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_next_auctions_and_nomination_gates.py
--rw-r--r--   0 root         (0) root         (0)     4451 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     3770 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2793 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     2597 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_values_nomination_restriction.py
--rw-r--r--   0 root         (0) root         (0)     3682 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data.py
--rw-r--r--   0 root         (0) root         (0)     3111 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2508 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)    13963 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_organisation_details.py
--rw-r--r--   0 root         (0) root         (0)     1037 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_participant_overview_api.py
--rw-r--r--   0 root         (0) root         (0)    13355 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_overview_data.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_overview_data_contact_information.py
--rw-r--r--   0 root         (0) root         (0)     2119 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_overview_data_finance_overview.py
--rw-r--r--   0 root         (0) root         (0)     2073 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_participant_overview_data_organisation_members.py
--rw-r--r--   0 root         (0) root         (0)      904 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_permission.py
--rw-r--r--   0 root         (0) root         (0)      961 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_platform_appearance.py
--rw-r--r--   0 root         (0) root         (0)     9632 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_profile.py
--rw-r--r--   0 root         (0) root         (0)     1878 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_profile_api.py
--rw-r--r--   0 root         (0) root         (0)     6602 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_profile_details.py
--rw-r--r--   0 root         (0) root         (0)     6518 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_profile_user.py
--rw-r--r--   0 root         (0) root         (0)     1957 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_profile_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     3975 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_aggregated_nominations_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     3390 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_aggregated_nominations_overview_response_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2322 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_aggregated_nominations_overview_response_mtus_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2277 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_aggregated_nominations_overview_response_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     1225 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_public_allocated_auction_api.py
--rw-r--r--   0 root         (0) root         (0)     3880 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_allocated_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     3171 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_auction.py
--rw-r--r--   0 root         (0) root         (0)     2243 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_public_auction_api.py
--rw-r--r--   0 root         (0) root         (0)     3867 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_auction_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     1012 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_auction_filter_status.py
--rw-r--r--   0 root         (0) root         (0)      969 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_auction_status.py
--rw-r--r--   0 root         (0) root         (0)     5142 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_day_ahead_auction.py
--rw-r--r--   0 root         (0) root         (0)     2909 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_day_ahead_or_intra_day_auction_mtu_results.py
--rw-r--r--   0 root         (0) root         (0)     2405 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_day_ahead_or_intra_day_auction_mtu_results_bids.py
--rw-r--r--   0 root         (0) root         (0)     3636 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_day_ahead_or_intra_day_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     5142 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_intra_day_auction.py
--rw-r--r--   0 root         (0) root         (0)     5328 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_long_term_auction.py
--rw-r--r--   0 root         (0) root         (0)     3496 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_long_term_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     2245 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_public_long_term_auction_results_bids.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_public_nominations_api.py
--rw-r--r--   0 root         (0) root         (0)     1873 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_purchased_by_organisation.py
--rw-r--r--   0 root         (0) root         (0)     3216 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_reporting_api.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_reserve_price_publish_type.py
--rw-r--r--   0 root         (0) root         (0)     2392 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_return_auction.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_sage_code.py
--rw-r--r--   0 root         (0) root         (0)     5595 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_api.py
--rw-r--r--   0 root         (0) root         (0)     1943 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_capacity_price_mtu.py
--rw-r--r--   0 root         (0) root         (0)    11251 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     3310 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py
--rw-r--r--   0 root         (0) root         (0)     2998 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py
--rw-r--r--   0 root         (0) root         (0)     7374 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py
--rw-r--r--   0 root         (0) root         (0)     2407 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2843 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_options.py
--rw-r--r--   0 root         (0) root         (0)     2940 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py
--rw-r--r--   0 root         (0) root         (0)     4443 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2224 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2942 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options.py
--rw-r--r--   0 root         (0) root         (0)     2365 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus.py
--rw-r--r--   0 root         (0) root         (0)     8232 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2663 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_entry_details.py
--rw-r--r--   0 root         (0) root         (0)     6617 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_entry_response.py
--rw-r--r--   0 root         (0) root         (0)     2020 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_options.py
--rw-r--r--   0 root         (0) root         (0)     2117 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_response_options.py
--rw-r--r--   0 root         (0) root         (0)     2047 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_transfer_request_options.py
--rw-r--r--   0 root         (0) root         (0)     2949 2024-03-11 12:43:50.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     3775 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_noticeboard_entry_batch.py
--rw-r--r--   0 root         (0) root         (0)     1097 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_noticeboard_entry_status.py
--rw-r--r--   0 root         (0) root         (0)     3735 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_return_request.py
--rw-r--r--   0 root         (0) root         (0)     4567 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_return_request_batch.py
--rw-r--r--   0 root         (0) root         (0)     1076 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_return_request_status.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     4629 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_request_batch.py
--rw-r--r--   0 root         (0) root         (0)     1090 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_request_status.py
--rw-r--r--   0 root         (0) root         (0)     1076 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_request_type.py
--rw-r--r--   0 root         (0) root         (0)     2202 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_transmission_rights_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2305 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_settlement.py
--rw-r--r--   0 root         (0) root         (0)     1810 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_settlement_item.py
--rw-r--r--   0 root         (0) root         (0)     2485 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_settlement_per_source.py
--rw-r--r--   0 root         (0) root         (0)      976 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_settlement_source_type.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_settlement_sub_source_type.py
--rw-r--r--   0 root         (0) root         (0)     2950 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_source_auction.py
--rw-r--r--   0 root         (0) root         (0)     1954 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_source_auction_display_data.py
--rw-r--r--   0 root         (0) root         (0)     1831 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_source_auction_result.py
--rw-r--r--   0 root         (0) root         (0)     3534 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_submit_day_ahead_or_intra_day_bids_request.py
--rw-r--r--   0 root         (0) root         (0)     2965 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_bids.py
--rw-r--r--   0 root         (0) root         (0)     2671 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_submit_long_term_bids_request.py
--rw-r--r--   0 root         (0) root         (0)     2185 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_submit_long_term_bids_request_bids.py
--rw-r--r--   0 root         (0) root         (0)     1775 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_submit_nominations_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2306 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_submit_timescale_nominations_request.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_system_message_category.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_mtu_status.py
--rw-r--r--   0 root         (0) root         (0)     2189 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     2069 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_options_window_timing.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_status.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_type.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_window_status.py
--rw-r--r--   0 root         (0) root         (0)     3296 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_timescale_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2350 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_timescale_nominations_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2113 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_timescale_nominations_mtus_current_nomination.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_transmission_right_api.py
--rw-r--r--   0 root         (0) root         (0)     3795 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_transmission_rights_overview.py
--rw-r--r--   0 root         (0) root         (0)     3278 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_transmission_rights_overview_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2633 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_transmission_rights_overview_mtus_values.py
--rw-r--r--   0 root         (0) root         (0)     2086 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_transmission_rights_overview_mtus_values_timescales.py
--rw-r--r--   0 root         (0) root         (0)     1729 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_uiosi_not_resold.py
--rw-r--r--   0 root         (0) root         (0)     3216 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_uiosi_overview.py
--rw-r--r--   0 root         (0) root         (0)     2728 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_uiosi_overview_per_mtu.py
--rw-r--r--   0 root         (0) root         (0)     1788 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_uiosi_resold.py
--rw-r--r--   0 root         (0) root         (0)     1739 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_unread_messages_response.py
--rw-r--r--   0 root         (0) root         (0)     3715 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_update_day_ahead_or_intra_day_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2862 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_update_day_ahead_or_intra_day_default_bid_request_bids.py
--rw-r--r--   0 root         (0) root         (0)     2238 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_update_day_ahead_or_intra_day_default_bid_request_bids_mtus.py
--rw-r--r--   0 root         (0) root         (0)     2554 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_update_default_nomination_request.py
--rw-r--r--   0 root         (0) root         (0)     2578 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_update_long_term_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     1928 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_update_profile_details_request.py
--rw-r--r--   0 root         (0) root         (0)     1887 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     6507 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_user.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-03-11 12:43:52.000000 empire-platform-api-public-client-3.0.6/test/test_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1788 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     4232 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_user_preferences.py
--rw-r--r--   0 root         (0) root         (0)     3166 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_user_preferences_general_notifications.py
--rw-r--r--   0 root         (0) root         (0)     2600 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_user_preferences_subscription_notifications.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_user_role.py
--rw-r--r--   0 root         (0) root         (0)      905 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_user_status.py
--rw-r--r--   0 root         (0) root         (0)      913 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_vat_rate_type.py
--rw-r--r--   0 root         (0) root         (0)     1631 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_version.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-03-11 12:43:51.000000 empire-platform-api-public-client-3.0.6/test/test_zendesk_chat_token_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:50:43.429079 empire-platform-api-public-client-3.0.7/
+-rw-r--r--   0 root         (0) root         (0)      568 2024-04-15 08:50:43.429079 empire-platform-api-public-client-3.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    55385 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:50:43.359080 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/
+-rw-r--r--   0 root         (0) root         (0)    43655 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:50:43.359080 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26235 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/allocated_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)    10436 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/attachment_api.py
+-rw-r--r--   0 root         (0) root         (0)   126206 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/auction_api.py
+-rw-r--r--   0 root         (0) root         (0)    19476 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/audit_log_api.py
+-rw-r--r--   0 root         (0) root         (0)    15523 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/bidding_configuration_api.py
+-rw-r--r--   0 root         (0) root         (0)    17494 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/buy_now_offers_api.py
+-rw-r--r--   0 root         (0) root         (0)    73532 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/default_bid_api.py
+-rw-r--r--   0 root         (0) root         (0)    48329 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/default_nomination_api.py
+-rw-r--r--   0 root         (0) root         (0)    47142 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/finance_api.py
+-rw-r--r--   0 root         (0) root         (0)     8015 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/finance_information_api.py
+-rw-r--r--   0 root         (0) root         (0)    24382 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/manual_file_upload_api.py
+-rw-r--r--   0 root         (0) root         (0)    30817 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/messages_api.py
+-rw-r--r--   0 root         (0) root         (0)     6792 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    51180 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/nomination_api.py
+-rw-r--r--   0 root         (0) root         (0)    20162 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/organisation_api.py
+-rw-r--r--   0 root         (0) root         (0)    35765 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/organisation_document_api.py
+-rw-r--r--   0 root         (0) root         (0)    71824 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/participant_dashboard_api.py
+-rw-r--r--   0 root         (0) root         (0)     8059 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/participant_overview_api.py
+-rw-r--r--   0 root         (0) root         (0)    55942 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/profile_api.py
+-rw-r--r--   0 root         (0) root         (0)    22948 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/public_allocated_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)    69040 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/public_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)     8795 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/public_nominations_api.py
+-rw-r--r--   0 root         (0) root         (0)   142505 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/reporting_api.py
+-rw-r--r--   0 root         (0) root         (0)   214379 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/secondary_market_api.py
+-rw-r--r--   0 root         (0) root         (0)    11195 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/transmission_right_api.py
+-rw-r--r--   0 root         (0) root         (0)    49549 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/user_api.py
+-rw-r--r--   0 root         (0) root         (0)    30604 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api_client.py
+-rw-r--r--   0 root         (0) root         (0)      852 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api_response.py
+-rw-r--r--   0 root         (0) root         (0)    15731 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5598 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:50:43.389080 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/
+-rw-r--r--   0 root         (0) root         (0)    40703 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     5328 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_allocated_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     2439 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nomination_options_nominee_participants.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nomination_type.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2914 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb.py
+-rw-r--r--   0 root         (0) root         (0)     3990 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_mtu_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_mtu_value.py
+-rw-r--r--   0 root         (0) root         (0)     2852 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_nl.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_eprogram_values.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_pre_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_pre_nomination_options_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     5292 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/allocated_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/allocated_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/allocated_auction_participant_status.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/allocated_auction_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/attachment.py
+-rw-r--r--   0 root         (0) root         (0)     5832 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_allocation_resolution.py
+-rw-r--r--   0 root         (0) root         (0)     2818 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_bid_participant.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     3086 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_bidding_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_bidding_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_filter_status.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_intra_day_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     6529 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_process_steps_absolute.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_reduction_period.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_result_congestion_rent.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_result_participant.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_status.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     4663 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_domain.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_payload.py
+-rw-r--r--   0 root         (0) root         (0)      963 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      933 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_status.py
+-rw-r--r--   0 root         (0) root         (0)     8159 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_type.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_user.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bid_value.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bidding_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3112 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bidding_configuration_per_direction.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bidding_configuration_secondary_market_notices.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bidding_configuration_values.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/border_direction.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/border_direction_with_both.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/border_direction_with_both_and_none.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/buy_now_day_ahead_offer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     5687 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/buy_now_offer.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/buy_now_offer_mtus.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/buy_now_offer_status.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_api_key_request.py
+-rw-r--r--   0 root         (0) root         (0)     5997 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     3752 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_default_nomination_request.py
+-rw-r--r--   0 root         (0) root         (0)     5761 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_long_term_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_organisation_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     3924 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_long_term_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_return_request.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_default_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_organisation_document.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_long_term_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_return_request_identifier.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/credit_cover_type.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/dashboard_next_nomination_gate.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/dashboard_next_nomination_gate_window.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/dashboard_next_nomination_window_status.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/date_period.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/date_time_period.py
+-rw-r--r--   0 root         (0) root         (0)     6273 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group.py
+-rw-r--r--   0 root         (0) root         (0)     3235 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2861 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_bid_results.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_batch.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_bids.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_bids_bid.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2920 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_value.py
+-rw-r--r--   0 root         (0) root         (0)     4161 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     5984 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid_bids_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid_options.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      941 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_declaration_type.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_details.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     1342 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_status.py
+-rw-r--r--   0 root         (0) root         (0)     9640 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/error_code.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     5470 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_bank_deposits.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_letter_of_credits.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_lockable_amount.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_lockable_date.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_lockable_period.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_market_vat_details.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_sage_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6273 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/intra_day_auction.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_batch.py
+-rw-r--r--   0 root         (0) root         (0)     8176 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_details.py
+-rw-r--r--   0 root         (0) root         (0)     3168 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_history.py
+-rw-r--r--   0 root         (0) root         (0)     4486 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_line_item.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_participant_details.py
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_status.py
+-rw-r--r--   0 root         (0) root         (0)     3964 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_vat_rate.py
+-rw-r--r--   0 root         (0) root         (0)     6429 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid.py
+-rw-r--r--   0 root         (0) root         (0)     3797 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid_result.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid_result_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid_results.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_results_allocated_capacity.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_results_bids.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_offered_capacity.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_reserve_price.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_reserve_price_steps.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/manual_file_upload_request.py
+-rw-r--r--   0 root         (0) root         (0)      873 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/market.py
+-rw-r--r--   0 root         (0) root         (0)     4125 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_batch.py
+-rw-r--r--   0 root         (0) root         (0)      978 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_category.py
+-rw-r--r--   0 root         (0) root         (0)      918 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_sender.py
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_type.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/mtu_period.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/mtu_size.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/mtu_size_per_auction_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/mtu_size_per_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/nested_error.py
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/nomination_capacity_resolution.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/nomination_restriction_type.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/noticeboard_entry_type.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/noticeboard_entry_type_with_both.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/notification_preference.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/notification_preference_with_sms.py
+-rw-r--r--   0 root         (0) root         (0)     3498 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/ntc_overview_mtu_data.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/offered_capacity_setup.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_auth_method.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_contact.py
+-rw-r--r--   0 root         (0) root         (0)     3339 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_contact_information.py
+-rw-r--r--   0 root         (0) root         (0)     4298 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_file_type.py
+-rw-r--r--   0 root         (0) root         (0)     3068 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_options.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      995 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_status.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_uploaded_by_user.py
+-rw-r--r--   0 root         (0) root         (0)     2439 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_uploaded_by_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_user.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_file_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_market_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_market_settings_gb_nomination_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_market_settings_nl_nomination_settings.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_status.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_type.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_user.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_user_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/other_party.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_default_bids_and_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_finance_overview_data.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_finance_overview_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     3143 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data.py
+-rw-r--r--   0 root         (0) root         (0)     4434 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     3207 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     4504 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_aggregated_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     4903 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_next_auction.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_next_auctions_and_nomination_gates.py
+-rw-r--r--   0 root         (0) root         (0)     3252 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     3720 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     4041 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_values_nomination_restriction.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     4429 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_organisation_details.py
+-rw-r--r--   0 root         (0) root         (0)     5035 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_overview_data.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_overview_data_contact_information.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_overview_data_finance_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_overview_data_organisation_members.py
+-rw-r--r--   0 root         (0) root         (0)     6843 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/permission.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/platform_appearance.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/profile.py
+-rw-r--r--   0 root         (0) root         (0)     3081 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/profile_details.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/profile_user.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/profile_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     3115 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_allocated_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction_filter_status.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction_status.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_day_ahead_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results.py
+-rw-r--r--   0 root         (0) root         (0)     3117 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results_bids.py
+-rw-r--r--   0 root         (0) root         (0)     3628 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_intra_day_auction.py
+-rw-r--r--   0 root         (0) root         (0)     5877 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_long_term_auction.py
+-rw-r--r--   0 root         (0) root         (0)     4169 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_long_term_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_long_term_auction_results_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/purchased_by_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/reserve_price_publish_type.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/return_auction.py
+-rw-r--r--   0 root         (0) root         (0)     5215 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/sage_code.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_capacity_price_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     4592 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4594 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py
+-rw-r--r--   0 root         (0) root         (0)     4952 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py
+-rw-r--r--   0 root         (0) root         (0)     4120 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_options.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py
+-rw-r--r--   0 root         (0) root         (0)     6549 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4309 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_details.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_response.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_options.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_response_options.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_transfer_request_options.py
+-rw-r--r--   0 root         (0) root         (0)     5332 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_status.py
+-rw-r--r--   0 root         (0) root         (0)     4441 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_return_request.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_return_request_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_return_request_status.py
+-rw-r--r--   0 root         (0) root         (0)     6453 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_request_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_request_status.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_request_type.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_transmission_rights_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement_item.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement_per_source.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement_sub_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/source_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/source_auction_display_data.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/source_auction_result.py
+-rw-r--r--   0 root         (0) root         (0)     2914 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_long_term_bids_request.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_long_term_bids_request_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_nominations_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_timescale_nominations_request.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/system_message_category.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_mtu_status.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_options_window_timing.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_status.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_type.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_window_status.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     5019 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nominations_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nominations_mtus_current_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/transmission_rights_overview.py
+-rw-r--r--   0 root         (0) root         (0)     3356 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/transmission_rights_overview_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/transmission_rights_overview_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/transmission_rights_overview_mtus_values_timescales.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/uiosi_not_resold.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/uiosi_overview.py
+-rw-r--r--   0 root         (0) root         (0)     4015 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/uiosi_overview_per_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/uiosi_resold.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/unread_messages_response.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request_bids.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request_bids_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     3318 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_default_nomination_request.py
+-rw-r--r--   0 root         (0) root         (0)     5075 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_long_term_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_profile_details_request.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_preferences.py
+-rw-r--r--   0 root         (0) root         (0)     3806 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_preferences_general_notifications.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_preferences_subscription_notifications.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_role.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_status.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/vat_rate_type.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/version.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/zendesk_chat_token_response.py
+-rw-r--r--   0 root         (0) root         (0)    13115 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:50:43.359080 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      568 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    45898 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-15 08:50:43.000000 empire-platform-api-public-client-3.0.7/empire_platform_api_public_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-15 08:50:43.429079 empire-platform-api-public-client-3.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1646 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:50:43.429079 empire-platform-api-public-client-3.0.7/test/
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_address.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_allocated_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nomination_options_nominee_participants.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nomination_type.py
+-rw-r--r--   0 root         (0) root         (0)     8340 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_mns_or_gb.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_mns_or_gb_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_mtu_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_mtu_value.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_nl.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_nl_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_nl_mtus_eprogram_values.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_pre_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_aggregated_pre_nomination_options_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_allocated_auction.py
+-rw-r--r--   0 root         (0) root         (0)     1166 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_allocated_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)     3807 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_allocated_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_allocated_auction_participant_status.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_allocated_auction_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_attachment.py
+-rw-r--r--   0 root         (0) root         (0)      977 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_attachment_api.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_allocation_resolution.py
+-rw-r--r--   0 root         (0) root         (0)     3220 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_bid_participant.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_bidding_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      962 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_bidding_mode.py
+-rw-r--r--   0 root         (0) root         (0)      969 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_filter_status.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_intra_day_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_process_steps_absolute.py
+-rw-r--r--   0 root         (0) root         (0)      962 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_reduction_period.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_result_congestion_rent.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_result_participant.py
+-rw-r--r--   0 root         (0) root         (0)      927 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_status.py
+-rw-r--r--   0 root         (0) root         (0)      947 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_auction_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_api.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_batch.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_domain.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_payload.py
+-rw-r--r--   0 root         (0) root         (0)      935 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_status.py
+-rw-r--r--   0 root         (0) root         (0)      920 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_type.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_user.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_audit_log_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_bid_value.py
+-rw-r--r--   0 root         (0) root         (0)     3326 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_bidding_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_bidding_configuration_api.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2024-04-15 08:50:38.000000 empire-platform-api-public-client-3.0.7/test/test_bidding_configuration_per_direction.py
+-rw-r--r--   0 root         (0) root         (0)     2131 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_bidding_configuration_secondary_market_notices.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_bidding_configuration_values.py
+-rw-r--r--   0 root         (0) root         (0)      940 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_border_direction.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_border_direction_with_both.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_border_direction_with_both_and_none.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_buy_now_day_ahead_offer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_buy_now_offer.py
+-rw-r--r--   0 root         (0) root         (0)     1738 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_buy_now_offer_mtus.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_buy_now_offer_status.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_buy_now_offers_api.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_api_key_request.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_day_ahead_or_intra_day_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_day_ahead_or_intra_day_default_bid_request_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_default_nomination_request.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_long_term_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_organisation_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     7234 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     6649 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_long_term_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_long_term_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_return_request.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_default_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_organisation_document.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_long_term_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_long_term_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_return_request_identifier.py
+-rw-r--r--   0 root         (0) root         (0)      941 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_credit_cover_type.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_dashboard_next_nomination_gate.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_dashboard_next_nomination_gate_window.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_dashboard_next_nomination_window_status.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_date_period.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_date_time_period.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_auction.py
+-rw-r--r--   0 root         (0) root         (0)     4056 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_bids_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_bids_bid_results.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_result.py
+-rw-r--r--   0 root         (0) root         (0)     4730 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_result_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_result_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_result_bids_bid.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_mtu_results.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_mtu_results_bids.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_participant_results.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_participant_results_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_value.py
+-rw-r--r--   0 root         (0) root         (0)     3831 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_results_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     3873 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_default_bid_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_default_bid_bids_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_default_bid_api.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_bid_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_bid_options.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_bid_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_default_nomination_api.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_nomination_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_nomination_declaration_type.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_nomination_details.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_nomination_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_nomination_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_default_nomination_status.py
+-rw-r--r--   0 root         (0) root         (0)      898 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_error_code.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_finance_api.py
+-rw-r--r--   0 root         (0) root         (0)     9777 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_finance_information.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_finance_information_api.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_finance_information_bank_deposits.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_finance_information_letter_of_credits.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_finance_information_lockable_amount.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_finance_information_lockable_date.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_finance_information_lockable_period.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_finance_information_market_vat_details.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_finance_information_sage_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_intra_day_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice.py
+-rw-r--r--   0 root         (0) root         (0)      955 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice_batch.py
+-rw-r--r--   0 root         (0) root         (0)     7263 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice_details.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice_history.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice_line_item.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice_participant_details.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice_status.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice_summary.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_invoice_vat_rate.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid_result.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid_result_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid_results.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     4405 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     2557 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_auction_results_allocated_capacity.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_auction_results_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_offered_capacity.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-04-15 08:50:39.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_reserve_price.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_long_term_reserve_price_steps.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_manual_file_upload_api.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_manual_file_upload_request.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_market.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_message_batch.py
+-rw-r--r--   0 root         (0) root         (0)      940 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_message_category.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_message_sender.py
+-rw-r--r--   0 root         (0) root         (0)      940 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_message_severity.py
+-rw-r--r--   0 root         (0) root         (0)      927 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_message_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      912 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_messages_api.py
+-rw-r--r--   0 root         (0) root         (0)      955 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_mtu_period.py
+-rw-r--r--   0 root         (0) root         (0)      884 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_mtu_size.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_mtu_size_per_auction_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_mtu_size_per_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_nested_error.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_nomination_api.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_nomination_capacity_resolution.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_nomination_restriction_type.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_noticeboard_entry_type.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_noticeboard_entry_type_with_both.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_notification_preference.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_notification_preference_with_sms.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_ntc_overview_mtu_data.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_offered_capacity_setup.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_api.py
+-rw-r--r--   0 root         (0) root         (0)      990 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_auth_method.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_contact.py
+-rw-r--r--   0 root         (0) root         (0)    11039 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_contact_information.py
+-rw-r--r--   0 root         (0) root         (0)     3480 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_api.py
+-rw-r--r--   0 root         (0) root         (0)     4509 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_file_type.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_options.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1019 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_status.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_uploaded_by_user.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_uploaded_by_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_document_user.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_file_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_market_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_market_settings_gb_nomination_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_market_settings_nl_nomination_settings.py
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_status.py
+-rw-r--r--   0 root         (0) root         (0)      947 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_type.py
+-rw-r--r--   0 root         (0) root         (0)     6297 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_user.py
+-rw-r--r--   0 root         (0) root         (0)     7009 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_user_batch.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_organisation_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_other_party.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant.py
+-rw-r--r--   0 root         (0) root         (0)     2770 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_api.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_default_bids_and_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     3833 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_finance_overview_data.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_finance_overview_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_data.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_data_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_graph_data.py
+-rw-r--r--   0 root         (0) root         (0)     3447 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_netted_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     3340 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_netted_nominations_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_netted_nominations_data_mtus_aggregated_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_netted_nominations_data_mtus_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_next_auction.py
+-rw-r--r--   0 root         (0) root         (0)     7431 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_next_auctions_and_nomination_gates.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_values_nomination_restriction.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)    13963 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_organisation_details.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_participant_overview_api.py
+-rw-r--r--   0 root         (0) root         (0)    13355 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_overview_data.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_overview_data_contact_information.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_overview_data_finance_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_participant_overview_data_organisation_members.py
+-rw-r--r--   0 root         (0) root         (0)      904 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_platform_appearance.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_profile_api.py
+-rw-r--r--   0 root         (0) root         (0)     6602 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_profile_details.py
+-rw-r--r--   0 root         (0) root         (0)     6518 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_profile_user.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_profile_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     3975 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_aggregated_nominations_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_aggregated_nominations_overview_response_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_aggregated_nominations_overview_response_mtus_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_aggregated_nominations_overview_response_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_public_allocated_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_allocated_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     3171 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_public_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)     3867 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_auction_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_auction_filter_status.py
+-rw-r--r--   0 root         (0) root         (0)      969 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_auction_status.py
+-rw-r--r--   0 root         (0) root         (0)     5142 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_day_ahead_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_day_ahead_or_intra_day_auction_mtu_results.py
+-rw-r--r--   0 root         (0) root         (0)     2405 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_day_ahead_or_intra_day_auction_mtu_results_bids.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_day_ahead_or_intra_day_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     5142 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_intra_day_auction.py
+-rw-r--r--   0 root         (0) root         (0)     5328 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_long_term_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3496 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_long_term_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_public_long_term_auction_results_bids.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_public_nominations_api.py
+-rw-r--r--   0 root         (0) root         (0)     1873 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_purchased_by_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_reporting_api.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_reserve_price_publish_type.py
+-rw-r--r--   0 root         (0) root         (0)     2392 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_return_auction.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_sage_code.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_api.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_capacity_price_mtu.py
+-rw-r--r--   0 root         (0) root         (0)    11251 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_options.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py
+-rw-r--r--   0 root         (0) root         (0)     4443 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     8232 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_entry_details.py
+-rw-r--r--   0 root         (0) root         (0)     6617 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_entry_response.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_options.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_response_options.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_transfer_request_options.py
+-rw-r--r--   0 root         (0) root         (0)     2949 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_noticeboard_entry_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_noticeboard_entry_status.py
+-rw-r--r--   0 root         (0) root         (0)     3735 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_return_request.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_return_request_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_return_request_status.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     4629 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_request_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_request_status.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_request_type.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_transmission_rights_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_settlement.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_settlement_item.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-04-15 08:50:40.000000 empire-platform-api-public-client-3.0.7/test/test_settlement_per_source.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_settlement_source_type.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_settlement_sub_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_source_auction.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_source_auction_display_data.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_source_auction_result.py
+-rw-r--r--   0 root         (0) root         (0)     3534 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_submit_day_ahead_or_intra_day_bids_request.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_submit_long_term_bids_request.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_submit_long_term_bids_request_bids.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_submit_nominations_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_submit_timescale_nominations_request.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_system_message_category.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_mtu_status.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_options_window_timing.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_status.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_type.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_window_status.py
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_timescale_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_timescale_nominations_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_timescale_nominations_mtus_current_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_transmission_right_api.py
+-rw-r--r--   0 root         (0) root         (0)     3795 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_transmission_rights_overview.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_transmission_rights_overview_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2633 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_transmission_rights_overview_mtus_values.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_transmission_rights_overview_mtus_values_timescales.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_uiosi_not_resold.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_uiosi_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_uiosi_overview_per_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_uiosi_resold.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_unread_messages_response.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_update_day_ahead_or_intra_day_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_update_day_ahead_or_intra_day_default_bid_request_bids.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_update_day_ahead_or_intra_day_default_bid_request_bids_mtus.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_update_default_nomination_request.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_update_long_term_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_update_profile_details_request.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     6507 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_user.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-04-15 08:50:42.000000 empire-platform-api-public-client-3.0.7/test/test_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     4232 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_user_preferences.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_user_preferences_general_notifications.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_user_preferences_subscription_notifications.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_user_role.py
+-rw-r--r--   0 root         (0) root         (0)      905 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_user_status.py
+-rw-r--r--   0 root         (0) root         (0)      913 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_vat_rate_type.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-15 08:50:41.000000 empire-platform-api-public-client-3.0.7/test/test_zendesk_chat_token_response.py
```

### Comparing `empire-platform-api-public-client-3.0.6/PKG-INFO` & `empire-platform-api-public-client-3.0.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empire-platform-api-public-client
-Version: 3.0.6
+Version: 3.0.7
 Summary: Platform API
 Home-page: UNKNOWN
 Author: BritNed
 Author-email: britned.info@britned.com
 License: UNKNOWN
 Description:     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API&#39;s [GitHub repository](https://github.com/britned/empire-platform-api)
```

### Comparing `empire-platform-api-public-client-3.0.6/README.md` & `empire-platform-api-public-client-3.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 ---
 
 Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api)
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 3.0.6
-- Package version: 3.0.6
+- API version: 3.0.7
+- Package version: 3.0.7
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.britned.com](https://www.britned.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/__init__.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "3.0.6"
+__version__ = "3.0.7"
 
 # import apis into sdk package
 from empire_platform_api_public_client.api.allocated_auction_api import AllocatedAuctionApi
 from empire_platform_api_public_client.api.attachment_api import AttachmentApi
 from empire_platform_api_public_client.api.auction_api import AuctionApi
 from empire_platform_api_public_client.api.audit_log_api import AuditLogApi
 from empire_platform_api_public_client.api.bidding_configuration_api import BiddingConfigurationApi
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/__init__.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/allocated_auction_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/allocated_auction_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/attachment_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/attachment_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/auction_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/auction_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/audit_log_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/audit_log_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/bidding_configuration_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/bidding_configuration_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/buy_now_offers_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/buy_now_offers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/default_bid_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/default_bid_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/default_nomination_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/default_nomination_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/finance_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/finance_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/finance_information_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/finance_information_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/manual_file_upload_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/manual_file_upload_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/messages_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/messages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/metadata_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/nomination_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/nomination_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/organisation_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/organisation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/organisation_document_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/organisation_document_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/participant_dashboard_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/participant_dashboard_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/participant_overview_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/participant_overview_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/profile_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/profile_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/public_allocated_auction_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/public_allocated_auction_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/public_auction_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/public_auction_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/public_nominations_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/public_nominations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/reporting_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/reporting_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/secondary_market_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/secondary_market_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/transmission_right_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/transmission_right_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api/user_api.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api_client.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.0.6/python'
+        self.user_agent = 'OpenAPI-Generator/3.0.7/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/api_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/api_response.py`

 * *Files identical despite different names*

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/configuration.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -393,16 +393,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 3.0.6\n"\
-               "SDK Package Version: 3.0.6".\
+               "Version of the API: 3.0.7\n"\
+               "SDK Package Version: 3.0.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/exceptions.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/__init__.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/address.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_allocated_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_allocated_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nomination_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nomination_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nomination_options_nominee_participants.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nomination_options_nominee_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nomination_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nomination_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_mtu_netted_nominations.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_mtu_netted_nominations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_mtu_value.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_mtu_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_nl.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_nl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_eprogram_values.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_eprogram_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_pre_nomination_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_pre_nomination_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/aggregated_pre_nomination_options_timescale.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/aggregated_pre_nomination_options_timescale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/allocated_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/allocated_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/allocated_auction_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/allocated_auction_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/allocated_auction_participant_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/allocated_auction_participant_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/allocated_auction_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/allocated_auction_sort_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/api_key.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/api_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/attachment.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_allocation_resolution.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_allocation_resolution.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_bid_participant.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_bid_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_bid_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_bid_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_bidding_configuration.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_bidding_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_bidding_mode.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_bidding_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_filter_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_filter_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_intra_day_product_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_intra_day_product_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_process_steps_absolute.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_process_steps_absolute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_product_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_product_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_reduction_period.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_reduction_period.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_result_congestion_rent.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_result_congestion_rent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_result_participant.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_result_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_sort_by.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/auction_timescale.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/auction_timescale.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_api_key.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_domain.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_domain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_payload.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_sort_by.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_user.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/audit_log_user_organisation.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/audit_log_user_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bid_value.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bid_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bidding_configuration.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bidding_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bidding_configuration_per_direction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bidding_configuration_per_direction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bidding_configuration_secondary_market_notices.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bidding_configuration_secondary_market_notices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/bidding_configuration_values.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/bidding_configuration_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/border_direction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/border_direction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/border_direction_with_both.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/border_direction_with_both.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/border_direction_with_both_and_none.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/border_direction_with_both_and_none.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/buy_now_day_ahead_offer_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/buy_now_day_ahead_offer_sort_by.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/buy_now_offer.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/buy_now_offer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/buy_now_offer_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/buy_now_offer_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/buy_now_offer_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/buy_now_offer_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_api_key_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_api_key_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_default_nomination_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_default_nomination_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_long_term_default_bid_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_long_term_default_bid_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_organisation_document_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_organisation_document_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_long_term_transfer_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_long_term_transfer_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/create_secondary_market_return_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/create_secondary_market_return_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_api_key.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_api_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_default_bid.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_default_bid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_default_nomination.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_default_nomination.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_organisation_document.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_organisation_document.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_long_term_transfer_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_long_term_transfer_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/created_secondary_market_return_request_identifier.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/created_secondary_market_return_request_identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/credit_cover_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/credit_cover_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/dashboard_next_nomination_gate.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/dashboard_next_nomination_gate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/dashboard_next_nomination_gate_window.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/dashboard_next_nomination_gate_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/dashboard_next_nomination_window_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/dashboard_next_nomination_window_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/date_period.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/date_period.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/date_time_period.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/date_time_period.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_bid.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_bid_results.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_bid_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_bids_bid.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_result_bids_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results_bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_value.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results_mtu.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results_mtu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid_bids_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid_bids_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid_sort_by.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_bid_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_bid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_declaration_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_declaration_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_details.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_mtu.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_mtu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/default_nomination_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/default_nomination_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/error_code.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/error_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/error_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_bank_deposits.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_bank_deposits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_letter_of_credits.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_letter_of_credits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_lockable_amount.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_lockable_amount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_lockable_date.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_lockable_date.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_lockable_period.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_lockable_period.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_market_vat_details.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_market_vat_details.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/finance_information_sage_settings.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/finance_information_sage_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/intra_day_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/intra_day_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_action_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_action_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_details.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_history.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_line_item.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_line_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_participant_details.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_participant_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_summary.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/invoice_vat_rate.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/invoice_vat_rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid_result.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid_result_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid_result_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid_results.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_bid_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_bid_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_results.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_results_allocated_capacity.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_results_allocated_capacity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_auction_results_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_auction_results_bids.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_default_bid.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_default_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_offered_capacity.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_offered_capacity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_reserve_price.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_reserve_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/long_term_reserve_price_steps.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/long_term_reserve_price_steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/manual_file_upload_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/manual_file_upload_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/market.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_category.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_category.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_sender.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_severity.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_severity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_sort_by.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/message_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/message_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/mtu_period.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/mtu_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/mtu_size.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/mtu_size.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/mtu_size_per_auction_product_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/mtu_size_per_auction_product_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/mtu_size_per_timescale.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/mtu_size_per_timescale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/nested_error.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/nested_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/nomination_capacity_resolution.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/nomination_capacity_resolution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/nomination_restriction_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/nomination_restriction_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/noticeboard_entry_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/noticeboard_entry_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/noticeboard_entry_type_with_both.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/noticeboard_entry_type_with_both.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/notification_preference.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/notification_preference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/notification_preference_with_sms.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/notification_preference_with_sms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/ntc_overview_mtu_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/ntc_overview_mtu_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/offered_capacity_setup.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/offered_capacity_setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_auth_method.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_auth_method.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_contact.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_contact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_contact_information.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_contact_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_file_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_file_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_organisation.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_organisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_uploaded_by_user.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_uploaded_by_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_uploaded_by_user_organisation.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_uploaded_by_user_organisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_document_user.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_document_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_file_settings.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_file_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_market_settings.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_market_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_market_settings_gb_nomination_settings.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_market_settings_gb_nomination_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_market_settings_nl_nomination_settings.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_market_settings_nl_nomination_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_user.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_user_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_user_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/organisation_user_sort_by.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/organisation_user_sort_by.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/other_party.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/other_party.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_default_bids_and_nominations_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_default_bids_and_nominations_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_finance_overview_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_finance_overview_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_finance_overview_invoice.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_finance_overview_invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_values.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_netted_nominations.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_netted_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_values.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_messages.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_aggregated_nominations.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_aggregated_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_netted_nominations.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_netted_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_next_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_next_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_next_auctions_and_nomination_gates.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_next_auctions_and_nomination_gates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_values.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_values_nomination_restriction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_values_nomination_restriction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_values.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_organisation_details.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_organisation_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_overview_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_overview_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_overview_data_contact_information.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_overview_data_contact_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_overview_data_finance_overview.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_overview_data_finance_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/participant_overview_data_organisation_members.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/participant_overview_data_organisation_members.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/permission.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/platform_appearance.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/platform_appearance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/profile.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/profile_details.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/profile_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/profile_user.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/profile_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/profile_user_organisation.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/profile_user_organisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_netted_nominations.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_netted_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_values.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_allocated_auction_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_allocated_auction_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction_bid_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction_bid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction_filter_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction_filter_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_auction_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_auction_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_day_ahead_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_day_ahead_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results_bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_results.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_intra_day_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_intra_day_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_long_term_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_long_term_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_long_term_auction_results.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_long_term_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/public_long_term_auction_results_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/public_long_term_auction_results_bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/purchased_by_organisation.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/purchased_by_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/reserve_price_publish_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/reserve_price_publish_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/return_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/return_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/sage_code.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/sage_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_capacity_price_mtu.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_capacity_price_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_details.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_response_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_response_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_long_term_transfer_request_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_long_term_transfer_request_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_return_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_return_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_return_request_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_return_request_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_return_request_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_return_request_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_request_batch.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_request_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_request_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_request_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_request_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_request_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/secondary_market_transfer_transmission_rights_mtu.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/secondary_market_transfer_transmission_rights_mtu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement_item.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement_per_source.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement_per_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement_source_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement_source_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/settlement_sub_source_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/settlement_sub_source_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/source_auction.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/source_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/source_auction_display_data.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/source_auction_display_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/source_auction_result.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/source_auction_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_long_term_bids_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_long_term_bids_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_long_term_bids_request_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_long_term_bids_request_bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_nominations_mtu.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_nominations_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/submit_timescale_nominations_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/submit_timescale_nominations_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/system_message_category.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/system_message_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_mtu_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_mtu_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_options.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_options_window_timing.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_options_window_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nomination_window_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nomination_window_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nominations.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nominations_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nominations_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/timescale_nominations_mtus_current_nomination.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/timescale_nominations_mtus_current_nomination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/transmission_rights_overview.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/transmission_rights_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/transmission_rights_overview_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/transmission_rights_overview_mtus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/transmission_rights_overview_mtus_values.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/transmission_rights_overview_mtus_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/transmission_rights_overview_mtus_values_timescales.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/transmission_rights_overview_mtus_values_timescales.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/uiosi_not_resold.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/uiosi_not_resold.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/uiosi_overview.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/uiosi_overview.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/uiosi_overview_per_mtu.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/uiosi_overview_per_mtu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/uiosi_resold.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/uiosi_resold.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/unread_messages_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/unread_messages_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request_bids.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request_bids_mtus.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request_bids_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_default_nomination_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_default_nomination_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_long_term_default_bid_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_long_term_default_bid_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_profile_details_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_profile_details_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/update_user_request.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/update_user_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_organisation.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_organisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_preferences.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_preferences_general_notifications.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_preferences_general_notifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_preferences_subscription_notifications.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_preferences_subscription_notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_role.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/user_status.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/user_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/vat_rate_type.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/vat_rate_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/version.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/models/zendesk_chat_token_response.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/models/zendesk_chat_token_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client/rest.py` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client.egg-info/PKG-INFO` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empire-platform-api-public-client
-Version: 3.0.6
+Version: 3.0.7
 Summary: Platform API
 Home-page: UNKNOWN
 Author: BritNed
 Author-email: britned.info@britned.com
 License: UNKNOWN
 Description:     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API&#39;s [GitHub repository](https://github.com/britned/empire-platform-api)
```

### Comparing `empire-platform-api-public-client-3.0.6/empire_platform_api_public_client.egg-info/SOURCES.txt` & `empire-platform-api-public-client-3.0.7/empire_platform_api_public_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `empire-platform-api-public-client-3.0.6/pyproject.toml` & `empire-platform-api-public-client-3.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "empire_platform_api_public_client"
-version = "3.0.6"
+version = "3.0.7"
 description = "Platform API"
 authors = ["BritNed <britned.info@britned.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Platform API"]
 include = ["empire_platform_api_public_client/py.typed"]
```

### Comparing `empire-platform-api-public-client-3.0.6/setup.py` & `empire-platform-api-public-client-3.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "empire-platform-api-public-client"
-VERSION = "3.0.6"
+VERSION = "3.0.7"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_address.py` & `empire-platform-api-public-client-3.0.7/test/test_address.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_allocated_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_allocated_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nomination_options.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nomination_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nomination_options_nominee_participants.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nomination_options_nominee_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nomination_type.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nomination_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_mns_or_gb.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_mns_or_gb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_mns_or_gb_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_mns_or_gb_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_mtu_netted_nominations.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_mtu_netted_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_mtu_value.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_mtu_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_nl.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_nl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_nl_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_nl_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_nominations_nl_mtus_eprogram_values.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_nominations_nl_mtus_eprogram_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_pre_nomination_options.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_pre_nomination_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_aggregated_pre_nomination_options_timescale.py` & `empire-platform-api-public-client-3.0.7/test/test_aggregated_pre_nomination_options_timescale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_allocated_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_allocated_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_allocated_auction_api.py` & `empire-platform-api-public-client-3.0.7/test/test_allocated_auction_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_allocated_auction_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_allocated_auction_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_allocated_auction_participant_status.py` & `empire-platform-api-public-client-3.0.7/test/test_allocated_auction_participant_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_allocated_auction_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_allocated_auction_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_api_key.py` & `empire-platform-api-public-client-3.0.7/test/test_api_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_attachment.py` & `empire-platform-api-public-client-3.0.7/test/test_attachment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_attachment_api.py` & `empire-platform-api-public-client-3.0.7/test/test_attachment_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_allocation_resolution.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_allocation_resolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_api.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_bid_participant.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_bid_participant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_bid_status.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_bid_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_bidding_configuration.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_bidding_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_bidding_mode.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_bidding_mode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_filter_status.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_filter_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_intra_day_product_type.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_intra_day_product_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_process_steps_absolute.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_process_steps_absolute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_product_type.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_product_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_reduction_period.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_reduction_period.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_result_congestion_rent.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_result_congestion_rent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_result_participant.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_result_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_status.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_auction_timescale.py` & `empire-platform-api-public-client-3.0.7/test/test_auction_timescale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_api.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_api_key.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_domain.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_payload.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_status.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_type.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_user.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_audit_log_user_organisation.py` & `empire-platform-api-public-client-3.0.7/test/test_audit_log_user_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_bid_value.py` & `empire-platform-api-public-client-3.0.7/test/test_bid_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_bidding_configuration.py` & `empire-platform-api-public-client-3.0.7/test/test_bidding_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_bidding_configuration_api.py` & `empire-platform-api-public-client-3.0.7/test/test_bidding_configuration_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_bidding_configuration_per_direction.py` & `empire-platform-api-public-client-3.0.7/test/test_bidding_configuration_per_direction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_bidding_configuration_secondary_market_notices.py` & `empire-platform-api-public-client-3.0.7/test/test_bidding_configuration_secondary_market_notices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_bidding_configuration_values.py` & `empire-platform-api-public-client-3.0.7/test/test_bidding_configuration_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_border_direction.py` & `empire-platform-api-public-client-3.0.7/test/test_border_direction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_border_direction_with_both.py` & `empire-platform-api-public-client-3.0.7/test/test_border_direction_with_both.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_border_direction_with_both_and_none.py` & `empire-platform-api-public-client-3.0.7/test/test_border_direction_with_both_and_none.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_buy_now_day_ahead_offer_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_buy_now_day_ahead_offer_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_buy_now_offer.py` & `empire-platform-api-public-client-3.0.7/test/test_buy_now_offer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_buy_now_offer_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_buy_now_offer_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_buy_now_offer_status.py` & `empire-platform-api-public-client-3.0.7/test/test_buy_now_offer_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_buy_now_offers_api.py` & `empire-platform-api-public-client-3.0.7/test/test_buy_now_offers_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_api_key_request.py` & `empire-platform-api-public-client-3.0.7/test/test_create_api_key_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_day_ahead_or_intra_day_default_bid_request.py` & `empire-platform-api-public-client-3.0.7/test/test_create_day_ahead_or_intra_day_default_bid_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_day_ahead_or_intra_day_default_bid_request_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_create_day_ahead_or_intra_day_default_bid_request_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_default_nomination_request.py` & `empire-platform-api-public-client-3.0.7/test/test_create_default_nomination_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_long_term_default_bid_request.py` & `empire-platform-api-public-client-3.0.7/test/test_create_long_term_default_bid_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_organisation_document_request.py` & `empire-platform-api-public-client-3.0.7/test/test_create_organisation_document_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py` & `empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_long_term_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_long_term_noticeboard_response.py` & `empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_long_term_noticeboard_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_long_term_transfer_request.py` & `empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_long_term_transfer_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_create_secondary_market_return_request.py` & `empire-platform-api-public-client-3.0.7/test/test_create_secondary_market_return_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_api_key.py` & `empire-platform-api-public-client-3.0.7/test/test_created_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_default_bid.py` & `empire-platform-api-public-client-3.0.7/test/test_created_default_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_default_nomination.py` & `empire-platform-api-public-client-3.0.7/test/test_created_default_nomination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_organisation_document.py` & `empire-platform-api-public-client-3.0.7/test/test_created_organisation_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py` & `empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_long_term_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_long_term_noticeboard_response.py` & `empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_long_term_noticeboard_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_long_term_transfer_request.py` & `empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_long_term_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_created_secondary_market_return_request_identifier.py` & `empire-platform-api-public-client-3.0.7/test/test_created_secondary_market_return_request_identifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_credit_cover_type.py` & `empire-platform-api-public-client-3.0.7/test/test_credit_cover_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_dashboard_next_nomination_gate.py` & `empire-platform-api-public-client-3.0.7/test/test_dashboard_next_nomination_gate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_dashboard_next_nomination_gate_window.py` & `empire-platform-api-public-client-3.0.7/test/test_dashboard_next_nomination_gate_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_dashboard_next_nomination_window_status.py` & `empire-platform-api-public-client-3.0.7/test/test_dashboard_next_nomination_window_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_date_period.py` & `empire-platform-api-public-client-3.0.7/test/test_date_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_date_time_period.py` & `empire-platform-api-public-client-3.0.7/test/test_date_time_period.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_bids_bid.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_bids_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_bids_bid_results.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_bids_bid_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_result.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_result_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_result_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_result_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_result_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_bid_group_result_bids_bid.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_bid_group_result_bids_bid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_mtu.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_mtu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_mtu_results.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_mtu_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_mtu_results_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_mtu_results_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_participant_results.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_participant_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_participant_results_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_participant_results_mtus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_value.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_results.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_auction_results_mtu.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_auction_results_mtu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_default_bid.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_default_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_default_bid_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_default_bid_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_day_ahead_or_intra_day_default_bid_bids_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_day_ahead_or_intra_day_default_bid_bids_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_bid.py` & `empire-platform-api-public-client-3.0.7/test/test_default_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_bid_api.py` & `empire-platform-api-public-client-3.0.7/test/test_default_bid_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_bid_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_default_bid_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_bid_options.py` & `empire-platform-api-public-client-3.0.7/test/test_default_bid_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_bid_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_default_bid_sort_by.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_bid_status.py` & `empire-platform-api-public-client-3.0.7/test/test_default_bid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_nomination.py` & `empire-platform-api-public-client-3.0.7/test/test_default_nomination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_nomination_api.py` & `empire-platform-api-public-client-3.0.7/test/test_default_nomination_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_nomination_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_default_nomination_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_nomination_declaration_type.py` & `empire-platform-api-public-client-3.0.7/test/test_default_nomination_declaration_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_nomination_details.py` & `empire-platform-api-public-client-3.0.7/test/test_default_nomination_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_nomination_mtu.py` & `empire-platform-api-public-client-3.0.7/test/test_default_nomination_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_nomination_options.py` & `empire-platform-api-public-client-3.0.7/test/test_default_nomination_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_nomination_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_default_nomination_sort_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_default_nomination_status.py` & `empire-platform-api-public-client-3.0.7/test/test_default_nomination_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_error_code.py` & `empire-platform-api-public-client-3.0.7/test/test_error_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_error_response.py` & `empire-platform-api-public-client-3.0.7/test/test_error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_api.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_information.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_information_api.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_information_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_information_bank_deposits.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_information_bank_deposits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_information_letter_of_credits.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_information_letter_of_credits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_information_lockable_amount.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_information_lockable_amount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_information_lockable_date.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_information_lockable_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_information_lockable_period.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_information_lockable_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_information_market_vat_details.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_information_market_vat_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_finance_information_sage_settings.py` & `empire-platform-api-public-client-3.0.7/test/test_finance_information_sage_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_intra_day_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_intra_day_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice_action_type.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice_action_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice_batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice_details.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice_history.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice_line_item.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice_line_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice_participant_details.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice_participant_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice_status.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice_summary.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice_summary.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_invoice_vat_rate.py` & `empire-platform-api-public-client-3.0.7/test/test_invoice_vat_rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid_result.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid_result_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid_result_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid_results.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_auction_bid_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_auction_bid_sort_by.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_auction_results.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_auction_results_allocated_capacity.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_auction_results_allocated_capacity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_auction_results_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_auction_results_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_default_bid.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_default_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_offered_capacity.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_offered_capacity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_reserve_price.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_reserve_price.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_long_term_reserve_price_steps.py` & `empire-platform-api-public-client-3.0.7/test/test_long_term_reserve_price_steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_manual_file_upload_api.py` & `empire-platform-api-public-client-3.0.7/test/test_manual_file_upload_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_manual_file_upload_request.py` & `empire-platform-api-public-client-3.0.7/test/test_manual_file_upload_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_market.py` & `empire-platform-api-public-client-3.0.7/test/test_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_message.py` & `empire-platform-api-public-client-3.0.7/test/test_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_message_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_message_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_message_category.py` & `empire-platform-api-public-client-3.0.7/test/test_message_category.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_message_sender.py` & `empire-platform-api-public-client-3.0.7/test/test_message_sender.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_message_severity.py` & `empire-platform-api-public-client-3.0.7/test/test_message_severity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_message_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_message_sort_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_message_type.py` & `empire-platform-api-public-client-3.0.7/test/test_message_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_messages_api.py` & `empire-platform-api-public-client-3.0.7/test/test_messages_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_metadata_api.py` & `empire-platform-api-public-client-3.0.7/test/test_metadata_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_mtu_period.py` & `empire-platform-api-public-client-3.0.7/test/test_mtu_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_mtu_size.py` & `empire-platform-api-public-client-3.0.7/test/test_mtu_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_mtu_size_per_auction_product_type.py` & `empire-platform-api-public-client-3.0.7/test/test_mtu_size_per_auction_product_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_mtu_size_per_timescale.py` & `empire-platform-api-public-client-3.0.7/test/test_mtu_size_per_timescale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_nested_error.py` & `empire-platform-api-public-client-3.0.7/test/test_nested_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_nomination_api.py` & `empire-platform-api-public-client-3.0.7/test/test_nomination_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_nomination_capacity_resolution.py` & `empire-platform-api-public-client-3.0.7/test/test_nomination_capacity_resolution.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_nomination_restriction_type.py` & `empire-platform-api-public-client-3.0.7/test/test_nomination_restriction_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_noticeboard_entry_type.py` & `empire-platform-api-public-client-3.0.7/test/test_noticeboard_entry_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_noticeboard_entry_type_with_both.py` & `empire-platform-api-public-client-3.0.7/test/test_noticeboard_entry_type_with_both.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_notification_preference.py` & `empire-platform-api-public-client-3.0.7/test/test_notification_preference.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_notification_preference_with_sms.py` & `empire-platform-api-public-client-3.0.7/test/test_notification_preference_with_sms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_ntc_overview_mtu_data.py` & `empire-platform-api-public-client-3.0.7/test/test_ntc_overview_mtu_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_offered_capacity_setup.py` & `empire-platform-api-public-client-3.0.7/test/test_offered_capacity_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_api.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_auth_method.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_auth_method.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_contact.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_contact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_contact_information.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_contact_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_api.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_file_type.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_file_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_options.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_organisation.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_organisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_status.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_uploaded_by_user.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_uploaded_by_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_uploaded_by_user_organisation.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_uploaded_by_user_organisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_document_user.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_document_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_file_settings.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_file_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_market_settings.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_market_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_market_settings_gb_nomination_settings.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_market_settings_gb_nomination_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_market_settings_nl_nomination_settings.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_market_settings_nl_nomination_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_status.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_type.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_user.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_user_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_user_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_organisation_user_sort_by.py` & `empire-platform-api-public-client-3.0.7/test/test_organisation_user_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_other_party.py` & `empire-platform-api-public-client-3.0.7/test/test_other_party.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant.py` & `empire-platform-api-public-client-3.0.7/test/test_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_api.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_default_bids_and_nominations_data.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_default_bids_and_nominations_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_finance_overview_data.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_finance_overview_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_finance_overview_invoice.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_finance_overview_invoice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_data.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_data_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_data_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_data_mtus_values.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_data_mtus_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_graph_data.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_graph_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_netted_nominations.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_netted_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_values.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_messages.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_netted_nominations_data.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_netted_nominations_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_netted_nominations_data_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_netted_nominations_data_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_netted_nominations_data_mtus_aggregated_nominations.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_netted_nominations_data_mtus_aggregated_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_netted_nominations_data_mtus_netted_nominations.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_netted_nominations_data_mtus_netted_nominations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_next_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_next_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_next_auctions_and_nomination_gates.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_next_auctions_and_nomination_gates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_data.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_values.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_values_nomination_restriction.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_values_nomination_restriction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_values.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_organisation_details.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_organisation_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_overview_api.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_overview_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_overview_data.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_overview_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_overview_data_contact_information.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_overview_data_contact_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_overview_data_finance_overview.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_overview_data_finance_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_participant_overview_data_organisation_members.py` & `empire-platform-api-public-client-3.0.7/test/test_participant_overview_data_organisation_members.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_permission.py` & `empire-platform-api-public-client-3.0.7/test/test_permission.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_platform_appearance.py` & `empire-platform-api-public-client-3.0.7/test/test_platform_appearance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_profile.py` & `empire-platform-api-public-client-3.0.7/test/test_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_profile_api.py` & `empire-platform-api-public-client-3.0.7/test/test_profile_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_profile_details.py` & `empire-platform-api-public-client-3.0.7/test/test_profile_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_profile_user.py` & `empire-platform-api-public-client-3.0.7/test/test_profile_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_profile_user_organisation.py` & `empire-platform-api-public-client-3.0.7/test/test_profile_user_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_aggregated_nominations_overview_response.py` & `empire-platform-api-public-client-3.0.7/test/test_public_aggregated_nominations_overview_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_aggregated_nominations_overview_response_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_public_aggregated_nominations_overview_response_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_aggregated_nominations_overview_response_mtus_netted_nominations.py` & `empire-platform-api-public-client-3.0.7/test/test_public_aggregated_nominations_overview_response_mtus_netted_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_aggregated_nominations_overview_response_mtus_values.py` & `empire-platform-api-public-client-3.0.7/test/test_public_aggregated_nominations_overview_response_mtus_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_allocated_auction_api.py` & `empire-platform-api-public-client-3.0.7/test/test_public_allocated_auction_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_allocated_auction_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_public_allocated_auction_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_public_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_auction_api.py` & `empire-platform-api-public-client-3.0.7/test/test_public_auction_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_auction_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_public_auction_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_auction_bid_status.py` & `empire-platform-api-public-client-3.0.7/test/test_public_auction_bid_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_auction_filter_status.py` & `empire-platform-api-public-client-3.0.7/test/test_public_auction_filter_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_auction_status.py` & `empire-platform-api-public-client-3.0.7/test/test_public_auction_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_day_ahead_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_public_day_ahead_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_day_ahead_or_intra_day_auction_mtu_results.py` & `empire-platform-api-public-client-3.0.7/test/test_public_day_ahead_or_intra_day_auction_mtu_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_day_ahead_or_intra_day_auction_mtu_results_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_public_day_ahead_or_intra_day_auction_mtu_results_bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_day_ahead_or_intra_day_auction_results.py` & `empire-platform-api-public-client-3.0.7/test/test_public_day_ahead_or_intra_day_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_intra_day_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_public_intra_day_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_long_term_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_public_long_term_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_long_term_auction_results.py` & `empire-platform-api-public-client-3.0.7/test/test_public_long_term_auction_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_long_term_auction_results_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_public_long_term_auction_results_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_public_nominations_api.py` & `empire-platform-api-public-client-3.0.7/test/test_public_nominations_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_purchased_by_organisation.py` & `empire-platform-api-public-client-3.0.7/test/test_purchased_by_organisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_reporting_api.py` & `empire-platform-api-public-client-3.0.7/test/test_reporting_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_reserve_price_publish_type.py` & `empire-platform-api-public-client-3.0.7/test/test_reserve_price_publish_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_return_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_return_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_sage_code.py` & `empire-platform-api-public-client-3.0.7/test/test_sage_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_api.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_capacity_price_mtu.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_capacity_price_mtu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_options.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_entry_details.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_entry_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_entry_response.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_entry_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_options.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_noticeboard_response_options.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_noticeboard_response_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_long_term_transfer_request_options.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_long_term_transfer_request_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_noticeboard_entry.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_noticeboard_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_noticeboard_entry_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_noticeboard_entry_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_noticeboard_entry_status.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_noticeboard_entry_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_return_request.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_return_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_return_request_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_return_request_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_return_request_status.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_return_request_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_request.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_request_batch.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_request_batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_request_status.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_request_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_request_type.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_request_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_secondary_market_transfer_transmission_rights_mtu.py` & `empire-platform-api-public-client-3.0.7/test/test_secondary_market_transfer_transmission_rights_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_settlement.py` & `empire-platform-api-public-client-3.0.7/test/test_settlement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_settlement_item.py` & `empire-platform-api-public-client-3.0.7/test/test_settlement_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_settlement_per_source.py` & `empire-platform-api-public-client-3.0.7/test/test_settlement_per_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_settlement_source_type.py` & `empire-platform-api-public-client-3.0.7/test/test_settlement_source_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_settlement_sub_source_type.py` & `empire-platform-api-public-client-3.0.7/test/test_settlement_sub_source_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_source_auction.py` & `empire-platform-api-public-client-3.0.7/test/test_source_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_source_auction_display_data.py` & `empire-platform-api-public-client-3.0.7/test/test_source_auction_display_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_source_auction_result.py` & `empire-platform-api-public-client-3.0.7/test/test_source_auction_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_submit_day_ahead_or_intra_day_bids_request.py` & `empire-platform-api-public-client-3.0.7/test/test_submit_day_ahead_or_intra_day_bids_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups.py` & `empire-platform-api-public-client-3.0.7/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_submit_long_term_bids_request.py` & `empire-platform-api-public-client-3.0.7/test/test_submit_long_term_bids_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_submit_long_term_bids_request_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_submit_long_term_bids_request_bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_submit_nominations_mtu.py` & `empire-platform-api-public-client-3.0.7/test/test_submit_nominations_mtu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_submit_timescale_nominations_request.py` & `empire-platform-api-public-client-3.0.7/test/test_submit_timescale_nominations_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_system_message_category.py` & `empire-platform-api-public-client-3.0.7/test/test_system_message_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_mtu_status.py` & `empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_mtu_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_options.py` & `empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_options_window_timing.py` & `empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_options_window_timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_status.py` & `empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_type.py` & `empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_timescale_nomination_window_status.py` & `empire-platform-api-public-client-3.0.7/test/test_timescale_nomination_window_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_timescale_nominations.py` & `empire-platform-api-public-client-3.0.7/test/test_timescale_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_timescale_nominations_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_timescale_nominations_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_timescale_nominations_mtus_current_nomination.py` & `empire-platform-api-public-client-3.0.7/test/test_timescale_nominations_mtus_current_nomination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_transmission_right_api.py` & `empire-platform-api-public-client-3.0.7/test/test_transmission_right_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_transmission_rights_overview.py` & `empire-platform-api-public-client-3.0.7/test/test_transmission_rights_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_transmission_rights_overview_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_transmission_rights_overview_mtus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_transmission_rights_overview_mtus_values.py` & `empire-platform-api-public-client-3.0.7/test/test_transmission_rights_overview_mtus_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_transmission_rights_overview_mtus_values_timescales.py` & `empire-platform-api-public-client-3.0.7/test/test_transmission_rights_overview_mtus_values_timescales.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_uiosi_not_resold.py` & `empire-platform-api-public-client-3.0.7/test/test_uiosi_not_resold.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_uiosi_overview.py` & `empire-platform-api-public-client-3.0.7/test/test_uiosi_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_uiosi_overview_per_mtu.py` & `empire-platform-api-public-client-3.0.7/test/test_uiosi_overview_per_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_uiosi_resold.py` & `empire-platform-api-public-client-3.0.7/test/test_uiosi_resold.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_unread_messages_response.py` & `empire-platform-api-public-client-3.0.7/test/test_unread_messages_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_update_day_ahead_or_intra_day_default_bid_request.py` & `empire-platform-api-public-client-3.0.7/test/test_update_day_ahead_or_intra_day_default_bid_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_update_day_ahead_or_intra_day_default_bid_request_bids.py` & `empire-platform-api-public-client-3.0.7/test/test_update_day_ahead_or_intra_day_default_bid_request_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_update_day_ahead_or_intra_day_default_bid_request_bids_mtus.py` & `empire-platform-api-public-client-3.0.7/test/test_update_day_ahead_or_intra_day_default_bid_request_bids_mtus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_update_default_nomination_request.py` & `empire-platform-api-public-client-3.0.7/test/test_update_default_nomination_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_update_long_term_default_bid_request.py` & `empire-platform-api-public-client-3.0.7/test/test_update_long_term_default_bid_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_update_profile_details_request.py` & `empire-platform-api-public-client-3.0.7/test/test_update_profile_details_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_update_user_request.py` & `empire-platform-api-public-client-3.0.7/test/test_update_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_user.py` & `empire-platform-api-public-client-3.0.7/test/test_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_user_api.py` & `empire-platform-api-public-client-3.0.7/test/test_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_user_organisation.py` & `empire-platform-api-public-client-3.0.7/test/test_user_organisation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_user_preferences.py` & `empire-platform-api-public-client-3.0.7/test/test_user_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_user_preferences_general_notifications.py` & `empire-platform-api-public-client-3.0.7/test/test_user_preferences_general_notifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_user_preferences_subscription_notifications.py` & `empire-platform-api-public-client-3.0.7/test/test_user_preferences_subscription_notifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_user_role.py` & `empire-platform-api-public-client-3.0.7/test/test_user_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_user_status.py` & `empire-platform-api-public-client-3.0.7/test/test_user_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_vat_rate_type.py` & `empire-platform-api-public-client-3.0.7/test/test_vat_rate_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_version.py` & `empire-platform-api-public-client-3.0.7/test/test_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `empire-platform-api-public-client-3.0.6/test/test_zendesk_chat_token_response.py` & `empire-platform-api-public-client-3.0.7/test/test_zendesk_chat_token_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Platform API
 
     _OpenAPI specification for the **Platform API** of **Empire**, the allocation and nomination platform of BritNed_  ---  Additional documentation available in the API's [GitHub repository](https://github.com/britned/empire-platform-api) 
 
-    The version of the OpenAPI document: 3.0.6
+    The version of the OpenAPI document: 3.0.7
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

