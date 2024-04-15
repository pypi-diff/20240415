# Comparing `tmp/longship-2024.3.15.tar.gz` & `tmp/longship-2024.4.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longship-2024.3.15.tar", max compression
+gzip compressed data, was "longship-2024.4.15.tar", max compression
```

## Comparing `longship-2024.3.15.tar` & `longship-2024.4.15.tar`

### file list

```diff
@@ -1,331 +1,331 @@
--rw-r--r--   0        0        0     1072 2023-06-26 16:00:19.878825 longship-2024.3.15/LICENSE
--rw-r--r--   0        0        0     4661 2023-06-26 16:47:23.288883 longship-2024.3.15/README.md
--rw-r--r--   0        0        0     7668 2024-03-14 10:00:43.390594 longship-2024.3.15/longship/client.py
--rw-r--r--   0        0        0      112 2023-06-26 16:00:19.886682 longship-2024.3.15/longship/errors.py
--rw-r--r--   0        0        0     4614 2024-03-14 15:13:41.390085 longship-2024.3.15/longship/types.py
--rw-r--r--   0        0        0      155 2024-03-14 10:00:43.400336 longship-2024.3.15/longship_api_client/__init__.py
--rw-r--r--   0        0        0       45 2024-03-14 10:00:43.406391 longship-2024.3.15/longship_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.682314 longship-2024.3.15/longship_api_client/api/cdrs/__init__.py
--rw-r--r--   0        0        0     4458 2024-03-14 10:00:43.406514 longship-2024.3.15/longship_api_client/api/cdrs/cdr_get.py
--rw-r--r--   0        0        0     5023 2024-03-14 10:00:43.407007 longship-2024.3.15/longship_api_client/api/cdrs/cdr_patch.py
--rw-r--r--   0        0        0    19502 2024-03-14 10:00:43.406262 longship-2024.3.15/longship_api_client/api/cdrs/get_all_cdrs.py
--rw-r--r--   0        0        0     7993 2024-03-14 10:00:43.405805 longship-2024.3.15/longship_api_client/api/cdrs/get_all_interchangeformat.py
--rw-r--r--   0        0        0     5989 2024-03-14 10:00:43.406956 longship-2024.3.15/longship_api_client/api/cdrs/get_file_full_download_cdrs.py
--rw-r--r--   0        0        0     5968 2024-03-14 10:00:43.405408 longship-2024.3.15/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.674498 longship-2024.3.15/longship_api_client/api/chargepoint_status/__init__.py
--rw-r--r--   0        0        0     4767 2024-03-14 10:00:43.385685 longship-2024.3.15/longship_api_client/api/chargepoint_status/chargepoint_status_get.py
--rw-r--r--   0        0        0     6490 2024-03-14 10:00:43.387537 longship-2024.3.15/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.675963 longship-2024.3.15/longship_api_client/api/chargepoints/__init__.py
--rw-r--r--   0        0        0     4634 2024-03-14 10:00:43.392589 longship-2024.3.15/longship_api_client/api/chargepoints/chargepoint_get.py
--rw-r--r--   0        0        0     5162 2024-03-14 10:00:43.395682 longship-2024.3.15/longship_api_client/api/chargepoints/chargepoint_put.py
--rw-r--r--   0        0        0     5416 2024-03-14 10:00:43.394060 longship-2024.3.15/longship_api_client/api/chargepoints/chargepointauthorization_get.py
--rw-r--r--   0        0        0     5252 2024-03-14 10:00:43.396354 longship-2024.3.15/longship_api_client/api/chargepoints/chargepointauthorization_post.py
--rw-r--r--   0        0        0     9920 2024-03-14 10:00:43.395091 longship-2024.3.15/longship_api_client/api/chargepoints/get_all_chargepointauthorizations.py
--rw-r--r--   0        0        0    11723 2024-03-14 10:00:43.397704 longship-2024.3.15/longship_api_client/api/chargepoints/get_all_chargepointmessages.py
--rw-r--r--   0        0        0    16896 2024-03-14 10:00:43.393744 longship-2024.3.15/longship_api_client/api/chargepoints/get_all_chargepoints.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.692551 longship-2024.3.15/longship_api_client/api/commands/__init__.py
--rw-r--r--   0        0        0     5151 2024-03-14 10:00:43.390456 longship-2024.3.15/longship_api_client/api/commands/send_cancel_reservation_request.py
--rw-r--r--   0        0        0     5171 2024-03-14 10:00:43.389505 longship-2024.3.15/longship_api_client/api/commands/send_change_availability_request.py
--rw-r--r--   0        0        0     5191 2024-03-14 10:00:43.387399 longship-2024.3.15/longship_api_client/api/commands/send_change_configuration_request.py
--rw-r--r--   0        0        0     5011 2024-03-14 10:00:43.392082 longship-2024.3.15/longship_api_client/api/commands/send_clear_cache_request.py
--rw-r--r--   0        0        0     5212 2024-03-14 10:00:43.391762 longship-2024.3.15/longship_api_client/api/commands/send_clear_charging_profile_request.py
--rw-r--r--   0        0        0     5051 2024-03-14 10:00:43.385739 longship-2024.3.15/longship_api_client/api/commands/send_data_transfer_request.py
--rw-r--r--   0        0        0     5212 2024-03-14 10:00:43.386023 longship-2024.3.15/longship_api_client/api/commands/send_get_composite_schedule_request.py
--rw-r--r--   0        0        0     5131 2024-03-14 10:00:43.388186 longship-2024.3.15/longship_api_client/api/commands/send_get_configuration_request.py
--rw-r--r--   0        0        0     5091 2024-03-14 10:00:43.393330 longship-2024.3.15/longship_api_client/api/commands/send_get_diagnostics_request.py
--rw-r--r--   0        0        0     5193 2024-03-14 10:00:43.387750 longship-2024.3.15/longship_api_client/api/commands/send_get_local_list_version_request.py
--rw-r--r--   0        0        0     5241 2024-03-14 10:00:43.389115 longship-2024.3.15/longship_api_client/api/commands/send_remote_start_transaction_request.py
--rw-r--r--   0        0        0     5221 2024-03-14 10:00:43.393928 longship-2024.3.15/longship_api_client/api/commands/send_remote_stop_transaction_request.py
--rw-r--r--   0        0        0     5011 2024-03-14 10:00:43.393637 longship-2024.3.15/longship_api_client/api/commands/send_reserve_now_request.py
--rw-r--r--   0        0        0     4946 2024-03-14 10:00:43.394233 longship-2024.3.15/longship_api_client/api/commands/send_reset_request.py
--rw-r--r--   0        0        0     5072 2024-03-14 10:00:43.387393 longship-2024.3.15/longship_api_client/api/commands/send_send_local_list_request.py
--rw-r--r--   0        0        0     5172 2024-03-14 10:00:43.392386 longship-2024.3.15/longship_api_client/api/commands/send_set_charging_profile_request.py
--rw-r--r--   0        0        0     5091 2024-03-14 10:00:43.390998 longship-2024.3.15/longship_api_client/api/commands/send_trigger_message_request.py
--rw-r--r--   0        0        0     5111 2024-03-14 10:00:43.393047 longship-2024.3.15/longship_api_client/api/commands/send_unlock_connector_request.py
--rw-r--r--   0        0        0     5091 2024-03-14 10:00:43.387713 longship-2024.3.15/longship_api_client/api/commands/send_update_firmware_request.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.716248 longship-2024.3.15/longship_api_client/api/configurationitems/__init__.py
--rw-r--r--   0        0        0     5527 2024-03-14 10:00:43.400607 longship-2024.3.15/longship_api_client/api/configurationitems/configurationitem_get.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.702887 longship-2024.3.15/longship_api_client/api/localtokengroups/__init__.py
--rw-r--r--   0        0        0     6508 2024-03-14 10:00:43.391514 longship-2024.3.15/longship_api_client/api/localtokengroups/get_all_localtokengroups.py
--rw-r--r--   0        0        0     4437 2024-03-14 10:00:43.393156 longship-2024.3.15/longship_api_client/api/localtokengroups/local_token_group_delete.py
--rw-r--r--   0        0        0     5028 2024-03-14 10:00:43.392314 longship-2024.3.15/longship_api_client/api/localtokengroups/local_token_group_post.py
--rw-r--r--   0        0        0     5243 2024-03-14 10:00:43.392682 longship-2024.3.15/longship_api_client/api/localtokengroups/local_token_group_put.py
--rw-r--r--   0        0        0     4764 2024-03-14 10:00:43.392020 longship-2024.3.15/longship_api_client/api/localtokengroups/localtokengroup_get.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.716899 longship-2024.3.15/longship_api_client/api/localtokengroupstoken/__init__.py
--rw-r--r--   0        0        0     4848 2024-03-14 10:00:43.397440 longship-2024.3.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_delete.py
--rw-r--r--   0        0        0     5216 2024-03-14 10:00:43.398811 longship-2024.3.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_post.py
--rw-r--r--   0        0        0     6004 2024-03-14 10:00:43.397942 longship-2024.3.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_put.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.718809 longship-2024.3.15/longship_api_client/api/location/__init__.py
--rw-r--r--   0        0        0     5151 2024-03-14 10:00:43.406638 longship-2024.3.15/longship_api_client/api/location/location_patch.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.670046 longship-2024.3.15/longship_api_client/api/locations/__init__.py
--rw-r--r--   0        0        0    11635 2024-03-14 10:00:43.392842 longship-2024.3.15/longship_api_client/api/locations/get_all_locations.py
--rw-r--r--   0        0        0     4568 2024-03-14 10:00:43.393209 longship-2024.3.15/longship_api_client/api/locations/location_get.py
--rw-r--r--   0        0        0     5033 2024-03-14 10:00:43.395324 longship-2024.3.15/longship_api_client/api/locations/location_post.py
--rw-r--r--   0        0        0     4850 2024-03-14 10:00:43.391579 longship-2024.3.15/longship_api_client/api/locations/location_put.py
--rw-r--r--   0        0        0     5150 2024-03-14 10:00:43.394685 longship-2024.3.15/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py
--rw-r--r--   0        0        0     5484 2024-03-14 10:00:43.392214 longship-2024.3.15/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.691931 longship-2024.3.15/longship_api_client/api/mspreimbursement/__init__.py
--rw-r--r--   0        0        0     4499 2024-03-14 10:00:43.385600 longship-2024.3.15/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.689506 longship-2024.3.15/longship_api_client/api/organizationunits/__init__.py
--rw-r--r--   0        0        0     6531 2024-03-14 10:00:43.390454 longship-2024.3.15/longship_api_client/api/organizationunits/get_all_organizationunits.py
--rw-r--r--   0        0        0     4787 2024-03-14 10:00:43.390875 longship-2024.3.15/longship_api_client/api/organizationunits/organization_unit_get.py
--rw-r--r--   0        0        0     5049 2024-03-14 10:00:43.389094 longship-2024.3.15/longship_api_client/api/organizationunits/organization_unit_post.py
--rw-r--r--   0        0        0     5250 2024-03-14 10:00:43.389399 longship-2024.3.15/longship_api_client/api/organizationunits/organization_unit_put.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.687138 longship-2024.3.15/longship_api_client/api/reimbursement/__init__.py
--rw-r--r--   0        0        0    10500 2024-03-14 10:00:43.394239 longship-2024.3.15/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py
--rw-r--r--   0        0        0     5141 2024-03-14 10:00:43.393442 longship-2024.3.15/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py
--rw-r--r--   0        0        0     4745 2024-03-14 10:00:43.393736 longship-2024.3.15/longship_api_client/api/reimbursement/reimbursement_cdr_get.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.656022 longship-2024.3.15/longship_api_client/api/sessions/__init__.py
--rw-r--r--   0        0        0    20550 2024-03-14 10:00:43.396775 longship-2024.3.15/longship_api_client/api/sessions/get_all_sessions.py
--rw-r--r--   0        0        0     4546 2024-03-14 10:00:43.397040 longship-2024.3.15/longship_api_client/api/sessions/session_get.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.712617 longship-2024.3.15/longship_api_client/api/tariffdistributions/__init__.py
--rw-r--r--   0        0        0     8625 2024-03-14 10:00:43.402937 longship-2024.3.15/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py
--rw-r--r--   0        0        0     4583 2024-03-14 10:00:43.401925 longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_delete.py
--rw-r--r--   0        0        0     4683 2024-03-14 10:00:43.401414 longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_get.py
--rw-r--r--   0        0        0     5375 2024-03-14 10:00:43.403716 longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_patch.py
--rw-r--r--   0        0        0     4941 2024-03-14 10:00:43.403280 longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_post.py
--rw-r--r--   0        0        0     5613 2024-03-14 10:00:43.403652 longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_put.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.708940 longship-2024.3.15/longship_api_client/api/tariffs/__init__.py
--rw-r--r--   0        0        0     7355 2024-03-14 10:00:43.391260 longship-2024.3.15/longship_api_client/api/tariffs/get_all_tariffs.py
--rw-r--r--   0        0        0     4475 2024-03-14 10:00:43.388303 longship-2024.3.15/longship_api_client/api/tariffs/tariff_delete.py
--rw-r--r--   0        0        0     4524 2024-03-14 10:00:43.387975 longship-2024.3.15/longship_api_client/api/tariffs/tariff_get.py
--rw-r--r--   0        0        0     5134 2024-03-14 10:00:43.390452 longship-2024.3.15/longship_api_client/api/tariffs/tariff_patch.py
--rw-r--r--   0        0        0     4836 2024-03-14 10:00:43.389556 longship-2024.3.15/longship_api_client/api/tariffs/tariff_post.py
--rw-r--r--   0        0        0     5052 2024-03-14 10:00:43.391641 longship-2024.3.15/longship_api_client/api/tariffs/tariff_put.py
--rw-r--r--   0        0        0        0 2024-03-14 10:00:42.705886 longship-2024.3.15/longship_api_client/api/webhooks/__init__.py
--rw-r--r--   0        0        0     8087 2024-03-14 10:00:43.397419 longship-2024.3.15/longship_api_client/api/webhooks/get_all_webhooks.py
--rw-r--r--   0        0        0     4365 2024-03-14 10:00:43.395588 longship-2024.3.15/longship_api_client/api/webhooks/webhook_delete.py
--rw-r--r--   0        0        0     4586 2024-03-14 10:00:43.394818 longship-2024.3.15/longship_api_client/api/webhooks/webhook_get.py
--rw-r--r--   0        0        0     4856 2024-03-14 10:00:43.396638 longship-2024.3.15/longship_api_client/api/webhooks/webhook_post.py
--rw-r--r--   0        0        0     5248 2024-03-14 10:00:43.384917 longship-2024.3.15/longship_api_client/api/webhooks/webhook_put.py
--rw-r--r--   0        0        0    12209 2024-03-14 10:00:43.400951 longship-2024.3.15/longship_api_client/client.py
--rw-r--r--   0        0        0      546 2024-03-14 10:00:43.391153 longship-2024.3.15/longship_api_client/errors.py
--rw-r--r--   0        0        0    22439 2024-03-14 10:00:43.406800 longship-2024.3.15/longship_api_client/models/__init__.py
--rw-r--r--   0        0        0     2620 2024-03-14 10:00:43.399046 longship-2024.3.15/longship_api_client/models/additional_geo_location_dto.py
--rw-r--r--   0        0        0     3621 2024-03-14 10:00:43.398973 longship-2024.3.15/longship_api_client/models/authorization_assertion_dto.py
--rw-r--r--   0        0        0      644 2024-03-14 10:00:43.396779 longship-2024.3.15/longship_api_client/models/authorization_assertion_dto_auth_scenario_type.py
--rw-r--r--   0        0        0      278 2024-03-14 10:00:43.391125 longship-2024.3.15/longship_api_client/models/authorization_assertion_dto_status.py
--rw-r--r--   0        0        0     3446 2024-03-14 10:00:43.394912 longship-2024.3.15/longship_api_client/models/authorization_charger_context_dto.py
--rw-r--r--   0        0        0     3159 2024-03-14 10:00:43.404497 longship-2024.3.15/longship_api_client/models/authorization_context_details_dto.py
--rw-r--r--   0        0        0     2310 2024-03-14 10:00:43.389094 longship-2024.3.15/longship_api_client/models/authorization_data.py
--rw-r--r--   0        0        0     4257 2024-03-14 10:00:43.396084 longship-2024.3.15/longship_api_client/models/authorization_result_dto.py
--rw-r--r--   0        0        0      895 2024-03-14 10:00:43.404708 longship-2024.3.15/longship_api_client/models/authorization_result_dto_reason.py
--rw-r--r--   0        0        0      289 2024-03-14 10:00:43.398419 longship-2024.3.15/longship_api_client/models/authorization_result_dto_status.py
--rw-r--r--   0        0        0     2524 2024-03-14 10:00:43.396629 longship-2024.3.15/longship_api_client/models/authorization_tenant_context_dto.py
--rw-r--r--   0        0        0     2489 2024-03-14 10:00:43.404020 longship-2024.3.15/longship_api_client/models/business_details_dto.py
--rw-r--r--   0        0        0     1604 2024-03-14 10:00:43.403481 longship-2024.3.15/longship_api_client/models/cancel_reservation_request.py
--rw-r--r--   0        0        0    16479 2024-03-14 10:00:43.392777 longship-2024.3.15/longship_api_client/models/cdr_dto.py
--rw-r--r--   0        0        0      177 2024-03-14 10:00:43.398264 longship-2024.3.15/longship_api_client/models/cdr_dto_approval_status.py
--rw-r--r--   0        0        0      166 2024-03-14 10:00:43.392844 longship-2024.3.15/longship_api_client/models/cdr_dto_financial_type.py
--rw-r--r--   0        0        0     1903 2024-03-14 10:00:43.400902 longship-2024.3.15/longship_api_client/models/cdr_geo_location_dto.py
--rw-r--r--   0        0        0     6849 2024-03-14 10:00:43.402613 longship-2024.3.15/longship_api_client/models/cdr_location_dto.py
--rw-r--r--   0        0        0      202 2024-03-14 10:00:43.399107 longship-2024.3.15/longship_api_client/models/cdr_location_dto_power_type.py
--rw-r--r--   0        0        0     2233 2024-03-14 10:00:43.385433 longship-2024.3.15/longship_api_client/models/cdr_patch_dto.py
--rw-r--r--   0        0        0      182 2024-03-14 10:00:43.395736 longship-2024.3.15/longship_api_client/models/cdr_patch_dto_approval_status.py
--rw-r--r--   0        0        0     5364 2024-03-14 10:00:43.398121 longship-2024.3.15/longship_api_client/models/cdr_started_by_info_dto.py
--rw-r--r--   0        0        0      668 2024-03-14 10:00:43.399655 longship-2024.3.15/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py
--rw-r--r--   0        0        0      185 2024-03-14 10:00:43.405190 longship-2024.3.15/longship_api_client/models/cdr_started_by_info_dto_roaming_platform_type.py
--rw-r--r--   0        0        0     5630 2024-03-14 10:00:43.405065 longship-2024.3.15/longship_api_client/models/cdr_started_by_token_dto.py
--rw-r--r--   0        0        0      221 2024-03-14 10:00:43.394183 longship-2024.3.15/longship_api_client/models/cdr_started_by_token_dto_auth_method.py
--rw-r--r--   0        0        0      230 2024-03-14 10:00:43.399968 longship-2024.3.15/longship_api_client/models/cdr_started_by_token_dto_token_type.py
--rw-r--r--   0        0        0     2004 2024-03-14 10:00:43.387954 longship-2024.3.15/longship_api_client/models/change_availability_request.py
--rw-r--r--   0        0        0      194 2024-03-14 10:00:43.404124 longship-2024.3.15/longship_api_client/models/change_availability_request_type.py
--rw-r--r--   0        0        0     1659 2024-03-14 10:00:43.394574 longship-2024.3.15/longship_api_client/models/change_configuration_request.py
--rw-r--r--   0        0        0     6606 2024-03-14 10:00:43.394909 longship-2024.3.15/longship_api_client/models/charge_point_authorize_get_dto.py
--rw-r--r--   0        0        0      247 2024-03-14 10:00:43.406583 longship-2024.3.15/longship_api_client/models/charge_point_authorize_get_dto_authorization_request_type.py
--rw-r--r--   0        0        0     1952 2024-03-14 10:00:43.406750 longship-2024.3.15/longship_api_client/models/charge_point_authorize_post_dto.py
--rw-r--r--   0        0        0     3913 2024-03-14 10:00:43.406329 longship-2024.3.15/longship_api_client/models/chargepoint_configuration_items_dto.py
--rw-r--r--   0        0        0     6507 2024-03-14 10:00:43.407296 longship-2024.3.15/longship_api_client/models/chargepoint_connector_dto.py
--rw-r--r--   0        0        0      176 2024-03-14 10:00:43.388317 longship-2024.3.15/longship_api_client/models/chargepoint_connector_dto_format.py
--rw-r--r--   0        0        0      405 2024-03-14 10:00:43.397305 longship-2024.3.15/longship_api_client/models/chargepoint_connector_dto_operational_status.py
--rw-r--r--   0        0        0      211 2024-03-14 10:00:43.399501 longship-2024.3.15/longship_api_client/models/chargepoint_connector_dto_power_type.py
--rw-r--r--   0        0        0     1100 2024-03-14 10:00:43.397439 longship-2024.3.15/longship_api_client/models/chargepoint_connector_dto_standard.py
--rw-r--r--   0        0        0    17287 2024-03-14 10:00:43.400776 longship-2024.3.15/longship_api_client/models/chargepoint_dto.py
--rw-r--r--   0        0        0      183 2024-03-14 10:00:43.399850 longship-2024.3.15/longship_api_client/models/chargepoint_dto_connectivity_status.py
--rw-r--r--   0        0        0     2642 2024-03-14 10:00:43.402024 longship-2024.3.15/longship_api_client/models/chargepoint_evse_dto.py
--rw-r--r--   0        0        0     3811 2024-03-14 10:00:43.386005 longship-2024.3.15/longship_api_client/models/chargepoint_put_dto.py
--rw-r--r--   0        0        0     7372 2024-03-14 10:00:43.405713 longship-2024.3.15/longship_api_client/models/chargepoint_status_dto.py
--rw-r--r--   0        0        0      189 2024-03-14 10:00:43.387542 longship-2024.3.15/longship_api_client/models/chargepoint_status_dto_connectivity_status.py
--rw-r--r--   0        0        0     3849 2024-03-14 10:00:43.406362 longship-2024.3.15/longship_api_client/models/charging_meter_value_dto.py
--rw-r--r--   0        0        0     1197 2024-03-14 10:00:43.395588 longship-2024.3.15/longship_api_client/models/charging_meter_value_dto_measurand.py
--rw-r--r--   0        0        0      402 2024-03-14 10:00:43.399843 longship-2024.3.15/longship_api_client/models/charging_meter_value_dto_unit.py
--rw-r--r--   0        0        0     3241 2024-03-14 10:00:43.395196 longship-2024.3.15/longship_api_client/models/charging_period_dto.py
--rw-r--r--   0        0        0     6302 2024-03-14 10:00:43.397179 longship-2024.3.15/longship_api_client/models/charging_profile.py
--rw-r--r--   0        0        0      219 2024-03-14 10:00:43.387532 longship-2024.3.15/longship_api_client/models/charging_profile_charging_profile_kind.py
--rw-r--r--   0        0        0      264 2024-03-14 10:00:43.388255 longship-2024.3.15/longship_api_client/models/charging_profile_charging_profile_purpose.py
--rw-r--r--   0        0        0      176 2024-03-14 10:00:43.398192 longship-2024.3.15/longship_api_client/models/charging_profile_recurrency_kind.py
--rw-r--r--   0        0        0     4464 2024-03-14 10:00:43.394437 longship-2024.3.15/longship_api_client/models/charging_schedule.py
--rw-r--r--   0        0        0      161 2024-03-14 10:00:43.390928 longship-2024.3.15/longship_api_client/models/charging_schedule_charging_rate_unit.py
--rw-r--r--   0        0        0     2112 2024-03-14 10:00:43.400009 longship-2024.3.15/longship_api_client/models/charging_schedule_period.py
--rw-r--r--   0        0        0     1234 2024-03-14 10:00:43.396332 longship-2024.3.15/longship_api_client/models/clear_cache_request.py
--rw-r--r--   0        0        0     3618 2024-03-14 10:00:43.388248 longship-2024.3.15/longship_api_client/models/clear_charging_profile_request.py
--rw-r--r--   0        0        0      276 2024-03-14 10:00:43.387911 longship-2024.3.15/longship_api_client/models/clear_charging_profile_request_charging_profile_purpose.py
--rw-r--r--   0        0        0     5852 2024-03-14 10:00:43.388304 longship-2024.3.15/longship_api_client/models/connector_dto.py
--rw-r--r--   0        0        0      165 2024-03-14 10:00:43.390722 longship-2024.3.15/longship_api_client/models/connector_dto_format.py
--rw-r--r--   0        0        0      200 2024-03-14 10:00:43.402324 longship-2024.3.15/longship_api_client/models/connector_dto_power_type.py
--rw-r--r--   0        0        0     1089 2024-03-14 10:00:43.395213 longship-2024.3.15/longship_api_client/models/connector_dto_standard.py
--rw-r--r--   0        0        0     3610 2024-03-14 10:00:43.390447 longship-2024.3.15/longship_api_client/models/connector_operational_status_dto.py
--rw-r--r--   0        0        0      411 2024-03-14 10:00:43.403778 longship-2024.3.15/longship_api_client/models/connector_operational_status_dto_operational_status.py
--rw-r--r--   0        0        0     6410 2024-03-14 10:00:43.396713 longship-2024.3.15/longship_api_client/models/cs_charging_profiles.py
--rw-r--r--   0        0        0      222 2024-03-14 10:00:43.401126 longship-2024.3.15/longship_api_client/models/cs_charging_profiles_charging_profile_kind.py
--rw-r--r--   0        0        0      267 2024-03-14 10:00:43.406839 longship-2024.3.15/longship_api_client/models/cs_charging_profiles_charging_profile_purpose.py
--rw-r--r--   0        0        0      179 2024-03-14 10:00:43.404753 longship-2024.3.15/longship_api_client/models/cs_charging_profiles_recurrency_kind.py
--rw-r--r--   0        0        0     2101 2024-03-14 10:00:43.404498 longship-2024.3.15/longship_api_client/models/data_transfer_request.py
--rw-r--r--   0        0        0     1830 2024-03-14 10:00:43.400511 longship-2024.3.15/longship_api_client/models/display_text_dto.py
--rw-r--r--   0        0        0     3861 2024-03-14 10:00:43.399972 longship-2024.3.15/longship_api_client/models/energy_mix_dto.py
--rw-r--r--   0        0        0     2332 2024-03-14 10:00:43.406434 longship-2024.3.15/longship_api_client/models/energy_source_dto.py
--rw-r--r--   0        0        0      316 2024-03-14 10:00:43.402698 longship-2024.3.15/longship_api_client/models/energy_source_dto_source.py
--rw-r--r--   0        0        0     2282 2024-03-14 10:00:43.401710 longship-2024.3.15/longship_api_client/models/entity_tag_header_value.py
--rw-r--r--   0        0        0     2459 2024-03-14 10:00:43.384560 longship-2024.3.15/longship_api_client/models/environmental_impact_dto.py
--rw-r--r--   0        0        0      209 2024-03-14 10:00:43.404028 longship-2024.3.15/longship_api_client/models/environmental_impact_dto_category.py
--rw-r--r--   0        0        0     2695 2024-03-14 10:00:43.401665 longship-2024.3.15/longship_api_client/models/exceptional_period_dto.py
--rw-r--r--   0        0        0     4745 2024-03-14 10:00:43.389696 longship-2024.3.15/longship_api_client/models/file_content_result.py
--rw-r--r--   0        0        0     1885 2024-03-14 10:00:43.401429 longship-2024.3.15/longship_api_client/models/geo_location_dto.py
--rw-r--r--   0        0        0      190 2024-03-14 10:00:43.387296 longship-2024.3.15/longship_api_client/models/get_all_cdrs_order_by.py
--rw-r--r--   0        0        0      215 2024-03-14 10:00:43.399044 longship-2024.3.15/longship_api_client/models/get_all_chargepoints_accesstype.py
--rw-r--r--   0        0        0      167 2024-03-14 10:00:43.405131 longship-2024.3.15/longship_api_client/models/get_all_chargepoints_chargerpowertype.py
--rw-r--r--   0        0        0      400 2024-03-14 10:00:43.404873 longship-2024.3.15/longship_api_client/models/get_all_chargepoints_operationalstatus.py
--rw-r--r--   0        0        0      224 2024-03-14 10:00:43.403790 longship-2024.3.15/longship_api_client/models/get_all_chargepoints_order_by.py
--rw-r--r--   0        0        0      232 2024-03-14 10:00:43.395683 longship-2024.3.15/longship_api_client/models/get_all_locations_accesstype.py
--rw-r--r--   0        0        0      164 2024-03-14 10:00:43.405284 longship-2024.3.15/longship_api_client/models/get_all_locations_chargerpowertype.py
--rw-r--r--   0        0        0      191 2024-03-14 10:00:43.395797 longship-2024.3.15/longship_api_client/models/get_all_locations_order_by.py
--rw-r--r--   0        0        0      203 2024-03-14 10:00:43.389216 longship-2024.3.15/longship_api_client/models/get_all_reimbursementcdrs_order_by.py
--rw-r--r--   0        0        0      164 2024-03-14 10:00:43.401691 longship-2024.3.15/longship_api_client/models/get_all_sessions_order_by.py
--rw-r--r--   0        0        0      221 2024-03-14 10:00:43.405872 longship-2024.3.15/longship_api_client/models/get_all_tariffdistributions_order_by.py
--rw-r--r--   0        0        0      203 2024-03-14 10:00:43.401563 longship-2024.3.15/longship_api_client/models/get_all_tariffs_order_by.py
--rw-r--r--   0        0        0      144 2024-03-14 10:00:43.393301 longship-2024.3.15/longship_api_client/models/get_all_webhooks_order_by.py
--rw-r--r--   0        0        0     2990 2024-03-14 10:00:43.387319 longship-2024.3.15/longship_api_client/models/get_composite_schedule_request.py
--rw-r--r--   0        0        0      172 2024-03-14 10:00:43.403362 longship-2024.3.15/longship_api_client/models/get_composite_schedule_request_charging_rate_unit.py
--rw-r--r--   0        0        0     1742 2024-03-14 10:00:43.399850 longship-2024.3.15/longship_api_client/models/get_configuration_request.py
--rw-r--r--   0        0        0     3449 2024-03-14 10:00:43.394675 longship-2024.3.15/longship_api_client/models/get_diagnostics_request.py
--rw-r--r--   0        0        0     1285 2024-03-14 10:00:43.399652 longship-2024.3.15/longship_api_client/models/get_local_list_version_request.py
--rw-r--r--   0        0        0     5058 2024-03-14 10:00:43.396277 longship-2024.3.15/longship_api_client/models/hours_dto.py
--rw-r--r--   0        0        0     2684 2024-03-14 10:00:43.385473 longship-2024.3.15/longship_api_client/models/id_tag_info.py
--rw-r--r--   0        0        0      252 2024-03-14 10:00:43.403797 longship-2024.3.15/longship_api_client/models/id_tag_info_status.py
--rw-r--r--   0        0        0     3196 2024-03-14 10:00:43.401368 longship-2024.3.15/longship_api_client/models/image_dto.py
--rw-r--r--   0        0        0      287 2024-03-14 10:00:43.399544 longship-2024.3.15/longship_api_client/models/image_dto_category.py
--rw-r--r--   0        0        0     8679 2024-03-14 10:00:43.396520 longship-2024.3.15/longship_api_client/models/interchange_format_cdr.py
--rw-r--r--   0        0        0     5779 2024-03-14 10:00:43.399553 longship-2024.3.15/longship_api_client/models/local_token_group_get_dto.py
--rw-r--r--   0        0        0     4431 2024-03-14 10:00:43.391839 longship-2024.3.15/longship_api_client/models/local_token_group_post_dto.py
--rw-r--r--   0        0        0     4394 2024-03-14 10:00:43.399014 longship-2024.3.15/longship_api_client/models/local_token_group_put_dto.py
--rw-r--r--   0        0        0     2829 2024-03-14 10:00:43.393545 longship-2024.3.15/longship_api_client/models/local_token_group_token_get_dto.py
--rw-r--r--   0        0        0     2416 2024-03-14 10:00:43.400733 longship-2024.3.15/longship_api_client/models/local_token_group_token_post_dto.py
--rw-r--r--   0        0        0     2411 2024-03-14 10:00:43.404437 longship-2024.3.15/longship_api_client/models/local_token_group_token_put_dto.py
--rw-r--r--   0        0        0     1722 2024-03-14 10:00:43.401217 longship-2024.3.15/longship_api_client/models/location_charge_point_dto.py
--rw-r--r--   0        0        0    19492 2024-03-14 10:00:43.392461 longship-2024.3.15/longship_api_client/models/location_dto.py
--rw-r--r--   0        0        0      706 2024-03-14 10:00:43.399757 longship-2024.3.15/longship_api_client/models/location_dto_facilities_item.py
--rw-r--r--   0        0        0      341 2024-03-14 10:00:43.401164 longship-2024.3.15/longship_api_client/models/location_dto_parking_type.py
--rw-r--r--   0        0        0    11758 2024-03-14 10:00:43.403137 longship-2024.3.15/longship_api_client/models/location_evse_dto.py
--rw-r--r--   0        0        0      698 2024-03-14 10:00:43.394385 longship-2024.3.15/longship_api_client/models/location_evse_dto_capabilities_item.py
--rw-r--r--   0        0        0      277 2024-03-14 10:00:43.396825 longship-2024.3.15/longship_api_client/models/location_evse_dto_parking_restrictions_item.py
--rw-r--r--   0        0        0      364 2024-03-14 10:00:43.404250 longship-2024.3.15/longship_api_client/models/location_evse_dto_status.py
--rw-r--r--   0        0        0    18398 2024-03-14 10:00:43.390585 longship-2024.3.15/longship_api_client/models/location_post_dto.py
--rw-r--r--   0        0        0      710 2024-03-14 10:00:43.401805 longship-2024.3.15/longship_api_client/models/location_post_dto_facilities_item.py
--rw-r--r--   0        0        0      345 2024-03-14 10:00:43.398124 longship-2024.3.15/longship_api_client/models/location_post_dto_parking_type.py
--rw-r--r--   0        0        0    19252 2024-03-14 10:00:43.385606 longship-2024.3.15/longship_api_client/models/location_put_dto.py
--rw-r--r--   0        0        0      709 2024-03-14 10:00:43.405258 longship-2024.3.15/longship_api_client/models/location_put_dto_facilities_item.py
--rw-r--r--   0        0        0      344 2024-03-14 10:00:43.401786 longship-2024.3.15/longship_api_client/models/location_put_dto_parking_type.py
--rw-r--r--   0        0        0     1957 2024-03-14 10:00:43.390770 longship-2024.3.15/longship_api_client/models/location_tariff_distribution_dto.py
--rw-r--r--   0        0        0     2482 2024-03-14 10:00:43.403888 longship-2024.3.15/longship_api_client/models/longship_error.py
--rw-r--r--   0        0        0     2024 2024-03-14 10:00:43.407015 longship-2024.3.15/longship_api_client/models/longship_error_detail.py
--rw-r--r--   0        0        0     6063 2024-03-14 10:00:43.395926 longship-2024.3.15/longship_api_client/models/message_log_dto.py
--rw-r--r--   0        0        0      219 2024-03-14 10:00:43.399742 longship-2024.3.15/longship_api_client/models/message_log_dto_direction.py
--rw-r--r--   0        0        0     1335 2024-03-14 10:00:43.393728 longship-2024.3.15/longship_api_client/models/message_log_dto_ocpp_message_type.py
--rw-r--r--   0        0        0      227 2024-03-14 10:00:43.389302 longship-2024.3.15/longship_api_client/models/message_log_dto_wamp_message_type.py
--rw-r--r--   0        0        0     2240 2024-03-14 10:00:43.395387 longship-2024.3.15/longship_api_client/models/organization_unit_financial_details_dto.py
--rw-r--r--   0        0        0    10140 2024-03-14 10:00:43.397943 longship-2024.3.15/longship_api_client/models/organization_unit_get_dto.py
--rw-r--r--   0        0        0     9365 2024-03-14 10:00:43.398320 longship-2024.3.15/longship_api_client/models/organization_unit_post_dto.py
--rw-r--r--   0        0        0     9113 2024-03-14 10:00:43.407072 longship-2024.3.15/longship_api_client/models/organization_unit_put_dto.py
--rw-r--r--   0        0        0     4903 2024-03-14 10:00:43.398119 longship-2024.3.15/longship_api_client/models/price_info_dto.py
--rw-r--r--   0        0        0     3434 2024-03-14 10:00:43.401373 longship-2024.3.15/longship_api_client/models/private_emp_tariff_dto.py
--rw-r--r--   0        0        0      161 2024-03-14 10:00:43.395316 longship-2024.3.15/longship_api_client/models/private_emp_tariff_dto_power_type.py
--rw-r--r--   0        0        0     3090 2024-03-14 10:00:43.403241 longship-2024.3.15/longship_api_client/models/publish_token_type_dto.py
--rw-r--r--   0        0        0      224 2024-03-14 10:00:43.399171 longship-2024.3.15/longship_api_client/models/publish_token_type_dto_type.py
--rw-r--r--   0        0        0     2202 2024-03-14 10:00:43.386145 longship-2024.3.15/longship_api_client/models/regular_hours_dto.py
--rw-r--r--   0        0        0    11542 2024-03-14 10:00:43.406027 longship-2024.3.15/longship_api_client/models/reimburse_info_dto.py
--rw-r--r--   0        0        0      205 2024-03-14 10:00:43.389673 longship-2024.3.15/longship_api_client/models/reimburse_info_dto_type.py
--rw-r--r--   0        0        0     4058 2024-03-14 10:00:43.399433 longship-2024.3.15/longship_api_client/models/reimburse_started_by_info_dto.py
--rw-r--r--   0        0        0      674 2024-03-14 10:00:43.400346 longship-2024.3.15/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py
--rw-r--r--   0        0        0     5786 2024-03-14 10:00:43.406140 longship-2024.3.15/longship_api_client/models/reimburse_started_by_token_dto.py
--rw-r--r--   0        0        0      227 2024-03-14 10:00:43.385921 longship-2024.3.15/longship_api_client/models/reimburse_started_by_token_dto_auth_method.py
--rw-r--r--   0        0        0      236 2024-03-14 10:00:43.401566 longship-2024.3.15/longship_api_client/models/reimburse_started_by_token_dto_token_type.py
--rw-r--r--   0        0        0     3030 2024-03-14 10:00:43.400184 longship-2024.3.15/longship_api_client/models/reimbursement_bank_details_dto.py
--rw-r--r--   0        0        0    21587 2024-03-14 10:00:43.403033 longship-2024.3.15/longship_api_client/models/reimbursement_cdr_dto.py
--rw-r--r--   0        0        0     1971 2024-03-14 10:00:43.390575 longship-2024.3.15/longship_api_client/models/reimbursement_cdr_geo_location_dto.py
--rw-r--r--   0        0        0     7191 2024-03-14 10:00:43.398692 longship-2024.3.15/longship_api_client/models/reimbursement_cdr_location_dto.py
--rw-r--r--   0        0        0      215 2024-03-14 10:00:43.393851 longship-2024.3.15/longship_api_client/models/reimbursement_cdr_location_dto_power_type.py
--rw-r--r--   0        0        0     2435 2024-03-14 10:00:43.394076 longship-2024.3.15/longship_api_client/models/reimbursement_customer_share_dto.py
--rw-r--r--   0        0        0     1917 2024-03-14 10:00:43.385561 longship-2024.3.15/longship_api_client/models/reimbursement_price_dto.py
--rw-r--r--   0        0        0     4698 2024-03-14 10:00:43.397039 longship-2024.3.15/longship_api_client/models/reimbursement_tariff_dto.py
--rw-r--r--   0        0        0      209 2024-03-14 10:00:43.396417 longship-2024.3.15/longship_api_client/models/reimbursement_tariff_dto_status.py
--rw-r--r--   0        0        0     2824 2024-03-14 10:00:43.389098 longship-2024.3.15/longship_api_client/models/remote_start_transaction_request.py
--rw-r--r--   0        0        0     1627 2024-03-14 10:00:43.389565 longship-2024.3.15/longship_api_client/models/remote_stop_transaction_request.py
--rw-r--r--   0        0        0     2644 2024-03-14 10:00:43.404201 longship-2024.3.15/longship_api_client/models/reserve_now_request.py
--rw-r--r--   0        0        0     1609 2024-03-14 10:00:43.406899 longship-2024.3.15/longship_api_client/models/reset_request.py
--rw-r--r--   0        0        0      157 2024-03-14 10:00:43.406506 longship-2024.3.15/longship_api_client/models/reset_request_type.py
--rw-r--r--   0        0        0     3534 2024-03-14 10:00:43.397290 longship-2024.3.15/longship_api_client/models/send_local_list_request.py
--rw-r--r--   0        0        0      187 2024-03-14 10:00:43.387685 longship-2024.3.15/longship_api_client/models/send_local_list_request_update_type.py
--rw-r--r--   0        0        0    20192 2024-03-14 10:00:43.398811 longship-2024.3.15/longship_api_client/models/session_dto.py
--rw-r--r--   0        0        0      194 2024-03-14 10:00:43.396332 longship-2024.3.15/longship_api_client/models/session_dto_approval_status.py
--rw-r--r--   0        0        0      166 2024-03-14 10:00:43.402399 longship-2024.3.15/longship_api_client/models/session_dto_review_scenario_type.py
--rw-r--r--   0        0        0      251 2024-03-14 10:00:43.400094 longship-2024.3.15/longship_api_client/models/session_dto_status.py
--rw-r--r--   0        0        0     1923 2024-03-14 10:00:43.400959 longship-2024.3.15/longship_api_client/models/session_geo_location_dto.py
--rw-r--r--   0        0        0     6933 2024-03-14 10:00:43.404992 longship-2024.3.15/longship_api_client/models/session_location_dto.py
--rw-r--r--   0        0        0      206 2024-03-14 10:00:43.389369 longship-2024.3.15/longship_api_client/models/session_location_dto_power_type.py
--rw-r--r--   0        0        0     3932 2024-03-14 10:00:43.404526 longship-2024.3.15/longship_api_client/models/session_threshold_check_dto.py
--rw-r--r--   0        0        0      265 2024-03-14 10:00:43.402372 longship-2024.3.15/longship_api_client/models/session_threshold_check_dto_status.py
--rw-r--r--   0        0        0      204 2024-03-14 10:00:43.402329 longship-2024.3.15/longship_api_client/models/session_threshold_check_dto_threshold_hit_outcome.py
--rw-r--r--   0        0        0     4472 2024-03-14 10:00:43.402697 longship-2024.3.15/longship_api_client/models/session_threshold_value_dto_decimal.py
--rw-r--r--   0        0        0      272 2024-03-14 10:00:43.404773 longship-2024.3.15/longship_api_client/models/session_threshold_value_dto_decimal_status.py
--rw-r--r--   0        0        0      211 2024-03-14 10:00:43.401072 longship-2024.3.15/longship_api_client/models/session_threshold_value_dto_decimal_threshold_hit_outcome.py
--rw-r--r--   0        0        0     4431 2024-03-14 10:00:43.399424 longship-2024.3.15/longship_api_client/models/session_threshold_value_dto_int_32.py
--rw-r--r--   0        0        0      270 2024-03-14 10:00:43.403276 longship-2024.3.15/longship_api_client/models/session_threshold_value_dto_int_32_status.py
--rw-r--r--   0        0        0      209 2024-03-14 10:00:43.390865 longship-2024.3.15/longship_api_client/models/session_threshold_value_dto_int_32_threshold_hit_outcome.py
--rw-r--r--   0        0        0    10700 2024-03-14 10:00:43.395766 longship-2024.3.15/longship_api_client/models/session_thresholds_dto.py
--rw-r--r--   0        0        0      462 2024-03-14 10:00:43.391236 longship-2024.3.15/longship_api_client/models/session_thresholds_dto_thresholds_hit_item.py
--rw-r--r--   0        0        0     2133 2024-03-14 10:00:43.400038 longship-2024.3.15/longship_api_client/models/set_charging_profile_request.py
--rw-r--r--   0        0        0     5270 2024-03-14 10:00:43.404434 longship-2024.3.15/longship_api_client/models/started_by_info_dto.py
--rw-r--r--   0        0        0      665 2024-03-14 10:00:43.395534 longship-2024.3.15/longship_api_client/models/started_by_info_dto_authorization_state.py
--rw-r--r--   0        0        0      182 2024-03-14 10:00:43.394970 longship-2024.3.15/longship_api_client/models/started_by_info_dto_roaming_platform_type.py
--rw-r--r--   0        0        0     5550 2024-03-14 10:00:43.397230 longship-2024.3.15/longship_api_client/models/started_by_token_dto.py
--rw-r--r--   0        0        0      218 2024-03-14 10:00:43.406246 longship-2024.3.15/longship_api_client/models/started_by_token_dto_auth_method.py
--rw-r--r--   0        0        0      227 2024-03-14 10:00:43.402124 longship-2024.3.15/longship_api_client/models/started_by_token_dto_token_type.py
--rw-r--r--   0        0        0     3399 2024-03-14 10:00:43.402604 longship-2024.3.15/longship_api_client/models/status_schedule_dto.py
--rw-r--r--   0        0        0      366 2024-03-14 10:00:43.401475 longship-2024.3.15/longship_api_client/models/status_schedule_dto_status.py
--rw-r--r--   0        0        0     2582 2024-03-14 10:00:43.398930 longship-2024.3.15/longship_api_client/models/string_segment.py
--rw-r--r--   0        0        0     2907 2024-03-14 10:00:43.400261 longship-2024.3.15/longship_api_client/models/tariff_assertion_dto.py
--rw-r--r--   0        0        0      283 2024-03-14 10:00:43.399193 longship-2024.3.15/longship_api_client/models/tariff_assertion_dto_tariff_type.py
--rw-r--r--   0        0        0     6610 2024-03-14 10:00:43.392773 longship-2024.3.15/longship_api_client/models/tariff_distribution_get_dto.py
--rw-r--r--   0        0        0     3723 2024-03-14 10:00:43.405157 longship-2024.3.15/longship_api_client/models/tariff_distribution_history_dto.py
--rw-r--r--   0        0        0     3517 2024-03-14 10:00:43.398890 longship-2024.3.15/longship_api_client/models/tariff_distribution_post_dto.py
--rw-r--r--   0        0        0     3512 2024-03-14 10:00:43.401398 longship-2024.3.15/longship_api_client/models/tariff_distribution_put_dto.py
--rw-r--r--   0        0        0    14683 2024-03-14 10:00:43.403523 longship-2024.3.15/longship_api_client/models/tariff_dto.py
--rw-r--r--   0        0        0      186 2024-03-14 10:00:43.402427 longship-2024.3.15/longship_api_client/models/tariff_dto_tariff_type.py
--rw-r--r--   0        0        0      241 2024-03-14 10:00:43.390794 longship-2024.3.15/longship_api_client/models/tariff_dto_usage_type.py
--rw-r--r--   0        0        0     6088 2024-03-14 10:00:43.400542 longship-2024.3.15/longship_api_client/models/tariff_info_dto.py
--rw-r--r--   0        0        0     8528 2024-03-14 10:00:43.402222 longship-2024.3.15/longship_api_client/models/tariff_post_dto.py
--rw-r--r--   0        0        0      245 2024-03-14 10:00:43.387798 longship-2024.3.15/longship_api_client/models/tariff_post_dto_usage_type.py
--rw-r--r--   0        0        0     9146 2024-03-14 10:00:43.404565 longship-2024.3.15/longship_api_client/models/tariff_price_dto.py
--rw-r--r--   0        0        0      209 2024-03-14 10:00:43.404494 longship-2024.3.15/longship_api_client/models/tariff_price_dto_approval_status.py
--rw-r--r--   0        0        0     8389 2024-03-14 10:00:43.405579 longship-2024.3.15/longship_api_client/models/tariff_put_dto.py
--rw-r--r--   0        0        0     3997 2024-03-14 10:00:43.407244 longship-2024.3.15/longship_api_client/models/tariff_restriction.py
--rw-r--r--   0        0        0      244 2024-03-14 10:00:43.399091 longship-2024.3.15/longship_api_client/models/tariff_restriction_day_of_week.py
--rw-r--r--   0        0        0     2645 2024-03-14 10:00:43.397585 longship-2024.3.15/longship_api_client/models/token_info_dto.py
--rw-r--r--   0        0        0      216 2024-03-14 10:00:43.395212 longship-2024.3.15/longship_api_client/models/token_info_dto_token_type.py
--rw-r--r--   0        0        0     2385 2024-03-14 10:00:43.400943 longship-2024.3.15/longship_api_client/models/trigger_message_request.py
--rw-r--r--   0        0        0      420 2024-03-14 10:00:43.395426 longship-2024.3.15/longship_api_client/models/trigger_message_request_requested_message.py
--rw-r--r--   0        0        0     1574 2024-03-14 10:00:43.404145 longship-2024.3.15/longship_api_client/models/unlock_connector_request.py
--rw-r--r--   0        0        0     2514 2024-03-14 10:00:43.402907 longship-2024.3.15/longship_api_client/models/update_firmware_request.py
--rw-r--r--   0        0        0     5498 2024-03-14 10:00:43.405706 longship-2024.3.15/longship_api_client/models/webhook_get_dto.py
--rw-r--r--   0        0        0      578 2024-03-14 10:00:43.401887 longship-2024.3.15/longship_api_client/models/webhook_get_dto_event_types_item.py
--rw-r--r--   0        0        0     1807 2024-03-14 10:00:43.404934 longship-2024.3.15/longship_api_client/models/webhook_header_dto.py
--rw-r--r--   0        0        0     4123 2024-03-14 10:00:43.386140 longship-2024.3.15/longship_api_client/models/webhook_post_dto.py
--rw-r--r--   0        0        0      579 2024-03-14 10:00:43.391338 longship-2024.3.15/longship_api_client/models/webhook_post_dto_event_types_item.py
--rw-r--r--   0        0        0     4113 2024-03-14 10:00:43.391630 longship-2024.3.15/longship_api_client/models/webhook_put_dto.py
--rw-r--r--   0        0        0      578 2024-03-14 10:00:43.403916 longship-2024.3.15/longship_api_client/models/webhook_put_dto_event_types_item.py
--rw-r--r--   0        0        0     4210 2024-03-14 10:00:43.398860 longship-2024.3.15/longship_api_client/models/webhook_summary_get_dto.py
--rw-r--r--   0        0        0      585 2024-03-14 10:00:43.394767 longship-2024.3.15/longship_api_client/models/webhook_summary_get_dto_event_types_item.py
--rw-r--r--   0        0        0       25 2024-03-14 10:00:42.547396 longship-2024.3.15/longship_api_client/py.typed
--rw-r--r--   0        0        0      985 2024-03-14 10:00:43.400218 longship-2024.3.15/longship_api_client/types.py
--rw-r--r--   0        0        0      818 2024-03-14 15:16:27.339962 longship-2024.3.15/pyproject.toml
--rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 longship-2024.3.15/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-26 16:00:19.878825 longship-2024.4.15/LICENSE
+-rw-r--r--   0        0        0     4661 2023-06-26 16:47:23.288883 longship-2024.4.15/README.md
+-rw-r--r--   0        0        0     7668 2024-03-14 10:00:43.390594 longship-2024.4.15/longship/client.py
+-rw-r--r--   0        0        0      112 2023-06-26 16:00:19.886682 longship-2024.4.15/longship/errors.py
+-rw-r--r--   0        0        0     4614 2024-03-14 15:13:41.390085 longship-2024.4.15/longship/types.py
+-rw-r--r--   0        0        0      155 2024-03-25 19:42:53.022260 longship-2024.4.15/longship_api_client/__init__.py
+-rw-r--r--   0        0        0       45 2024-03-25 19:42:53.025427 longship-2024.4.15/longship_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.296257 longship-2024.4.15/longship_api_client/api/cdrs/__init__.py
+-rw-r--r--   0        0        0     4458 2024-03-25 20:00:43.969808 longship-2024.4.15/longship_api_client/api/cdrs/cdr_get.py
+-rw-r--r--   0        0        0     5023 2024-03-25 20:00:43.970406 longship-2024.4.15/longship_api_client/api/cdrs/cdr_patch.py
+-rw-r--r--   0        0        0    19502 2024-03-25 20:00:43.970703 longship-2024.4.15/longship_api_client/api/cdrs/get_all_cdrs.py
+-rw-r--r--   0        0        0     7993 2024-03-25 20:00:43.971091 longship-2024.4.15/longship_api_client/api/cdrs/get_all_interchangeformat.py
+-rw-r--r--   0        0        0     5989 2024-03-25 20:00:43.971416 longship-2024.4.15/longship_api_client/api/cdrs/get_file_full_download_cdrs.py
+-rw-r--r--   0        0        0     5968 2024-03-25 20:00:43.971772 longship-2024.4.15/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.288563 longship-2024.4.15/longship_api_client/api/chargepoint_status/__init__.py
+-rw-r--r--   0        0        0     4767 2024-03-25 20:00:43.972132 longship-2024.4.15/longship_api_client/api/chargepoint_status/chargepoint_status_get.py
+-rw-r--r--   0        0        0     6490 2024-03-25 20:00:43.972453 longship-2024.4.15/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.289893 longship-2024.4.15/longship_api_client/api/chargepoints/__init__.py
+-rw-r--r--   0        0        0     4634 2024-03-25 20:00:43.972876 longship-2024.4.15/longship_api_client/api/chargepoints/chargepoint_get.py
+-rw-r--r--   0        0        0     5162 2024-03-25 20:00:43.973593 longship-2024.4.15/longship_api_client/api/chargepoints/chargepoint_put.py
+-rw-r--r--   0        0        0     5416 2024-03-25 20:00:43.973998 longship-2024.4.15/longship_api_client/api/chargepoints/chargepointauthorization_get.py
+-rw-r--r--   0        0        0     5252 2024-03-25 20:00:43.976187 longship-2024.4.15/longship_api_client/api/chargepoints/chargepointauthorization_post.py
+-rw-r--r--   0        0        0     9920 2024-03-25 20:00:43.976569 longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepointauthorizations.py
+-rw-r--r--   0        0        0    11723 2024-03-25 20:00:43.976947 longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepointmessages.py
+-rw-r--r--   0        0        0    16896 2024-03-25 20:00:43.977268 longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepoints.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.307087 longship-2024.4.15/longship_api_client/api/commands/__init__.py
+-rw-r--r--   0        0        0     5151 2024-03-25 20:00:43.977620 longship-2024.4.15/longship_api_client/api/commands/send_cancel_reservation_request.py
+-rw-r--r--   0        0        0     5171 2024-03-25 20:00:43.978017 longship-2024.4.15/longship_api_client/api/commands/send_change_availability_request.py
+-rw-r--r--   0        0        0     5191 2024-03-25 20:00:43.978353 longship-2024.4.15/longship_api_client/api/commands/send_change_configuration_request.py
+-rw-r--r--   0        0        0     5011 2024-03-25 19:42:53.020065 longship-2024.4.15/longship_api_client/api/commands/send_clear_cache_request.py
+-rw-r--r--   0        0        0     5212 2024-03-25 20:00:43.978639 longship-2024.4.15/longship_api_client/api/commands/send_clear_charging_profile_request.py
+-rw-r--r--   0        0        0     5051 2024-03-25 20:00:43.979167 longship-2024.4.15/longship_api_client/api/commands/send_data_transfer_request.py
+-rw-r--r--   0        0        0     5212 2024-03-25 20:00:43.979385 longship-2024.4.15/longship_api_client/api/commands/send_get_composite_schedule_request.py
+-rw-r--r--   0        0        0     5131 2024-03-25 19:42:53.015992 longship-2024.4.15/longship_api_client/api/commands/send_get_configuration_request.py
+-rw-r--r--   0        0        0     5091 2024-03-25 20:00:43.979633 longship-2024.4.15/longship_api_client/api/commands/send_get_diagnostics_request.py
+-rw-r--r--   0        0        0     5193 2024-03-25 20:00:43.979964 longship-2024.4.15/longship_api_client/api/commands/send_get_local_list_version_request.py
+-rw-r--r--   0        0        0     5241 2024-03-25 20:00:43.980364 longship-2024.4.15/longship_api_client/api/commands/send_remote_start_transaction_request.py
+-rw-r--r--   0        0        0     5221 2024-03-25 20:00:43.980710 longship-2024.4.15/longship_api_client/api/commands/send_remote_stop_transaction_request.py
+-rw-r--r--   0        0        0     5011 2024-03-25 20:00:43.981052 longship-2024.4.15/longship_api_client/api/commands/send_reserve_now_request.py
+-rw-r--r--   0        0        0     4946 2024-03-25 20:00:43.981436 longship-2024.4.15/longship_api_client/api/commands/send_reset_request.py
+-rw-r--r--   0        0        0     5072 2024-03-25 19:42:53.014730 longship-2024.4.15/longship_api_client/api/commands/send_send_local_list_request.py
+-rw-r--r--   0        0        0     5172 2024-03-25 20:00:43.981843 longship-2024.4.15/longship_api_client/api/commands/send_set_charging_profile_request.py
+-rw-r--r--   0        0        0     5091 2024-03-25 20:00:43.982152 longship-2024.4.15/longship_api_client/api/commands/send_trigger_message_request.py
+-rw-r--r--   0        0        0     5111 2024-03-25 19:42:53.021486 longship-2024.4.15/longship_api_client/api/commands/send_unlock_connector_request.py
+-rw-r--r--   0        0        0     5091 2024-03-25 20:00:43.982342 longship-2024.4.15/longship_api_client/api/commands/send_update_firmware_request.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.330382 longship-2024.4.15/longship_api_client/api/configurationitems/__init__.py
+-rw-r--r--   0        0        0     5527 2024-03-25 20:00:43.982664 longship-2024.4.15/longship_api_client/api/configurationitems/configurationitem_get.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.317516 longship-2024.4.15/longship_api_client/api/localtokengroups/__init__.py
+-rw-r--r--   0        0        0     6508 2024-03-25 20:00:43.982954 longship-2024.4.15/longship_api_client/api/localtokengroups/get_all_localtokengroups.py
+-rw-r--r--   0        0        0     4437 2024-03-25 19:42:53.009339 longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_delete.py
+-rw-r--r--   0        0        0     5028 2024-03-25 19:42:53.008522 longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_post.py
+-rw-r--r--   0        0        0     5243 2024-03-25 20:00:43.983235 longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_put.py
+-rw-r--r--   0        0        0     4764 2024-03-25 20:00:43.983514 longship-2024.4.15/longship_api_client/api/localtokengroups/localtokengroup_get.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.331027 longship-2024.4.15/longship_api_client/api/localtokengroupstoken/__init__.py
+-rw-r--r--   0        0        0     4848 2024-03-25 19:42:53.025042 longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_delete.py
+-rw-r--r--   0        0        0     5216 2024-03-25 20:00:43.983719 longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_post.py
+-rw-r--r--   0        0        0     6004 2024-03-25 20:00:43.984111 longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_put.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.332975 longship-2024.4.15/longship_api_client/api/location/__init__.py
+-rw-r--r--   0        0        0     5151 2024-03-25 20:00:43.984328 longship-2024.4.15/longship_api_client/api/location/location_patch.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.282660 longship-2024.4.15/longship_api_client/api/locations/__init__.py
+-rw-r--r--   0        0        0    11635 2024-03-25 20:00:43.984514 longship-2024.4.15/longship_api_client/api/locations/get_all_locations.py
+-rw-r--r--   0        0        0     4568 2024-03-25 20:00:43.984928 longship-2024.4.15/longship_api_client/api/locations/location_get.py
+-rw-r--r--   0        0        0     5033 2024-03-25 20:00:43.985237 longship-2024.4.15/longship_api_client/api/locations/location_post.py
+-rw-r--r--   0        0        0     4850 2024-03-25 20:00:43.985423 longship-2024.4.15/longship_api_client/api/locations/location_put.py
+-rw-r--r--   0        0        0     5150 2024-03-25 19:42:53.023748 longship-2024.4.15/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py
+-rw-r--r--   0        0        0     5484 2024-03-25 20:00:43.985706 longship-2024.4.15/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.306476 longship-2024.4.15/longship_api_client/api/mspreimbursement/__init__.py
+-rw-r--r--   0        0        0     4499 2024-03-25 19:42:53.013509 longship-2024.4.15/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.303969 longship-2024.4.15/longship_api_client/api/organizationunits/__init__.py
+-rw-r--r--   0        0        0     6531 2024-03-25 20:00:43.986158 longship-2024.4.15/longship_api_client/api/organizationunits/get_all_organizationunits.py
+-rw-r--r--   0        0        0     4787 2024-03-25 20:00:43.986377 longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_get.py
+-rw-r--r--   0        0        0     5049 2024-03-25 20:00:43.986553 longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_post.py
+-rw-r--r--   0        0        0     5250 2024-03-25 20:00:43.986734 longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_put.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.301307 longship-2024.4.15/longship_api_client/api/reimbursement/__init__.py
+-rw-r--r--   0        0        0    10500 2024-03-25 20:00:43.987077 longship-2024.4.15/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py
+-rw-r--r--   0        0        0     5141 2024-03-25 19:42:53.009738 longship-2024.4.15/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py
+-rw-r--r--   0        0        0     4745 2024-03-25 19:42:53.010083 longship-2024.4.15/longship_api_client/api/reimbursement/reimbursement_cdr_get.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.260831 longship-2024.4.15/longship_api_client/api/sessions/__init__.py
+-rw-r--r--   0        0        0    20550 2024-03-25 20:00:43.987351 longship-2024.4.15/longship_api_client/api/sessions/get_all_sessions.py
+-rw-r--r--   0        0        0     4546 2024-03-25 20:00:43.987624 longship-2024.4.15/longship_api_client/api/sessions/session_get.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.326877 longship-2024.4.15/longship_api_client/api/tariffdistributions/__init__.py
+-rw-r--r--   0        0        0     8625 2024-03-25 20:00:43.988058 longship-2024.4.15/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py
+-rw-r--r--   0        0        0     4583 2024-03-25 20:00:43.988413 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_delete.py
+-rw-r--r--   0        0        0     4683 2024-03-25 20:00:43.988748 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_get.py
+-rw-r--r--   0        0        0     5375 2024-03-25 20:00:43.989159 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_patch.py
+-rw-r--r--   0        0        0     4941 2024-03-25 20:00:43.989422 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_post.py
+-rw-r--r--   0        0        0     5613 2024-03-25 20:00:43.989810 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_put.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.323367 longship-2024.4.15/longship_api_client/api/tariffs/__init__.py
+-rw-r--r--   0        0        0     7355 2024-03-25 20:00:43.990037 longship-2024.4.15/longship_api_client/api/tariffs/get_all_tariffs.py
+-rw-r--r--   0        0        0     4475 2024-03-25 20:00:43.990394 longship-2024.4.15/longship_api_client/api/tariffs/tariff_delete.py
+-rw-r--r--   0        0        0     4524 2024-03-25 20:00:43.990763 longship-2024.4.15/longship_api_client/api/tariffs/tariff_get.py
+-rw-r--r--   0        0        0     5134 2024-03-25 20:00:43.990994 longship-2024.4.15/longship_api_client/api/tariffs/tariff_patch.py
+-rw-r--r--   0        0        0     4836 2024-03-25 20:00:43.991198 longship-2024.4.15/longship_api_client/api/tariffs/tariff_post.py
+-rw-r--r--   0        0        0     5052 2024-03-25 20:00:43.991391 longship-2024.4.15/longship_api_client/api/tariffs/tariff_put.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.320418 longship-2024.4.15/longship_api_client/api/webhooks/__init__.py
+-rw-r--r--   0        0        0     8087 2024-03-25 20:00:43.991710 longship-2024.4.15/longship_api_client/api/webhooks/get_all_webhooks.py
+-rw-r--r--   0        0        0     4365 2024-03-25 19:42:53.011639 longship-2024.4.15/longship_api_client/api/webhooks/webhook_delete.py
+-rw-r--r--   0        0        0     4586 2024-03-25 19:42:53.011295 longship-2024.4.15/longship_api_client/api/webhooks/webhook_get.py
+-rw-r--r--   0        0        0     4856 2024-03-25 20:00:43.992017 longship-2024.4.15/longship_api_client/api/webhooks/webhook_post.py
+-rw-r--r--   0        0        0     5248 2024-03-25 20:00:43.992356 longship-2024.4.15/longship_api_client/api/webhooks/webhook_put.py
+-rw-r--r--   0        0        0    12209 2024-03-25 19:42:53.022999 longship-2024.4.15/longship_api_client/client.py
+-rw-r--r--   0        0        0      546 2024-03-25 19:42:53.007596 longship-2024.4.15/longship_api_client/errors.py
+-rw-r--r--   0        0        0    22439 2024-03-25 19:42:53.021268 longship-2024.4.15/longship_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2637 2024-03-25 20:16:22.035460 longship-2024.4.15/longship_api_client/models/additional_geo_location_dto.py
+-rw-r--r--   0        0        0     3671 2024-03-25 20:16:03.746432 longship-2024.4.15/longship_api_client/models/authorization_assertion_dto.py
+-rw-r--r--   0        0        0      644 2024-03-25 19:42:53.007525 longship-2024.4.15/longship_api_client/models/authorization_assertion_dto_auth_scenario_type.py
+-rw-r--r--   0        0        0      278 2024-03-25 19:42:53.011158 longship-2024.4.15/longship_api_client/models/authorization_assertion_dto_status.py
+-rw-r--r--   0        0        0     3446 2024-03-25 19:42:53.013517 longship-2024.4.15/longship_api_client/models/authorization_charger_context_dto.py
+-rw-r--r--   0        0        0     3198 2024-03-25 20:16:06.745858 longship-2024.4.15/longship_api_client/models/authorization_context_details_dto.py
+-rw-r--r--   0        0        0     2334 2024-03-25 20:16:17.147771 longship-2024.4.15/longship_api_client/models/authorization_data.py
+-rw-r--r--   0        0        0     4295 2024-03-25 20:16:17.147874 longship-2024.4.15/longship_api_client/models/authorization_result_dto.py
+-rw-r--r--   0        0        0      895 2024-03-25 19:42:53.014619 longship-2024.4.15/longship_api_client/models/authorization_result_dto_reason.py
+-rw-r--r--   0        0        0      289 2024-03-25 19:42:53.019455 longship-2024.4.15/longship_api_client/models/authorization_result_dto_status.py
+-rw-r--r--   0        0        0     2524 2024-03-25 19:42:53.009051 longship-2024.4.15/longship_api_client/models/authorization_tenant_context_dto.py
+-rw-r--r--   0        0        0     2507 2024-03-25 20:01:26.710827 longship-2024.4.15/longship_api_client/models/business_details_dto.py
+-rw-r--r--   0        0        0     1604 2024-03-25 19:42:53.025922 longship-2024.4.15/longship_api_client/models/cancel_reservation_request.py
+-rw-r--r--   0        0        0    16774 2024-03-25 20:16:17.147727 longship-2024.4.15/longship_api_client/models/cdr_dto.py
+-rw-r--r--   0        0        0      177 2024-03-25 19:42:53.018594 longship-2024.4.15/longship_api_client/models/cdr_dto_approval_status.py
+-rw-r--r--   0        0        0      166 2024-03-25 19:42:53.011820 longship-2024.4.15/longship_api_client/models/cdr_dto_financial_type.py
+-rw-r--r--   0        0        0     1903 2024-03-25 19:42:53.021004 longship-2024.4.15/longship_api_client/models/cdr_geo_location_dto.py
+-rw-r--r--   0        0        0     6896 2024-03-25 20:16:17.145392 longship-2024.4.15/longship_api_client/models/cdr_location_dto.py
+-rw-r--r--   0        0        0      202 2024-03-25 19:42:53.020295 longship-2024.4.15/longship_api_client/models/cdr_location_dto_power_type.py
+-rw-r--r--   0        0        0     2261 2024-03-25 20:16:17.145494 longship-2024.4.15/longship_api_client/models/cdr_patch_dto.py
+-rw-r--r--   0        0        0      182 2024-03-25 19:42:53.016250 longship-2024.4.15/longship_api_client/models/cdr_patch_dto_approval_status.py
+-rw-r--r--   0        0        0     5453 2024-03-25 20:16:17.145534 longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto.py
+-rw-r--r--   0        0        0      668 2024-03-25 19:42:53.020391 longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py
+-rw-r--r--   0        0        0      185 2024-03-25 19:42:53.015245 longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto_roaming_platform_type.py
+-rw-r--r--   0        0        0     5677 2024-03-25 20:16:17.145633 longship-2024.4.15/longship_api_client/models/cdr_started_by_token_dto.py
+-rw-r--r--   0        0        0      221 2024-03-25 19:42:53.015398 longship-2024.4.15/longship_api_client/models/cdr_started_by_token_dto_auth_method.py
+-rw-r--r--   0        0        0      230 2024-03-25 19:42:53.020906 longship-2024.4.15/longship_api_client/models/cdr_started_by_token_dto_token_type.py
+-rw-r--r--   0        0        0     2004 2024-03-25 19:42:53.011062 longship-2024.4.15/longship_api_client/models/change_availability_request.py
+-rw-r--r--   0        0        0      194 2024-03-25 19:42:53.014134 longship-2024.4.15/longship_api_client/models/change_availability_request_type.py
+-rw-r--r--   0        0        0     1659 2024-03-25 19:42:53.012267 longship-2024.4.15/longship_api_client/models/change_configuration_request.py
+-rw-r--r--   0        0        0     6741 2024-03-25 20:16:17.148174 longship-2024.4.15/longship_api_client/models/charge_point_authorize_get_dto.py
+-rw-r--r--   0        0        0      247 2024-03-25 19:42:53.016677 longship-2024.4.15/longship_api_client/models/charge_point_authorize_get_dto_authorization_request_type.py
+-rw-r--r--   0        0        0     1952 2024-03-25 19:42:53.023232 longship-2024.4.15/longship_api_client/models/charge_point_authorize_post_dto.py
+-rw-r--r--   0        0        0     3974 2024-03-25 20:16:17.145652 longship-2024.4.15/longship_api_client/models/chargepoint_configuration_items_dto.py
+-rw-r--r--   0        0        0     6602 2024-03-25 20:16:17.147802 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto.py
+-rw-r--r--   0        0        0      176 2024-03-25 19:42:53.009231 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_format.py
+-rw-r--r--   0        0        0      405 2024-03-25 19:42:53.018023 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_operational_status.py
+-rw-r--r--   0        0        0      211 2024-03-25 19:42:53.010045 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_power_type.py
+-rw-r--r--   0        0        0     1100 2024-03-25 19:42:53.018437 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_standard.py
+-rw-r--r--   0        0        0    17389 2024-03-25 20:16:17.145591 longship-2024.4.15/longship_api_client/models/chargepoint_dto.py
+-rw-r--r--   0        0        0      183 2024-03-25 19:42:53.011286 longship-2024.4.15/longship_api_client/models/chargepoint_dto_connectivity_status.py
+-rw-r--r--   0        0        0     2642 2024-03-25 19:42:53.024330 longship-2024.4.15/longship_api_client/models/chargepoint_evse_dto.py
+-rw-r--r--   0        0        0     3811 2024-03-25 19:42:53.007865 longship-2024.4.15/longship_api_client/models/chargepoint_put_dto.py
+-rw-r--r--   0        0        0     7493 2024-03-25 20:16:17.145543 longship-2024.4.15/longship_api_client/models/chargepoint_status_dto.py
+-rw-r--r--   0        0        0      189 2024-03-25 19:42:53.009010 longship-2024.4.15/longship_api_client/models/chargepoint_status_dto_connectivity_status.py
+-rw-r--r--   0        0        0     3910 2024-03-25 20:16:17.145642 longship-2024.4.15/longship_api_client/models/charging_meter_value_dto.py
+-rw-r--r--   0        0        0     1197 2024-03-25 19:42:53.007491 longship-2024.4.15/longship_api_client/models/charging_meter_value_dto_measurand.py
+-rw-r--r--   0        0        0      402 2024-03-25 19:42:53.023405 longship-2024.4.15/longship_api_client/models/charging_meter_value_dto_unit.py
+-rw-r--r--   0        0        0     3263 2024-03-25 20:16:17.147852 longship-2024.4.15/longship_api_client/models/charging_period_dto.py
+-rw-r--r--   0        0        0     6374 2024-03-25 20:16:17.147690 longship-2024.4.15/longship_api_client/models/charging_profile.py
+-rw-r--r--   0        0        0      219 2024-03-25 19:42:53.008080 longship-2024.4.15/longship_api_client/models/charging_profile_charging_profile_kind.py
+-rw-r--r--   0        0        0      264 2024-03-25 19:42:53.011335 longship-2024.4.15/longship_api_client/models/charging_profile_charging_profile_purpose.py
+-rw-r--r--   0        0        0      176 2024-03-25 19:42:53.018510 longship-2024.4.15/longship_api_client/models/charging_profile_recurrency_kind.py
+-rw-r--r--   0        0        0     4491 2024-03-25 20:16:17.145717 longship-2024.4.15/longship_api_client/models/charging_schedule.py
+-rw-r--r--   0        0        0      161 2024-03-25 19:42:53.009681 longship-2024.4.15/longship_api_client/models/charging_schedule_charging_rate_unit.py
+-rw-r--r--   0        0        0     2112 2024-03-25 19:42:53.022080 longship-2024.4.15/longship_api_client/models/charging_schedule_period.py
+-rw-r--r--   0        0        0     1234 2024-03-25 19:42:53.014036 longship-2024.4.15/longship_api_client/models/clear_cache_request.py
+-rw-r--r--   0        0        0     3655 2024-03-25 20:16:17.145699 longship-2024.4.15/longship_api_client/models/clear_charging_profile_request.py
+-rw-r--r--   0        0        0      276 2024-03-25 19:42:53.008242 longship-2024.4.15/longship_api_client/models/clear_charging_profile_request_charging_profile_purpose.py
+-rw-r--r--   0        0        0     5941 2024-03-25 20:16:17.148149 longship-2024.4.15/longship_api_client/models/connector_dto.py
+-rw-r--r--   0        0        0      165 2024-03-25 19:42:53.010260 longship-2024.4.15/longship_api_client/models/connector_dto_format.py
+-rw-r--r--   0        0        0      200 2024-03-25 19:42:53.025462 longship-2024.4.15/longship_api_client/models/connector_dto_power_type.py
+-rw-r--r--   0        0        0     1089 2024-03-25 19:42:53.013664 longship-2024.4.15/longship_api_client/models/connector_dto_standard.py
+-rw-r--r--   0        0        0     3663 2024-03-25 20:16:17.145707 longship-2024.4.15/longship_api_client/models/connector_operational_status_dto.py
+-rw-r--r--   0        0        0      411 2024-03-25 19:42:53.023397 longship-2024.4.15/longship_api_client/models/connector_operational_status_dto_operational_status.py
+-rw-r--r--   0        0        0     6482 2024-03-25 20:16:17.256119 longship-2024.4.15/longship_api_client/models/cs_charging_profiles.py
+-rw-r--r--   0        0        0      222 2024-03-25 19:42:53.021273 longship-2024.4.15/longship_api_client/models/cs_charging_profiles_charging_profile_kind.py
+-rw-r--r--   0        0        0      267 2024-03-25 19:42:53.020067 longship-2024.4.15/longship_api_client/models/cs_charging_profiles_charging_profile_purpose.py
+-rw-r--r--   0        0        0      179 2024-03-25 19:42:53.023924 longship-2024.4.15/longship_api_client/models/cs_charging_profiles_recurrency_kind.py
+-rw-r--r--   0        0        0     2101 2024-03-25 19:42:53.016959 longship-2024.4.15/longship_api_client/models/data_transfer_request.py
+-rw-r--r--   0        0        0     1830 2024-03-25 19:42:53.020953 longship-2024.4.15/longship_api_client/models/display_text_dto.py
+-rw-r--r--   0        0        0     3861 2024-03-25 19:42:53.020545 longship-2024.4.15/longship_api_client/models/energy_mix_dto.py
+-rw-r--r--   0        0        0     2351 2024-03-25 20:16:17.145600 longship-2024.4.15/longship_api_client/models/energy_source_dto.py
+-rw-r--r--   0        0        0      316 2024-03-25 19:42:53.012770 longship-2024.4.15/longship_api_client/models/energy_source_dto_source.py
+-rw-r--r--   0        0        0     2298 2024-03-25 20:16:17.145551 longship-2024.4.15/longship_api_client/models/entity_tag_header_value.py
+-rw-r--r--   0        0        0     2480 2024-03-25 20:16:17.147583 longship-2024.4.15/longship_api_client/models/environmental_impact_dto.py
+-rw-r--r--   0        0        0      209 2024-03-25 19:42:53.026019 longship-2024.4.15/longship_api_client/models/environmental_impact_dto_category.py
+-rw-r--r--   0        0        0     2743 2024-03-25 20:16:17.119953 longship-2024.4.15/longship_api_client/models/exceptional_period_dto.py
+-rw-r--r--   0        0        0     4820 2024-03-25 20:16:17.148052 longship-2024.4.15/longship_api_client/models/file_content_result.py
+-rw-r--r--   0        0        0     1885 2024-03-25 19:42:53.012418 longship-2024.4.15/longship_api_client/models/geo_location_dto.py
+-rw-r--r--   0        0        0      190 2024-03-25 19:42:53.008926 longship-2024.4.15/longship_api_client/models/get_all_cdrs_order_by.py
+-rw-r--r--   0        0        0      215 2024-03-25 19:42:53.021733 longship-2024.4.15/longship_api_client/models/get_all_chargepoints_accesstype.py
+-rw-r--r--   0        0        0      167 2024-03-25 19:42:53.025610 longship-2024.4.15/longship_api_client/models/get_all_chargepoints_chargerpowertype.py
+-rw-r--r--   0        0        0      400 2024-03-25 19:42:53.024331 longship-2024.4.15/longship_api_client/models/get_all_chargepoints_operationalstatus.py
+-rw-r--r--   0        0        0      224 2024-03-25 19:42:53.016650 longship-2024.4.15/longship_api_client/models/get_all_chargepoints_order_by.py
+-rw-r--r--   0        0        0      232 2024-03-25 19:42:53.013135 longship-2024.4.15/longship_api_client/models/get_all_locations_accesstype.py
+-rw-r--r--   0        0        0      164 2024-03-25 19:42:53.017035 longship-2024.4.15/longship_api_client/models/get_all_locations_chargerpowertype.py
+-rw-r--r--   0        0        0      191 2024-03-25 19:42:53.013268 longship-2024.4.15/longship_api_client/models/get_all_locations_order_by.py
+-rw-r--r--   0        0        0      203 2024-03-25 19:42:53.009543 longship-2024.4.15/longship_api_client/models/get_all_reimbursementcdrs_order_by.py
+-rw-r--r--   0        0        0      164 2024-03-25 19:42:53.025145 longship-2024.4.15/longship_api_client/models/get_all_sessions_order_by.py
+-rw-r--r--   0        0        0      221 2024-03-25 19:42:53.016938 longship-2024.4.15/longship_api_client/models/get_all_tariffdistributions_order_by.py
+-rw-r--r--   0        0        0      203 2024-03-25 19:42:53.024996 longship-2024.4.15/longship_api_client/models/get_all_tariffs_order_by.py
+-rw-r--r--   0        0        0      144 2024-03-25 19:42:53.012343 longship-2024.4.15/longship_api_client/models/get_all_webhooks_order_by.py
+-rw-r--r--   0        0        0     3021 2024-03-25 20:16:17.147746 longship-2024.4.15/longship_api_client/models/get_composite_schedule_request.py
+-rw-r--r--   0        0        0      172 2024-03-25 19:42:53.013558 longship-2024.4.15/longship_api_client/models/get_composite_schedule_request_charging_rate_unit.py
+-rw-r--r--   0        0        0     1742 2024-03-25 20:00:43.999594 longship-2024.4.15/longship_api_client/models/get_configuration_request.py
+-rw-r--r--   0        0        0     3494 2024-03-25 20:16:17.147616 longship-2024.4.15/longship_api_client/models/get_diagnostics_request.py
+-rw-r--r--   0        0        0     1285 2024-03-25 19:42:53.022880 longship-2024.4.15/longship_api_client/models/get_local_list_version_request.py
+-rw-r--r--   0        0        0     5058 2024-03-25 20:00:43.999981 longship-2024.4.15/longship_api_client/models/hours_dto.py
+-rw-r--r--   0        0        0     2708 2024-03-25 20:16:17.147923 longship-2024.4.15/longship_api_client/models/id_tag_info.py
+-rw-r--r--   0        0        0      252 2024-03-25 19:42:53.014006 longship-2024.4.15/longship_api_client/models/id_tag_info_status.py
+-rw-r--r--   0        0        0     3271 2024-03-25 20:16:17.145569 longship-2024.4.15/longship_api_client/models/image_dto.py
+-rw-r--r--   0        0        0      287 2024-03-25 19:42:53.010942 longship-2024.4.15/longship_api_client/models/image_dto_category.py
+-rw-r--r--   0        0        0     8733 2024-03-25 20:16:17.148073 longship-2024.4.15/longship_api_client/models/interchange_format_cdr.py
+-rw-r--r--   0        0        0     5819 2024-03-25 20:16:17.119922 longship-2024.4.15/longship_api_client/models/local_token_group_get_dto.py
+-rw-r--r--   0        0        0     4431 2024-03-25 19:42:53.011938 longship-2024.4.15/longship_api_client/models/local_token_group_post_dto.py
+-rw-r--r--   0        0        0     4394 2024-03-25 19:42:53.010143 longship-2024.4.15/longship_api_client/models/local_token_group_put_dto.py
+-rw-r--r--   0        0        0     2829 2024-03-25 19:42:53.012581 longship-2024.4.15/longship_api_client/models/local_token_group_token_get_dto.py
+-rw-r--r--   0        0        0     2416 2024-03-25 19:42:53.020751 longship-2024.4.15/longship_api_client/models/local_token_group_token_post_dto.py
+-rw-r--r--   0        0        0     2411 2024-03-25 19:42:53.025595 longship-2024.4.15/longship_api_client/models/local_token_group_token_put_dto.py
+-rw-r--r--   0        0        0     1722 2024-03-25 19:42:53.012238 longship-2024.4.15/longship_api_client/models/location_charge_point_dto.py
+-rw-r--r--   0        0        0    19679 2024-03-25 20:16:17.112028 longship-2024.4.15/longship_api_client/models/location_dto.py
+-rw-r--r--   0        0        0      706 2024-03-25 19:42:53.011179 longship-2024.4.15/longship_api_client/models/location_dto_facilities_item.py
+-rw-r--r--   0        0        0      341 2024-03-25 19:42:53.021534 longship-2024.4.15/longship_api_client/models/location_dto_parking_type.py
+-rw-r--r--   0        0        0    11826 2024-03-25 20:16:17.145579 longship-2024.4.15/longship_api_client/models/location_evse_dto.py
+-rw-r--r--   0        0        0      698 2024-03-25 19:42:53.012072 longship-2024.4.15/longship_api_client/models/location_evse_dto_capabilities_item.py
+-rw-r--r--   0        0        0      277 2024-03-25 19:42:53.009142 longship-2024.4.15/longship_api_client/models/location_evse_dto_parking_restrictions_item.py
+-rw-r--r--   0        0        0      364 2024-03-25 19:42:53.014428 longship-2024.4.15/longship_api_client/models/location_evse_dto_status.py
+-rw-r--r--   0        0        0    18562 2024-03-25 20:16:17.147645 longship-2024.4.15/longship_api_client/models/location_post_dto.py
+-rw-r--r--   0        0        0      710 2024-03-25 19:42:53.024083 longship-2024.4.15/longship_api_client/models/location_post_dto_facilities_item.py
+-rw-r--r--   0        0        0      345 2024-03-25 19:42:53.009734 longship-2024.4.15/longship_api_client/models/location_post_dto_parking_type.py
+-rw-r--r--   0        0        0    19439 2024-03-25 20:16:17.148097 longship-2024.4.15/longship_api_client/models/location_put_dto.py
+-rw-r--r--   0        0        0      709 2024-03-25 19:42:53.024738 longship-2024.4.15/longship_api_client/models/location_put_dto_facilities_item.py
+-rw-r--r--   0        0        0      344 2024-03-25 19:42:53.025234 longship-2024.4.15/longship_api_client/models/location_put_dto_parking_type.py
+-rw-r--r--   0        0        0     1957 2024-03-25 20:00:44.002906 longship-2024.4.15/longship_api_client/models/location_tariff_distribution_dto.py
+-rw-r--r--   0        0        0     2508 2024-03-25 20:16:17.145478 longship-2024.4.15/longship_api_client/models/longship_error.py
+-rw-r--r--   0        0        0     2024 2024-03-25 19:42:53.020751 longship-2024.4.15/longship_api_client/models/longship_error_detail.py
+-rw-r--r--   0        0        0     6167 2024-03-25 20:16:17.147668 longship-2024.4.15/longship_api_client/models/message_log_dto.py
+-rw-r--r--   0        0        0      219 2024-03-25 19:42:53.023217 longship-2024.4.15/longship_api_client/models/message_log_dto_direction.py
+-rw-r--r--   0        0        0     1335 2024-03-25 19:42:53.013169 longship-2024.4.15/longship_api_client/models/message_log_dto_ocpp_message_type.py
+-rw-r--r--   0        0        0      227 2024-03-25 19:42:53.009907 longship-2024.4.15/longship_api_client/models/message_log_dto_wamp_message_type.py
+-rw-r--r--   0        0        0     2240 2024-03-25 19:42:53.013023 longship-2024.4.15/longship_api_client/models/organization_unit_financial_details_dto.py
+-rw-r--r--   0        0        0    10170 2024-03-25 20:16:17.147951 longship-2024.4.15/longship_api_client/models/organization_unit_get_dto.py
+-rw-r--r--   0        0        0     9395 2024-03-25 20:16:17.147828 longship-2024.4.15/longship_api_client/models/organization_unit_post_dto.py
+-rw-r--r--   0        0        0     9143 2024-03-25 20:16:17.145690 longship-2024.4.15/longship_api_client/models/organization_unit_put_dto.py
+-rw-r--r--   0        0        0     4903 2024-03-25 19:42:53.018883 longship-2024.4.15/longship_api_client/models/price_info_dto.py
+-rw-r--r--   0        0        0     3457 2024-03-25 20:16:17.145445 longship-2024.4.15/longship_api_client/models/private_emp_tariff_dto.py
+-rw-r--r--   0        0        0      161 2024-03-25 19:42:53.013747 longship-2024.4.15/longship_api_client/models/private_emp_tariff_dto_power_type.py
+-rw-r--r--   0        0        0     3107 2024-03-25 20:16:17.145610 longship-2024.4.15/longship_api_client/models/publish_token_type_dto.py
+-rw-r--r--   0        0        0      224 2024-03-25 19:42:53.020185 longship-2024.4.15/longship_api_client/models/publish_token_type_dto_type.py
+-rw-r--r--   0        0        0     2202 2024-03-25 19:42:53.008000 longship-2024.4.15/longship_api_client/models/regular_hours_dto.py
+-rw-r--r--   0        0        0    11559 2024-03-25 20:16:17.145620 longship-2024.4.15/longship_api_client/models/reimburse_info_dto.py
+-rw-r--r--   0        0        0      205 2024-03-25 19:42:53.009099 longship-2024.4.15/longship_api_client/models/reimburse_info_dto_type.py
+-rw-r--r--   0        0        0     4113 2024-03-25 20:16:17.120003 longship-2024.4.15/longship_api_client/models/reimburse_started_by_info_dto.py
+-rw-r--r--   0        0        0      674 2024-03-25 19:42:53.020677 longship-2024.4.15/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py
+-rw-r--r--   0        0        0     5833 2024-03-25 20:16:17.145452 longship-2024.4.15/longship_api_client/models/reimburse_started_by_token_dto.py
+-rw-r--r--   0        0        0      227 2024-03-25 19:42:53.007686 longship-2024.4.15/longship_api_client/models/reimburse_started_by_token_dto_auth_method.py
+-rw-r--r--   0        0        0      236 2024-03-25 19:42:53.014059 longship-2024.4.15/longship_api_client/models/reimburse_started_by_token_dto_token_type.py
+-rw-r--r--   0        0        0     3078 2024-03-25 20:16:17.148013 longship-2024.4.15/longship_api_client/models/reimbursement_bank_details_dto.py
+-rw-r--r--   0        0        0    21978 2024-03-25 20:16:17.145414 longship-2024.4.15/longship_api_client/models/reimbursement_cdr_dto.py
+-rw-r--r--   0        0        0     1971 2024-03-25 19:42:53.010185 longship-2024.4.15/longship_api_client/models/reimbursement_cdr_geo_location_dto.py
+-rw-r--r--   0        0        0     7238 2024-03-25 20:16:17.145366 longship-2024.4.15/longship_api_client/models/reimbursement_cdr_location_dto.py
+-rw-r--r--   0        0        0      215 2024-03-25 19:42:53.014885 longship-2024.4.15/longship_api_client/models/reimbursement_cdr_location_dto_power_type.py
+-rw-r--r--   0        0        0     2435 2024-03-25 19:42:53.015118 longship-2024.4.15/longship_api_client/models/reimbursement_customer_share_dto.py
+-rw-r--r--   0        0        0     1917 2024-03-25 19:42:53.007776 longship-2024.4.15/longship_api_client/models/reimbursement_price_dto.py
+-rw-r--r--   0        0        0     4783 2024-03-25 20:16:17.148122 longship-2024.4.15/longship_api_client/models/reimbursement_tariff_dto.py
+-rw-r--r--   0        0        0      209 2024-03-25 19:42:53.017372 longship-2024.4.15/longship_api_client/models/reimbursement_tariff_dto_status.py
+-rw-r--r--   0        0        0     2853 2024-03-25 20:16:17.145486 longship-2024.4.15/longship_api_client/models/remote_start_transaction_request.py
+-rw-r--r--   0        0        0     1627 2024-03-25 19:42:53.008755 longship-2024.4.15/longship_api_client/models/remote_stop_transaction_request.py
+-rw-r--r--   0        0        0     2644 2024-03-25 20:00:44.006730 longship-2024.4.15/longship_api_client/models/reserve_now_request.py
+-rw-r--r--   0        0        0     1609 2024-03-25 19:42:53.019871 longship-2024.4.15/longship_api_client/models/reset_request.py
+-rw-r--r--   0        0        0      157 2024-03-25 19:42:53.016585 longship-2024.4.15/longship_api_client/models/reset_request_type.py
+-rw-r--r--   0        0        0     3534 2024-03-25 19:42:53.008207 longship-2024.4.15/longship_api_client/models/send_local_list_request.py
+-rw-r--r--   0        0        0      187 2024-03-25 19:42:53.008152 longship-2024.4.15/longship_api_client/models/send_local_list_request_update_type.py
+-rw-r--r--   0        0        0    20526 2024-03-25 20:16:17.147904 longship-2024.4.15/longship_api_client/models/session_dto.py
+-rw-r--r--   0        0        0      194 2024-03-25 19:42:53.016855 longship-2024.4.15/longship_api_client/models/session_dto_approval_status.py
+-rw-r--r--   0        0        0      166 2024-03-25 19:42:53.022905 longship-2024.4.15/longship_api_client/models/session_dto_review_scenario_type.py
+-rw-r--r--   0        0        0      251 2024-03-25 19:42:53.022178 longship-2024.4.15/longship_api_client/models/session_dto_status.py
+-rw-r--r--   0        0        0     1923 2024-03-25 19:42:53.012037 longship-2024.4.15/longship_api_client/models/session_geo_location_dto.py
+-rw-r--r--   0        0        0     6980 2024-03-25 20:16:17.145434 longship-2024.4.15/longship_api_client/models/session_location_dto.py
+-rw-r--r--   0        0        0      206 2024-03-25 19:42:53.009978 longship-2024.4.15/longship_api_client/models/session_location_dto_power_type.py
+-rw-r--r--   0        0        0     3985 2024-03-25 20:16:17.145661 longship-2024.4.15/longship_api_client/models/session_threshold_check_dto.py
+-rw-r--r--   0        0        0      265 2024-03-25 19:42:53.014604 longship-2024.4.15/longship_api_client/models/session_threshold_check_dto_status.py
+-rw-r--r--   0        0        0      204 2024-03-25 19:42:53.023710 longship-2024.4.15/longship_api_client/models/session_threshold_check_dto_threshold_hit_outcome.py
+-rw-r--r--   0        0        0     4525 2024-03-25 20:16:17.145378 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_decimal.py
+-rw-r--r--   0        0        0      272 2024-03-25 19:42:53.024219 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_decimal_status.py
+-rw-r--r--   0        0        0      211 2024-03-25 19:42:53.023536 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_decimal_threshold_hit_outcome.py
+-rw-r--r--   0        0        0     4484 2024-03-25 20:16:17.145503 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_int_32.py
+-rw-r--r--   0        0        0      270 2024-03-25 19:42:53.025721 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_int_32_status.py
+-rw-r--r--   0        0        0      209 2024-03-25 19:42:53.011068 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_int_32_threshold_hit_outcome.py
+-rw-r--r--   0        0        0    10975 2024-03-25 20:16:17.145734 longship-2024.4.15/longship_api_client/models/session_thresholds_dto.py
+-rw-r--r--   0        0        0      462 2024-03-25 19:42:53.010379 longship-2024.4.15/longship_api_client/models/session_thresholds_dto_thresholds_hit_item.py
+-rw-r--r--   0        0        0     2133 2024-03-25 19:42:53.011494 longship-2024.4.15/longship_api_client/models/set_charging_profile_request.py
+-rw-r--r--   0        0        0     5359 2024-03-25 20:16:17.145671 longship-2024.4.15/longship_api_client/models/started_by_info_dto.py
+-rw-r--r--   0        0        0      665 2024-03-25 19:42:53.016182 longship-2024.4.15/longship_api_client/models/started_by_info_dto_authorization_state.py
+-rw-r--r--   0        0        0      182 2024-03-25 19:42:53.013508 longship-2024.4.15/longship_api_client/models/started_by_info_dto_roaming_platform_type.py
+-rw-r--r--   0        0        0     5597 2024-03-25 20:16:17.147985 longship-2024.4.15/longship_api_client/models/started_by_token_dto.py
+-rw-r--r--   0        0        0      218 2024-03-25 19:42:53.016010 longship-2024.4.15/longship_api_client/models/started_by_token_dto_auth_method.py
+-rw-r--r--   0        0        0      227 2024-03-25 19:42:53.023627 longship-2024.4.15/longship_api_client/models/started_by_token_dto_token_type.py
+-rw-r--r--   0        0        0     3466 2024-03-25 20:16:17.120060 longship-2024.4.15/longship_api_client/models/status_schedule_dto.py
+-rw-r--r--   0        0        0      366 2024-03-25 19:42:53.021753 longship-2024.4.15/longship_api_client/models/status_schedule_dto_status.py
+-rw-r--r--   0        0        0     2582 2024-03-25 19:42:53.021647 longship-2024.4.15/longship_api_client/models/string_segment.py
+-rw-r--r--   0        0        0     2931 2024-03-25 20:16:17.145561 longship-2024.4.15/longship_api_client/models/tariff_assertion_dto.py
+-rw-r--r--   0        0        0      283 2024-03-25 19:42:53.021845 longship-2024.4.15/longship_api_client/models/tariff_assertion_dto_tariff_type.py
+-rw-r--r--   0        0        0     6670 2024-03-25 20:16:17.145469 longship-2024.4.15/longship_api_client/models/tariff_distribution_get_dto.py
+-rw-r--r--   0        0        0     3746 2024-03-25 20:16:17.120079 longship-2024.4.15/longship_api_client/models/tariff_distribution_history_dto.py
+-rw-r--r--   0        0        0     3517 2024-03-25 19:42:53.019575 longship-2024.4.15/longship_api_client/models/tariff_distribution_post_dto.py
+-rw-r--r--   0        0        0     3512 2024-03-25 19:42:53.024792 longship-2024.4.15/longship_api_client/models/tariff_distribution_put_dto.py
+-rw-r--r--   0        0        0    14806 2024-03-25 20:16:17.145460 longship-2024.4.15/longship_api_client/models/tariff_dto.py
+-rw-r--r--   0        0        0      186 2024-03-25 19:42:53.025570 longship-2024.4.15/longship_api_client/models/tariff_dto_tariff_type.py
+-rw-r--r--   0        0        0      241 2024-03-25 19:42:53.009523 longship-2024.4.15/longship_api_client/models/tariff_dto_usage_type.py
+-rw-r--r--   0        0        0     6088 2024-03-25 19:42:53.022020 longship-2024.4.15/longship_api_client/models/tariff_info_dto.py
+-rw-r--r--   0        0        0     8582 2024-03-25 20:16:17.119980 longship-2024.4.15/longship_api_client/models/tariff_post_dto.py
+-rw-r--r--   0        0        0      245 2024-03-25 19:42:53.009116 longship-2024.4.15/longship_api_client/models/tariff_post_dto_usage_type.py
+-rw-r--r--   0        0        0     9227 2024-03-25 20:16:17.145424 longship-2024.4.15/longship_api_client/models/tariff_price_dto.py
+-rw-r--r--   0        0        0      209 2024-03-25 19:42:53.023536 longship-2024.4.15/longship_api_client/models/tariff_price_dto_approval_status.py
+-rw-r--r--   0        0        0     8440 2024-03-25 20:16:17.120039 longship-2024.4.15/longship_api_client/models/tariff_put_dto.py
+-rw-r--r--   0        0        0     4065 2024-03-25 20:16:17.145680 longship-2024.4.15/longship_api_client/models/tariff_restriction.py
+-rw-r--r--   0        0        0      244 2024-03-25 19:42:53.009878 longship-2024.4.15/longship_api_client/models/tariff_restriction_day_of_week.py
+-rw-r--r--   0        0        0     2668 2024-03-25 20:16:17.145523 longship-2024.4.15/longship_api_client/models/token_info_dto.py
+-rw-r--r--   0        0        0      216 2024-03-25 19:42:53.015173 longship-2024.4.15/longship_api_client/models/token_info_dto_token_type.py
+-rw-r--r--   0        0        0     2385 2024-03-25 19:42:53.021311 longship-2024.4.15/longship_api_client/models/trigger_message_request.py
+-rw-r--r--   0        0        0      420 2024-03-25 19:42:53.016098 longship-2024.4.15/longship_api_client/models/trigger_message_request_requested_message.py
+-rw-r--r--   0        0        0     1574 2024-03-25 19:42:53.014314 longship-2024.4.15/longship_api_client/models/unlock_connector_request.py
+-rw-r--r--   0        0        0     2514 2024-03-25 20:00:44.012302 longship-2024.4.15/longship_api_client/models/update_firmware_request.py
+-rw-r--r--   0        0        0     5538 2024-03-25 20:16:17.145402 longship-2024.4.15/longship_api_client/models/webhook_get_dto.py
+-rw-r--r--   0        0        0      578 2024-03-25 19:42:53.025317 longship-2024.4.15/longship_api_client/models/webhook_get_dto_event_types_item.py
+-rw-r--r--   0        0        0     1807 2024-03-25 19:42:53.024132 longship-2024.4.15/longship_api_client/models/webhook_header_dto.py
+-rw-r--r--   0        0        0     4123 2024-03-25 20:00:44.013135 longship-2024.4.15/longship_api_client/models/webhook_post_dto.py
+-rw-r--r--   0        0        0      579 2024-03-25 19:42:53.011270 longship-2024.4.15/longship_api_client/models/webhook_post_dto_event_types_item.py
+-rw-r--r--   0        0        0     4113 2024-03-25 19:42:53.010850 longship-2024.4.15/longship_api_client/models/webhook_put_dto.py
+-rw-r--r--   0        0        0      578 2024-03-25 19:42:53.014129 longship-2024.4.15/longship_api_client/models/webhook_put_dto_event_types_item.py
+-rw-r--r--   0        0        0     4250 2024-03-25 20:16:17.145514 longship-2024.4.15/longship_api_client/models/webhook_summary_get_dto.py
+-rw-r--r--   0        0        0      585 2024-03-25 19:42:53.012248 longship-2024.4.15/longship_api_client/models/webhook_summary_get_dto_event_types_item.py
+-rw-r--r--   0        0        0       25 2024-03-25 19:42:52.041583 longship-2024.4.15/longship_api_client/py.typed
+-rw-r--r--   0        0        0      985 2024-03-25 19:42:53.022168 longship-2024.4.15/longship_api_client/types.py
+-rw-r--r--   0        0        0      818 2024-04-15 16:03:15.114118 longship-2024.4.15/pyproject.toml
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 longship-2024.4.15/PKG-INFO
```

### Comparing `longship-2024.3.15/LICENSE` & `longship-2024.4.15/LICENSE`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/README.md` & `longship-2024.4.15/README.md`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship/client.py` & `longship-2024.4.15/longship/client.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship/types.py` & `longship-2024.4.15/longship/types.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/cdrs/cdr_get.py` & `longship-2024.4.15/longship_api_client/api/cdrs/cdr_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/cdrs/cdr_patch.py` & `longship-2024.4.15/longship_api_client/api/cdrs/cdr_patch.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/cdrs/get_all_cdrs.py` & `longship-2024.4.15/longship_api_client/api/cdrs/get_all_cdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/cdrs/get_all_interchangeformat.py` & `longship-2024.4.15/longship_api_client/api/cdrs/get_all_interchangeformat.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/cdrs/get_file_full_download_cdrs.py` & `longship-2024.4.15/longship_api_client/api/cdrs/get_file_full_download_cdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py` & `longship-2024.4.15/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/chargepoint_status/chargepoint_status_get.py` & `longship-2024.4.15/longship_api_client/api/chargepoint_status/chargepoint_status_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py` & `longship-2024.4.15/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/chargepoints/chargepoint_get.py` & `longship-2024.4.15/longship_api_client/api/chargepoints/chargepoint_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/chargepoints/chargepoint_put.py` & `longship-2024.4.15/longship_api_client/api/chargepoints/chargepoint_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/chargepoints/chargepointauthorization_get.py` & `longship-2024.4.15/longship_api_client/api/chargepoints/chargepointauthorization_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/chargepoints/chargepointauthorization_post.py` & `longship-2024.4.15/longship_api_client/api/chargepoints/chargepointauthorization_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/chargepoints/get_all_chargepointauthorizations.py` & `longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepointauthorizations.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/chargepoints/get_all_chargepointmessages.py` & `longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepointmessages.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/chargepoints/get_all_chargepoints.py` & `longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepoints.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_cancel_reservation_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_cancel_reservation_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_change_availability_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_change_availability_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_change_configuration_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_change_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_clear_cache_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_clear_cache_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_clear_charging_profile_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_clear_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_data_transfer_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_data_transfer_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_get_composite_schedule_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_get_composite_schedule_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_get_configuration_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_get_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_get_diagnostics_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_get_diagnostics_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_get_local_list_version_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_get_local_list_version_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_remote_start_transaction_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_remote_start_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_remote_stop_transaction_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_remote_stop_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_reserve_now_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_reserve_now_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_reset_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_reset_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_send_local_list_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_send_local_list_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_set_charging_profile_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_set_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_trigger_message_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_trigger_message_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_unlock_connector_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_unlock_connector_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/commands/send_update_firmware_request.py` & `longship-2024.4.15/longship_api_client/api/commands/send_update_firmware_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/configurationitems/configurationitem_get.py` & `longship-2024.4.15/longship_api_client/api/configurationitems/configurationitem_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/localtokengroups/get_all_localtokengroups.py` & `longship-2024.4.15/longship_api_client/api/localtokengroups/get_all_localtokengroups.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/localtokengroups/local_token_group_delete.py` & `longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/localtokengroups/local_token_group_post.py` & `longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/localtokengroups/local_token_group_put.py` & `longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/localtokengroups/localtokengroup_get.py` & `longship-2024.4.15/longship_api_client/api/localtokengroups/localtokengroup_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_delete.py` & `longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_post.py` & `longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_put.py` & `longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/location/location_patch.py` & `longship-2024.4.15/longship_api_client/api/location/location_patch.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/locations/get_all_locations.py` & `longship-2024.4.15/longship_api_client/api/locations/get_all_locations.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/locations/location_get.py` & `longship-2024.4.15/longship_api_client/api/locations/location_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/locations/location_post.py` & `longship-2024.4.15/longship_api_client/api/locations/location_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/locations/location_put.py` & `longship-2024.4.15/longship_api_client/api/locations/location_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py` & `longship-2024.4.15/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py` & `longship-2024.4.15/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py` & `longship-2024.4.15/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/organizationunits/get_all_organizationunits.py` & `longship-2024.4.15/longship_api_client/api/organizationunits/get_all_organizationunits.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/organizationunits/organization_unit_get.py` & `longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/organizationunits/organization_unit_post.py` & `longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/organizationunits/organization_unit_put.py` & `longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py` & `longship-2024.4.15/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py` & `longship-2024.4.15/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/reimbursement/reimbursement_cdr_get.py` & `longship-2024.4.15/longship_api_client/api/reimbursement/reimbursement_cdr_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/sessions/get_all_sessions.py` & `longship-2024.4.15/longship_api_client/api/sessions/get_all_sessions.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/sessions/session_get.py` & `longship-2024.4.15/longship_api_client/api/sessions/session_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py` & `longship-2024.4.15/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_delete.py` & `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_get.py` & `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_patch.py` & `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_patch.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_post.py` & `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffdistributions/tariffdistribution_put.py` & `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffs/get_all_tariffs.py` & `longship-2024.4.15/longship_api_client/api/tariffs/get_all_tariffs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffs/tariff_delete.py` & `longship-2024.4.15/longship_api_client/api/tariffs/tariff_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffs/tariff_get.py` & `longship-2024.4.15/longship_api_client/api/tariffs/tariff_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffs/tariff_patch.py` & `longship-2024.4.15/longship_api_client/api/tariffs/tariff_patch.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffs/tariff_post.py` & `longship-2024.4.15/longship_api_client/api/tariffs/tariff_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/tariffs/tariff_put.py` & `longship-2024.4.15/longship_api_client/api/tariffs/tariff_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/webhooks/get_all_webhooks.py` & `longship-2024.4.15/longship_api_client/api/webhooks/get_all_webhooks.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/webhooks/webhook_delete.py` & `longship-2024.4.15/longship_api_client/api/webhooks/webhook_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/webhooks/webhook_get.py` & `longship-2024.4.15/longship_api_client/api/webhooks/webhook_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/webhooks/webhook_post.py` & `longship-2024.4.15/longship_api_client/api/webhooks/webhook_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/api/webhooks/webhook_put.py` & `longship-2024.4.15/longship_api_client/api/webhooks/webhook_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/client.py` & `longship-2024.4.15/longship_api_client/client.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/errors.py` & `longship-2024.4.15/longship_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/__init__.py` & `longship-2024.4.15/longship_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/additional_geo_location_dto.py` & `longship-2024.4.15/longship_api_client/models/additional_geo_location_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         d = src_dict.copy()
         latitude = d.pop("latitude", UNSET)
 
         longitude = d.pop("longitude", UNSET)
 
         _name = d.pop("name", UNSET)
         name: Union[Unset, DisplayTextDto]
-        if isinstance(_name, Unset):
+        if isinstance(_name, Unset) or _name is None:
             name = UNSET
         else:
             name = DisplayTextDto.from_dict(_name)
 
         additional_geo_location_dto = cls(
             latitude=latitude,
             longitude=longitude,
```

### Comparing `longship-2024.3.15/longship_api_client/models/authorization_assertion_dto.py` & `longship-2024.4.15/longship_api_client/models/authorization_assertion_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,26 +61,26 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _auth_scenario_type = d.pop("authScenarioType", UNSET)
         auth_scenario_type: Union[Unset, AuthorizationAssertionDtoAuthScenarioType]
-        if isinstance(_auth_scenario_type, Unset):
+        if isinstance(_auth_scenario_type, Unset) or _auth_scenario_type is None:
             auth_scenario_type = UNSET
         else:
             auth_scenario_type = AuthorizationAssertionDtoAuthScenarioType(
                 _auth_scenario_type
             )
 
         auth_result = d.pop("authResult", UNSET)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, AuthorizationAssertionDtoStatus]
-        if isinstance(_status, Unset):
+        if isinstance(_status, Unset) or _status is None:
             status = UNSET
         else:
             status = AuthorizationAssertionDtoStatus(_status)
 
         authorization_assertion_dto = cls(
             auth_scenario_type=auth_scenario_type,
             auth_result=auth_result,
```

### Comparing `longship-2024.3.15/longship_api_client/models/authorization_assertion_dto_auth_scenario_type.py` & `longship-2024.4.15/longship_api_client/models/authorization_assertion_dto_auth_scenario_type.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/authorization_charger_context_dto.py` & `longship-2024.4.15/longship_api_client/models/authorization_charger_context_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/authorization_context_details_dto.py` & `longship-2024.4.15/longship_api_client/models/authorization_context_details_dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,22 +59,22 @@
         from ..models.authorization_tenant_context_dto import (
             AuthorizationTenantContextDto,
         )
 
         d = src_dict.copy()
         _charger = d.pop("charger", UNSET)
         charger: Union[Unset, AuthorizationChargerContextDto]
-        if isinstance(_charger, Unset):
+        if isinstance(_charger, Unset) or _charger is None:
             charger = UNSET
         else:
             charger = AuthorizationChargerContextDto.from_dict(_charger)
 
         _tenant = d.pop("tenant", UNSET)
         tenant: Union[Unset, AuthorizationTenantContextDto]
-        if isinstance(_tenant, Unset):
+        if isinstance(_tenant, Unset) or _tenant is None:
             tenant = UNSET
         else:
             tenant = AuthorizationTenantContextDto.from_dict(_tenant)
 
         authorization_context_details_dto = cls(
             charger=charger,
             tenant=tenant,
```

### Comparing `longship-2024.3.15/longship_api_client/models/authorization_data.py` & `longship-2024.4.15/longship_api_client/models/authorization_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         from ..models.id_tag_info import IdTagInfo
 
         d = src_dict.copy()
         id_tag = d.pop("idTag")
 
         _id_tag_info = d.pop("idTagInfo", UNSET)
         id_tag_info: Union[Unset, IdTagInfo]
-        if isinstance(_id_tag_info, Unset):
+        if isinstance(_id_tag_info, Unset) or _id_tag_info is None:
             id_tag_info = UNSET
         else:
             id_tag_info = IdTagInfo.from_dict(_id_tag_info)
 
         authorization_data = cls(
             id_tag=id_tag,
             id_tag_info=id_tag_info,
```

### Comparing `longship-2024.3.15/longship_api_client/models/authorization_result_dto.py` & `longship-2024.4.15/longship_api_client/models/authorization_result_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,22 +81,22 @@
         for assertion_item_data in _assertion or []:
             assertion_item = AuthorizationAssertionDto.from_dict(assertion_item_data)
 
             assertion.append(assertion_item)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, AuthorizationResultDtoStatus]
-        if isinstance(_status, Unset):
+        if isinstance(_status, Unset) or _status is None:
             status = UNSET
         else:
             status = AuthorizationResultDtoStatus(_status)
 
         _reason = d.pop("reason", UNSET)
         reason: Union[Unset, AuthorizationResultDtoReason]
-        if isinstance(_reason, Unset):
+        if isinstance(_reason, Unset) or _reason is None:
             reason = UNSET
         else:
             reason = AuthorizationResultDtoReason(_reason)
 
         description = d.pop("description", UNSET)
 
         authorization_result_dto = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/authorization_result_dto_reason.py` & `longship-2024.4.15/longship_api_client/models/authorization_result_dto_reason.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/authorization_tenant_context_dto.py` & `longship-2024.4.15/longship_api_client/models/authorization_tenant_context_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/business_details_dto.py` & `longship-2024.4.15/longship_api_client/models/business_details_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         d = src_dict.copy()
         name = d.pop("name", UNSET)
 
         website = d.pop("website", UNSET)
 
         _image = d.pop("image", UNSET)
         image: Union[Unset, ImageDto]
-        if isinstance(_image, Unset):
+        if isinstance(_image, Unset) or _image is None:
             image = UNSET
         else:
             image = ImageDto.from_dict(_image)
 
         business_details_dto = cls(
             name=name,
             website=website,
```

### Comparing `longship-2024.3.15/longship_api_client/models/cancel_reservation_request.py` & `longship-2024.4.15/longship_api_client/models/cancel_reservation_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/cdr_dto.py` & `longship-2024.4.15/longship_api_client/models/cdr_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -266,40 +266,40 @@
 
         charge_point_id = d.pop("chargePointId", UNSET)
 
         connector_id = d.pop("connectorId", UNSET)
 
         _cdr_location = d.pop("cdrLocation", UNSET)
         cdr_location: Union[Unset, CdrLocationDto]
-        if isinstance(_cdr_location, Unset):
+        if isinstance(_cdr_location, Unset) or _cdr_location is None:
             cdr_location = UNSET
         else:
             cdr_location = CdrLocationDto.from_dict(_cdr_location)
 
         _start_datetime = d.pop("startDatetime", UNSET)
         start_datetime: Union[Unset, datetime.datetime]
-        if isinstance(_start_datetime, Unset):
+        if isinstance(_start_datetime, Unset) or _start_datetime is None:
             start_datetime = UNSET
         else:
             start_datetime = isoparse(_start_datetime)
 
         _end_date_time = d.pop("endDateTime", UNSET)
         end_date_time: Union[Unset, datetime.datetime]
-        if isinstance(_end_date_time, Unset):
+        if isinstance(_end_date_time, Unset) or _end_date_time is None:
             end_date_time = UNSET
         else:
             end_date_time = isoparse(_end_date_time)
 
         session_id = d.pop("sessionId", UNSET)
 
         token = d.pop("token", UNSET)
 
         _started_by_info = d.pop("startedByInfo", UNSET)
         started_by_info: Union[Unset, CdrStartedByInfoDto]
-        if isinstance(_started_by_info, Unset):
+        if isinstance(_started_by_info, Unset) or _started_by_info is None:
             started_by_info = UNSET
         else:
             started_by_info = CdrStartedByInfoDto.from_dict(_started_by_info)
 
         total_energy_in_kwh = d.pop("totalEnergyInKwh", UNSET)
 
         total_time_in_hours = d.pop("totalTimeInHours", UNSET)
@@ -313,22 +313,22 @@
 
             charging_periods.append(charging_periods_item)
 
         total_price = d.pop("totalPrice", UNSET)
 
         _created = d.pop("created", UNSET)
         created: Union[Unset, datetime.datetime]
-        if isinstance(_created, Unset):
+        if isinstance(_created, Unset) or _created is None:
             created = UNSET
         else:
             created = isoparse(_created)
 
         _last_updated = d.pop("lastUpdated", UNSET)
         last_updated: Union[Unset, datetime.datetime]
-        if isinstance(_last_updated, Unset):
+        if isinstance(_last_updated, Unset) or _last_updated is None:
             last_updated = UNSET
         else:
             last_updated = isoparse(_last_updated)
 
         ou = d.pop("ou", UNSET)
 
         ou_id = d.pop("ouId", UNSET)
@@ -345,43 +345,43 @@
 
         charging_time_tariff = d.pop("chargingTimeTariff", UNSET)
 
         parking_time_tariff = d.pop("parkingTimeTariff", UNSET)
 
         _price_info = d.pop("priceInfo", UNSET)
         price_info: Union[Unset, PriceInfoDto]
-        if isinstance(_price_info, Unset):
+        if isinstance(_price_info, Unset) or _price_info is None:
             price_info = UNSET
         else:
             price_info = PriceInfoDto.from_dict(_price_info)
 
         _local_start_date_time = d.pop("localStartDateTime", UNSET)
         local_start_date_time: Union[Unset, datetime.datetime]
-        if isinstance(_local_start_date_time, Unset):
+        if isinstance(_local_start_date_time, Unset) or _local_start_date_time is None:
             local_start_date_time = UNSET
         else:
             local_start_date_time = isoparse(_local_start_date_time)
 
         _local_end_date_time = d.pop("localEndDateTime", UNSET)
         local_end_date_time: Union[Unset, datetime.datetime]
-        if isinstance(_local_end_date_time, Unset):
+        if isinstance(_local_end_date_time, Unset) or _local_end_date_time is None:
             local_end_date_time = UNSET
         else:
             local_end_date_time = isoparse(_local_end_date_time)
 
         _approval_status = d.pop("approvalStatus", UNSET)
         approval_status: Union[Unset, CdrDtoApprovalStatus]
-        if isinstance(_approval_status, Unset):
+        if isinstance(_approval_status, Unset) or _approval_status is None:
             approval_status = UNSET
         else:
             approval_status = CdrDtoApprovalStatus(_approval_status)
 
         _financial_type = d.pop("financialType", UNSET)
         financial_type: Union[Unset, CdrDtoFinancialType]
-        if isinstance(_financial_type, Unset):
+        if isinstance(_financial_type, Unset) or _financial_type is None:
             financial_type = UNSET
         else:
             financial_type = CdrDtoFinancialType(_financial_type)
 
         debit_cdr_id = d.pop("debitCdrId", UNSET)
 
         cdr_dto = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/cdr_geo_location_dto.py` & `longship-2024.4.15/longship_api_client/models/cdr_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/cdr_location_dto.py` & `longship-2024.4.15/longship_api_client/models/cdr_location_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
         evse_id = d.pop("evseId", UNSET)
 
         _power_type = d.pop("powerType", UNSET)
         power_type: Union[Unset, CdrLocationDtoPowerType]
-        if isinstance(_power_type, Unset):
+        if isinstance(_power_type, Unset) or _power_type is None:
             power_type = UNSET
         else:
             power_type = CdrLocationDtoPowerType(_power_type)
 
         country_code = d.pop("country_code", UNSET)
 
         party_id = d.pop("party_id", UNSET)
@@ -169,15 +169,15 @@
 
         country = d.pop("country", UNSET)
 
         hotline_phonenumber = d.pop("hotline_phonenumber", UNSET)
 
         _coordinates = d.pop("coordinates", UNSET)
         coordinates: Union[Unset, CdrGeoLocationDto]
-        if isinstance(_coordinates, Unset):
+        if isinstance(_coordinates, Unset) or _coordinates is None:
             coordinates = UNSET
         else:
             coordinates = CdrGeoLocationDto.from_dict(_coordinates)
 
         time_zone = d.pop("time_zone", UNSET)
 
         has_reimbursement = d.pop("hasReimbursement", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/cdr_patch_dto.py` & `longship-2024.4.15/longship_api_client/models/cdr_patch_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _approval_status = d.pop("approvalStatus", UNSET)
         approval_status: Union[Unset, CdrPatchDtoApprovalStatus]
-        if isinstance(_approval_status, Unset):
+        if isinstance(_approval_status, Unset) or _approval_status is None:
             approval_status = UNSET
         else:
             approval_status = CdrPatchDtoApprovalStatus(_approval_status)
 
         cdr_patch_dto = cls(
             approval_status=approval_status,
         )
```

### Comparing `longship-2024.3.15/longship_api_client/models/cdr_started_by_info_dto.py` & `longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,31 +83,31 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.cdr_started_by_token_dto import CdrStartedByTokenDto
 
         d = src_dict.copy()
         _token_info = d.pop("tokenInfo", UNSET)
         token_info: Union[Unset, CdrStartedByTokenDto]
-        if isinstance(_token_info, Unset):
+        if isinstance(_token_info, Unset) or _token_info is None:
             token_info = UNSET
         else:
             token_info = CdrStartedByTokenDto.from_dict(_token_info)
 
         _roaming_platform_type = d.pop("roamingPlatformType", UNSET)
         roaming_platform_type: Union[Unset, CdrStartedByInfoDtoRoamingPlatformType]
-        if isinstance(_roaming_platform_type, Unset):
+        if isinstance(_roaming_platform_type, Unset) or _roaming_platform_type is None:
             roaming_platform_type = UNSET
         else:
             roaming_platform_type = CdrStartedByInfoDtoRoamingPlatformType(
                 _roaming_platform_type
             )
 
         _authorization_state = d.pop("authorizationState", UNSET)
         authorization_state: Union[Unset, CdrStartedByInfoDtoAuthorizationState]
-        if isinstance(_authorization_state, Unset):
+        if isinstance(_authorization_state, Unset) or _authorization_state is None:
             authorization_state = UNSET
         else:
             authorization_state = CdrStartedByInfoDtoAuthorizationState(
                 _authorization_state
             )
 
         roaming_platform_connection_id = d.pop("roamingPlatformConnectionId", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py` & `longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/cdr_started_by_token_dto.py` & `longship-2024.4.15/longship_api_client/models/cdr_started_by_token_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,24 +105,24 @@
         d = src_dict.copy()
         uid = d.pop("uid", UNSET)
 
         auth_reference = d.pop("authReference", UNSET)
 
         _token_type = d.pop("tokenType", UNSET)
         token_type: Union[Unset, CdrStartedByTokenDtoTokenType]
-        if isinstance(_token_type, Unset):
+        if isinstance(_token_type, Unset) or _token_type is None:
             token_type = UNSET
         else:
             token_type = CdrStartedByTokenDtoTokenType(_token_type)
 
         contract_id = d.pop("contractId", UNSET)
 
         _auth_method = d.pop("authMethod", UNSET)
         auth_method: Union[Unset, CdrStartedByTokenDtoAuthMethod]
-        if isinstance(_auth_method, Unset):
+        if isinstance(_auth_method, Unset) or _auth_method is None:
             auth_method = UNSET
         else:
             auth_method = CdrStartedByTokenDtoAuthMethod(_auth_method)
 
         provider_country_code = d.pop("providerCountryCode", UNSET)
 
         provider_party_id = d.pop("providerPartyId", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/change_availability_request.py` & `longship-2024.4.15/longship_api_client/models/change_availability_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/change_configuration_request.py` & `longship-2024.4.15/longship_api_client/models/change_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/charge_point_authorize_get_dto.py` & `longship-2024.4.15/longship_api_client/models/charge_point_authorize_get_dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,51 +107,51 @@
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
         message_id = d.pop("messageId", UNSET)
 
         _created = d.pop("created", UNSET)
         created: Union[Unset, datetime.datetime]
-        if isinstance(_created, Unset):
+        if isinstance(_created, Unset) or _created is None:
             created = UNSET
         else:
             created = isoparse(_created)
 
         _token_info = d.pop("tokenInfo", UNSET)
         token_info: Union[Unset, TokenInfoDto]
-        if isinstance(_token_info, Unset):
+        if isinstance(_token_info, Unset) or _token_info is None:
             token_info = UNSET
         else:
             token_info = TokenInfoDto.from_dict(_token_info)
 
         _authorization_request_type = d.pop("authorizationRequestType", UNSET)
         authorization_request_type: Union[
             Unset, ChargePointAuthorizeGetDtoAuthorizationRequestType
         ]
-        if isinstance(_authorization_request_type, Unset):
+        if isinstance(_authorization_request_type, Unset) or _authorization_request_type is None:
             authorization_request_type = UNSET
         else:
             authorization_request_type = (
                 ChargePointAuthorizeGetDtoAuthorizationRequestType(
                     _authorization_request_type
                 )
             )
 
         _authorization_result = d.pop("authorizationResult", UNSET)
         authorization_result: Union[Unset, AuthorizationResultDto]
-        if isinstance(_authorization_result, Unset):
+        if isinstance(_authorization_result, Unset) or _authorization_result is None:
             authorization_result = UNSET
         else:
             authorization_result = AuthorizationResultDto.from_dict(
                 _authorization_result
             )
 
         _context = d.pop("context", UNSET)
         context: Union[Unset, AuthorizationContextDetailsDto]
-        if isinstance(_context, Unset):
+        if isinstance(_context, Unset) or _context is None:
             context = UNSET
         else:
             context = AuthorizationContextDetailsDto.from_dict(_context)
 
         charge_point_authorize_get_dto = cls(
             id=id,
             message_id=message_id,
```

### Comparing `longship-2024.3.15/longship_api_client/models/charge_point_authorize_post_dto.py` & `longship-2024.4.15/longship_api_client/models/charge_point_authorize_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/chargepoint_configuration_items_dto.py` & `longship-2024.4.15/longship_api_client/models/chargepoint_configuration_items_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,29 +80,29 @@
 
         read_only = d.pop("readOnly", UNSET)
 
         value = d.pop("value", UNSET)
 
         _created = d.pop("created", UNSET)
         created: Union[Unset, datetime.datetime]
-        if isinstance(_created, Unset):
+        if isinstance(_created, Unset) or _created is None:
             created = UNSET
         else:
             created = isoparse(_created)
 
         _modified = d.pop("modified", UNSET)
         modified: Union[Unset, datetime.datetime]
-        if isinstance(_modified, Unset):
+        if isinstance(_modified, Unset) or _modified is None:
             modified = UNSET
         else:
             modified = isoparse(_modified)
 
         _deleted = d.pop("deleted", UNSET)
         deleted: Union[Unset, datetime.datetime]
-        if isinstance(_deleted, Unset):
+        if isinstance(_deleted, Unset) or _deleted is None:
             deleted = UNSET
         else:
             deleted = isoparse(_deleted)
 
         chargepoint_configuration_items_dto = cls(
             id=id,
             read_only=read_only,
```

### Comparing `longship-2024.3.15/longship_api_client/models/chargepoint_connector_dto.py` & `longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,38 +112,38 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
         _operational_status = d.pop("operationalStatus", UNSET)
         operational_status: Union[Unset, ChargepointConnectorDtoOperationalStatus]
-        if isinstance(_operational_status, Unset):
+        if isinstance(_operational_status, Unset) or _operational_status is None:
             operational_status = UNSET
         else:
             operational_status = ChargepointConnectorDtoOperationalStatus(
                 _operational_status
             )
 
         _standard = d.pop("standard", UNSET)
         standard: Union[Unset, ChargepointConnectorDtoStandard]
-        if isinstance(_standard, Unset):
+        if isinstance(_standard, Unset) or _standard is None:
             standard = UNSET
         else:
             standard = ChargepointConnectorDtoStandard(_standard)
 
         _format_ = d.pop("format", UNSET)
         format_: Union[Unset, ChargepointConnectorDtoFormat]
-        if isinstance(_format_, Unset):
+        if isinstance(_format_, Unset) or _format_ is None:
             format_ = UNSET
         else:
             format_ = ChargepointConnectorDtoFormat(_format_)
 
         _power_type = d.pop("powerType", UNSET)
         power_type: Union[Unset, ChargepointConnectorDtoPowerType]
-        if isinstance(_power_type, Unset):
+        if isinstance(_power_type, Unset) or _power_type is None:
             power_type = UNSET
         else:
             power_type = ChargepointConnectorDtoPowerType(_power_type)
 
         max_voltage = d.pop("maxVoltage", UNSET)
 
         max_amperage = d.pop("maxAmperage", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/chargepoint_connector_dto_standard.py` & `longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_standard.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/chargepoint_dto.py` & `longship-2024.4.15/longship_api_client/models/chargepoint_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
         charge_point_id = d.pop("chargePointId", UNSET)
 
         _date_deleted = d.pop("dateDeleted", UNSET)
         date_deleted: Union[Unset, datetime.datetime]
-        if isinstance(_date_deleted, Unset):
+        if isinstance(_date_deleted, Unset) or _date_deleted is None:
             date_deleted = UNSET
         else:
             date_deleted = isoparse(_date_deleted)
 
         display_name = d.pop("displayName", UNSET)
 
         roaming_name = d.pop("roamingName", UNSET)
@@ -336,15 +336,15 @@
 
         charge_point_vendor = d.pop("chargePointVendor", UNSET)
 
         firmware_version = d.pop("firmwareVersion", UNSET)
 
         _connectivity_status = d.pop("connectivityStatus", UNSET)
         connectivity_status: Union[Unset, ChargepointDtoConnectivityStatus]
-        if isinstance(_connectivity_status, Unset):
+        if isinstance(_connectivity_status, Unset) or _connectivity_status is None:
             connectivity_status = UNSET
         else:
             connectivity_status = ChargepointDtoConnectivityStatus(_connectivity_status)
 
         iccid = d.pop("iccid", UNSET)
 
         imsi = d.pop("imsi", UNSET)
@@ -368,22 +368,22 @@
 
         location_id = d.pop("locationId", UNSET)
 
         allow_any_token = d.pop("allowAnyToken", UNSET)
 
         _date_created = d.pop("dateCreated", UNSET)
         date_created: Union[Unset, datetime.datetime]
-        if isinstance(_date_created, Unset):
+        if isinstance(_date_created, Unset) or _date_created is None:
             date_created = UNSET
         else:
             date_created = isoparse(_date_created)
 
         _updated = d.pop("updated", UNSET)
         updated: Union[Unset, datetime.datetime]
-        if isinstance(_updated, Unset):
+        if isinstance(_updated, Unset) or _updated is None:
             updated = UNSET
         else:
             updated = isoparse(_updated)
 
         ou = d.pop("ou", UNSET)
 
         ou_id = d.pop("ouId", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/chargepoint_evse_dto.py` & `longship-2024.4.15/longship_api_client/models/chargepoint_evse_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/chargepoint_put_dto.py` & `longship-2024.4.15/longship_api_client/models/chargepoint_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/chargepoint_status_dto.py` & `longship-2024.4.15/longship_api_client/models/chargepoint_status_dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,22 +136,22 @@
 
         ou_id = d.pop("ouId", UNSET)
 
         ou_name = d.pop("ouName", UNSET)
 
         _timestamp = d.pop("timestamp", UNSET)
         timestamp: Union[Unset, datetime.datetime]
-        if isinstance(_timestamp, Unset):
+        if isinstance(_timestamp, Unset) or _timestamp is None:
             timestamp = UNSET
         else:
             timestamp = isoparse(_timestamp)
 
         _connectivity_status = d.pop("connectivityStatus", UNSET)
         connectivity_status: Union[Unset, ChargepointStatusDtoConnectivityStatus]
-        if isinstance(_connectivity_status, Unset):
+        if isinstance(_connectivity_status, Unset) or _connectivity_status is None:
             connectivity_status = UNSET
         else:
             connectivity_status = ChargepointStatusDtoConnectivityStatus(
                 _connectivity_status
             )
 
         connectors = []
@@ -161,22 +161,22 @@
                 connectors_item_data
             )
 
             connectors.append(connectors_item)
 
         _websocket_connected = d.pop("websocketConnected", UNSET)
         websocket_connected: Union[Unset, datetime.datetime]
-        if isinstance(_websocket_connected, Unset):
+        if isinstance(_websocket_connected, Unset) or _websocket_connected is None:
             websocket_connected = UNSET
         else:
             websocket_connected = isoparse(_websocket_connected)
 
         _websocket_disconnected = d.pop("websocketDisconnected", UNSET)
         websocket_disconnected: Union[Unset, datetime.datetime]
-        if isinstance(_websocket_disconnected, Unset):
+        if isinstance(_websocket_disconnected, Unset) or _websocket_disconnected is None:
             websocket_disconnected = UNSET
         else:
             websocket_disconnected = isoparse(_websocket_disconnected)
 
         chargepoint_status_dto = cls(
             id=id,
             display_name=display_name,
```

### Comparing `longship-2024.3.15/longship_api_client/models/charging_meter_value_dto.py` & `longship-2024.4.15/longship_api_client/models/charging_meter_value_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,31 +67,31 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _timestamp = d.pop("timestamp", UNSET)
         timestamp: Union[Unset, datetime.datetime]
-        if isinstance(_timestamp, Unset):
+        if isinstance(_timestamp, Unset) or _timestamp is None:
             timestamp = UNSET
         else:
             timestamp = isoparse(_timestamp)
 
         value = d.pop("value", UNSET)
 
         _measurand = d.pop("measurand", UNSET)
         measurand: Union[Unset, ChargingMeterValueDtoMeasurand]
-        if isinstance(_measurand, Unset):
+        if isinstance(_measurand, Unset) or _measurand is None:
             measurand = UNSET
         else:
             measurand = ChargingMeterValueDtoMeasurand(_measurand)
 
         _unit = d.pop("unit", UNSET)
         unit: Union[Unset, ChargingMeterValueDtoUnit]
-        if isinstance(_unit, Unset):
+        if isinstance(_unit, Unset) or _unit is None:
             unit = UNSET
         else:
             unit = ChargingMeterValueDtoUnit(_unit)
 
         charging_meter_value_dto = cls(
             timestamp=timestamp,
             value=value,
```

### Comparing `longship-2024.3.15/longship_api_client/models/charging_meter_value_dto_measurand.py` & `longship-2024.4.15/longship_api_client/models/charging_meter_value_dto_measurand.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/charging_period_dto.py` & `longship-2024.4.15/longship_api_client/models/charging_period_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _timestamp = d.pop("timestamp", UNSET)
         timestamp: Union[Unset, datetime.datetime]
-        if isinstance(_timestamp, Unset):
+        if isinstance(_timestamp, Unset) or _timestamp is None:
             timestamp = UNSET
         else:
             timestamp = isoparse(_timestamp)
 
         delta_kwh = d.pop("deltaKwh", UNSET)
 
         absolute_kwh = d.pop("absoluteKwh", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/charging_profile.py` & `longship-2024.4.15/longship_api_client/models/charging_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,29 +126,29 @@
 
         charging_schedule = ChargingSchedule.from_dict(d.pop("chargingSchedule"))
 
         transaction_id = d.pop("transactionId", UNSET)
 
         _recurrency_kind = d.pop("recurrencyKind", UNSET)
         recurrency_kind: Union[Unset, ChargingProfileRecurrencyKind]
-        if isinstance(_recurrency_kind, Unset):
+        if isinstance(_recurrency_kind, Unset) or _recurrency_kind is None:
             recurrency_kind = UNSET
         else:
             recurrency_kind = ChargingProfileRecurrencyKind(_recurrency_kind)
 
         _valid_from = d.pop("validFrom", UNSET)
         valid_from: Union[Unset, datetime.datetime]
-        if isinstance(_valid_from, Unset):
+        if isinstance(_valid_from, Unset) or _valid_from is None:
             valid_from = UNSET
         else:
             valid_from = isoparse(_valid_from)
 
         _valid_to = d.pop("validTo", UNSET)
         valid_to: Union[Unset, datetime.datetime]
-        if isinstance(_valid_to, Unset):
+        if isinstance(_valid_to, Unset) or _valid_to is None:
             valid_to = UNSET
         else:
             valid_to = isoparse(_valid_to)
 
         charging_profile = cls(
             charging_profile_id=charging_profile_id,
             stack_level=stack_level,
```

### Comparing `longship-2024.3.15/longship_api_client/models/charging_schedule.py` & `longship-2024.4.15/longship_api_client/models/charging_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
             charging_schedule_period.append(charging_schedule_period_item)
 
         duration = d.pop("duration", UNSET)
 
         _start_schedule = d.pop("startSchedule", UNSET)
         start_schedule: Union[Unset, datetime.datetime]
-        if isinstance(_start_schedule, Unset):
+        if isinstance(_start_schedule, Unset) or _start_schedule is None:
             start_schedule = UNSET
         else:
             start_schedule = isoparse(_start_schedule)
 
         min_charging_rate = d.pop("minChargingRate", UNSET)
 
         charging_schedule = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/charging_schedule_period.py` & `longship-2024.4.15/longship_api_client/models/charging_schedule_period.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/clear_cache_request.py` & `longship-2024.4.15/longship_api_client/models/clear_cache_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/clear_charging_profile_request.py` & `longship-2024.4.15/longship_api_client/models/clear_charging_profile_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
         connector_id = d.pop("connectorId", UNSET)
 
         _charging_profile_purpose = d.pop("chargingProfilePurpose", UNSET)
         charging_profile_purpose: Union[
             Unset, ClearChargingProfileRequestChargingProfilePurpose
         ]
-        if isinstance(_charging_profile_purpose, Unset):
+        if isinstance(_charging_profile_purpose, Unset) or _charging_profile_purpose is None:
             charging_profile_purpose = UNSET
         else:
             charging_profile_purpose = (
                 ClearChargingProfileRequestChargingProfilePurpose(
                     _charging_profile_purpose
                 )
             )
```

### Comparing `longship-2024.3.15/longship_api_client/models/connector_dto.py` & `longship-2024.4.15/longship_api_client/models/connector_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,44 +99,44 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
         _standard = d.pop("standard", UNSET)
         standard: Union[Unset, ConnectorDtoStandard]
-        if isinstance(_standard, Unset):
+        if isinstance(_standard, Unset) or _standard is None:
             standard = UNSET
         else:
             standard = ConnectorDtoStandard(_standard)
 
         _format_ = d.pop("format", UNSET)
         format_: Union[Unset, ConnectorDtoFormat]
-        if isinstance(_format_, Unset):
+        if isinstance(_format_, Unset) or _format_ is None:
             format_ = UNSET
         else:
             format_ = ConnectorDtoFormat(_format_)
 
         _power_type = d.pop("power_type", UNSET)
         power_type: Union[Unset, ConnectorDtoPowerType]
-        if isinstance(_power_type, Unset):
+        if isinstance(_power_type, Unset) or _power_type is None:
             power_type = UNSET
         else:
             power_type = ConnectorDtoPowerType(_power_type)
 
         max_voltage = d.pop("max_voltage", UNSET)
 
         max_amperage = d.pop("max_amperage", UNSET)
 
         max_electric_power = d.pop("max_electric_power", UNSET)
 
         calc_max_electric_power = d.pop("calc_max_electric_power", UNSET)
 
         _last_updated = d.pop("last_updated", UNSET)
         last_updated: Union[Unset, datetime.datetime]
-        if isinstance(_last_updated, Unset):
+        if isinstance(_last_updated, Unset) or _last_updated is None:
             last_updated = UNSET
         else:
             last_updated = isoparse(_last_updated)
 
         connector_dto = cls(
             id=id,
             standard=standard,
```

### Comparing `longship-2024.3.15/longship_api_client/models/connector_dto_standard.py` & `longship-2024.4.15/longship_api_client/models/connector_dto_standard.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/connector_operational_status_dto.py` & `longship-2024.4.15/longship_api_client/models/connector_operational_status_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,24 +62,24 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         connector_number = d.pop("connectorNumber", UNSET)
 
         _operational_status = d.pop("operationalStatus", UNSET)
         operational_status: Union[Unset, ConnectorOperationalStatusDtoOperationalStatus]
-        if isinstance(_operational_status, Unset):
+        if isinstance(_operational_status, Unset) or _operational_status is None:
             operational_status = UNSET
         else:
             operational_status = ConnectorOperationalStatusDtoOperationalStatus(
                 _operational_status
             )
 
         _timestamp = d.pop("timestamp", UNSET)
         timestamp: Union[Unset, datetime.datetime]
-        if isinstance(_timestamp, Unset):
+        if isinstance(_timestamp, Unset) or _timestamp is None:
             timestamp = UNSET
         else:
             timestamp = isoparse(_timestamp)
 
         connector_operational_status_dto = cls(
             connector_number=connector_number,
             operational_status=operational_status,
```

### Comparing `longship-2024.3.15/longship_api_client/models/cs_charging_profiles.py` & `longship-2024.4.15/longship_api_client/models/cs_charging_profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,29 +129,29 @@
 
         charging_schedule = ChargingSchedule.from_dict(d.pop("chargingSchedule"))
 
         transaction_id = d.pop("transactionId", UNSET)
 
         _recurrency_kind = d.pop("recurrencyKind", UNSET)
         recurrency_kind: Union[Unset, CsChargingProfilesRecurrencyKind]
-        if isinstance(_recurrency_kind, Unset):
+        if isinstance(_recurrency_kind, Unset) or _recurrency_kind is None:
             recurrency_kind = UNSET
         else:
             recurrency_kind = CsChargingProfilesRecurrencyKind(_recurrency_kind)
 
         _valid_from = d.pop("validFrom", UNSET)
         valid_from: Union[Unset, datetime.datetime]
-        if isinstance(_valid_from, Unset):
+        if isinstance(_valid_from, Unset) or _valid_from is None:
             valid_from = UNSET
         else:
             valid_from = isoparse(_valid_from)
 
         _valid_to = d.pop("validTo", UNSET)
         valid_to: Union[Unset, datetime.datetime]
-        if isinstance(_valid_to, Unset):
+        if isinstance(_valid_to, Unset) or _valid_to is None:
             valid_to = UNSET
         else:
             valid_to = isoparse(_valid_to)
 
         cs_charging_profiles = cls(
             charging_profile_id=charging_profile_id,
             stack_level=stack_level,
```

### Comparing `longship-2024.3.15/longship_api_client/models/data_transfer_request.py` & `longship-2024.4.15/longship_api_client/models/data_transfer_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/display_text_dto.py` & `longship-2024.4.15/longship_api_client/models/display_text_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/energy_mix_dto.py` & `longship-2024.4.15/longship_api_client/models/energy_mix_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/energy_source_dto.py` & `longship-2024.4.15/longship_api_client/models/energy_source_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _source = d.pop("source", UNSET)
         source: Union[Unset, EnergySourceDtoSource]
-        if isinstance(_source, Unset):
+        if isinstance(_source, Unset) or _source is None:
             source = UNSET
         else:
             source = EnergySourceDtoSource(_source)
 
         percentage = d.pop("percentage", UNSET)
 
         energy_source_dto = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/entity_tag_header_value.py` & `longship-2024.4.15/longship_api_client/models/entity_tag_header_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.string_segment import StringSegment
 
         d = src_dict.copy()
         _tag = d.pop("tag", UNSET)
         tag: Union[Unset, StringSegment]
-        if isinstance(_tag, Unset):
+        if isinstance(_tag, Unset) or _tag is None:
             tag = UNSET
         else:
             tag = StringSegment.from_dict(_tag)
 
         is_weak = d.pop("isWeak", UNSET)
 
         entity_tag_header_value = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/environmental_impact_dto.py` & `longship-2024.4.15/longship_api_client/models/environmental_impact_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _category = d.pop("category", UNSET)
         category: Union[Unset, EnvironmentalImpactDtoCategory]
-        if isinstance(_category, Unset):
+        if isinstance(_category, Unset) or _category is None:
             category = UNSET
         else:
             category = EnvironmentalImpactDtoCategory(_category)
 
         amount = d.pop("amount", UNSET)
 
         environmental_impact_dto = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/exceptional_period_dto.py` & `longship-2024.4.15/longship_api_client/models/exceptional_period_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,22 +48,22 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _period_begin = d.pop("period_begin", UNSET)
         period_begin: Union[Unset, datetime.datetime]
-        if isinstance(_period_begin, Unset):
+        if isinstance(_period_begin, Unset) or _period_begin is None:
             period_begin = UNSET
         else:
             period_begin = isoparse(_period_begin)
 
         _period_end = d.pop("period_end", UNSET)
         period_end: Union[Unset, datetime.datetime]
-        if isinstance(_period_end, Unset):
+        if isinstance(_period_end, Unset) or _period_end is None:
             period_end = UNSET
         else:
             period_end = isoparse(_period_end)
 
         exceptional_period_dto = cls(
             period_begin=period_begin,
             period_end=period_end,
```

### Comparing `longship-2024.3.15/longship_api_client/models/file_content_result.py` & `longship-2024.4.15/longship_api_client/models/file_content_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,33 +81,33 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.entity_tag_header_value import EntityTagHeaderValue
 
         d = src_dict.copy()
         _file_contents = d.pop("fileContents", UNSET)
         file_contents: Union[Unset, File]
-        if isinstance(_file_contents, Unset):
+        if isinstance(_file_contents, Unset) or _file_contents is None:
             file_contents = UNSET
         else:
             file_contents = File(payload=BytesIO(_file_contents))
 
         content_type = d.pop("contentType", UNSET)
 
         file_download_name = d.pop("fileDownloadName", UNSET)
 
         _last_modified = d.pop("lastModified", UNSET)
         last_modified: Union[Unset, datetime.datetime]
-        if isinstance(_last_modified, Unset):
+        if isinstance(_last_modified, Unset) or _last_modified is None:
             last_modified = UNSET
         else:
             last_modified = isoparse(_last_modified)
 
         _entity_tag = d.pop("entityTag", UNSET)
         entity_tag: Union[Unset, EntityTagHeaderValue]
-        if isinstance(_entity_tag, Unset):
+        if isinstance(_entity_tag, Unset) or _entity_tag is None:
             entity_tag = UNSET
         else:
             entity_tag = EntityTagHeaderValue.from_dict(_entity_tag)
 
         enable_range_processing = d.pop("enableRangeProcessing", UNSET)
 
         file_content_result = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/geo_location_dto.py` & `longship-2024.4.15/longship_api_client/models/geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/get_composite_schedule_request.py` & `longship-2024.4.15/longship_api_client/models/get_composite_schedule_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         d = src_dict.copy()
         connector_id = d.pop("connectorId")
 
         duration = d.pop("duration")
 
         _charging_rate_unit = d.pop("chargingRateUnit", UNSET)
         charging_rate_unit: Union[Unset, GetCompositeScheduleRequestChargingRateUnit]
-        if isinstance(_charging_rate_unit, Unset):
+        if isinstance(_charging_rate_unit, Unset) or _charging_rate_unit is None:
             charging_rate_unit = UNSET
         else:
             charging_rate_unit = GetCompositeScheduleRequestChargingRateUnit(
                 _charging_rate_unit
             )
 
         get_composite_schedule_request = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/get_configuration_request.py` & `longship-2024.4.15/longship_api_client/models/get_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/get_diagnostics_request.py` & `longship-2024.4.15/longship_api_client/models/get_diagnostics_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,22 +74,22 @@
 
         retries = d.pop("retries", UNSET)
 
         retry_interval = d.pop("retryInterval", UNSET)
 
         _start_time = d.pop("startTime", UNSET)
         start_time: Union[Unset, datetime.datetime]
-        if isinstance(_start_time, Unset):
+        if isinstance(_start_time, Unset) or _start_time is None:
             start_time = UNSET
         else:
             start_time = isoparse(_start_time)
 
         _stop_time = d.pop("stopTime", UNSET)
         stop_time: Union[Unset, datetime.datetime]
-        if isinstance(_stop_time, Unset):
+        if isinstance(_stop_time, Unset) or _stop_time is None:
             stop_time = UNSET
         else:
             stop_time = isoparse(_stop_time)
 
         get_diagnostics_request = cls(
             location=location,
             retries=retries,
```

### Comparing `longship-2024.3.15/longship_api_client/models/get_local_list_version_request.py` & `longship-2024.4.15/longship_api_client/models/get_local_list_version_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/hours_dto.py` & `longship-2024.4.15/longship_api_client/models/hours_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/id_tag_info.py` & `longship-2024.4.15/longship_api_client/models/id_tag_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         status = IdTagInfoStatus(d.pop("status"))
 
         _expiry_date = d.pop("expiryDate", UNSET)
         expiry_date: Union[Unset, datetime.datetime]
-        if isinstance(_expiry_date, Unset):
+        if isinstance(_expiry_date, Unset) or _expiry_date is None:
             expiry_date = UNSET
         else:
             expiry_date = isoparse(_expiry_date)
 
         parent_id_tag = d.pop("parentIdTag", UNSET)
 
         id_tag_info = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/image_dto.py` & `longship-2024.4.15/longship_api_client/models/image_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,22 +66,24 @@
         if height is not UNSET:
             field_dict["height"] = height
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        if src_dict is None:
+            return UNSET
         d = src_dict.copy()
         url = d.pop("url", UNSET)
 
         thumbnail = d.pop("thumbnail", UNSET)
 
         _category = d.pop("category", UNSET)
         category: Union[Unset, ImageDtoCategory]
-        if isinstance(_category, Unset):
+        if isinstance(_category, Unset) or _category is None:
             category = UNSET
         else:
             category = ImageDtoCategory(_category)
 
         type = d.pop("type", UNSET)
 
         width = d.pop("width", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/interchange_format_cdr.py` & `longship-2024.4.15/longship_api_client/models/interchange_format_cdr.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,22 +158,22 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         cdr_id = d.pop("cdrId", UNSET)
 
         _start_date_time = d.pop("startDateTime", UNSET)
         start_date_time: Union[Unset, datetime.datetime]
-        if isinstance(_start_date_time, Unset):
+        if isinstance(_start_date_time, Unset) or _start_date_time is None:
             start_date_time = UNSET
         else:
             start_date_time = isoparse(_start_date_time)
 
         _end_date_time = d.pop("endDateTime", UNSET)
         end_date_time: Union[Unset, datetime.datetime]
-        if isinstance(_end_date_time, Unset):
+        if isinstance(_end_date_time, Unset) or _end_date_time is None:
             end_date_time = UNSET
         else:
             end_date_time = isoparse(_end_date_time)
 
         duration = d.pop("duration", UNSET)
 
         volume = d.pop("volume", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/local_token_group_get_dto.py` & `longship-2024.4.15/longship_api_client/models/local_token_group_get_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,22 +124,22 @@
 
         target_chargepoint_ids = cast(List[str], d.pop("targetChargepointIds", UNSET))
 
         override_tariff_id = d.pop("overrideTariffId", UNSET)
 
         _created = d.pop("created", UNSET)
         created: Union[Unset, datetime.datetime]
-        if isinstance(_created, Unset):
+        if isinstance(_created, Unset) or _created is None:
             created = UNSET
         else:
             created = isoparse(_created)
 
         _updated = d.pop("updated", UNSET)
         updated: Union[Unset, datetime.datetime]
-        if isinstance(_updated, Unset):
+        if isinstance(_updated, Unset) or _updated is None:
             updated = UNSET
         else:
             updated = isoparse(_updated)
 
         local_token_group_get_dto = cls(
             id=id,
             oucode=oucode,
```

### Comparing `longship-2024.3.15/longship_api_client/models/local_token_group_post_dto.py` & `longship-2024.4.15/longship_api_client/models/local_token_group_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/local_token_group_put_dto.py` & `longship-2024.4.15/longship_api_client/models/local_token_group_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/local_token_group_token_get_dto.py` & `longship-2024.4.15/longship_api_client/models/local_token_group_token_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/local_token_group_token_post_dto.py` & `longship-2024.4.15/longship_api_client/models/local_token_group_token_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/local_token_group_token_put_dto.py` & `longship-2024.4.15/longship_api_client/models/local_token_group_token_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/location_charge_point_dto.py` & `longship-2024.4.15/longship_api_client/models/location_charge_point_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/location_dto.py` & `longship-2024.4.15/longship_api_client/models/location_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,15 @@
                 related_locations_item_data
             )
 
             related_locations.append(related_locations_item)
 
         _parking_type = d.pop("parking_type", UNSET)
         parking_type: Union[Unset, LocationDtoParkingType]
-        if isinstance(_parking_type, Unset):
+        if isinstance(_parking_type, Unset) or _parking_type is None:
             parking_type = UNSET
         else:
             parking_type = LocationDtoParkingType(_parking_type)
 
         evses = []
         _evses = d.pop("evses", UNSET)
         for evses_item_data in _evses or []:
@@ -395,43 +395,43 @@
         for directions_item_data in _directions or []:
             directions_item = DisplayTextDto.from_dict(directions_item_data)
 
             directions.append(directions_item)
 
         _operator = d.pop("operator", UNSET)
         operator: Union[Unset, BusinessDetailsDto]
-        if isinstance(_operator, Unset):
+        if isinstance(_operator, Unset) or _operator is None:
             operator = UNSET
         else:
             operator = BusinessDetailsDto.from_dict(_operator)
 
         _suboperator = d.pop("suboperator", UNSET)
         suboperator: Union[Unset, BusinessDetailsDto]
-        if isinstance(_suboperator, Unset):
+        if isinstance(_suboperator, Unset) or _suboperator is None:
             suboperator = UNSET
         else:
             suboperator = BusinessDetailsDto.from_dict(_suboperator)
 
         _owner = d.pop("owner", UNSET)
         owner: Union[Unset, BusinessDetailsDto]
-        if isinstance(_owner, Unset):
+        if isinstance(_owner, Unset) or _owner is None:
             owner = UNSET
         else:
             owner = BusinessDetailsDto.from_dict(_owner)
 
         facilities = []
         _facilities = d.pop("facilities", UNSET)
         for facilities_item_data in _facilities or []:
             facilities_item = LocationDtoFacilitiesItem(facilities_item_data)
 
             facilities.append(facilities_item)
 
         _opening_times = d.pop("opening_times", UNSET)
         opening_times: Union[Unset, HoursDto]
-        if isinstance(_opening_times, Unset):
+        if isinstance(_opening_times, Unset) or _opening_times is None:
             opening_times = UNSET
         else:
             opening_times = HoursDto.from_dict(_opening_times)
 
         charging_when_closed = d.pop("charging_when_closed", UNSET)
 
         images = []
@@ -439,31 +439,31 @@
         for images_item_data in _images or []:
             images_item = ImageDto.from_dict(images_item_data)
 
             images.append(images_item)
 
         _energy_mix = d.pop("energy_mix", UNSET)
         energy_mix: Union[Unset, EnergyMixDto]
-        if isinstance(_energy_mix, Unset):
+        if isinstance(_energy_mix, Unset) or _energy_mix is None:
             energy_mix = UNSET
         else:
             energy_mix = EnergyMixDto.from_dict(_energy_mix)
 
         _deleted_on = d.pop("deletedOn", UNSET)
         deleted_on: Union[Unset, datetime.datetime]
-        if isinstance(_deleted_on, Unset):
+        if isinstance(_deleted_on, Unset) or _deleted_on is None:
             deleted_on = UNSET
         else:
             deleted_on = isoparse(_deleted_on)
 
         has_reimbursement = d.pop("hasReimbursement", UNSET)
 
         _reimburse_info = d.pop("reimburseInfo", UNSET)
         reimburse_info: Union[Unset, ReimburseInfoDto]
-        if isinstance(_reimburse_info, Unset):
+        if isinstance(_reimburse_info, Unset) or _reimburse_info is None:
             reimburse_info = UNSET
         else:
             reimburse_info = ReimburseInfoDto.from_dict(_reimburse_info)
 
         operator_id = d.pop("operatorId", UNSET)
 
         ou = d.pop("ou", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/location_dto_facilities_item.py` & `longship-2024.4.15/longship_api_client/models/location_dto_facilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/location_evse_dto.py` & `longship-2024.4.15/longship_api_client/models/location_evse_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
         uid = d.pop("uid", UNSET)
 
         evse_id = d.pop("evse_id", UNSET)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, LocationEVSEDtoStatus]
-        if isinstance(_status, Unset):
+        if isinstance(_status, Unset) or _status is None:
             status = UNSET
         else:
             status = LocationEVSEDtoStatus(_status)
 
         status_schedule = []
         _status_schedule = d.pop("status_schedule", UNSET)
         for status_schedule_item_data in _status_schedule or []:
@@ -234,15 +234,15 @@
 
             connectors.append(connectors_item)
 
         floor_level = d.pop("floor_level", UNSET)
 
         _coordinates = d.pop("coordinates", UNSET)
         coordinates: Union[Unset, GeoLocationDto]
-        if isinstance(_coordinates, Unset):
+        if isinstance(_coordinates, Unset) or _coordinates is None:
             coordinates = UNSET
         else:
             coordinates = GeoLocationDto.from_dict(_coordinates)
 
         physical_reference = d.pop("physical_reference", UNSET)
 
         directions = []
@@ -266,15 +266,15 @@
         for images_item_data in _images or []:
             images_item = ImageDto.from_dict(images_item_data)
 
             images.append(images_item)
 
         _last_updated = d.pop("last_updated", UNSET)
         last_updated: Union[Unset, datetime.datetime]
-        if isinstance(_last_updated, Unset):
+        if isinstance(_last_updated, Unset) or _last_updated is None:
             last_updated = UNSET
         else:
             last_updated = isoparse(_last_updated)
 
         location_evse_dto = cls(
             id=id,
             chargepointid=chargepointid,
```

### Comparing `longship-2024.3.15/longship_api_client/models/location_evse_dto_capabilities_item.py` & `longship-2024.4.15/longship_api_client/models/location_evse_dto_capabilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/location_post_dto.py` & `longship-2024.4.15/longship_api_client/models/location_post_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -342,15 +342,15 @@
                 related_locations_item_data
             )
 
             related_locations.append(related_locations_item)
 
         _parking_type = d.pop("parkingType", UNSET)
         parking_type: Union[Unset, LocationPostDtoParkingType]
-        if isinstance(_parking_type, Unset):
+        if isinstance(_parking_type, Unset) or _parking_type is None:
             parking_type = UNSET
         else:
             parking_type = LocationPostDtoParkingType(_parking_type)
 
         evses = []
         _evses = d.pop("evses", UNSET)
         for evses_item_data in _evses or []:
@@ -363,43 +363,43 @@
         for directions_item_data in _directions or []:
             directions_item = DisplayTextDto.from_dict(directions_item_data)
 
             directions.append(directions_item)
 
         _operator = d.pop("operator", UNSET)
         operator: Union[Unset, BusinessDetailsDto]
-        if isinstance(_operator, Unset):
+        if isinstance(_operator, Unset) or _operator is None:
             operator = UNSET
         else:
             operator = BusinessDetailsDto.from_dict(_operator)
 
         _suboperator = d.pop("suboperator", UNSET)
         suboperator: Union[Unset, BusinessDetailsDto]
-        if isinstance(_suboperator, Unset):
+        if isinstance(_suboperator, Unset) or _suboperator is None:
             suboperator = UNSET
         else:
             suboperator = BusinessDetailsDto.from_dict(_suboperator)
 
         _owner = d.pop("owner", UNSET)
         owner: Union[Unset, BusinessDetailsDto]
-        if isinstance(_owner, Unset):
+        if isinstance(_owner, Unset) or _owner is None:
             owner = UNSET
         else:
             owner = BusinessDetailsDto.from_dict(_owner)
 
         facilities = []
         _facilities = d.pop("facilities", UNSET)
         for facilities_item_data in _facilities or []:
             facilities_item = LocationPostDtoFacilitiesItem(facilities_item_data)
 
             facilities.append(facilities_item)
 
         _opening_times = d.pop("openingTimes", UNSET)
         opening_times: Union[Unset, HoursDto]
-        if isinstance(_opening_times, Unset):
+        if isinstance(_opening_times, Unset) or _opening_times is None:
             opening_times = UNSET
         else:
             opening_times = HoursDto.from_dict(_opening_times)
 
         charging_when_closed = d.pop("chargingWhenClosed", UNSET)
 
         images = []
@@ -407,24 +407,24 @@
         for images_item_data in _images or []:
             images_item = ImageDto.from_dict(images_item_data)
 
             images.append(images_item)
 
         _energy_mix = d.pop("energyMix", UNSET)
         energy_mix: Union[Unset, EnergyMixDto]
-        if isinstance(_energy_mix, Unset):
+        if isinstance(_energy_mix, Unset) or _energy_mix is None:
             energy_mix = UNSET
         else:
             energy_mix = EnergyMixDto.from_dict(_energy_mix)
 
         has_reimbursement = d.pop("hasReimbursement", UNSET)
 
         _reimburse_info = d.pop("reimburseInfo", UNSET)
         reimburse_info: Union[Unset, ReimburseInfoDto]
-        if isinstance(_reimburse_info, Unset):
+        if isinstance(_reimburse_info, Unset) or _reimburse_info is None:
             reimburse_info = UNSET
         else:
             reimburse_info = ReimburseInfoDto.from_dict(_reimburse_info)
 
         operator_id = d.pop("operatorId", UNSET)
 
         ou = d.pop("ou", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/location_post_dto_facilities_item.py` & `longship-2024.4.15/longship_api_client/models/location_post_dto_facilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/location_put_dto.py` & `longship-2024.4.15/longship_api_client/models/location_put_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,15 +368,15 @@
                 related_locations_item_data
             )
 
             related_locations.append(related_locations_item)
 
         _parking_type = d.pop("parking_type", UNSET)
         parking_type: Union[Unset, LocationPutDtoParkingType]
-        if isinstance(_parking_type, Unset):
+        if isinstance(_parking_type, Unset) or _parking_type is None:
             parking_type = UNSET
         else:
             parking_type = LocationPutDtoParkingType(_parking_type)
 
         evses = []
         _evses = d.pop("evses", UNSET)
         for evses_item_data in _evses or []:
@@ -389,43 +389,43 @@
         for directions_item_data in _directions or []:
             directions_item = DisplayTextDto.from_dict(directions_item_data)
 
             directions.append(directions_item)
 
         _operator = d.pop("operator", UNSET)
         operator: Union[Unset, BusinessDetailsDto]
-        if isinstance(_operator, Unset):
+        if isinstance(_operator, Unset) or _operator is None:
             operator = UNSET
         else:
             operator = BusinessDetailsDto.from_dict(_operator)
 
         _suboperator = d.pop("suboperator", UNSET)
         suboperator: Union[Unset, BusinessDetailsDto]
-        if isinstance(_suboperator, Unset):
+        if isinstance(_suboperator, Unset) or _suboperator is None:
             suboperator = UNSET
         else:
             suboperator = BusinessDetailsDto.from_dict(_suboperator)
 
         _owner = d.pop("owner", UNSET)
         owner: Union[Unset, BusinessDetailsDto]
-        if isinstance(_owner, Unset):
+        if isinstance(_owner, Unset) or _owner is None:
             owner = UNSET
         else:
             owner = BusinessDetailsDto.from_dict(_owner)
 
         facilities = []
         _facilities = d.pop("facilities", UNSET)
         for facilities_item_data in _facilities or []:
             facilities_item = LocationPutDtoFacilitiesItem(facilities_item_data)
 
             facilities.append(facilities_item)
 
         _opening_times = d.pop("opening_times", UNSET)
         opening_times: Union[Unset, HoursDto]
-        if isinstance(_opening_times, Unset):
+        if isinstance(_opening_times, Unset) or _opening_times is None:
             opening_times = UNSET
         else:
             opening_times = HoursDto.from_dict(_opening_times)
 
         charging_when_closed = d.pop("charging_when_closed", UNSET)
 
         images = []
@@ -433,31 +433,31 @@
         for images_item_data in _images or []:
             images_item = ImageDto.from_dict(images_item_data)
 
             images.append(images_item)
 
         _energy_mix = d.pop("energy_mix", UNSET)
         energy_mix: Union[Unset, EnergyMixDto]
-        if isinstance(_energy_mix, Unset):
+        if isinstance(_energy_mix, Unset) or _energy_mix is None:
             energy_mix = UNSET
         else:
             energy_mix = EnergyMixDto.from_dict(_energy_mix)
 
         _deleted_on = d.pop("deletedOn", UNSET)
         deleted_on: Union[Unset, datetime.datetime]
-        if isinstance(_deleted_on, Unset):
+        if isinstance(_deleted_on, Unset) or _deleted_on is None:
             deleted_on = UNSET
         else:
             deleted_on = isoparse(_deleted_on)
 
         has_reimbursement = d.pop("hasReimbursement", UNSET)
 
         _reimburse_info = d.pop("reimburseInfo", UNSET)
         reimburse_info: Union[Unset, ReimburseInfoDto]
-        if isinstance(_reimburse_info, Unset):
+        if isinstance(_reimburse_info, Unset) or _reimburse_info is None:
             reimburse_info = UNSET
         else:
             reimburse_info = ReimburseInfoDto.from_dict(_reimburse_info)
 
         ou = d.pop("ou", UNSET)
 
         ou_id = d.pop("ouId", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/location_put_dto_facilities_item.py` & `longship-2024.4.15/longship_api_client/models/location_put_dto_facilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/location_tariff_distribution_dto.py` & `longship-2024.4.15/longship_api_client/models/location_tariff_distribution_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/longship_error.py` & `longship-2024.4.15/longship_api_client/models/longship_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         from ..models.longship_error_detail import LongshipErrorDetail
 
         d = src_dict.copy()
         code = d.pop("code", UNSET)
 
         _error_details = d.pop("errorDetails", UNSET)
         error_details: Union[Unset, LongshipErrorDetail]
-        if isinstance(_error_details, Unset):
+        if isinstance(_error_details, Unset) or _error_details is None:
             error_details = UNSET
         else:
             error_details = LongshipErrorDetail.from_dict(_error_details)
 
         longship_error = cls(
             code=code,
             error_details=error_details,
```

### Comparing `longship-2024.3.15/longship_api_client/models/longship_error_detail.py` & `longship-2024.4.15/longship_api_client/models/longship_error_detail.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/message_log_dto.py` & `longship-2024.4.15/longship_api_client/models/message_log_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,40 +108,40 @@
 
         charge_point_id = d.pop("chargePointId", UNSET)
 
         message_id = d.pop("messageId", UNSET)
 
         _wamp_message_type = d.pop("wampMessageType", UNSET)
         wamp_message_type: Union[Unset, MessageLogDtoWampMessageType]
-        if isinstance(_wamp_message_type, Unset):
+        if isinstance(_wamp_message_type, Unset) or _wamp_message_type is None:
             wamp_message_type = UNSET
         else:
             wamp_message_type = MessageLogDtoWampMessageType(_wamp_message_type)
 
         _ocpp_message_type = d.pop("ocppMessageType", UNSET)
         ocpp_message_type: Union[Unset, MessageLogDtoOcppMessageType]
-        if isinstance(_ocpp_message_type, Unset):
+        if isinstance(_ocpp_message_type, Unset) or _ocpp_message_type is None:
             ocpp_message_type = UNSET
         else:
             ocpp_message_type = MessageLogDtoOcppMessageType(_ocpp_message_type)
 
         _direction = d.pop("direction", UNSET)
         direction: Union[Unset, MessageLogDtoDirection]
-        if isinstance(_direction, Unset):
+        if isinstance(_direction, Unset) or _direction is None:
             direction = UNSET
         else:
             direction = MessageLogDtoDirection(_direction)
 
         tenant_id = d.pop("tenantId", UNSET)
 
         payload = d.pop("payload", UNSET)
 
         _timestamp = d.pop("timestamp", UNSET)
         timestamp: Union[Unset, datetime.datetime]
-        if isinstance(_timestamp, Unset):
+        if isinstance(_timestamp, Unset) or _timestamp is None:
             timestamp = UNSET
         else:
             timestamp = isoparse(_timestamp)
 
         message_log_dto = cls(
             id=id,
             charge_point_id=charge_point_id,
```

### Comparing `longship-2024.3.15/longship_api_client/models/message_log_dto_ocpp_message_type.py` & `longship-2024.4.15/longship_api_client/models/message_log_dto_ocpp_message_type.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/organization_unit_financial_details_dto.py` & `longship-2024.4.15/longship_api_client/models/organization_unit_financial_details_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/organization_unit_get_dto.py` & `longship-2024.4.15/longship_api_client/models/organization_unit_get_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
         msp_ou_code = d.pop("mspOuCode", UNSET)
 
         msp_external_id = d.pop("mspExternalId", UNSET)
 
         _financial_details = d.pop("financialDetails", UNSET)
         financial_details: Union[Unset, OrganizationUnitFinancialDetailsDto]
-        if isinstance(_financial_details, Unset):
+        if isinstance(_financial_details, Unset) or _financial_details is None:
             financial_details = UNSET
         else:
             financial_details = OrganizationUnitFinancialDetailsDto.from_dict(
                 _financial_details
             )
 
         organization_unit_get_dto = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/organization_unit_post_dto.py` & `longship-2024.4.15/longship_api_client/models/organization_unit_post_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
         msp_ou_code = d.pop("mspOuCode", UNSET)
 
         msp_external_id = d.pop("mspExternalId", UNSET)
 
         _financial_details = d.pop("financialDetails", UNSET)
         financial_details: Union[Unset, OrganizationUnitFinancialDetailsDto]
-        if isinstance(_financial_details, Unset):
+        if isinstance(_financial_details, Unset) or _financial_details is None:
             financial_details = UNSET
         else:
             financial_details = OrganizationUnitFinancialDetailsDto.from_dict(
                 _financial_details
             )
 
         organization_unit_post_dto = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/organization_unit_put_dto.py` & `longship-2024.4.15/longship_api_client/models/organization_unit_put_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
         msp_ou_code = d.pop("mspOuCode", UNSET)
 
         msp_external_id = d.pop("mspExternalId", UNSET)
 
         _financial_details = d.pop("financialDetails", UNSET)
         financial_details: Union[Unset, OrganizationUnitFinancialDetailsDto]
-        if isinstance(_financial_details, Unset):
+        if isinstance(_financial_details, Unset) or _financial_details is None:
             financial_details = UNSET
         else:
             financial_details = OrganizationUnitFinancialDetailsDto.from_dict(
                 _financial_details
             )
 
         organization_unit_put_dto = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/price_info_dto.py` & `longship-2024.4.15/longship_api_client/models/price_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/private_emp_tariff_dto.py` & `longship-2024.4.15/longship_api_client/models/private_emp_tariff_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         d = src_dict.copy()
         country_code = d.pop("country_code", UNSET)
 
         party_id = d.pop("party_id", UNSET)
 
         _power_type = d.pop("powerType", UNSET)
         power_type: Union[Unset, PrivateEmpTariffDtoPowerType]
-        if isinstance(_power_type, Unset):
+        if isinstance(_power_type, Unset) or _power_type is None:
             power_type = UNSET
         else:
             power_type = PrivateEmpTariffDtoPowerType(_power_type)
 
         use_public_tariff_when_kwh_is_cheaper = d.pop(
             "usePublicTariffWhenKwhIsCheaper", UNSET
         )
```

### Comparing `longship-2024.3.15/longship_api_client/models/publish_token_type_dto.py` & `longship-2024.4.15/longship_api_client/models/publish_token_type_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uid = d.pop("uid", UNSET)
 
         _type = d.pop("type", UNSET)
         type: Union[Unset, PublishTokenTypeDtoType]
-        if isinstance(_type, Unset):
+        if isinstance(_type, Unset) or _type is None:
             type = UNSET
         else:
             type = PublishTokenTypeDtoType(_type)
 
         visual_number = d.pop("visual_number", UNSET)
 
         issuer = d.pop("issuer", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/regular_hours_dto.py` & `longship-2024.4.15/longship_api_client/models/regular_hours_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/reimburse_info_dto.py` & `longship-2024.4.15/longship_api_client/models/reimburse_info_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         )
         from ..models.reimbursement_tariff_dto import ReimbursementTariffDto
         from ..models.reimbursement_bank_details_dto import ReimbursementBankDetailsDto
 
         d = src_dict.copy()
         _type = d.pop("type", UNSET)
         type: Union[Unset, ReimburseInfoDtoType]
-        if isinstance(_type, Unset):
+        if isinstance(_type, Unset) or _type is None:
             type = UNSET
         else:
             type = ReimburseInfoDtoType(_type)
 
         has_guest_usage = d.pop("hasGuestUsage", UNSET)
 
         has_guest_charging_reimbursement_fee = d.pop(
```

### Comparing `longship-2024.3.15/longship_api_client/models/reimburse_started_by_info_dto.py` & `longship-2024.4.15/longship_api_client/models/reimburse_started_by_info_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,22 +71,22 @@
         from ..models.reimburse_started_by_token_dto import ReimburseStartedByTokenDto
 
         d = src_dict.copy()
         id_tag = d.pop("idTag", UNSET)
 
         _token_info = d.pop("tokenInfo", UNSET)
         token_info: Union[Unset, ReimburseStartedByTokenDto]
-        if isinstance(_token_info, Unset):
+        if isinstance(_token_info, Unset) or _token_info is None:
             token_info = UNSET
         else:
             token_info = ReimburseStartedByTokenDto.from_dict(_token_info)
 
         _authorization_state = d.pop("authorizationState", UNSET)
         authorization_state: Union[Unset, ReimburseStartedByInfoDtoAuthorizationState]
-        if isinstance(_authorization_state, Unset):
+        if isinstance(_authorization_state, Unset) or _authorization_state is None:
             authorization_state = UNSET
         else:
             authorization_state = ReimburseStartedByInfoDtoAuthorizationState(
                 _authorization_state
             )
 
         is_guest_usage = d.pop("isGuestUsage", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py` & `longship-2024.4.15/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/reimburse_started_by_token_dto.py` & `longship-2024.4.15/longship_api_client/models/reimburse_started_by_token_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,24 +110,24 @@
         d = src_dict.copy()
         uid = d.pop("uid", UNSET)
 
         auth_reference = d.pop("authReference", UNSET)
 
         _token_type = d.pop("tokenType", UNSET)
         token_type: Union[Unset, ReimburseStartedByTokenDtoTokenType]
-        if isinstance(_token_type, Unset):
+        if isinstance(_token_type, Unset) or _token_type is None:
             token_type = UNSET
         else:
             token_type = ReimburseStartedByTokenDtoTokenType(_token_type)
 
         contract_id = d.pop("contractId", UNSET)
 
         _auth_method = d.pop("authMethod", UNSET)
         auth_method: Union[Unset, ReimburseStartedByTokenDtoAuthMethod]
-        if isinstance(_auth_method, Unset):
+        if isinstance(_auth_method, Unset) or _auth_method is None:
             auth_method = UNSET
         else:
             auth_method = ReimburseStartedByTokenDtoAuthMethod(_auth_method)
 
         provider_country_code = d.pop("providerCountryCode", UNSET)
 
         provider_party_id = d.pop("providerPartyId", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/reimbursement_bank_details_dto.py` & `longship-2024.4.15/longship_api_client/models/reimbursement_bank_details_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,22 +56,22 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         bankaccount = d.pop("bankaccount", UNSET)
 
         _date_created = d.pop("dateCreated", UNSET)
         date_created: Union[Unset, datetime.datetime]
-        if isinstance(_date_created, Unset):
+        if isinstance(_date_created, Unset) or _date_created is None:
             date_created = UNSET
         else:
             date_created = isoparse(_date_created)
 
         _valid_from = d.pop("validFrom", UNSET)
         valid_from: Union[Unset, datetime.datetime]
-        if isinstance(_valid_from, Unset):
+        if isinstance(_valid_from, Unset) or _valid_from is None:
             valid_from = UNSET
         else:
             valid_from = isoparse(_valid_from)
 
         reimbursement_bank_details_dto = cls(
             bankaccount=bankaccount,
             date_created=date_created,
```

### Comparing `longship-2024.3.15/longship_api_client/models/reimbursement_cdr_dto.py` & `longship-2024.4.15/longship_api_client/models/reimbursement_cdr_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,38 +327,38 @@
 
         location_id = d.pop("locationId", UNSET)
 
         evse_id = d.pop("evseId", UNSET)
 
         _location = d.pop("location", UNSET)
         location: Union[Unset, ReimbursementCdrLocationDto]
-        if isinstance(_location, Unset):
+        if isinstance(_location, Unset) or _location is None:
             location = UNSET
         else:
             location = ReimbursementCdrLocationDto.from_dict(_location)
 
         _start_datetime = d.pop("startDatetime", UNSET)
         start_datetime: Union[Unset, datetime.datetime]
-        if isinstance(_start_datetime, Unset):
+        if isinstance(_start_datetime, Unset) or _start_datetime is None:
             start_datetime = UNSET
         else:
             start_datetime = isoparse(_start_datetime)
 
         _end_date_time = d.pop("endDateTime", UNSET)
         end_date_time: Union[Unset, datetime.datetime]
-        if isinstance(_end_date_time, Unset):
+        if isinstance(_end_date_time, Unset) or _end_date_time is None:
             end_date_time = UNSET
         else:
             end_date_time = isoparse(_end_date_time)
 
         session_id = d.pop("sessionId", UNSET)
 
         _started_by_info = d.pop("startedByInfo", UNSET)
         started_by_info: Union[Unset, ReimburseStartedByInfoDto]
-        if isinstance(_started_by_info, Unset):
+        if isinstance(_started_by_info, Unset) or _started_by_info is None:
             started_by_info = UNSET
         else:
             started_by_info = ReimburseStartedByInfoDto.from_dict(_started_by_info)
 
         meter_start_in_wh = d.pop("meterStartInWh", UNSET)
 
         meter_stop_in_wh = d.pop("meterStopInWh", UNSET)
@@ -367,22 +367,22 @@
 
         total_time_in_hours = d.pop("totalTimeInHours", UNSET)
 
         total_price = d.pop("totalPrice", UNSET)
 
         _created = d.pop("created", UNSET)
         created: Union[Unset, datetime.datetime]
-        if isinstance(_created, Unset):
+        if isinstance(_created, Unset) or _created is None:
             created = UNSET
         else:
             created = isoparse(_created)
 
         _last_updated = d.pop("lastUpdated", UNSET)
         last_updated: Union[Unset, datetime.datetime]
-        if isinstance(_last_updated, Unset):
+        if isinstance(_last_updated, Unset) or _last_updated is None:
             last_updated = UNSET
         else:
             last_updated = isoparse(_last_updated)
 
         ou = d.pop("ou", UNSET)
 
         ou_id = d.pop("ouId", UNSET)
@@ -395,31 +395,31 @@
 
         reimburse_tariff_price = d.pop("reimburseTariffPrice", UNSET)
 
         reimburse_tariff_calculated = d.pop("reimburseTariffCalculated", UNSET)
 
         _reimburse_price_calculated_on = d.pop("reimbursePriceCalculatedOn", UNSET)
         reimburse_price_calculated_on: Union[Unset, datetime.datetime]
-        if isinstance(_reimburse_price_calculated_on, Unset):
+        if isinstance(_reimburse_price_calculated_on, Unset) or _reimburse_price_calculated_on is None:
             reimburse_price_calculated_on = UNSET
         else:
             reimburse_price_calculated_on = isoparse(_reimburse_price_calculated_on)
 
         bank_account = d.pop("bankAccount", UNSET)
 
         _bank_account_created_on = d.pop("bankAccountCreatedOn", UNSET)
         bank_account_created_on: Union[Unset, datetime.datetime]
-        if isinstance(_bank_account_created_on, Unset):
+        if isinstance(_bank_account_created_on, Unset) or _bank_account_created_on is None:
             bank_account_created_on = UNSET
         else:
             bank_account_created_on = isoparse(_bank_account_created_on)
 
         _bank_account_valid_from = d.pop("bankAccountValidFrom", UNSET)
         bank_account_valid_from: Union[Unset, datetime.datetime]
-        if isinstance(_bank_account_valid_from, Unset):
+        if isinstance(_bank_account_valid_from, Unset) or _bank_account_valid_from is None:
             bank_account_valid_from = UNSET
         else:
             bank_account_valid_from = isoparse(_bank_account_valid_from)
 
         reimburse_tariff_original_price = d.pop("reimburseTariffOriginalPrice", UNSET)
 
         has_guest_charging_reimbursement_fee = d.pop(
@@ -430,42 +430,42 @@
 
         tenant_fee_calculated = d.pop("tenantFeeCalculated", UNSET)
 
         tariff_distribution_id = d.pop("tariffDistributionId", UNSET)
 
         _price_info = d.pop("priceInfo", UNSET)
         price_info: Union[Unset, PriceInfoDto]
-        if isinstance(_price_info, Unset):
+        if isinstance(_price_info, Unset) or _price_info is None:
             price_info = UNSET
         else:
             price_info = PriceInfoDto.from_dict(_price_info)
 
         customer_share = d.pop("customerShare", UNSET)
 
         energy_compensation = d.pop("energyCompensation", UNSET)
 
         _reimbursement_customer_share = d.pop("reimbursementCustomerShare", UNSET)
         reimbursement_customer_share: Union[Unset, ReimbursementCustomerShareDto]
-        if isinstance(_reimbursement_customer_share, Unset):
+        if isinstance(_reimbursement_customer_share, Unset) or _reimbursement_customer_share is None:
             reimbursement_customer_share = UNSET
         else:
             reimbursement_customer_share = ReimbursementCustomerShareDto.from_dict(
                 _reimbursement_customer_share
             )
 
         _local_start_date_time = d.pop("localStartDateTime", UNSET)
         local_start_date_time: Union[Unset, datetime.datetime]
-        if isinstance(_local_start_date_time, Unset):
+        if isinstance(_local_start_date_time, Unset) or _local_start_date_time is None:
             local_start_date_time = UNSET
         else:
             local_start_date_time = isoparse(_local_start_date_time)
 
         _local_end_date_time = d.pop("localEndDateTime", UNSET)
         local_end_date_time: Union[Unset, datetime.datetime]
-        if isinstance(_local_end_date_time, Unset):
+        if isinstance(_local_end_date_time, Unset) or _local_end_date_time is None:
             local_end_date_time = UNSET
         else:
             local_end_date_time = isoparse(_local_end_date_time)
 
         reimbursement_cdr_dto = cls(
             id=id,
             tenant_id=tenant_id,
```

### Comparing `longship-2024.3.15/longship_api_client/models/reimbursement_cdr_geo_location_dto.py` & `longship-2024.4.15/longship_api_client/models/reimbursement_cdr_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/reimbursement_cdr_location_dto.py` & `longship-2024.4.15/longship_api_client/models/reimbursement_cdr_location_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
         evse_id = d.pop("evseId", UNSET)
 
         _power_type = d.pop("powerType", UNSET)
         power_type: Union[Unset, ReimbursementCdrLocationDtoPowerType]
-        if isinstance(_power_type, Unset):
+        if isinstance(_power_type, Unset) or _power_type is None:
             power_type = UNSET
         else:
             power_type = ReimbursementCdrLocationDtoPowerType(_power_type)
 
         country_code = d.pop("country_code", UNSET)
 
         party_id = d.pop("party_id", UNSET)
@@ -176,15 +176,15 @@
 
         country = d.pop("country", UNSET)
 
         hotline_phonenumber = d.pop("hotline_phonenumber", UNSET)
 
         _coordinates = d.pop("coordinates", UNSET)
         coordinates: Union[Unset, ReimbursementCdrGeoLocationDto]
-        if isinstance(_coordinates, Unset):
+        if isinstance(_coordinates, Unset) or _coordinates is None:
             coordinates = UNSET
         else:
             coordinates = ReimbursementCdrGeoLocationDto.from_dict(_coordinates)
 
         time_zone = d.pop("time_zone", UNSET)
 
         has_reimbursement = d.pop("hasReimbursement", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/reimbursement_customer_share_dto.py` & `longship-2024.4.15/longship_api_client/models/reimbursement_customer_share_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/reimbursement_price_dto.py` & `longship-2024.4.15/longship_api_client/models/reimbursement_price_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/reimbursement_tariff_dto.py` & `longship-2024.4.15/longship_api_client/models/reimbursement_tariff_dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,38 +86,38 @@
         from ..models.reimbursement_price_dto import ReimbursementPriceDto
 
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
         _date_created = d.pop("dateCreated", UNSET)
         date_created: Union[Unset, datetime.datetime]
-        if isinstance(_date_created, Unset):
+        if isinstance(_date_created, Unset) or _date_created is None:
             date_created = UNSET
         else:
             date_created = isoparse(_date_created)
 
         _valid_from = d.pop("validFrom", UNSET)
         valid_from: Union[Unset, datetime.datetime]
-        if isinstance(_valid_from, Unset):
+        if isinstance(_valid_from, Unset) or _valid_from is None:
             valid_from = UNSET
         else:
             valid_from = isoparse(_valid_from)
 
         currency = d.pop("currency", UNSET)
 
         _price = d.pop("price", UNSET)
         price: Union[Unset, ReimbursementPriceDto]
-        if isinstance(_price, Unset):
+        if isinstance(_price, Unset) or _price is None:
             price = UNSET
         else:
             price = ReimbursementPriceDto.from_dict(_price)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, ReimbursementTariffDtoStatus]
-        if isinstance(_status, Unset):
+        if isinstance(_status, Unset) or _status is None:
             status = UNSET
         else:
             status = ReimbursementTariffDtoStatus(_status)
 
         reimbursement_tariff_dto = cls(
             id=id,
             date_created=date_created,
```

### Comparing `longship-2024.3.15/longship_api_client/models/remote_start_transaction_request.py` & `longship-2024.4.15/longship_api_client/models/remote_start_transaction_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         d = src_dict.copy()
         id_tag = d.pop("idTag")
 
         connector_id = d.pop("connectorId", UNSET)
 
         _charging_profile = d.pop("chargingProfile", UNSET)
         charging_profile: Union[Unset, ChargingProfile]
-        if isinstance(_charging_profile, Unset):
+        if isinstance(_charging_profile, Unset) or _charging_profile is None:
             charging_profile = UNSET
         else:
             charging_profile = ChargingProfile.from_dict(_charging_profile)
 
         remote_start_transaction_request = cls(
             id_tag=id_tag,
             connector_id=connector_id,
```

### Comparing `longship-2024.3.15/longship_api_client/models/remote_stop_transaction_request.py` & `longship-2024.4.15/longship_api_client/models/remote_stop_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/reserve_now_request.py` & `longship-2024.4.15/longship_api_client/models/reserve_now_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/reset_request.py` & `longship-2024.4.15/longship_api_client/models/reset_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/send_local_list_request.py` & `longship-2024.4.15/longship_api_client/models/send_local_list_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/session_dto.py` & `longship-2024.4.15/longship_api_client/models/session_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,33 +321,33 @@
 
         ocpp_transaction_id = d.pop("ocppTransactionId", UNSET)
 
         connector_id = d.pop("connectorId", UNSET)
 
         _session_location = d.pop("sessionLocation", UNSET)
         session_location: Union[Unset, SessionLocationDto]
-        if isinstance(_session_location, Unset):
+        if isinstance(_session_location, Unset) or _session_location is None:
             session_location = UNSET
         else:
             session_location = SessionLocationDto.from_dict(_session_location)
 
         id_tag = d.pop("idTag", UNSET)
 
         _started_by_info = d.pop("startedByInfo", UNSET)
         started_by_info: Union[Unset, StartedByInfoDto]
-        if isinstance(_started_by_info, Unset):
+        if isinstance(_started_by_info, Unset) or _started_by_info is None:
             started_by_info = UNSET
         else:
             started_by_info = StartedByInfoDto.from_dict(_started_by_info)
 
         meter_start_in_wh = d.pop("meterStartInWh", UNSET)
 
         _session_start = d.pop("sessionStart", UNSET)
         session_start: Union[Unset, datetime.datetime]
-        if isinstance(_session_start, Unset):
+        if isinstance(_session_start, Unset) or _session_start is None:
             session_start = UNSET
         else:
             session_start = isoparse(_session_start)
 
         charging_periods = []
         _charging_periods = d.pop("chargingPeriods", UNSET)
         for charging_periods_item_data in _charging_periods or []:
@@ -366,74 +366,74 @@
 
             charging_meter_values.append(charging_meter_values_item)
 
         meter_stop_in_wh = d.pop("meterStopInWh", UNSET)
 
         _session_stop = d.pop("sessionStop", UNSET)
         session_stop: Union[Unset, datetime.datetime]
-        if isinstance(_session_stop, Unset):
+        if isinstance(_session_stop, Unset) or _session_stop is None:
             session_stop = UNSET
         else:
             session_stop = isoparse(_session_stop)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, SessionDtoStatus]
-        if isinstance(_status, Unset):
+        if isinstance(_status, Unset) or _status is None:
             status = UNSET
         else:
             status = SessionDtoStatus(_status)
 
         _approval_status = d.pop("approvalStatus", UNSET)
         approval_status: Union[Unset, SessionDtoApprovalStatus]
-        if isinstance(_approval_status, Unset):
+        if isinstance(_approval_status, Unset) or _approval_status is None:
             approval_status = UNSET
         else:
             approval_status = SessionDtoApprovalStatus(_approval_status)
 
         _review_scenario_type = d.pop("reviewScenarioType", UNSET)
         review_scenario_type: Union[Unset, SessionDtoReviewScenarioType]
-        if isinstance(_review_scenario_type, Unset):
+        if isinstance(_review_scenario_type, Unset) or _review_scenario_type is None:
             review_scenario_type = UNSET
         else:
             review_scenario_type = SessionDtoReviewScenarioType(_review_scenario_type)
 
         total_energy_in_kwh = d.pop("totalEnergyInKwh", UNSET)
 
         total_price = d.pop("totalPrice", UNSET)
 
         _created = d.pop("created", UNSET)
         created: Union[Unset, datetime.datetime]
-        if isinstance(_created, Unset):
+        if isinstance(_created, Unset) or _created is None:
             created = UNSET
         else:
             created = isoparse(_created)
 
         _last_updated = d.pop("lastUpdated", UNSET)
         last_updated: Union[Unset, datetime.datetime]
-        if isinstance(_last_updated, Unset):
+        if isinstance(_last_updated, Unset) or _last_updated is None:
             last_updated = UNSET
         else:
             last_updated = isoparse(_last_updated)
 
         ou = d.pop("ou", UNSET)
 
         ou_id = d.pop("ouId", UNSET)
 
         ou_name = d.pop("ouName", UNSET)
 
         _tariff_info = d.pop("tariffInfo", UNSET)
         tariff_info: Union[Unset, TariffInfoDto]
-        if isinstance(_tariff_info, Unset):
+        if isinstance(_tariff_info, Unset) or _tariff_info is None:
             tariff_info = UNSET
         else:
             tariff_info = TariffInfoDto.from_dict(_tariff_info)
 
         _price_info = d.pop("priceInfo", UNSET)
         price_info: Union[Unset, PriceInfoDto]
-        if isinstance(_price_info, Unset):
+        if isinstance(_price_info, Unset) or _price_info is None:
             price_info = UNSET
         else:
             price_info = PriceInfoDto.from_dict(_price_info)
 
         tariff_id = d.pop("tariffId", UNSET)
 
         tariff_name = d.pop("tariffName", UNSET)
@@ -442,26 +442,26 @@
 
         tariff_price = d.pop("tariffPrice", UNSET)
 
         parking_tariff = d.pop("parkingTariff", UNSET)
 
         _thresholds = d.pop("thresholds", UNSET)
         thresholds: Union[Unset, SessionThresholdsDto]
-        if isinstance(_thresholds, Unset):
+        if isinstance(_thresholds, Unset) or _thresholds is None:
             thresholds = UNSET
         else:
             thresholds = SessionThresholdsDto.from_dict(_thresholds)
 
         parking_step_size = d.pop("parkingStepSize", UNSET)
 
         delay_in_minutes = d.pop("delayInMinutes", UNSET)
 
         _parking_time_start = d.pop("parkingTimeStart", UNSET)
         parking_time_start: Union[Unset, datetime.datetime]
-        if isinstance(_parking_time_start, Unset):
+        if isinstance(_parking_time_start, Unset) or _parking_time_start is None:
             parking_time_start = UNSET
         else:
             parking_time_start = isoparse(_parking_time_start)
 
         session_dto = cls(
             id=id,
             tenant_id=tenant_id,
```

### Comparing `longship-2024.3.15/longship_api_client/models/session_geo_location_dto.py` & `longship-2024.4.15/longship_api_client/models/session_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/session_location_dto.py` & `longship-2024.4.15/longship_api_client/models/session_location_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
         evse_id = d.pop("evseId", UNSET)
 
         _power_type = d.pop("powerType", UNSET)
         power_type: Union[Unset, SessionLocationDtoPowerType]
-        if isinstance(_power_type, Unset):
+        if isinstance(_power_type, Unset) or _power_type is None:
             power_type = UNSET
         else:
             power_type = SessionLocationDtoPowerType(_power_type)
 
         country_code = d.pop("country_code", UNSET)
 
         party_id = d.pop("party_id", UNSET)
@@ -169,15 +169,15 @@
 
         country = d.pop("country", UNSET)
 
         hotline_phonenumber = d.pop("hotline_phonenumber", UNSET)
 
         _coordinates = d.pop("coordinates", UNSET)
         coordinates: Union[Unset, SessionGeoLocationDto]
-        if isinstance(_coordinates, Unset):
+        if isinstance(_coordinates, Unset) or _coordinates is None:
             coordinates = UNSET
         else:
             coordinates = SessionGeoLocationDto.from_dict(_coordinates)
 
         time_zone = d.pop("time_zone", UNSET)
 
         has_reimbursement = d.pop("hasReimbursement", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/session_threshold_check_dto.py` & `longship-2024.4.15/longship_api_client/models/session_threshold_check_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,24 +67,24 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _threshold_hit_outcome = d.pop("thresholdHitOutcome", UNSET)
         threshold_hit_outcome: Union[Unset, SessionThresholdCheckDtoThresholdHitOutcome]
-        if isinstance(_threshold_hit_outcome, Unset):
+        if isinstance(_threshold_hit_outcome, Unset) or _threshold_hit_outcome is None:
             threshold_hit_outcome = UNSET
         else:
             threshold_hit_outcome = SessionThresholdCheckDtoThresholdHitOutcome(
                 _threshold_hit_outcome
             )
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, SessionThresholdCheckDtoStatus]
-        if isinstance(_status, Unset):
+        if isinstance(_status, Unset) or _status is None:
             status = UNSET
         else:
             status = SessionThresholdCheckDtoStatus(_status)
 
         result = d.pop("result", UNSET)
 
         is_enabled = d.pop("isEnabled", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/session_threshold_value_dto_decimal.py` & `longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_decimal.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,24 +80,24 @@
         d = src_dict.copy()
         threshold_value = d.pop("thresholdValue", UNSET)
 
         _threshold_hit_outcome = d.pop("thresholdHitOutcome", UNSET)
         threshold_hit_outcome: Union[
             Unset, SessionThresholdValueDtoDecimalThresholdHitOutcome
         ]
-        if isinstance(_threshold_hit_outcome, Unset):
+        if isinstance(_threshold_hit_outcome, Unset) or _threshold_hit_outcome is None:
             threshold_hit_outcome = UNSET
         else:
             threshold_hit_outcome = SessionThresholdValueDtoDecimalThresholdHitOutcome(
                 _threshold_hit_outcome
             )
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, SessionThresholdValueDtoDecimalStatus]
-        if isinstance(_status, Unset):
+        if isinstance(_status, Unset) or _status is None:
             status = UNSET
         else:
             status = SessionThresholdValueDtoDecimalStatus(_status)
 
         result = d.pop("result", UNSET)
 
         is_enabled = d.pop("isEnabled", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/session_threshold_value_dto_int_32.py` & `longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_int_32.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,24 +80,24 @@
         d = src_dict.copy()
         threshold_value = d.pop("thresholdValue", UNSET)
 
         _threshold_hit_outcome = d.pop("thresholdHitOutcome", UNSET)
         threshold_hit_outcome: Union[
             Unset, SessionThresholdValueDtoInt32ThresholdHitOutcome
         ]
-        if isinstance(_threshold_hit_outcome, Unset):
+        if isinstance(_threshold_hit_outcome, Unset) or _threshold_hit_outcome is None:
             threshold_hit_outcome = UNSET
         else:
             threshold_hit_outcome = SessionThresholdValueDtoInt32ThresholdHitOutcome(
                 _threshold_hit_outcome
             )
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, SessionThresholdValueDtoInt32Status]
-        if isinstance(_status, Unset):
+        if isinstance(_status, Unset) or _status is None:
             status = UNSET
         else:
             status = SessionThresholdValueDtoInt32Status(_status)
 
         result = d.pop("result", UNSET)
 
         is_enabled = d.pop("isEnabled", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/session_thresholds_dto.py` & `longship-2024.4.15/longship_api_client/models/session_thresholds_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,79 +142,79 @@
                 thresholds_hit_item_data
             )
 
             thresholds_hit.append(thresholds_hit_item)
 
         _min_kwh_ac = d.pop("minKwhAc", UNSET)
         min_kwh_ac: Union[Unset, SessionThresholdValueDtoDecimal]
-        if isinstance(_min_kwh_ac, Unset):
+        if isinstance(_min_kwh_ac, Unset) or _min_kwh_ac is None:
             min_kwh_ac = UNSET
         else:
             min_kwh_ac = SessionThresholdValueDtoDecimal.from_dict(_min_kwh_ac)
 
         _max_kwh_ac = d.pop("maxKwhAc", UNSET)
         max_kwh_ac: Union[Unset, SessionThresholdValueDtoDecimal]
-        if isinstance(_max_kwh_ac, Unset):
+        if isinstance(_max_kwh_ac, Unset) or _max_kwh_ac is None:
             max_kwh_ac = UNSET
         else:
             max_kwh_ac = SessionThresholdValueDtoDecimal.from_dict(_max_kwh_ac)
 
         _min_kwh_dc = d.pop("minKwhDc", UNSET)
         min_kwh_dc: Union[Unset, SessionThresholdValueDtoDecimal]
-        if isinstance(_min_kwh_dc, Unset):
+        if isinstance(_min_kwh_dc, Unset) or _min_kwh_dc is None:
             min_kwh_dc = UNSET
         else:
             min_kwh_dc = SessionThresholdValueDtoDecimal.from_dict(_min_kwh_dc)
 
         _max_kwh_dc = d.pop("maxKwhDc", UNSET)
         max_kwh_dc: Union[Unset, SessionThresholdValueDtoDecimal]
-        if isinstance(_max_kwh_dc, Unset):
+        if isinstance(_max_kwh_dc, Unset) or _max_kwh_dc is None:
             max_kwh_dc = UNSET
         else:
             max_kwh_dc = SessionThresholdValueDtoDecimal.from_dict(_max_kwh_dc)
 
         _min_duration_in_minutes_ac = d.pop("minDurationInMinutesAc", UNSET)
         min_duration_in_minutes_ac: Union[Unset, SessionThresholdValueDtoInt32]
-        if isinstance(_min_duration_in_minutes_ac, Unset):
+        if isinstance(_min_duration_in_minutes_ac, Unset) or _min_duration_in_minutes_ac is None:
             min_duration_in_minutes_ac = UNSET
         else:
             min_duration_in_minutes_ac = SessionThresholdValueDtoInt32.from_dict(
                 _min_duration_in_minutes_ac
             )
 
         _min_duration_in_minutes_dc = d.pop("minDurationInMinutesDc", UNSET)
         min_duration_in_minutes_dc: Union[Unset, SessionThresholdValueDtoInt32]
-        if isinstance(_min_duration_in_minutes_dc, Unset):
+        if isinstance(_min_duration_in_minutes_dc, Unset) or _min_duration_in_minutes_dc is None:
             min_duration_in_minutes_dc = UNSET
         else:
             min_duration_in_minutes_dc = SessionThresholdValueDtoInt32.from_dict(
                 _min_duration_in_minutes_dc
             )
 
         _max_session_age_in_days = d.pop("maxSessionAgeInDays", UNSET)
         max_session_age_in_days: Union[Unset, SessionThresholdValueDtoInt32]
-        if isinstance(_max_session_age_in_days, Unset):
+        if isinstance(_max_session_age_in_days, Unset) or _max_session_age_in_days is None:
             max_session_age_in_days = UNSET
         else:
             max_session_age_in_days = SessionThresholdValueDtoInt32.from_dict(
                 _max_session_age_in_days
             )
 
         _check_charging_speed = d.pop("checkChargingSpeed", UNSET)
         check_charging_speed: Union[Unset, SessionThresholdCheckDto]
-        if isinstance(_check_charging_speed, Unset):
+        if isinstance(_check_charging_speed, Unset) or _check_charging_speed is None:
             check_charging_speed = UNSET
         else:
             check_charging_speed = SessionThresholdCheckDto.from_dict(
                 _check_charging_speed
             )
 
         _check_session_in_future = d.pop("checkSessionInFuture", UNSET)
         check_session_in_future: Union[Unset, SessionThresholdCheckDto]
-        if isinstance(_check_session_in_future, Unset):
+        if isinstance(_check_session_in_future, Unset) or _check_session_in_future is None:
             check_session_in_future = UNSET
         else:
             check_session_in_future = SessionThresholdCheckDto.from_dict(
                 _check_session_in_future
             )
 
         session_thresholds_dto = cls(
```

### Comparing `longship-2024.3.15/longship_api_client/models/set_charging_profile_request.py` & `longship-2024.4.15/longship_api_client/models/set_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/started_by_info_dto.py` & `longship-2024.4.15/longship_api_client/models/started_by_info_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,31 +83,31 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.started_by_token_dto import StartedByTokenDto
 
         d = src_dict.copy()
         _token_info = d.pop("tokenInfo", UNSET)
         token_info: Union[Unset, StartedByTokenDto]
-        if isinstance(_token_info, Unset):
+        if isinstance(_token_info, Unset) or _token_info is None:
             token_info = UNSET
         else:
             token_info = StartedByTokenDto.from_dict(_token_info)
 
         _roaming_platform_type = d.pop("roamingPlatformType", UNSET)
         roaming_platform_type: Union[Unset, StartedByInfoDtoRoamingPlatformType]
-        if isinstance(_roaming_platform_type, Unset):
+        if isinstance(_roaming_platform_type, Unset) or _roaming_platform_type is None:
             roaming_platform_type = UNSET
         else:
             roaming_platform_type = StartedByInfoDtoRoamingPlatformType(
                 _roaming_platform_type
             )
 
         _authorization_state = d.pop("authorizationState", UNSET)
         authorization_state: Union[Unset, StartedByInfoDtoAuthorizationState]
-        if isinstance(_authorization_state, Unset):
+        if isinstance(_authorization_state, Unset) or _authorization_state is None:
             authorization_state = UNSET
         else:
             authorization_state = StartedByInfoDtoAuthorizationState(
                 _authorization_state
             )
 
         roaming_platform_connection_id = d.pop("roamingPlatformConnectionId", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/started_by_info_dto_authorization_state.py` & `longship-2024.4.15/longship_api_client/models/started_by_info_dto_authorization_state.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/started_by_token_dto.py` & `longship-2024.4.15/longship_api_client/models/started_by_token_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,24 +104,24 @@
         d = src_dict.copy()
         uid = d.pop("uid", UNSET)
 
         auth_reference = d.pop("authReference", UNSET)
 
         _token_type = d.pop("tokenType", UNSET)
         token_type: Union[Unset, StartedByTokenDtoTokenType]
-        if isinstance(_token_type, Unset):
+        if isinstance(_token_type, Unset) or _token_type is None:
             token_type = UNSET
         else:
             token_type = StartedByTokenDtoTokenType(_token_type)
 
         contract_id = d.pop("contractId", UNSET)
 
         _auth_method = d.pop("authMethod", UNSET)
         auth_method: Union[Unset, StartedByTokenDtoAuthMethod]
-        if isinstance(_auth_method, Unset):
+        if isinstance(_auth_method, Unset) or _auth_method is None:
             auth_method = UNSET
         else:
             auth_method = StartedByTokenDtoAuthMethod(_auth_method)
 
         provider_country_code = d.pop("providerCountryCode", UNSET)
 
         provider_party_id = d.pop("providerPartyId", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/status_schedule_dto.py` & `longship-2024.4.15/longship_api_client/models/status_schedule_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,29 +57,29 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _period_begin = d.pop("period_begin", UNSET)
         period_begin: Union[Unset, datetime.datetime]
-        if isinstance(_period_begin, Unset):
+        if isinstance(_period_begin, Unset) or _period_begin is None:
             period_begin = UNSET
         else:
             period_begin = isoparse(_period_begin)
 
         _period_end = d.pop("period_end", UNSET)
         period_end: Union[Unset, datetime.datetime]
-        if isinstance(_period_end, Unset):
+        if isinstance(_period_end, Unset) or _period_end is None:
             period_end = UNSET
         else:
             period_end = isoparse(_period_end)
 
         _status = d.pop("status", UNSET)
         status: Union[Unset, StatusScheduleDtoStatus]
-        if isinstance(_status, Unset):
+        if isinstance(_status, Unset) or _status is None:
             status = UNSET
         else:
             status = StatusScheduleDtoStatus(_status)
 
         status_schedule_dto = cls(
             period_begin=period_begin,
             period_end=period_end,
```

### Comparing `longship-2024.3.15/longship_api_client/models/string_segment.py` & `longship-2024.4.15/longship_api_client/models/string_segment.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_assertion_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_assertion_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _tariff_type = d.pop("tariffType", UNSET)
         tariff_type: Union[Unset, TariffAssertionDtoTariffType]
-        if isinstance(_tariff_type, Unset):
+        if isinstance(_tariff_type, Unset) or _tariff_type is None:
             tariff_type = UNSET
         else:
             tariff_type = TariffAssertionDtoTariffType(_tariff_type)
 
         is_tariff_used = d.pop("isTariffUsed", UNSET)
 
         tariff_result = d.pop("tariffResult", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_distribution_get_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_distribution_get_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -141,29 +141,29 @@
                 price_history_item_data
             )
 
             price_history.append(price_history_item)
 
         _created = d.pop("created", UNSET)
         created: Union[Unset, datetime.datetime]
-        if isinstance(_created, Unset):
+        if isinstance(_created, Unset) or _created is None:
             created = UNSET
         else:
             created = isoparse(_created)
 
         _deleted = d.pop("deleted", UNSET)
         deleted: Union[Unset, datetime.datetime]
-        if isinstance(_deleted, Unset):
+        if isinstance(_deleted, Unset) or _deleted is None:
             deleted = UNSET
         else:
             deleted = isoparse(_deleted)
 
         _updated = d.pop("updated", UNSET)
         updated: Union[Unset, datetime.datetime]
-        if isinstance(_updated, Unset):
+        if isinstance(_updated, Unset) or _updated is None:
             updated = UNSET
         else:
             updated = isoparse(_updated)
 
         tariff_distribution_get_dto = cls(
             id=id,
             name=name,
```

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_distribution_history_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_distribution_history_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _valid_from = d.pop("validFrom", UNSET)
         valid_from: Union[Unset, datetime.datetime]
-        if isinstance(_valid_from, Unset):
+        if isinstance(_valid_from, Unset) or _valid_from is None:
             valid_from = UNSET
         else:
             valid_from = isoparse(_valid_from)
 
         energy_compensation = d.pop("energyCompensation", UNSET)
 
         fixed_tenant_k_wh_fee = d.pop("fixedTenantKWhFee", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_distribution_post_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_distribution_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_distribution_put_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_distribution_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,29 +261,29 @@
 
         price_incl_vat = d.pop("priceInclVat", UNSET)
 
         currency = d.pop("currency", UNSET)
 
         _last_updated = d.pop("last_updated", UNSET)
         last_updated: Union[Unset, datetime.datetime]
-        if isinstance(_last_updated, Unset):
+        if isinstance(_last_updated, Unset) or _last_updated is None:
             last_updated = UNSET
         else:
             last_updated = isoparse(_last_updated)
 
         _usage_type = d.pop("usageType", UNSET)
         usage_type: Union[Unset, TariffDtoUsageType]
-        if isinstance(_usage_type, Unset):
+        if isinstance(_usage_type, Unset) or _usage_type is None:
             usage_type = UNSET
         else:
             usage_type = TariffDtoUsageType(_usage_type)
 
         _tariff_type = d.pop("tariffType", UNSET)
         tariff_type: Union[Unset, TariffDtoTariffType]
-        if isinstance(_tariff_type, Unset):
+        if isinstance(_tariff_type, Unset) or _tariff_type is None:
             tariff_type = UNSET
         else:
             tariff_type = TariffDtoTariffType(_tariff_type)
 
         vat = d.pop("vat", UNSET)
 
         is_vat_relevant = d.pop("isVatRelevant", UNSET)
@@ -294,15 +294,15 @@
 
         location_id = d.pop("locationId", UNSET)
 
         is_private_emp_tariff = d.pop("isPrivateEmpTariff", UNSET)
 
         _private_emp_tariff = d.pop("privateEmpTariff", UNSET)
         private_emp_tariff: Union[Unset, PrivateEmpTariffDto]
-        if isinstance(_private_emp_tariff, Unset):
+        if isinstance(_private_emp_tariff, Unset) or _private_emp_tariff is None:
             private_emp_tariff = UNSET
         else:
             private_emp_tariff = PrivateEmpTariffDto.from_dict(_private_emp_tariff)
 
         parking_tariff = d.pop("parkingTariff", UNSET)
 
         parking_step_size_in_minutes = d.pop("parkingStepSizeInMinutes", UNSET)
@@ -331,15 +331,15 @@
 
             price_history.append(price_history_item)
 
         external_reference = d.pop("externalReference", UNSET)
 
         _deleted = d.pop("deleted", UNSET)
         deleted: Union[Unset, datetime.datetime]
-        if isinstance(_deleted, Unset):
+        if isinstance(_deleted, Unset) or _deleted is None:
             deleted = UNSET
         else:
             deleted = isoparse(_deleted)
 
         tariff_dto = cls(
             tenant_id=tenant_id,
             id=id,
```

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_info_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_post_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_post_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,22 +139,22 @@
         d = src_dict.copy()
         name = d.pop("name", UNSET)
 
         currency = d.pop("currency", UNSET)
 
         _usage_type = d.pop("usageType", UNSET)
         usage_type: Union[Unset, TariffPostDtoUsageType]
-        if isinstance(_usage_type, Unset):
+        if isinstance(_usage_type, Unset) or _usage_type is None:
             usage_type = UNSET
         else:
             usage_type = TariffPostDtoUsageType(_usage_type)
 
         _private_emp_tariff = d.pop("privateEmpTariff", UNSET)
         private_emp_tariff: Union[Unset, PrivateEmpTariffDto]
-        if isinstance(_private_emp_tariff, Unset):
+        if isinstance(_private_emp_tariff, Unset) or _private_emp_tariff is None:
             private_emp_tariff = UNSET
         else:
             private_emp_tariff = PrivateEmpTariffDto.from_dict(_private_emp_tariff)
 
         start_tariff = d.pop("startTariff", UNSET)
 
         price = d.pop("price", UNSET)
```

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_price_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_price_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,22 +139,22 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.tariff_restriction import TariffRestriction
 
         d = src_dict.copy()
         _created_timestamp = d.pop("createdTimestamp", UNSET)
         created_timestamp: Union[Unset, datetime.datetime]
-        if isinstance(_created_timestamp, Unset):
+        if isinstance(_created_timestamp, Unset) or _created_timestamp is None:
             created_timestamp = UNSET
         else:
             created_timestamp = isoparse(_created_timestamp)
 
         _valid_from = d.pop("validFrom", UNSET)
         valid_from: Union[Unset, datetime.datetime]
-        if isinstance(_valid_from, Unset):
+        if isinstance(_valid_from, Unset) or _valid_from is None:
             valid_from = UNSET
         else:
             valid_from = isoparse(_valid_from)
 
         start_tariff = d.pop("startTariff", UNSET)
 
         price_per_kwh = d.pop("pricePerKwh", UNSET)
@@ -182,15 +182,15 @@
 
         time_step_size_in_minutes = d.pop("timeStepSizeInMinutes", UNSET)
 
         time_grace_period_in_minutes = d.pop("timeGracePeriodInMinutes", UNSET)
 
         _approval_status = d.pop("approvalStatus", UNSET)
         approval_status: Union[Unset, TariffPriceDtoApprovalStatus]
-        if isinstance(_approval_status, Unset):
+        if isinstance(_approval_status, Unset) or _approval_status is None:
             approval_status = UNSET
         else:
             approval_status = TariffPriceDtoApprovalStatus(_approval_status)
 
         tariff_price_dto = cls(
             created_timestamp=created_timestamp,
             valid_from=valid_from,
```

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_put_dto.py` & `longship-2024.4.15/longship_api_client/models/tariff_put_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         d = src_dict.copy()
         name = d.pop("name", UNSET)
 
         hubject_id = d.pop("hubjectId", UNSET)
 
         _private_emp_tariff = d.pop("privateEmpTariff", UNSET)
         private_emp_tariff: Union[Unset, PrivateEmpTariffDto]
-        if isinstance(_private_emp_tariff, Unset):
+        if isinstance(_private_emp_tariff, Unset) or _private_emp_tariff is None:
             private_emp_tariff = UNSET
         else:
             private_emp_tariff = PrivateEmpTariffDto.from_dict(_private_emp_tariff)
 
         start_tariff = d.pop("startTariff", UNSET)
 
         price = d.pop("price", UNSET)
@@ -174,15 +174,15 @@
 
         time_grace_period_in_minutes = d.pop("timeGracePeriodInMinutes", UNSET)
 
         external_reference = d.pop("externalReference", UNSET)
 
         _deleted = d.pop("deleted", UNSET)
         deleted: Union[Unset, datetime.datetime]
-        if isinstance(_deleted, Unset):
+        if isinstance(_deleted, Unset) or _deleted is None:
             deleted = UNSET
         else:
             deleted = isoparse(_deleted)
 
         tariff_put_dto = cls(
             name=name,
             hubject_id=hubject_id,
```

### Comparing `longship-2024.3.15/longship_api_client/models/tariff_restriction.py` & `longship-2024.4.15/longship_api_client/models/tariff_restriction.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,29 +75,29 @@
         d = src_dict.copy()
         start_time = d.pop("startTime", UNSET)
 
         end_time = d.pop("endTime", UNSET)
 
         _start_date = d.pop("startDate", UNSET)
         start_date: Union[Unset, datetime.datetime]
-        if isinstance(_start_date, Unset):
+        if isinstance(_start_date, Unset) or _start_date is None:
             start_date = UNSET
         else:
             start_date = isoparse(_start_date)
 
         _end_date = d.pop("endDate", UNSET)
         end_date: Union[Unset, datetime.datetime]
-        if isinstance(_end_date, Unset):
+        if isinstance(_end_date, Unset) or _end_date is None:
             end_date = UNSET
         else:
             end_date = isoparse(_end_date)
 
         _day_of_week = d.pop("dayOfWeek", UNSET)
         day_of_week: Union[Unset, TariffRestrictionDayOfWeek]
-        if isinstance(_day_of_week, Unset):
+        if isinstance(_day_of_week, Unset) or _day_of_week is None:
             day_of_week = UNSET
         else:
             day_of_week = TariffRestrictionDayOfWeek(_day_of_week)
 
         tariff_restriction = cls(
             start_time=start_time,
             end_time=end_time,
```

### Comparing `longship-2024.3.15/longship_api_client/models/token_info_dto.py` & `longship-2024.4.15/longship_api_client/models/token_info_dto.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         d = src_dict.copy()
         id_tag = d.pop("idTag", UNSET)
 
         contract_id = d.pop("contractId", UNSET)
 
         _token_type = d.pop("tokenType", UNSET)
         token_type: Union[Unset, TokenInfoDtoTokenType]
-        if isinstance(_token_type, Unset):
+        if isinstance(_token_type, Unset) or _token_type is None:
             token_type = UNSET
         else:
             token_type = TokenInfoDtoTokenType(_token_type)
 
         token_info_dto = cls(
             id_tag=id_tag,
             contract_id=contract_id,
```

### Comparing `longship-2024.3.15/longship_api_client/models/trigger_message_request.py` & `longship-2024.4.15/longship_api_client/models/trigger_message_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/unlock_connector_request.py` & `longship-2024.4.15/longship_api_client/models/unlock_connector_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/update_firmware_request.py` & `longship-2024.4.15/longship_api_client/models/update_firmware_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/webhook_get_dto.py` & `longship-2024.4.15/longship_api_client/models/webhook_get_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,22 +130,22 @@
 
             headers.append(headers_item)
 
         url = d.pop("url", UNSET)
 
         _created = d.pop("created", UNSET)
         created: Union[Unset, datetime.datetime]
-        if isinstance(_created, Unset):
+        if isinstance(_created, Unset) or _created is None:
             created = UNSET
         else:
             created = isoparse(_created)
 
         _updated = d.pop("updated", UNSET)
         updated: Union[Unset, datetime.datetime]
-        if isinstance(_updated, Unset):
+        if isinstance(_updated, Unset) or _updated is None:
             updated = UNSET
         else:
             updated = isoparse(_updated)
 
         webhook_get_dto = cls(
             id=id,
             name=name,
```

### Comparing `longship-2024.3.15/longship_api_client/models/webhook_get_dto_event_types_item.py` & `longship-2024.4.15/longship_api_client/models/webhook_get_dto_event_types_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/webhook_header_dto.py` & `longship-2024.4.15/longship_api_client/models/webhook_header_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/webhook_post_dto.py` & `longship-2024.4.15/longship_api_client/models/webhook_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/webhook_post_dto_event_types_item.py` & `longship-2024.4.15/longship_api_client/models/webhook_post_dto_event_types_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/webhook_put_dto.py` & `longship-2024.4.15/longship_api_client/models/webhook_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/webhook_put_dto_event_types_item.py` & `longship-2024.4.15/longship_api_client/models/webhook_put_dto_event_types_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/models/webhook_summary_get_dto.py` & `longship-2024.4.15/longship_api_client/models/webhook_summary_get_dto.py`

 * *Files 11% similar despite different names*

```diff
@@ -93,22 +93,22 @@
         for event_types_item_data in _event_types or []:
             event_types_item = WebhookSummaryGetDtoEventTypesItem(event_types_item_data)
 
             event_types.append(event_types_item)
 
         _created = d.pop("created", UNSET)
         created: Union[Unset, datetime.datetime]
-        if isinstance(_created, Unset):
+        if isinstance(_created, Unset) or _created is None:
             created = UNSET
         else:
             created = isoparse(_created)
 
         _updated = d.pop("updated", UNSET)
         updated: Union[Unset, datetime.datetime]
-        if isinstance(_updated, Unset):
+        if isinstance(_updated, Unset) or _updated is None:
             updated = UNSET
         else:
             updated = isoparse(_updated)
 
         webhook_summary_get_dto = cls(
             id=id,
             name=name,
```

### Comparing `longship-2024.3.15/longship_api_client/models/webhook_summary_get_dto_event_types_item.py` & `longship-2024.4.15/longship_api_client/models/webhook_summary_get_dto_event_types_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/longship_api_client/types.py` & `longship-2024.4.15/longship_api_client/types.py`

 * *Files identical despite different names*

### Comparing `longship-2024.3.15/pyproject.toml` & `longship-2024.4.15/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "longship"
-version = "2024.03.15"
+version = "2024.04.15"
 description = "A client library for accessing Longship API"
 
 authors = ["Wojtek Siudzinski <admin@suda.pl>"]
 
 readme = "README.md"
 packages = [
     {include = "longship_api_client"},
```

### Comparing `longship-2024.3.15/PKG-INFO` & `longship-2024.4.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longship
-Version: 2024.3.15
+Version: 2024.4.15
 Summary: A client library for accessing Longship API
 Author: Wojtek Siudzinski
 Author-email: admin@suda.pl
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

