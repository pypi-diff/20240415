# Comparing `tmp/pylogram-0.4.4.tar.gz` & `tmp/pylogram-0.5.0.tar.gz`

## Comparing `pylogram-0.4.4.tar` & `pylogram-0.5.0.tar`

### file list

```diff
@@ -1,459 +1,476 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pylogram-0.4.4/dev-requirements.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pylogram-0.4.4/tox.ini
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/__init__.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/api/__init__.py
--rw-r--r--   0        0        0    22549 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/api/compiler.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/api/source/auth_key.tl
--rw-r--r--   0        0        0   198353 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/api/source/main_api.tl
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/api/source/sys_msgs.tl
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/api/template/combinator.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/api/template/type.txt
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/__init__.py
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/compiler.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/sort.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/template/class.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pylogram-0.4.4/compiler/errors/template/sub_class.txt
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/__init__.py
--rw-r--r--   0        0        0    41892 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/client.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/constants.py
--rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/dispatcher.py
--rw-r--r--   0        0        0   208082 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/emoji.py
--rw-r--r--   0        0        0    15215 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/file_id.py
--rw-r--r--   0        0        0    24894 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/filters.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/middleware.py
--rw-r--r--   0        0        0    61976 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/mime_types.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/peers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/py.typed
--rw-r--r--   0        0        0    20661 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw_parsers.py
--rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/utils.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/__init__.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/connection.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/crypto/__init__.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/crypto/aes.py
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/crypto/prime.py
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/crypto/rsa.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/auto_name.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/chat_action.py
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/chat_type.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/message_media_type.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/poll_type.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/enums/user_status.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/errors/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/errors/lib_errors.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/errors/rpc_error.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/__init__.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/handler.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/message_handler.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/__init__.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/business/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/business/get_connected_bots.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/business/update_business_away_message.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/business/update_business_greeting_message.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/business/update_business_location.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/business/update_business_work_hours.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/business/update_connected_bot.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/middleware.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/forums/__init__.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/forums/create_forum_topic.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/forums/delete_topic_history.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/forums/edit_forum_topic.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/forums/get_forum_topics.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/forums/get_forum_topics_by_id.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/forums/reorder_pinned_forum_topics.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/forums/toggle_view_forum_as_messages.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/forums/update_pinned_forum_topic.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10436 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    13083 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    12862 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    10746 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    20122 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_message.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0     8287 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_reaction.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    12232 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_video.py
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/premium/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/premium/apply_boost.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/premium/get_boosts_list.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/premium/get_boosts_status.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/premium/get_my_boosts.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/premium/get_premium_promo.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/premium/get_user_boosts.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/__init__.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/block_user.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/get_users.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/set_username.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/add_middleware.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/remove_middleware.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/run.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/parser/__init__.py
--rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/parser/html.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/parser/markdown.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/parser/parser.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/parser/utils.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/list.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/message.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/session/__init__.py
--rw-r--r--   0        0        0    11507 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/session/auth.py
--rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/session/session.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/session/internals/seq_no.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/storage/__init__.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/storage/file_storage.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/storage/memory_storage.py
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/storage/storage.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/list.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/object.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/update.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    13241 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5322 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0   147111 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0    19896 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    14854 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pylogram-0.4.4/pylogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pylogram-0.4.4/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pylogram-0.4.4/LICENSE
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pylogram-0.4.4/NOTICE
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 pylogram-0.4.4/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pylogram-0.4.4/hatch_build.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 pylogram-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    44442 2020-02-02 00:00:00.000000 pylogram-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pylogram-0.5.0/dev-requirements.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pylogram-0.5.0/tox.ini
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/__init__.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/api/__init__.py
+-rw-r--r--   0        0        0    22549 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/api/compiler.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/api/source/auth_key.tl
+-rw-r--r--   0        0        0   198353 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/api/source/main_api.tl
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/api/source/sys_msgs.tl
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/api/template/combinator.txt
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/api/template/type.txt
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/__init__.py
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/compiler.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/sort.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/template/class.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pylogram-0.5.0/compiler/errors/template/sub_class.txt
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/__init__.py
+-rw-r--r--   0        0        0    41892 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/client.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/constants.py
+-rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/dispatcher.py
+-rw-r--r--   0        0        0   208082 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/emoji.py
+-rw-r--r--   0        0        0    15215 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/file_id.py
+-rw-r--r--   0        0        0    24894 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/filters.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/middleware.py
+-rw-r--r--   0        0        0    61976 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/mime_types.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/peers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/py.typed
+-rw-r--r--   0        0        0    20661 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw_parsers.py
+-rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/utils.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/__init__.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/connection.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/transport/__init__.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_intermediate_o.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/crypto/__init__.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/crypto/aes.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/crypto/mtproto.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/crypto/prime.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/crypto/rsa.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/auto_name.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/chat_action.py
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/chat_event_action.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/chat_member_status.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/chat_members_filter.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/chat_type.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/message_entity_type.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/message_media_type.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/message_service_type.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/messages_filter.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/next_code_type.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/parse_mode.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/poll_type.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/sent_code_type.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/enums/user_status.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/errors/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/errors/lib_errors.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/errors/rpc_error.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/__init__.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/callback_query_handler.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/disconnect_handler.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/edited_message_handler.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/handler.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/inline_query_handler.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/message_handler.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/poll_handler.py
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/raw_update_handler.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/handlers/user_status_handler.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/__init__.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/advanced/__init__.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/advanced/invoke.py
+-rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/advanced/save_file.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/check_password.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/connect.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/disconnect.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/get_password_hint.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/initialize.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/log_out.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/recover_password.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/resend_code.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/send_code.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/sign_in.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/sign_up.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/auth/terminate.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/__init__.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/send_game.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/bots/set_game_score.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/business/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/business/get_connected_bots.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/business/update_business_away_message.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/business/update_business_greeting_message.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/business/update_business_location.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/business/update_business_work_hours.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/business/update_connected_bot.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/check_chat_list_invite.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/delete_dialog_filter.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/edit_exported_invite.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/export_chat_list_invite.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/export_dialog_filter.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/export_dialog_filter_invite.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/get_chat_list_updates.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/get_dialog_filters.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/get_exported_invites.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/get_suggested_dialog_filters.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/join_chat_list_invite.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/join_chat_list_updates.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/leave_dialog_filter.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/update_dialog_filter.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/update_dialog_filters_order.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chat_lists/update_exported_invite.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/__init__.py
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/add_chat_members.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/archive_chats.py
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/create_channel.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/create_group.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/create_supergroup.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/delete_channel.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/delete_user_history.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_chat.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_chat_member.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_chat_members.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_dialogs.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/join_chat.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/leave_chat.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/set_chat_description.py
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/set_chat_title.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/set_chat_username.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/contacts/__init__.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/contacts/add_contact.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/contacts/get_contacts.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/contacts/import_contacts.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/__init__.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/middleware.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_message.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_poll.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/decorators/on_user_status.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/forums/__init__.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/forums/create_forum_topic.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/forums/delete_topic_history.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/forums/edit_forum_topic.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/forums/get_forum_topics.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/forums/get_forum_topics_by_id.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/forums/reorder_pinned_forum_topics.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/forums/toggle_view_forum_as_messages.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/forums/update_pinned_forum_topic.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/__init__.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/invite_links/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/__init__.py
+-rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/copy_media_group.py
+-rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/copy_message.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/delete_messages.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/download_media.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0        0        0    10436 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0        0        0    13083 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/edit_message_media.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/edit_message_text.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/forward_messages.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/get_chat_history.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/get_media_group.py
+-rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/get_messages.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/inline_session.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/read_chat_history.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/retract_vote.py
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/search_global.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/search_global_count.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/search_messages.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/search_messages_count.py
+-rw-r--r--   0        0        0    12862 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_animation.py
+-rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_audio.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_cached_media.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_chat_action.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_contact.py
+-rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_dice.py
+-rw-r--r--   0        0        0    10746 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_document.py
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_location.py
+-rw-r--r--   0        0        0    20122 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_media_group.py
+-rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_message.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_photo.py
+-rw-r--r--   0        0        0     8287 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_poll.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_reaction.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_sticker.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_venue.py
+-rw-r--r--   0        0        0    12232 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_video.py
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_video_note.py
+-rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/send_voice.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/stop_poll.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/stream_media.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/messages/vote_poll.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/password/__init__.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/password/change_cloud_password.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/password/remove_cloud_password.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/premium/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/premium/apply_boost.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/premium/get_boosts_list.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/premium/get_boosts_status.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/premium/get_my_boosts.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/premium/get_premium_promo.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/premium/get_user_boosts.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/block_user.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/get_chat_photos.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/get_common_chats.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/get_me.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/get_users.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/set_emoji_status.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/set_profile_photo.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/set_username.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/unblock_user.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/users/update_profile.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/__init__.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/add_handler.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/add_middleware.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/compose.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/export_session_string.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/idle.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/remove_handler.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/remove_middleware.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/restart.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/run.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/start.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/stop.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/parser/__init__.py
+-rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/parser/html.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/parser/markdown.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/parser/parser.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/parser/utils.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/__init__.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/future_salt.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/future_salts.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/gzip_packed.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/list.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/message.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/msg_container.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/tl_object.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/primitives/__init__.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/primitives/bool.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/primitives/bytes.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/primitives/double.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/primitives/int.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/primitives/string.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/raw/core/primitives/vector.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/session/__init__.py
+-rw-r--r--   0        0        0    11507 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/session/auth.py
+-rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/session/session.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/session/internals/__init__.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/session/internals/data_center.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/session/internals/msg_factory.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/session/internals/msg_id.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/session/internals/seq_no.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/storage/__init__.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/storage/file_storage.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/storage/memory_storage.py
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/storage/sqlite_storage.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/storage/storage.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/list.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/object.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/update.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/authorization/__init__.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/authorization/sent_code.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/authorization/terms_of_service.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0        0        0    13241 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/bots_and_keyboards/web_app_info.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/__init__.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0        0        0     5322 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_voice.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_media/__init__.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_media/input_media.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_media/input_media_animation.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_media/input_media_audio.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_media/input_media_document.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_media/input_media_photo.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_media/input_media_video.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_media/input_phone_contact.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_message_content/__init__.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/__init__.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/animation.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/audio.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/contact.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/dice.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/document.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/game.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/location.py
+-rw-r--r--   0        0        0   147111 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/message.py
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/photo.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/poll.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/reaction.py
+-rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/sticker.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/venue.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/video.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/video_note.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/voice.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/messages_and_media/web_page.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/__init__.py
+-rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0        0        0    19896 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/dialog.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/restriction.py
+-rw-r--r--   0        0        0    14854 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/user.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/username.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pylogram-0.5.0/pylogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pylogram-0.5.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pylogram-0.5.0/LICENSE
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pylogram-0.5.0/NOTICE
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 pylogram-0.5.0/README.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pylogram-0.5.0/hatch_build.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 pylogram-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    44442 2020-02-02 00:00:00.000000 pylogram-0.5.0/PKG-INFO
```

### Comparing `pylogram-0.4.4/compiler/__init__.py` & `pylogram-0.5.0/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/api/__init__.py` & `pylogram-0.5.0/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/api/compiler.py` & `pylogram-0.5.0/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/api/source/auth_key.tl` & `pylogram-0.5.0/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/api/source/main_api.tl` & `pylogram-0.5.0/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/api/source/sys_msgs.tl` & `pylogram-0.5.0/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/api/template/combinator.txt` & `pylogram-0.5.0/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/errors/__init__.py` & `pylogram-0.5.0/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/errors/compiler.py` & `pylogram-0.5.0/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/errors/sort.py` & `pylogram-0.5.0/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/errors/source/400_BAD_REQUEST.tsv` & `pylogram-0.5.0/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/errors/source/401_UNAUTHORIZED.tsv` & `pylogram-0.5.0/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/errors/source/403_FORBIDDEN.tsv` & `pylogram-0.5.0/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `pylogram-0.5.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `pylogram-0.5.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/__init__.py` & `pylogram-0.5.0/pylogram/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pylogram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.4.4"
+__version__ = "0.5.0"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 from . import crypto
 from . import emoji
```

### Comparing `pylogram-0.4.4/pylogram/client.py` & `pylogram-0.5.0/pylogram/client.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/dispatcher.py` & `pylogram-0.5.0/pylogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/emoji.py` & `pylogram-0.5.0/pylogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/file_id.py` & `pylogram-0.5.0/pylogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/filters.py` & `pylogram-0.5.0/pylogram/filters.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/mime_types.py` & `pylogram-0.5.0/pylogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/peers.py` & `pylogram-0.5.0/pylogram/peers.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw_parsers.py` & `pylogram-0.5.0/pylogram/raw_parsers.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/utils.py` & `pylogram-0.5.0/pylogram/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -469,7 +469,18 @@
         for arg in typing.get_args(base_type):
             if is_tl_object_of_base_type(value, arg):
                 return True
 
         return False
 
     return False
+
+
+CHAT_LIST_INVITE_LINK_PREFIX: str = "https://t.me/addlist/"
+
+
+def slug_to_chat_list_invite_link(slug: str) -> str:
+    return f"{self.CHAT_LIST_INVITE_LINK_PREFIX}{slug}"
+
+
+def chat_list_invite_link_to_slug(link: str) -> str:
+    return link.replace(self.CHAT_LIST_INVITE_LINK_PREFIX, '')
```

### Comparing `pylogram-0.4.4/pylogram/connection/__init__.py` & `pylogram-0.5.0/pylogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/connection/connection.py` & `pylogram-0.5.0/pylogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/connection/transport/__init__.py` & `pylogram-0.5.0/pylogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/connection/transport/tcp/__init__.py` & `pylogram-0.5.0/pylogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/connection/transport/tcp/tcp.py` & `pylogram-0.5.0/pylogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_abridged.py` & `pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_abridged_o.py` & `pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_full.py` & `pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_intermediate.py` & `pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/connection/transport/tcp/tcp_intermediate_o.py` & `pylogram-0.5.0/pylogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/crypto/__init__.py` & `pylogram-0.5.0/pylogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/crypto/aes.py` & `pylogram-0.5.0/pylogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/crypto/mtproto.py` & `pylogram-0.5.0/pylogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/crypto/prime.py` & `pylogram-0.5.0/pylogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/crypto/rsa.py` & `pylogram-0.5.0/pylogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/__init__.py` & `pylogram-0.5.0/pylogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/auto_name.py` & `pylogram-0.5.0/pylogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/chat_action.py` & `pylogram-0.5.0/pylogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/chat_event_action.py` & `pylogram-0.5.0/pylogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/chat_member_status.py` & `pylogram-0.5.0/pylogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/chat_members_filter.py` & `pylogram-0.5.0/pylogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/chat_type.py` & `pylogram-0.5.0/pylogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/message_entity_type.py` & `pylogram-0.5.0/pylogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/message_media_type.py` & `pylogram-0.5.0/pylogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/message_service_type.py` & `pylogram-0.5.0/pylogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/messages_filter.py` & `pylogram-0.5.0/pylogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/next_code_type.py` & `pylogram-0.5.0/pylogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/parse_mode.py` & `pylogram-0.5.0/pylogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/poll_type.py` & `pylogram-0.5.0/pylogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/sent_code_type.py` & `pylogram-0.5.0/pylogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/enums/user_status.py` & `pylogram-0.5.0/pylogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/errors/__init__.py` & `pylogram-0.5.0/pylogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/errors/rpc_error.py` & `pylogram-0.5.0/pylogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/__init__.py` & `pylogram-0.5.0/pylogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/callback_query_handler.py` & `pylogram-0.5.0/pylogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/chat_join_request_handler.py` & `pylogram-0.5.0/pylogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/chat_member_updated_handler.py` & `pylogram-0.5.0/pylogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/chosen_inline_result_handler.py` & `pylogram-0.5.0/pylogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/deleted_messages_handler.py` & `pylogram-0.5.0/pylogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/disconnect_handler.py` & `pylogram-0.5.0/pylogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/edited_message_handler.py` & `pylogram-0.5.0/pylogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/handler.py` & `pylogram-0.5.0/pylogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/inline_query_handler.py` & `pylogram-0.5.0/pylogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/message_handler.py` & `pylogram-0.5.0/pylogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/poll_handler.py` & `pylogram-0.5.0/pylogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/raw_update_handler.py` & `pylogram-0.5.0/pylogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/handlers/user_status_handler.py` & `pylogram-0.5.0/pylogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/__init__.py` & `pylogram-0.5.0/pylogram/methods/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pylogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from .advanced import Advanced
 from .auth import Auth
 from .bots import Bots
 from .business import Business
+from .chat_lists import ChatLists
 from .chats import Chats
 from .contacts import Contacts
 from .decorators import Decorators
 from .forums import Forums
 from .invite_links import InviteLinks
 from .messages import Messages
 from .password import Password
@@ -34,14 +35,15 @@
 
 
 class Methods(
     Advanced,
     Auth,
     Bots,
     Business,
+    ChatLists,
     Chats,
     Contacts,
     Decorators,
     Forums,
     InviteLinks,
     Messages,
     Password,
```

### Comparing `pylogram-0.4.4/pylogram/methods/advanced/__init__.py` & `pylogram-0.5.0/pylogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/advanced/invoke.py` & `pylogram-0.5.0/pylogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/advanced/resolve_peer.py` & `pylogram-0.5.0/pylogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/advanced/save_file.py` & `pylogram-0.5.0/pylogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/__init__.py` & `pylogram-0.5.0/pylogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/accept_terms_of_service.py` & `pylogram-0.5.0/pylogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/check_password.py` & `pylogram-0.5.0/pylogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/connect.py` & `pylogram-0.5.0/pylogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/disconnect.py` & `pylogram-0.5.0/pylogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/get_password_hint.py` & `pylogram-0.5.0/pylogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/initialize.py` & `pylogram-0.5.0/pylogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/log_out.py` & `pylogram-0.5.0/pylogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/recover_password.py` & `pylogram-0.5.0/pylogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/resend_code.py` & `pylogram-0.5.0/pylogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/send_code.py` & `pylogram-0.5.0/pylogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/send_recovery_code.py` & `pylogram-0.5.0/pylogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/sign_in.py` & `pylogram-0.5.0/pylogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/sign_in_bot.py` & `pylogram-0.5.0/pylogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/sign_up.py` & `pylogram-0.5.0/pylogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/auth/terminate.py` & `pylogram-0.5.0/pylogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/__init__.py` & `pylogram-0.5.0/pylogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/answer_callback_query.py` & `pylogram-0.5.0/pylogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/answer_inline_query.py` & `pylogram-0.5.0/pylogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/answer_web_app_query.py` & `pylogram-0.5.0/pylogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/delete_bot_commands.py` & `pylogram-0.5.0/pylogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/get_bot_commands.py` & `pylogram-0.5.0/pylogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/get_bot_default_privileges.py` & `pylogram-0.5.0/pylogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/get_chat_menu_button.py` & `pylogram-0.5.0/pylogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/get_game_high_scores.py` & `pylogram-0.5.0/pylogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/get_inline_bot_results.py` & `pylogram-0.5.0/pylogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/request_callback_answer.py` & `pylogram-0.5.0/pylogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/send_game.py` & `pylogram-0.5.0/pylogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/send_inline_bot_result.py` & `pylogram-0.5.0/pylogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/set_bot_commands.py` & `pylogram-0.5.0/pylogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/set_bot_default_privileges.py` & `pylogram-0.5.0/pylogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/set_chat_menu_button.py` & `pylogram-0.5.0/pylogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/bots/set_game_score.py` & `pylogram-0.5.0/pylogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/business/__init__.py` & `pylogram-0.5.0/pylogram/methods/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/business/update_business_away_message.py` & `pylogram-0.5.0/pylogram/methods/business/update_business_away_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/business/update_business_greeting_message.py` & `pylogram-0.5.0/pylogram/methods/business/update_business_greeting_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/business/update_business_location.py` & `pylogram-0.5.0/pylogram/methods/business/update_business_location.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/business/update_business_work_hours.py` & `pylogram-0.5.0/pylogram/methods/business/update_business_work_hours.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/business/update_connected_bot.py` & `pylogram-0.5.0/pylogram/methods/business/update_connected_bot.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/__init__.py` & `pylogram-0.5.0/pylogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/add_chat_members.py` & `pylogram-0.5.0/pylogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/archive_chats.py` & `pylogram-0.5.0/pylogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/ban_chat_member.py` & `pylogram-0.5.0/pylogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/create_channel.py` & `pylogram-0.5.0/pylogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/create_group.py` & `pylogram-0.5.0/pylogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/create_supergroup.py` & `pylogram-0.5.0/pylogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/delete_channel.py` & `pylogram-0.5.0/pylogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/delete_chat_photo.py` & `pylogram-0.5.0/pylogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/delete_supergroup.py` & `pylogram-0.5.0/pylogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/delete_user_history.py` & `pylogram-0.5.0/pylogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_chat.py` & `pylogram-0.5.0/pylogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_chat_event_log.py` & `pylogram-0.5.0/pylogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_chat_member.py` & `pylogram-0.5.0/pylogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_chat_members.py` & `pylogram-0.5.0/pylogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_chat_members_count.py` & `pylogram-0.5.0/pylogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_chat_online_count.py` & `pylogram-0.5.0/pylogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_dialogs.py` & `pylogram-0.5.0/pylogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_dialogs_count.py` & `pylogram-0.5.0/pylogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_nearby_chats.py` & `pylogram-0.5.0/pylogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/get_send_as_chats.py` & `pylogram-0.5.0/pylogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/join_chat.py` & `pylogram-0.5.0/pylogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/leave_chat.py` & `pylogram-0.5.0/pylogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/mark_chat_unread.py` & `pylogram-0.5.0/pylogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/pin_chat_message.py` & `pylogram-0.5.0/pylogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/promote_chat_member.py` & `pylogram-0.5.0/pylogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/restrict_chat_member.py` & `pylogram-0.5.0/pylogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/set_administrator_title.py` & `pylogram-0.5.0/pylogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/set_chat_description.py` & `pylogram-0.5.0/pylogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/set_chat_permissions.py` & `pylogram-0.5.0/pylogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/set_chat_photo.py` & `pylogram-0.5.0/pylogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/set_chat_protected_content.py` & `pylogram-0.5.0/pylogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/set_chat_title.py` & `pylogram-0.5.0/pylogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/set_chat_username.py` & `pylogram-0.5.0/pylogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/set_send_as_chat.py` & `pylogram-0.5.0/pylogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/set_slow_mode.py` & `pylogram-0.5.0/pylogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/unarchive_chats.py` & `pylogram-0.5.0/pylogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/unban_chat_member.py` & `pylogram-0.5.0/pylogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/unpin_all_chat_messages.py` & `pylogram-0.5.0/pylogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/chats/unpin_chat_message.py` & `pylogram-0.5.0/pylogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/contacts/__init__.py` & `pylogram-0.5.0/pylogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/contacts/add_contact.py` & `pylogram-0.5.0/pylogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/contacts/delete_contacts.py` & `pylogram-0.5.0/pylogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/contacts/get_contacts.py` & `pylogram-0.5.0/pylogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/contacts/get_contacts_count.py` & `pylogram-0.5.0/pylogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/contacts/import_contacts.py` & `pylogram-0.5.0/pylogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/__init__.py` & `pylogram-0.5.0/pylogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/middleware.py` & `pylogram-0.5.0/pylogram/methods/decorators/middleware.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_callback_query.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_chat_join_request.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_chat_member_updated.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_chosen_inline_result.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_deleted_messages.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_disconnect.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_edited_message.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_inline_query.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_message.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_poll.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_raw_update.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/decorators/on_user_status.py` & `pylogram-0.5.0/pylogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/forums/__init__.py` & `pylogram-0.5.0/pylogram/methods/forums/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/forums/create_forum_topic.py` & `pylogram-0.5.0/pylogram/methods/forums/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/forums/edit_forum_topic.py` & `pylogram-0.5.0/pylogram/methods/forums/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/forums/get_forum_topics.py` & `pylogram-0.5.0/pylogram/methods/forums/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/forums/reorder_pinned_forum_topics.py` & `pylogram-0.5.0/pylogram/methods/forums/reorder_pinned_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/forums/update_pinned_forum_topic.py` & `pylogram-0.5.0/pylogram/methods/forums/update_pinned_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/__init__.py` & `pylogram-0.5.0/pylogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/approve_all_chat_join_requests.py` & `pylogram-0.5.0/pylogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/approve_chat_join_request.py` & `pylogram-0.5.0/pylogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/create_chat_invite_link.py` & `pylogram-0.5.0/pylogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/decline_all_chat_join_requests.py` & `pylogram-0.5.0/pylogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/decline_chat_join_request.py` & `pylogram-0.5.0/pylogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pylogram-0.5.0/pylogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/delete_chat_invite_link.py` & `pylogram-0.5.0/pylogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/edit_chat_invite_link.py` & `pylogram-0.5.0/pylogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/export_chat_invite_link.py` & `pylogram-0.5.0/pylogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/get_chat_admin_invite_links.py` & `pylogram-0.5.0/pylogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pylogram-0.5.0/pylogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pylogram-0.5.0/pylogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/get_chat_invite_link.py` & `pylogram-0.5.0/pylogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pylogram-0.5.0/pylogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pylogram-0.5.0/pylogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/get_chat_join_requests.py` & `pylogram-0.5.0/pylogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/invite_links/revoke_chat_invite_link.py` & `pylogram-0.5.0/pylogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/__init__.py` & `pylogram-0.5.0/pylogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/copy_media_group.py` & `pylogram-0.5.0/pylogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/copy_message.py` & `pylogram-0.5.0/pylogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/delete_messages.py` & `pylogram-0.5.0/pylogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/download_media.py` & `pylogram-0.5.0/pylogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/edit_inline_caption.py` & `pylogram-0.5.0/pylogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/edit_inline_media.py` & `pylogram-0.5.0/pylogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/edit_inline_reply_markup.py` & `pylogram-0.5.0/pylogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/edit_inline_text.py` & `pylogram-0.5.0/pylogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/edit_message_caption.py` & `pylogram-0.5.0/pylogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/edit_message_media.py` & `pylogram-0.5.0/pylogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/edit_message_reply_markup.py` & `pylogram-0.5.0/pylogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/edit_message_text.py` & `pylogram-0.5.0/pylogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/forward_messages.py` & `pylogram-0.5.0/pylogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/get_chat_history.py` & `pylogram-0.5.0/pylogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/get_chat_history_count.py` & `pylogram-0.5.0/pylogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/get_custom_emoji_stickers.py` & `pylogram-0.5.0/pylogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/get_discussion_message.py` & `pylogram-0.5.0/pylogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/get_discussion_replies.py` & `pylogram-0.5.0/pylogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/get_discussion_replies_count.py` & `pylogram-0.5.0/pylogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/get_media_group.py` & `pylogram-0.5.0/pylogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/get_messages.py` & `pylogram-0.5.0/pylogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/inline_session.py` & `pylogram-0.5.0/pylogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/read_chat_history.py` & `pylogram-0.5.0/pylogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/retract_vote.py` & `pylogram-0.5.0/pylogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/search_global.py` & `pylogram-0.5.0/pylogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/search_global_count.py` & `pylogram-0.5.0/pylogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/search_messages.py` & `pylogram-0.5.0/pylogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/search_messages_count.py` & `pylogram-0.5.0/pylogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_animation.py` & `pylogram-0.5.0/pylogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_audio.py` & `pylogram-0.5.0/pylogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_cached_media.py` & `pylogram-0.5.0/pylogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_chat_action.py` & `pylogram-0.5.0/pylogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_contact.py` & `pylogram-0.5.0/pylogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_dice.py` & `pylogram-0.5.0/pylogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_document.py` & `pylogram-0.5.0/pylogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_location.py` & `pylogram-0.5.0/pylogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_media_group.py` & `pylogram-0.5.0/pylogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_message.py` & `pylogram-0.5.0/pylogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_photo.py` & `pylogram-0.5.0/pylogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_poll.py` & `pylogram-0.5.0/pylogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_reaction.py` & `pylogram-0.5.0/pylogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_sticker.py` & `pylogram-0.5.0/pylogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_venue.py` & `pylogram-0.5.0/pylogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_video.py` & `pylogram-0.5.0/pylogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_video_note.py` & `pylogram-0.5.0/pylogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/send_voice.py` & `pylogram-0.5.0/pylogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/stop_poll.py` & `pylogram-0.5.0/pylogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/stream_media.py` & `pylogram-0.5.0/pylogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/messages/vote_poll.py` & `pylogram-0.5.0/pylogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/password/__init__.py` & `pylogram-0.5.0/pylogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/password/change_cloud_password.py` & `pylogram-0.5.0/pylogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/password/enable_cloud_password.py` & `pylogram-0.5.0/pylogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/password/remove_cloud_password.py` & `pylogram-0.5.0/pylogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/premium/get_boosts_list.py` & `pylogram-0.5.0/pylogram/methods/premium/get_boosts_list.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/premium/get_user_boosts.py` & `pylogram-0.5.0/pylogram/methods/premium/get_user_boosts.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/__init__.py` & `pylogram-0.5.0/pylogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/block_user.py` & `pylogram-0.5.0/pylogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/delete_profile_photos.py` & `pylogram-0.5.0/pylogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/get_chat_photos.py` & `pylogram-0.5.0/pylogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/get_chat_photos_count.py` & `pylogram-0.5.0/pylogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/get_common_chats.py` & `pylogram-0.5.0/pylogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/get_default_emoji_statuses.py` & `pylogram-0.5.0/pylogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/get_me.py` & `pylogram-0.5.0/pylogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/get_users.py` & `pylogram-0.5.0/pylogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/set_emoji_status.py` & `pylogram-0.5.0/pylogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/set_profile_photo.py` & `pylogram-0.5.0/pylogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/set_username.py` & `pylogram-0.5.0/pylogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/unblock_user.py` & `pylogram-0.5.0/pylogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/users/update_profile.py` & `pylogram-0.5.0/pylogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/__init__.py` & `pylogram-0.5.0/pylogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/add_handler.py` & `pylogram-0.5.0/pylogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/add_middleware.py` & `pylogram-0.5.0/pylogram/methods/utilities/add_middleware.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/compose.py` & `pylogram-0.5.0/pylogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/export_session_string.py` & `pylogram-0.5.0/pylogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/idle.py` & `pylogram-0.5.0/pylogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/remove_handler.py` & `pylogram-0.5.0/pylogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/remove_middleware.py` & `pylogram-0.5.0/pylogram/methods/utilities/remove_middleware.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/restart.py` & `pylogram-0.5.0/pylogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/run.py` & `pylogram-0.5.0/pylogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/start.py` & `pylogram-0.5.0/pylogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/stop.py` & `pylogram-0.5.0/pylogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/methods/utilities/stop_transmission.py` & `pylogram-0.5.0/pylogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/parser/__init__.py` & `pylogram-0.5.0/pylogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/parser/html.py` & `pylogram-0.5.0/pylogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/parser/markdown.py` & `pylogram-0.5.0/pylogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/parser/parser.py` & `pylogram-0.5.0/pylogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/parser/utils.py` & `pylogram-0.5.0/pylogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/__init__.py` & `pylogram-0.5.0/pylogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/__init__.py` & `pylogram-0.5.0/pylogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/future_salt.py` & `pylogram-0.5.0/pylogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/future_salts.py` & `pylogram-0.5.0/pylogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/gzip_packed.py` & `pylogram-0.5.0/pylogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/list.py` & `pylogram-0.5.0/pylogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/message.py` & `pylogram-0.5.0/pylogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/msg_container.py` & `pylogram-0.5.0/pylogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/tl_object.py` & `pylogram-0.5.0/pylogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/primitives/__init__.py` & `pylogram-0.5.0/pylogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/primitives/bool.py` & `pylogram-0.5.0/pylogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/primitives/bytes.py` & `pylogram-0.5.0/pylogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/primitives/double.py` & `pylogram-0.5.0/pylogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/primitives/int.py` & `pylogram-0.5.0/pylogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/primitives/string.py` & `pylogram-0.5.0/pylogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/raw/core/primitives/vector.py` & `pylogram-0.5.0/pylogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/session/__init__.py` & `pylogram-0.5.0/pylogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/session/auth.py` & `pylogram-0.5.0/pylogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/session/session.py` & `pylogram-0.5.0/pylogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/session/internals/__init__.py` & `pylogram-0.5.0/pylogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/session/internals/data_center.py` & `pylogram-0.5.0/pylogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/session/internals/msg_factory.py` & `pylogram-0.5.0/pylogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/session/internals/msg_id.py` & `pylogram-0.5.0/pylogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/session/internals/seq_no.py` & `pylogram-0.5.0/pylogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/storage/__init__.py` & `pylogram-0.5.0/pylogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/storage/file_storage.py` & `pylogram-0.5.0/pylogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/storage/memory_storage.py` & `pylogram-0.5.0/pylogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/storage/sqlite_storage.py` & `pylogram-0.5.0/pylogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/storage/storage.py` & `pylogram-0.5.0/pylogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/__init__.py` & `pylogram-0.5.0/pylogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/list.py` & `pylogram-0.5.0/pylogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/object.py` & `pylogram-0.5.0/pylogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/update.py` & `pylogram-0.5.0/pylogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/authorization/__init__.py` & `pylogram-0.5.0/pylogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/authorization/sent_code.py` & `pylogram-0.5.0/pylogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/authorization/terms_of_service.py` & `pylogram-0.5.0/pylogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/__init__.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/callback_game.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/callback_query.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/force_reply.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/game_high_score.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/keyboard_button.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/login_url.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/menu_button.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/menu_button_commands.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/menu_button_default.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/menu_button_web_app.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/sent_web_app_message.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/bots_and_keyboards/web_app_info.py` & `pylogram-0.5.0/pylogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/__init__.py` & `pylogram-0.5.0/pylogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/chosen_inline_result.py` & `pylogram-0.5.0/pylogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_animation.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_article.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_audio.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_animation.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_audio.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_document.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_photo.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_video.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_cached_voice.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_contact.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_document.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_location.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_photo.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_venue.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_video.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/inline_mode/inline_query_result_voice.py` & `pylogram-0.5.0/pylogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_media/__init__.py` & `pylogram-0.5.0/pylogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_media/input_media.py` & `pylogram-0.5.0/pylogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_media/input_media_animation.py` & `pylogram-0.5.0/pylogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_media/input_media_audio.py` & `pylogram-0.5.0/pylogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_media/input_media_document.py` & `pylogram-0.5.0/pylogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_media/input_media_photo.py` & `pylogram-0.5.0/pylogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_media/input_media_video.py` & `pylogram-0.5.0/pylogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_media/input_phone_contact.py` & `pylogram-0.5.0/pylogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_message_content/__init__.py` & `pylogram-0.5.0/pylogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_message_content/input_message_content.py` & `pylogram-0.5.0/pylogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/input_message_content/input_text_message_content.py` & `pylogram-0.5.0/pylogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/__init__.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/animation.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/audio.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/contact.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/dice.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/document.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/game.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/location.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/message.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/message_entity.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/message_reactions.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/photo.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/poll.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/poll_option.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/reaction.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/sticker.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/stripped_thumbnail.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/thumbnail.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/venue.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/video.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/video_note.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/voice.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/web_app_data.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/messages_and_media/web_page.py` & `pylogram-0.5.0/pylogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/__init__.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_event.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_event_filter.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_invite_link.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_join_request.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_joiner.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_member.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_member_updated.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_permissions.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_photo.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_preview.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_privileges.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/chat_reactions.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/dialog.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/emoji_status.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/invite_link_importer.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/restriction.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/user.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/username.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/video_chat_ended.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/video_chat_members_invited.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/video_chat_scheduled.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pylogram/types/user_and_chats/video_chat_started.py` & `pylogram-0.5.0/pylogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/.gitignore` & `pylogram-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/LICENSE` & `pylogram-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/NOTICE` & `pylogram-0.5.0/NOTICE`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/README.md` & `pylogram-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/hatch_build.py` & `pylogram-0.5.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/pyproject.toml` & `pylogram-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylogram-0.4.4/PKG-INFO` & `pylogram-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pylogram
-Version: 0.4.4
+Version: 0.5.0
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Project-URL: Source, https://github.com/pylakey/pylogram
 Project-URL: Homepage, https://github.com/pylakey/pylogram
 Author-email: Dan <dan@pyrogram.org>, Pylakey <pylakey@protonmail.com>
 Maintainer-email: Pylakey <pylakey@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

