# Comparing `tmp/openapiopenai-1.0.0-py3-none-any.whl.zip` & `tmp/openapiopenai-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,75 +1,265 @@
-Zip file size: 125406 bytes, number of entries: 73
--rw-r--r--  2.0 unx     6292 b- defN 24-Mar-16 07:22 openapiopenai/__init__.py
--rw-r--r--  2.0 unx    25774 b- defN 24-Mar-16 07:22 openapiopenai/api_client.py
--rw-r--r--  2.0 unx      652 b- defN 24-Mar-16 07:22 openapiopenai/api_response.py
--rw-r--r--  2.0 unx    14486 b- defN 24-Mar-16 07:22 openapiopenai/configuration.py
--rw-r--r--  2.0 unx     5961 b- defN 24-Mar-16 07:22 openapiopenai/exceptions.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-16 07:22 openapiopenai/py.typed
--rw-r--r--  2.0 unx     9220 b- defN 24-Mar-16 07:22 openapiopenai/rest.py
--rw-r--r--  2.0 unx      100 b- defN 24-Mar-16 07:22 openapiopenai/api/__init__.py
--rw-r--r--  2.0 unx   271073 b- defN 24-Mar-16 07:22 openapiopenai/api/open_ai_api.py
--rw-r--r--  2.0 unx     5705 b- defN 24-Mar-16 07:22 openapiopenai/models/__init__.py
--rw-r--r--  2.0 unx     3245 b- defN 24-Mar-16 07:22 openapiopenai/models/chat_completion_functions.py
--rw-r--r--  2.0 unx     4112 b- defN 24-Mar-16 07:22 openapiopenai/models/chat_completion_request_message.py
--rw-r--r--  2.0 unx     3115 b- defN 24-Mar-16 07:22 openapiopenai/models/chat_completion_request_message_function_call.py
--rw-r--r--  2.0 unx     3839 b- defN 24-Mar-16 07:22 openapiopenai/models/chat_completion_response_message.py
--rw-r--r--  2.0 unx     3937 b- defN 24-Mar-16 07:22 openapiopenai/models/chat_completion_stream_response_delta.py
--rw-r--r--  2.0 unx    11563 b- defN 24-Mar-16 07:22 openapiopenai/models/create_chat_completion_request.py
--rw-r--r--  2.0 unx     6371 b- defN 24-Mar-16 07:22 openapiopenai/models/create_chat_completion_request_function_call.py
--rw-r--r--  2.0 unx     2645 b- defN 24-Mar-16 07:22 openapiopenai/models/create_chat_completion_request_function_call_one_of.py
--rw-r--r--  2.0 unx     5455 b- defN 24-Mar-16 07:22 openapiopenai/models/create_chat_completion_request_model.py
--rw-r--r--  2.0 unx     5556 b- defN 24-Mar-16 07:22 openapiopenai/models/create_chat_completion_request_stop.py
--rw-r--r--  2.0 unx     3839 b- defN 24-Mar-16 07:22 openapiopenai/models/create_chat_completion_response.py
--rw-r--r--  2.0 unx     3553 b- defN 24-Mar-16 07:22 openapiopenai/models/create_chat_completion_response_choices_inner.py
--rw-r--r--  2.0 unx     3440 b- defN 24-Mar-16 07:22 openapiopenai/models/create_chat_completion_stream_response.py
--rw-r--r--  2.0 unx     3576 b- defN 24-Mar-16 07:22 openapiopenai/models/create_chat_completion_stream_response_choices_inner.py
--rw-r--r--  2.0 unx    13317 b- defN 24-Mar-16 07:22 openapiopenai/models/create_completion_request.py
--rw-r--r--  2.0 unx     5469 b- defN 24-Mar-16 07:22 openapiopenai/models/create_completion_request_model.py
--rw-r--r--  2.0 unx     7599 b- defN 24-Mar-16 07:22 openapiopenai/models/create_completion_request_prompt.py
--rw-r--r--  2.0 unx     5705 b- defN 24-Mar-16 07:22 openapiopenai/models/create_completion_request_stop.py
--rw-r--r--  2.0 unx     3806 b- defN 24-Mar-16 07:22 openapiopenai/models/create_completion_response.py
--rw-r--r--  2.0 unx     3761 b- defN 24-Mar-16 07:22 openapiopenai/models/create_completion_response_choices_inner.py
--rw-r--r--  2.0 unx     3042 b- defN 24-Mar-16 07:22 openapiopenai/models/create_completion_response_choices_inner_logprobs.py
--rw-r--r--  2.0 unx     2771 b- defN 24-Mar-16 07:22 openapiopenai/models/create_completion_response_usage.py
--rw-r--r--  2.0 unx     5373 b- defN 24-Mar-16 07:22 openapiopenai/models/create_edit_request.py
--rw-r--r--  2.0 unx     5338 b- defN 24-Mar-16 07:22 openapiopenai/models/create_edit_request_model.py
--rw-r--r--  2.0 unx     3605 b- defN 24-Mar-16 07:22 openapiopenai/models/create_edit_response.py
--rw-r--r--  2.0 unx     3847 b- defN 24-Mar-16 07:22 openapiopenai/models/create_edit_response_choices_inner.py
--rw-r--r--  2.0 unx     3546 b- defN 24-Mar-16 07:22 openapiopenai/models/create_embedding_request.py
--rw-r--r--  2.0 unx     7569 b- defN 24-Mar-16 07:22 openapiopenai/models/create_embedding_request_input.py
--rw-r--r--  2.0 unx     5462 b- defN 24-Mar-16 07:22 openapiopenai/models/create_embedding_request_model.py
--rw-r--r--  2.0 unx     3583 b- defN 24-Mar-16 07:22 openapiopenai/models/create_embedding_response.py
--rw-r--r--  2.0 unx     2752 b- defN 24-Mar-16 07:22 openapiopenai/models/create_embedding_response_data_inner.py
--rw-r--r--  2.0 unx     2650 b- defN 24-Mar-16 07:22 openapiopenai/models/create_embedding_response_usage.py
--rw-r--r--  2.0 unx    11600 b- defN 24-Mar-16 07:22 openapiopenai/models/create_fine_tune_request.py
--rw-r--r--  2.0 unx     5626 b- defN 24-Mar-16 07:22 openapiopenai/models/create_fine_tune_request_model.py
--rw-r--r--  2.0 unx     5018 b- defN 24-Mar-16 07:22 openapiopenai/models/create_image_request.py
--rw-r--r--  2.0 unx     3282 b- defN 24-Mar-16 07:22 openapiopenai/models/create_moderation_request.py
--rw-r--r--  2.0 unx     5404 b- defN 24-Mar-16 07:22 openapiopenai/models/create_moderation_request_input.py
--rw-r--r--  2.0 unx     5703 b- defN 24-Mar-16 07:22 openapiopenai/models/create_moderation_request_model.py
--rw-r--r--  2.0 unx     3197 b- defN 24-Mar-16 07:22 openapiopenai/models/create_moderation_response.py
--rw-r--r--  2.0 unx     3697 b- defN 24-Mar-16 07:22 openapiopenai/models/create_moderation_response_results_inner.py
--rw-r--r--  2.0 unx     3296 b- defN 24-Mar-16 07:22 openapiopenai/models/create_moderation_response_results_inner_categories.py
--rw-r--r--  2.0 unx     3464 b- defN 24-Mar-16 07:22 openapiopenai/models/create_moderation_response_results_inner_category_scores.py
--rw-r--r--  2.0 unx     5350 b- defN 24-Mar-16 07:22 openapiopenai/models/create_transcription_request_model.py
--rw-r--r--  2.0 unx     2513 b- defN 24-Mar-16 07:22 openapiopenai/models/create_transcription_response.py
--rw-r--r--  2.0 unx     2505 b- defN 24-Mar-16 07:22 openapiopenai/models/create_translation_response.py
--rw-r--r--  2.0 unx     2632 b- defN 24-Mar-16 07:22 openapiopenai/models/delete_file_response.py
--rw-r--r--  2.0 unx     2636 b- defN 24-Mar-16 07:22 openapiopenai/models/delete_model_response.py
--rw-r--r--  2.0 unx     3068 b- defN 24-Mar-16 07:22 openapiopenai/models/error.py
--rw-r--r--  2.0 unx     2703 b- defN 24-Mar-16 07:22 openapiopenai/models/error_response.py
--rw-r--r--  2.0 unx     5631 b- defN 24-Mar-16 07:22 openapiopenai/models/fine_tune.py
--rw-r--r--  2.0 unx     2711 b- defN 24-Mar-16 07:22 openapiopenai/models/fine_tune_event.py
--rw-r--r--  2.0 unx     3028 b- defN 24-Mar-16 07:22 openapiopenai/models/images_response.py
--rw-r--r--  2.0 unx     2618 b- defN 24-Mar-16 07:22 openapiopenai/models/images_response_data_inner.py
--rw-r--r--  2.0 unx     2983 b- defN 24-Mar-16 07:22 openapiopenai/models/list_files_response.py
--rw-r--r--  2.0 unx     3031 b- defN 24-Mar-16 07:22 openapiopenai/models/list_fine_tune_events_response.py
--rw-r--r--  2.0 unx     2990 b- defN 24-Mar-16 07:22 openapiopenai/models/list_fine_tunes_response.py
--rw-r--r--  2.0 unx     2965 b- defN 24-Mar-16 07:22 openapiopenai/models/list_models_response.py
--rw-r--r--  2.0 unx     2659 b- defN 24-Mar-16 07:22 openapiopenai/models/model.py
--rw-r--r--  2.0 unx     3303 b- defN 24-Mar-16 07:22 openapiopenai/models/open_ai_file.py
--rw-r--r--  2.0 unx      518 b- defN 24-Mar-16 07:22 openapiopenai-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-16 07:22 openapiopenai-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Mar-16 07:22 openapiopenai-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7676 b- defN 24-Mar-16 07:22 openapiopenai-1.0.0.dist-info/RECORD
-73 files, 604617 bytes uncompressed, 112692 bytes compressed:  81.4%
+Zip file size: 460754 bytes, number of entries: 263
+-rw-r--r--  2.0 unx    25243 b- defN 24-Apr-15 14:28 openapiopenai/__init__.py
+-rw-r--r--  2.0 unx    25816 b- defN 24-Apr-15 14:28 openapiopenai/api_client.py
+-rw-r--r--  2.0 unx      652 b- defN 24-Apr-15 14:28 openapiopenai/api_response.py
+-rw-r--r--  2.0 unx    14794 b- defN 24-Apr-15 14:28 openapiopenai/configuration.py
+-rw-r--r--  2.0 unx     6003 b- defN 24-Apr-15 14:28 openapiopenai/exceptions.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-15 14:28 openapiopenai/py.typed
+-rw-r--r--  2.0 unx     9262 b- defN 24-Apr-15 14:28 openapiopenai/rest.py
+-rw-r--r--  2.0 unx      595 b- defN 24-Apr-15 14:28 openapiopenai/api/__init__.py
+-rw-r--r--  2.0 unx   348085 b- defN 24-Apr-15 14:28 openapiopenai/api/assistants_api.py
+-rw-r--r--  2.0 unx    51057 b- defN 24-Apr-15 14:28 openapiopenai/api/audio_api.py
+-rw-r--r--  2.0 unx    11934 b- defN 24-Apr-15 14:28 openapiopenai/api/chat_api.py
+-rw-r--r--  2.0 unx    11758 b- defN 24-Apr-15 14:28 openapiopenai/api/completions_api.py
+-rw-r--r--  2.0 unx    11704 b- defN 24-Apr-15 14:28 openapiopenai/api/embeddings_api.py
+-rw-r--r--  2.0 unx    55024 b- defN 24-Apr-15 14:28 openapiopenai/api/files_api.py
+-rw-r--r--  2.0 unx    68656 b- defN 24-Apr-15 14:28 openapiopenai/api/fine_tuning_api.py
+-rw-r--r--  2.0 unx    48258 b- defN 24-Apr-15 14:28 openapiopenai/api/images_api.py
+-rw-r--r--  2.0 unx    30486 b- defN 24-Apr-15 14:28 openapiopenai/api/models_api.py
+-rw-r--r--  2.0 unx    11704 b- defN 24-Apr-15 14:28 openapiopenai/api/moderations_api.py
+-rw-r--r--  2.0 unx    24161 b- defN 24-Apr-15 14:28 openapiopenai/models/__init__.py
+-rw-r--r--  2.0 unx     3438 b- defN 24-Apr-15 14:27 openapiopenai/models/assistant_file_object.py
+-rw-r--r--  2.0 unx     6668 b- defN 24-Apr-15 14:27 openapiopenai/models/assistant_object.py
+-rw-r--r--  2.0 unx     6568 b- defN 24-Apr-15 14:27 openapiopenai/models/assistant_object_tools_inner.py
+-rw-r--r--  2.0 unx     9384 b- defN 24-Apr-15 14:27 openapiopenai/models/assistant_stream_event.py
+-rw-r--r--  2.0 unx     2872 b- defN 24-Apr-15 14:27 openapiopenai/models/assistant_tools_code.py
+-rw-r--r--  2.0 unx     3250 b- defN 24-Apr-15 14:27 openapiopenai/models/assistant_tools_function.py
+-rw-r--r--  2.0 unx     2871 b- defN 24-Apr-15 14:27 openapiopenai/models/assistant_tools_retrieval.py
+-rw-r--r--  2.0 unx     3553 b- defN 24-Apr-15 14:27 openapiopenai/models/assistants_api_named_tool_choice.py
+-rw-r--r--  2.0 unx     3202 b- defN 24-Apr-15 14:27 openapiopenai/models/assistants_api_response_format.py
+-rw-r--r--  2.0 unx     6522 b- defN 24-Apr-15 14:27 openapiopenai/models/assistants_api_response_format_option.py
+-rw-r--r--  2.0 unx     6250 b- defN 24-Apr-15 14:27 openapiopenai/models/assistants_api_tool_choice_option.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_function_call_option.py
+-rw-r--r--  2.0 unx     3433 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_functions.py
+-rw-r--r--  2.0 unx     3499 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_message_tool_call.py
+-rw-r--r--  2.0 unx     3747 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_message_tool_call_chunk.py
+-rw-r--r--  2.0 unx     3119 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_message_tool_call_chunk_function.py
+-rw-r--r--  2.0 unx     3039 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_message_tool_call_function.py
+-rw-r--r--  2.0 unx     3455 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_named_tool_choice.py
+-rw-r--r--  2.0 unx     2659 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_named_tool_choice_function.py
+-rw-r--r--  2.0 unx     4963 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_assistant_message.py
+-rw-r--r--  2.0 unx     3167 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_assistant_message_function_call.py
+-rw-r--r--  2.0 unx     3426 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_function_message.py
+-rw-r--r--  2.0 unx     9484 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_message.py
+-rw-r--r--  2.0 unx     6573 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_message_content_part.py
+-rw-r--r--  2.0 unx     3495 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_message_content_part_image.py
+-rw-r--r--  2.0 unx     3389 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_message_content_part_image_image_url.py
+-rw-r--r--  2.0 unx     3033 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_message_content_part_text.py
+-rw-r--r--  2.0 unx     3304 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_system_message.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_tool_message.py
+-rw-r--r--  2.0 unx     3635 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_user_message.py
+-rw-r--r--  2.0 unx     6506 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_request_user_message_content.py
+-rw-r--r--  2.0 unx     4608 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_response_message.py
+-rw-r--r--  2.0 unx      883 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_role.py
+-rw-r--r--  2.0 unx     4693 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_stream_response_delta.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_stream_response_delta_function_call.py
+-rw-r--r--  2.0 unx     4439 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_token_logprob.py
+-rw-r--r--  2.0 unx     3604 b- defN 24-Apr-15 14:27 openapiopenai/models/chat_completion_token_logprob_top_logprobs_inner.py
+-rw-r--r--  2.0 unx     3254 b- defN 24-Apr-15 14:28 openapiopenai/models/chat_completion_tool.py
+-rw-r--r--  2.0 unx     6336 b- defN 24-Apr-15 14:28 openapiopenai/models/chat_completion_tool_choice_option.py
+-rw-r--r--  2.0 unx     3006 b- defN 24-Apr-15 14:28 openapiopenai/models/completion_usage.py
+-rw-r--r--  2.0 unx     2775 b- defN 24-Apr-15 14:28 openapiopenai/models/create_assistant_file_request.py
+-rw-r--r--  2.0 unx     6133 b- defN 24-Apr-15 14:28 openapiopenai/models/create_assistant_request.py
+-rw-r--r--  2.0 unx     5089 b- defN 24-Apr-15 14:28 openapiopenai/models/create_assistant_request_model.py
+-rw-r--r--  2.0 unx     5017 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_function_response.py
+-rw-r--r--  2.0 unx     3997 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_function_response_choices_inner.py
+-rw-r--r--  2.0 unx    15719 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_request.py
+-rw-r--r--  2.0 unx     6449 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_request_function_call.py
+-rw-r--r--  2.0 unx     5072 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_request_model.py
+-rw-r--r--  2.0 unx     3868 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_request_response_format.py
+-rw-r--r--  2.0 unx     5598 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_request_stop.py
+-rw-r--r--  2.0 unx     4960 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_response.py
+-rw-r--r--  2.0 unx     4809 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_response_choices_inner.py
+-rw-r--r--  2.0 unx     3480 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_response_choices_inner_logprobs.py
+-rw-r--r--  2.0 unx     4721 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_stream_response.py
+-rw-r--r--  2.0 unx     5136 b- defN 24-Apr-15 14:28 openapiopenai/models/create_chat_completion_stream_response_choices_inner.py
+-rw-r--r--  2.0 unx    14071 b- defN 24-Apr-15 14:28 openapiopenai/models/create_completion_request.py
+-rw-r--r--  2.0 unx     5094 b- defN 24-Apr-15 14:28 openapiopenai/models/create_completion_request_model.py
+-rw-r--r--  2.0 unx     7641 b- defN 24-Apr-15 14:28 openapiopenai/models/create_completion_request_prompt.py
+-rw-r--r--  2.0 unx     5747 b- defN 24-Apr-15 14:28 openapiopenai/models/create_completion_request_stop.py
+-rw-r--r--  2.0 unx     4973 b- defN 24-Apr-15 14:28 openapiopenai/models/create_completion_response.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-Apr-15 14:28 openapiopenai/models/create_completion_response_choices_inner.py
+-rw-r--r--  2.0 unx     3110 b- defN 24-Apr-15 14:28 openapiopenai/models/create_completion_response_choices_inner_logprobs.py
+-rw-r--r--  2.0 unx     4592 b- defN 24-Apr-15 14:28 openapiopenai/models/create_embedding_request.py
+-rw-r--r--  2.0 unx     8107 b- defN 24-Apr-15 14:28 openapiopenai/models/create_embedding_request_input.py
+-rw-r--r--  2.0 unx     5089 b- defN 24-Apr-15 14:28 openapiopenai/models/create_embedding_request_model.py
+-rw-r--r--  2.0 unx     4001 b- defN 24-Apr-15 14:28 openapiopenai/models/create_embedding_response.py
+-rw-r--r--  2.0 unx     2844 b- defN 24-Apr-15 14:28 openapiopenai/models/create_embedding_response_usage.py
+-rw-r--r--  2.0 unx     7102 b- defN 24-Apr-15 14:28 openapiopenai/models/create_fine_tuning_job_request.py
+-rw-r--r--  2.0 unx     4419 b- defN 24-Apr-15 14:28 openapiopenai/models/create_fine_tuning_job_request_hyperparameters.py
+-rw-r--r--  2.0 unx     5719 b- defN 24-Apr-15 14:28 openapiopenai/models/create_fine_tuning_job_request_hyperparameters_batch_size.py
+-rw-r--r--  2.0 unx     5844 b- defN 24-Apr-15 14:28 openapiopenai/models/create_fine_tuning_job_request_hyperparameters_learning_rate_multiplier.py
+-rw-r--r--  2.0 unx     5677 b- defN 24-Apr-15 14:28 openapiopenai/models/create_fine_tuning_job_request_hyperparameters_n_epochs.py
+-rw-r--r--  2.0 unx     3532 b- defN 24-Apr-15 14:28 openapiopenai/models/create_fine_tuning_job_request_integrations_inner.py
+-rw-r--r--  2.0 unx     4866 b- defN 24-Apr-15 14:28 openapiopenai/models/create_fine_tuning_job_request_integrations_inner_type.py
+-rw-r--r--  2.0 unx     4270 b- defN 24-Apr-15 14:28 openapiopenai/models/create_fine_tuning_job_request_integrations_inner_wandb.py
+-rw-r--r--  2.0 unx     5042 b- defN 24-Apr-15 14:28 openapiopenai/models/create_fine_tuning_job_request_model.py
+-rw-r--r--  2.0 unx     5067 b- defN 24-Apr-15 14:28 openapiopenai/models/create_image_edit_request_model.py
+-rw-r--r--  2.0 unx     7606 b- defN 24-Apr-15 14:28 openapiopenai/models/create_image_request.py
+-rw-r--r--  2.0 unx     5004 b- defN 24-Apr-15 14:28 openapiopenai/models/create_image_request_model.py
+-rw-r--r--  2.0 unx     4422 b- defN 24-Apr-15 14:28 openapiopenai/models/create_message_request.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Apr-15 14:28 openapiopenai/models/create_moderation_request.py
+-rw-r--r--  2.0 unx     5446 b- defN 24-Apr-15 14:28 openapiopenai/models/create_moderation_request_input.py
+-rw-r--r--  2.0 unx     5328 b- defN 24-Apr-15 14:28 openapiopenai/models/create_moderation_request_model.py
+-rw-r--r--  2.0 unx     3478 b- defN 24-Apr-15 14:28 openapiopenai/models/create_moderation_response.py
+-rw-r--r--  2.0 unx     3818 b- defN 24-Apr-15 14:28 openapiopenai/models/create_moderation_response_results_inner.py
+-rw-r--r--  2.0 unx     5537 b- defN 24-Apr-15 14:28 openapiopenai/models/create_moderation_response_results_inner_categories.py
+-rw-r--r--  2.0 unx     4877 b- defN 24-Apr-15 14:28 openapiopenai/models/create_moderation_response_results_inner_category_scores.py
+-rw-r--r--  2.0 unx    11473 b- defN 24-Apr-15 14:28 openapiopenai/models/create_run_request.py
+-rw-r--r--  2.0 unx     5186 b- defN 24-Apr-15 14:28 openapiopenai/models/create_run_request_model.py
+-rw-r--r--  2.0 unx     4822 b- defN 24-Apr-15 14:28 openapiopenai/models/create_speech_request.py
+-rw-r--r--  2.0 unx     4944 b- defN 24-Apr-15 14:28 openapiopenai/models/create_speech_request_model.py
+-rw-r--r--  2.0 unx    10233 b- defN 24-Apr-15 14:28 openapiopenai/models/create_thread_and_run_request.py
+-rw-r--r--  2.0 unx     6648 b- defN 24-Apr-15 14:28 openapiopenai/models/create_thread_and_run_request_tools_inner.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-15 14:28 openapiopenai/models/create_thread_request.py
+-rw-r--r--  2.0 unx     6190 b- defN 24-Apr-15 14:28 openapiopenai/models/create_transcription200_response.py
+-rw-r--r--  2.0 unx     5024 b- defN 24-Apr-15 14:28 openapiopenai/models/create_transcription_request_model.py
+-rw-r--r--  2.0 unx     2675 b- defN 24-Apr-15 14:28 openapiopenai/models/create_transcription_response_json.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-Apr-15 14:28 openapiopenai/models/create_transcription_response_verbose_json.py
+-rw-r--r--  2.0 unx     6106 b- defN 24-Apr-15 14:28 openapiopenai/models/create_translation200_response.py
+-rw-r--r--  2.0 unx     2563 b- defN 24-Apr-15 14:28 openapiopenai/models/create_translation_response_json.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-Apr-15 14:28 openapiopenai/models/create_translation_response_verbose_json.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-15 14:28 openapiopenai/models/delete_assistant_file_response.py
+-rw-r--r--  2.0 unx     2972 b- defN 24-Apr-15 14:28 openapiopenai/models/delete_assistant_response.py
+-rw-r--r--  2.0 unx     2926 b- defN 24-Apr-15 14:28 openapiopenai/models/delete_file_response.py
+-rw-r--r--  2.0 unx     2974 b- defN 24-Apr-15 14:28 openapiopenai/models/delete_message_response.py
+-rw-r--r--  2.0 unx     2678 b- defN 24-Apr-15 14:28 openapiopenai/models/delete_model_response.py
+-rw-r--r--  2.0 unx     2954 b- defN 24-Apr-15 14:28 openapiopenai/models/delete_thread_response.py
+-rw-r--r--  2.0 unx     3054 b- defN 24-Apr-15 14:28 openapiopenai/models/done_event.py
+-rw-r--r--  2.0 unx     3349 b- defN 24-Apr-15 14:28 openapiopenai/models/embedding.py
+-rw-r--r--  2.0 unx     3110 b- defN 24-Apr-15 14:28 openapiopenai/models/error.py
+-rw-r--r--  2.0 unx     3175 b- defN 24-Apr-15 14:28 openapiopenai/models/error_event.py
+-rw-r--r--  2.0 unx     2745 b- defN 24-Apr-15 14:28 openapiopenai/models/error_response.py
+-rw-r--r--  2.0 unx     3378 b- defN 24-Apr-15 14:28 openapiopenai/models/fine_tuning_integration.py
+-rw-r--r--  2.0 unx     9097 b- defN 24-Apr-15 14:28 openapiopenai/models/fine_tuning_job.py
+-rw-r--r--  2.0 unx     4442 b- defN 24-Apr-15 14:28 openapiopenai/models/fine_tuning_job_checkpoint.py
+-rw-r--r--  2.0 unx     3634 b- defN 24-Apr-15 14:28 openapiopenai/models/fine_tuning_job_checkpoint_metrics.py
+-rw-r--r--  2.0 unx     3258 b- defN 24-Apr-15 14:28 openapiopenai/models/fine_tuning_job_error.py
+-rw-r--r--  2.0 unx     3393 b- defN 24-Apr-15 14:28 openapiopenai/models/fine_tuning_job_event.py
+-rw-r--r--  2.0 unx     3050 b- defN 24-Apr-15 14:28 openapiopenai/models/fine_tuning_job_hyperparameters.py
+-rw-r--r--  2.0 unx     5744 b- defN 24-Apr-15 14:28 openapiopenai/models/fine_tuning_job_hyperparameters_n_epochs.py
+-rw-r--r--  2.0 unx     4848 b- defN 24-Apr-15 14:28 openapiopenai/models/fine_tuning_job_integrations_inner.py
+-rw-r--r--  2.0 unx     3397 b- defN 24-Apr-15 14:28 openapiopenai/models/function_object.py
+-rw-r--r--  2.0 unx     3122 b- defN 24-Apr-15 14:28 openapiopenai/models/image.py
+-rw-r--r--  2.0 unx     2995 b- defN 24-Apr-15 14:28 openapiopenai/models/images_response.py
+-rw-r--r--  2.0 unx     3349 b- defN 24-Apr-15 14:28 openapiopenai/models/list_assistant_files_response.py
+-rw-r--r--  2.0 unx     3316 b- defN 24-Apr-15 14:28 openapiopenai/models/list_assistants_response.py
+-rw-r--r--  2.0 unx     3277 b- defN 24-Apr-15 14:28 openapiopenai/models/list_files_response.py
+-rw-r--r--  2.0 unx     4128 b- defN 24-Apr-15 14:28 openapiopenai/models/list_fine_tuning_job_checkpoints_response.py
+-rw-r--r--  2.0 unx     3366 b- defN 24-Apr-15 14:28 openapiopenai/models/list_fine_tuning_job_events_response.py
+-rw-r--r--  2.0 unx     3333 b- defN 24-Apr-15 14:28 openapiopenai/models/list_message_files_response.py
+-rw-r--r--  2.0 unx     3300 b- defN 24-Apr-15 14:28 openapiopenai/models/list_messages_response.py
+-rw-r--r--  2.0 unx     3259 b- defN 24-Apr-15 14:28 openapiopenai/models/list_models_response.py
+-rw-r--r--  2.0 unx     3455 b- defN 24-Apr-15 14:28 openapiopenai/models/list_paginated_fine_tuning_jobs_response.py
+-rw-r--r--  2.0 unx     3301 b- defN 24-Apr-15 14:28 openapiopenai/models/list_run_steps_response.py
+-rw-r--r--  2.0 unx     3268 b- defN 24-Apr-15 14:28 openapiopenai/models/list_runs_response.py
+-rw-r--r--  2.0 unx     3292 b- defN 24-Apr-15 14:28 openapiopenai/models/list_threads_response.py
+-rw-r--r--  2.0 unx     3432 b- defN 24-Apr-15 14:28 openapiopenai/models/message_content_image_file_object.py
+-rw-r--r--  2.0 unx     2719 b- defN 24-Apr-15 14:28 openapiopenai/models/message_content_image_file_object_image_file.py
+-rw-r--r--  2.0 unx     4155 b- defN 24-Apr-15 14:28 openapiopenai/models/message_content_text_annotations_file_citation_object.py
+-rw-r--r--  2.0 unx     2899 b- defN 24-Apr-15 14:28 openapiopenai/models/message_content_text_annotations_file_citation_object_file_citation.py
+-rw-r--r--  2.0 unx     3968 b- defN 24-Apr-15 14:28 openapiopenai/models/message_content_text_annotations_file_path_object.py
+-rw-r--r--  2.0 unx     2732 b- defN 24-Apr-15 14:28 openapiopenai/models/message_content_text_annotations_file_path_object_file_path.py
+-rw-r--r--  2.0 unx     3264 b- defN 24-Apr-15 14:28 openapiopenai/models/message_content_text_object.py
+-rw-r--r--  2.0 unx     3331 b- defN 24-Apr-15 14:28 openapiopenai/models/message_content_text_object_text.py
+-rw-r--r--  2.0 unx     6664 b- defN 24-Apr-15 14:28 openapiopenai/models/message_content_text_object_text_annotations_inner.py
+-rw-r--r--  2.0 unx     3644 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_content_image_file_object.py
+-rw-r--r--  2.0 unx     2773 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_content_image_file_object_image_file.py
+-rw-r--r--  2.0 unx     4433 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_content_text_annotations_file_citation_object.py
+-rw-r--r--  2.0 unx     2977 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_content_text_annotations_file_citation_object_file_citation.py
+-rw-r--r--  2.0 unx     4246 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_content_text_annotations_file_path_object.py
+-rw-r--r--  2.0 unx     2786 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_content_text_annotations_file_path_object_file_path.py
+-rw-r--r--  2.0 unx     3476 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_content_text_object.py
+-rw-r--r--  2.0 unx     3423 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_content_text_object_text.py
+-rw-r--r--  2.0 unx     6876 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_content_text_object_text_annotations_inner.py
+-rw-r--r--  2.0 unx     3512 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_object.py
+-rw-r--r--  2.0 unx     4191 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_object_delta.py
+-rw-r--r--  2.0 unx     6130 b- defN 24-Apr-15 14:28 openapiopenai/models/message_delta_object_delta_content_inner.py
+-rw-r--r--  2.0 unx     3471 b- defN 24-Apr-15 14:28 openapiopenai/models/message_file_object.py
+-rw-r--r--  2.0 unx     8642 b- defN 24-Apr-15 14:28 openapiopenai/models/message_object.py
+-rw-r--r--  2.0 unx     5878 b- defN 24-Apr-15 14:28 openapiopenai/models/message_object_content_inner.py
+-rw-r--r--  2.0 unx     3075 b- defN 24-Apr-15 14:28 openapiopenai/models/message_object_incomplete_details.py
+-rw-r--r--  2.0 unx     8520 b- defN 24-Apr-15 14:28 openapiopenai/models/message_stream_event.py
+-rw-r--r--  2.0 unx     3224 b- defN 24-Apr-15 14:28 openapiopenai/models/message_stream_event_one_of.py
+-rw-r--r--  2.0 unx     3256 b- defN 24-Apr-15 14:28 openapiopenai/models/message_stream_event_one_of1.py
+-rw-r--r--  2.0 unx     3261 b- defN 24-Apr-15 14:28 openapiopenai/models/message_stream_event_one_of2.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-Apr-15 14:28 openapiopenai/models/message_stream_event_one_of3.py
+-rw-r--r--  2.0 unx     3250 b- defN 24-Apr-15 14:28 openapiopenai/models/message_stream_event_one_of4.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Apr-15 14:28 openapiopenai/models/model.py
+-rw-r--r--  2.0 unx     5925 b- defN 24-Apr-15 14:28 openapiopenai/models/modify_assistant_request.py
+-rw-r--r--  2.0 unx     3068 b- defN 24-Apr-15 14:28 openapiopenai/models/modify_message_request.py
+-rw-r--r--  2.0 unx     3052 b- defN 24-Apr-15 14:28 openapiopenai/models/modify_run_request.py
+-rw-r--r--  2.0 unx     3064 b- defN 24-Apr-15 14:28 openapiopenai/models/modify_thread_request.py
+-rw-r--r--  2.0 unx     4819 b- defN 24-Apr-15 14:28 openapiopenai/models/open_ai_file.py
+-rw-r--r--  2.0 unx     3134 b- defN 24-Apr-15 14:28 openapiopenai/models/run_completion_usage.py
+-rw-r--r--  2.0 unx    14169 b- defN 24-Apr-15 14:28 openapiopenai/models/run_object.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-Apr-15 14:28 openapiopenai/models/run_object_incomplete_details.py
+-rw-r--r--  2.0 unx     3166 b- defN 24-Apr-15 14:28 openapiopenai/models/run_object_last_error.py
+-rw-r--r--  2.0 unx     3557 b- defN 24-Apr-15 14:28 openapiopenai/models/run_object_required_action.py
+-rw-r--r--  2.0 unx     3201 b- defN 24-Apr-15 14:28 openapiopenai/models/run_object_required_action_submit_tool_outputs.py
+-rw-r--r--  2.0 unx     3131 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_completion_usage.py
+-rw-r--r--  2.0 unx     3519 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_object.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_object_delta.py
+-rw-r--r--  2.0 unx     6444 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_object_delta_step_details.py
+-rw-r--r--  2.0 unx     3629 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_message_creation_object.py
+-rw-r--r--  2.0 unx     2828 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_message_creation_object_message_creation.py
+-rw-r--r--  2.0 unx     3993 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_code_object.py
+-rw-r--r--  2.0 unx     3794 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_code_object_code_interpreter.py
+-rw-r--r--  2.0 unx     7127 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_code_object_code_interpreter_outputs_inner.py
+-rw-r--r--  2.0 unx     3676 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_code_output_image_object.py
+-rw-r--r--  2.0 unx     2810 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_code_output_image_object_image.py
+-rw-r--r--  2.0 unx     3290 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_code_output_logs_object.py
+-rw-r--r--  2.0 unx     3878 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_function_object.py
+-rw-r--r--  2.0 unx     3381 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_function_object_function.py
+-rw-r--r--  2.0 unx     3846 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_object.py
+-rw-r--r--  2.0 unx     8026 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_object_tool_calls_inner.py
+-rw-r--r--  2.0 unx     3504 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_delta_step_details_tool_calls_retrieval_object.py
+-rw-r--r--  2.0 unx     3537 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_message_creation_object.py
+-rw-r--r--  2.0 unx     2758 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_message_creation_object_message_creation.py
+-rw-r--r--  2.0 unx     3722 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_code_object.py
+-rw-r--r--  2.0 unx     3671 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_code_object_code_interpreter.py
+-rw-r--r--  2.0 unx     6745 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_code_object_code_interpreter_outputs_inner.py
+-rw-r--r--  2.0 unx     3426 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_code_output_image_object.py
+-rw-r--r--  2.0 unx     2740 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_code_output_image_object_image.py
+-rw-r--r--  2.0 unx     3080 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_code_output_logs_object.py
+-rw-r--r--  2.0 unx     3598 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_function_object.py
+-rw-r--r--  2.0 unx     3292 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_function_object_function.py
+-rw-r--r--  2.0 unx     3747 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_object.py
+-rw-r--r--  2.0 unx     7489 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_object_tool_calls_inner.py
+-rw-r--r--  2.0 unx     3255 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_details_tool_calls_retrieval_object.py
+-rw-r--r--  2.0 unx     8854 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_object.py
+-rw-r--r--  2.0 unx     3128 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_object_last_error.py
+-rw-r--r--  2.0 unx     6064 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_object_step_details.py
+-rw-r--r--  2.0 unx    10393 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_stream_event.py
+-rw-r--r--  2.0 unx     3229 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_stream_event_one_of.py
+-rw-r--r--  2.0 unx     3261 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_stream_event_one_of1.py
+-rw-r--r--  2.0 unx     3266 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_stream_event_one_of2.py
+-rw-r--r--  2.0 unx     3238 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_stream_event_one_of3.py
+-rw-r--r--  2.0 unx     3225 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_stream_event_one_of4.py
+-rw-r--r--  2.0 unx     3238 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_stream_event_one_of5.py
+-rw-r--r--  2.0 unx     3229 b- defN 24-Apr-15 14:28 openapiopenai/models/run_step_stream_event_one_of6.py
+-rw-r--r--  2.0 unx    11608 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event.py
+-rw-r--r--  2.0 unx     3184 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event_one_of.py
+-rw-r--r--  2.0 unx     3197 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event_one_of1.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event_one_of2.py
+-rw-r--r--  2.0 unx     3224 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event_one_of3.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event_one_of4.py
+-rw-r--r--  2.0 unx     3176 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event_one_of5.py
+-rw-r--r--  2.0 unx     3209 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event_one_of6.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event_one_of7.py
+-rw-r--r--  2.0 unx     3180 b- defN 24-Apr-15 14:28 openapiopenai/models/run_stream_event_one_of8.py
+-rw-r--r--  2.0 unx     3581 b- defN 24-Apr-15 14:28 openapiopenai/models/run_tool_call_object.py
+-rw-r--r--  2.0 unx     2776 b- defN 24-Apr-15 14:28 openapiopenai/models/run_tool_call_object_function.py
+-rw-r--r--  2.0 unx     3798 b- defN 24-Apr-15 14:28 openapiopenai/models/submit_tool_outputs_run_request.py
+-rw-r--r--  2.0 unx     3013 b- defN 24-Apr-15 14:28 openapiopenai/models/submit_tool_outputs_run_request_tool_outputs_inner.py
+-rw-r--r--  2.0 unx     3817 b- defN 24-Apr-15 14:28 openapiopenai/models/thread_object.py
+-rw-r--r--  2.0 unx     4763 b- defN 24-Apr-15 14:28 openapiopenai/models/thread_stream_event.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-15 14:28 openapiopenai/models/thread_stream_event_one_of.py
+-rw-r--r--  2.0 unx     4247 b- defN 24-Apr-15 14:28 openapiopenai/models/transcription_segment.py
+-rw-r--r--  2.0 unx     2890 b- defN 24-Apr-15 14:28 openapiopenai/models/transcription_word.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-Apr-15 14:28 openapiopenai/models/truncation_object.py
+-rw-r--r--  2.0 unx      556 b- defN 24-Apr-15 14:28 openapiopenai-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 14:28 openapiopenai-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-15 14:28 openapiopenai-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    29608 b- defN 24-Apr-15 14:28 openapiopenai-1.1.0.dist-info/RECORD
+263 files, 1837616 bytes uncompressed, 411424 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -18,56 +18,206 @@
 
 Filename: openapiopenai/rest.py
 Comment: 
 
 Filename: openapiopenai/api/__init__.py
 Comment: 
 
-Filename: openapiopenai/api/open_ai_api.py
+Filename: openapiopenai/api/assistants_api.py
+Comment: 
+
+Filename: openapiopenai/api/audio_api.py
+Comment: 
+
+Filename: openapiopenai/api/chat_api.py
+Comment: 
+
+Filename: openapiopenai/api/completions_api.py
+Comment: 
+
+Filename: openapiopenai/api/embeddings_api.py
+Comment: 
+
+Filename: openapiopenai/api/files_api.py
+Comment: 
+
+Filename: openapiopenai/api/fine_tuning_api.py
+Comment: 
+
+Filename: openapiopenai/api/images_api.py
+Comment: 
+
+Filename: openapiopenai/api/models_api.py
+Comment: 
+
+Filename: openapiopenai/api/moderations_api.py
 Comment: 
 
 Filename: openapiopenai/models/__init__.py
 Comment: 
 
+Filename: openapiopenai/models/assistant_file_object.py
+Comment: 
+
+Filename: openapiopenai/models/assistant_object.py
+Comment: 
+
+Filename: openapiopenai/models/assistant_object_tools_inner.py
+Comment: 
+
+Filename: openapiopenai/models/assistant_stream_event.py
+Comment: 
+
+Filename: openapiopenai/models/assistant_tools_code.py
+Comment: 
+
+Filename: openapiopenai/models/assistant_tools_function.py
+Comment: 
+
+Filename: openapiopenai/models/assistant_tools_retrieval.py
+Comment: 
+
+Filename: openapiopenai/models/assistants_api_named_tool_choice.py
+Comment: 
+
+Filename: openapiopenai/models/assistants_api_response_format.py
+Comment: 
+
+Filename: openapiopenai/models/assistants_api_response_format_option.py
+Comment: 
+
+Filename: openapiopenai/models/assistants_api_tool_choice_option.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_function_call_option.py
+Comment: 
+
 Filename: openapiopenai/models/chat_completion_functions.py
 Comment: 
 
+Filename: openapiopenai/models/chat_completion_message_tool_call.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_message_tool_call_chunk.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_message_tool_call_chunk_function.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_message_tool_call_function.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_named_tool_choice.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_named_tool_choice_function.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_assistant_message.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_assistant_message_function_call.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_function_message.py
+Comment: 
+
 Filename: openapiopenai/models/chat_completion_request_message.py
 Comment: 
 
-Filename: openapiopenai/models/chat_completion_request_message_function_call.py
+Filename: openapiopenai/models/chat_completion_request_message_content_part.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_message_content_part_image.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_message_content_part_image_image_url.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_message_content_part_text.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_system_message.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_tool_message.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_user_message.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_request_user_message_content.py
 Comment: 
 
 Filename: openapiopenai/models/chat_completion_response_message.py
 Comment: 
 
+Filename: openapiopenai/models/chat_completion_role.py
+Comment: 
+
 Filename: openapiopenai/models/chat_completion_stream_response_delta.py
 Comment: 
 
+Filename: openapiopenai/models/chat_completion_stream_response_delta_function_call.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_token_logprob.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_token_logprob_top_logprobs_inner.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_tool.py
+Comment: 
+
+Filename: openapiopenai/models/chat_completion_tool_choice_option.py
+Comment: 
+
+Filename: openapiopenai/models/completion_usage.py
+Comment: 
+
+Filename: openapiopenai/models/create_assistant_file_request.py
+Comment: 
+
+Filename: openapiopenai/models/create_assistant_request.py
+Comment: 
+
+Filename: openapiopenai/models/create_assistant_request_model.py
+Comment: 
+
+Filename: openapiopenai/models/create_chat_completion_function_response.py
+Comment: 
+
+Filename: openapiopenai/models/create_chat_completion_function_response_choices_inner.py
+Comment: 
+
 Filename: openapiopenai/models/create_chat_completion_request.py
 Comment: 
 
 Filename: openapiopenai/models/create_chat_completion_request_function_call.py
 Comment: 
 
-Filename: openapiopenai/models/create_chat_completion_request_function_call_one_of.py
+Filename: openapiopenai/models/create_chat_completion_request_model.py
 Comment: 
 
-Filename: openapiopenai/models/create_chat_completion_request_model.py
+Filename: openapiopenai/models/create_chat_completion_request_response_format.py
 Comment: 
 
 Filename: openapiopenai/models/create_chat_completion_request_stop.py
 Comment: 
 
 Filename: openapiopenai/models/create_chat_completion_response.py
 Comment: 
 
 Filename: openapiopenai/models/create_chat_completion_response_choices_inner.py
 Comment: 
 
+Filename: openapiopenai/models/create_chat_completion_response_choices_inner_logprobs.py
+Comment: 
+
 Filename: openapiopenai/models/create_chat_completion_stream_response.py
 Comment: 
 
 Filename: openapiopenai/models/create_chat_completion_stream_response_choices_inner.py
 Comment: 
 
 Filename: openapiopenai/models/create_completion_request.py
@@ -87,56 +237,68 @@
 
 Filename: openapiopenai/models/create_completion_response_choices_inner.py
 Comment: 
 
 Filename: openapiopenai/models/create_completion_response_choices_inner_logprobs.py
 Comment: 
 
-Filename: openapiopenai/models/create_completion_response_usage.py
+Filename: openapiopenai/models/create_embedding_request.py
 Comment: 
 
-Filename: openapiopenai/models/create_edit_request.py
+Filename: openapiopenai/models/create_embedding_request_input.py
 Comment: 
 
-Filename: openapiopenai/models/create_edit_request_model.py
+Filename: openapiopenai/models/create_embedding_request_model.py
 Comment: 
 
-Filename: openapiopenai/models/create_edit_response.py
+Filename: openapiopenai/models/create_embedding_response.py
 Comment: 
 
-Filename: openapiopenai/models/create_edit_response_choices_inner.py
+Filename: openapiopenai/models/create_embedding_response_usage.py
 Comment: 
 
-Filename: openapiopenai/models/create_embedding_request.py
+Filename: openapiopenai/models/create_fine_tuning_job_request.py
 Comment: 
 
-Filename: openapiopenai/models/create_embedding_request_input.py
+Filename: openapiopenai/models/create_fine_tuning_job_request_hyperparameters.py
 Comment: 
 
-Filename: openapiopenai/models/create_embedding_request_model.py
+Filename: openapiopenai/models/create_fine_tuning_job_request_hyperparameters_batch_size.py
 Comment: 
 
-Filename: openapiopenai/models/create_embedding_response.py
+Filename: openapiopenai/models/create_fine_tuning_job_request_hyperparameters_learning_rate_multiplier.py
 Comment: 
 
-Filename: openapiopenai/models/create_embedding_response_data_inner.py
+Filename: openapiopenai/models/create_fine_tuning_job_request_hyperparameters_n_epochs.py
 Comment: 
 
-Filename: openapiopenai/models/create_embedding_response_usage.py
+Filename: openapiopenai/models/create_fine_tuning_job_request_integrations_inner.py
+Comment: 
+
+Filename: openapiopenai/models/create_fine_tuning_job_request_integrations_inner_type.py
 Comment: 
 
-Filename: openapiopenai/models/create_fine_tune_request.py
+Filename: openapiopenai/models/create_fine_tuning_job_request_integrations_inner_wandb.py
 Comment: 
 
-Filename: openapiopenai/models/create_fine_tune_request_model.py
+Filename: openapiopenai/models/create_fine_tuning_job_request_model.py
+Comment: 
+
+Filename: openapiopenai/models/create_image_edit_request_model.py
 Comment: 
 
 Filename: openapiopenai/models/create_image_request.py
 Comment: 
 
+Filename: openapiopenai/models/create_image_request_model.py
+Comment: 
+
+Filename: openapiopenai/models/create_message_request.py
+Comment: 
+
 Filename: openapiopenai/models/create_moderation_request.py
 Comment: 
 
 Filename: openapiopenai/models/create_moderation_request_input.py
 Comment: 
 
 Filename: openapiopenai/models/create_moderation_request_model.py
@@ -150,71 +312,479 @@
 
 Filename: openapiopenai/models/create_moderation_response_results_inner_categories.py
 Comment: 
 
 Filename: openapiopenai/models/create_moderation_response_results_inner_category_scores.py
 Comment: 
 
+Filename: openapiopenai/models/create_run_request.py
+Comment: 
+
+Filename: openapiopenai/models/create_run_request_model.py
+Comment: 
+
+Filename: openapiopenai/models/create_speech_request.py
+Comment: 
+
+Filename: openapiopenai/models/create_speech_request_model.py
+Comment: 
+
+Filename: openapiopenai/models/create_thread_and_run_request.py
+Comment: 
+
+Filename: openapiopenai/models/create_thread_and_run_request_tools_inner.py
+Comment: 
+
+Filename: openapiopenai/models/create_thread_request.py
+Comment: 
+
+Filename: openapiopenai/models/create_transcription200_response.py
+Comment: 
+
 Filename: openapiopenai/models/create_transcription_request_model.py
 Comment: 
 
-Filename: openapiopenai/models/create_transcription_response.py
+Filename: openapiopenai/models/create_transcription_response_json.py
+Comment: 
+
+Filename: openapiopenai/models/create_transcription_response_verbose_json.py
+Comment: 
+
+Filename: openapiopenai/models/create_translation200_response.py
+Comment: 
+
+Filename: openapiopenai/models/create_translation_response_json.py
+Comment: 
+
+Filename: openapiopenai/models/create_translation_response_verbose_json.py
 Comment: 
 
-Filename: openapiopenai/models/create_translation_response.py
+Filename: openapiopenai/models/delete_assistant_file_response.py
+Comment: 
+
+Filename: openapiopenai/models/delete_assistant_response.py
 Comment: 
 
 Filename: openapiopenai/models/delete_file_response.py
 Comment: 
 
+Filename: openapiopenai/models/delete_message_response.py
+Comment: 
+
 Filename: openapiopenai/models/delete_model_response.py
 Comment: 
 
+Filename: openapiopenai/models/delete_thread_response.py
+Comment: 
+
+Filename: openapiopenai/models/done_event.py
+Comment: 
+
+Filename: openapiopenai/models/embedding.py
+Comment: 
+
 Filename: openapiopenai/models/error.py
 Comment: 
 
+Filename: openapiopenai/models/error_event.py
+Comment: 
+
 Filename: openapiopenai/models/error_response.py
 Comment: 
 
-Filename: openapiopenai/models/fine_tune.py
+Filename: openapiopenai/models/fine_tuning_integration.py
+Comment: 
+
+Filename: openapiopenai/models/fine_tuning_job.py
+Comment: 
+
+Filename: openapiopenai/models/fine_tuning_job_checkpoint.py
+Comment: 
+
+Filename: openapiopenai/models/fine_tuning_job_checkpoint_metrics.py
+Comment: 
+
+Filename: openapiopenai/models/fine_tuning_job_error.py
+Comment: 
+
+Filename: openapiopenai/models/fine_tuning_job_event.py
+Comment: 
+
+Filename: openapiopenai/models/fine_tuning_job_hyperparameters.py
+Comment: 
+
+Filename: openapiopenai/models/fine_tuning_job_hyperparameters_n_epochs.py
+Comment: 
+
+Filename: openapiopenai/models/fine_tuning_job_integrations_inner.py
 Comment: 
 
-Filename: openapiopenai/models/fine_tune_event.py
+Filename: openapiopenai/models/function_object.py
+Comment: 
+
+Filename: openapiopenai/models/image.py
 Comment: 
 
 Filename: openapiopenai/models/images_response.py
 Comment: 
 
-Filename: openapiopenai/models/images_response_data_inner.py
+Filename: openapiopenai/models/list_assistant_files_response.py
+Comment: 
+
+Filename: openapiopenai/models/list_assistants_response.py
 Comment: 
 
 Filename: openapiopenai/models/list_files_response.py
 Comment: 
 
-Filename: openapiopenai/models/list_fine_tune_events_response.py
+Filename: openapiopenai/models/list_fine_tuning_job_checkpoints_response.py
+Comment: 
+
+Filename: openapiopenai/models/list_fine_tuning_job_events_response.py
 Comment: 
 
-Filename: openapiopenai/models/list_fine_tunes_response.py
+Filename: openapiopenai/models/list_message_files_response.py
+Comment: 
+
+Filename: openapiopenai/models/list_messages_response.py
 Comment: 
 
 Filename: openapiopenai/models/list_models_response.py
 Comment: 
 
+Filename: openapiopenai/models/list_paginated_fine_tuning_jobs_response.py
+Comment: 
+
+Filename: openapiopenai/models/list_run_steps_response.py
+Comment: 
+
+Filename: openapiopenai/models/list_runs_response.py
+Comment: 
+
+Filename: openapiopenai/models/list_threads_response.py
+Comment: 
+
+Filename: openapiopenai/models/message_content_image_file_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_content_image_file_object_image_file.py
+Comment: 
+
+Filename: openapiopenai/models/message_content_text_annotations_file_citation_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_content_text_annotations_file_citation_object_file_citation.py
+Comment: 
+
+Filename: openapiopenai/models/message_content_text_annotations_file_path_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_content_text_annotations_file_path_object_file_path.py
+Comment: 
+
+Filename: openapiopenai/models/message_content_text_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_content_text_object_text.py
+Comment: 
+
+Filename: openapiopenai/models/message_content_text_object_text_annotations_inner.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_content_image_file_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_content_image_file_object_image_file.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_content_text_annotations_file_citation_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_content_text_annotations_file_citation_object_file_citation.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_content_text_annotations_file_path_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_content_text_annotations_file_path_object_file_path.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_content_text_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_content_text_object_text.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_content_text_object_text_annotations_inner.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_object_delta.py
+Comment: 
+
+Filename: openapiopenai/models/message_delta_object_delta_content_inner.py
+Comment: 
+
+Filename: openapiopenai/models/message_file_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_object.py
+Comment: 
+
+Filename: openapiopenai/models/message_object_content_inner.py
+Comment: 
+
+Filename: openapiopenai/models/message_object_incomplete_details.py
+Comment: 
+
+Filename: openapiopenai/models/message_stream_event.py
+Comment: 
+
+Filename: openapiopenai/models/message_stream_event_one_of.py
+Comment: 
+
+Filename: openapiopenai/models/message_stream_event_one_of1.py
+Comment: 
+
+Filename: openapiopenai/models/message_stream_event_one_of2.py
+Comment: 
+
+Filename: openapiopenai/models/message_stream_event_one_of3.py
+Comment: 
+
+Filename: openapiopenai/models/message_stream_event_one_of4.py
+Comment: 
+
 Filename: openapiopenai/models/model.py
 Comment: 
 
+Filename: openapiopenai/models/modify_assistant_request.py
+Comment: 
+
+Filename: openapiopenai/models/modify_message_request.py
+Comment: 
+
+Filename: openapiopenai/models/modify_run_request.py
+Comment: 
+
+Filename: openapiopenai/models/modify_thread_request.py
+Comment: 
+
 Filename: openapiopenai/models/open_ai_file.py
 Comment: 
 
-Filename: openapiopenai-1.0.0.dist-info/METADATA
+Filename: openapiopenai/models/run_completion_usage.py
+Comment: 
+
+Filename: openapiopenai/models/run_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_object_incomplete_details.py
+Comment: 
+
+Filename: openapiopenai/models/run_object_last_error.py
+Comment: 
+
+Filename: openapiopenai/models/run_object_required_action.py
+Comment: 
+
+Filename: openapiopenai/models/run_object_required_action_submit_tool_outputs.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_completion_usage.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_object_delta.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_object_delta_step_details.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_message_creation_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_message_creation_object_message_creation.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_code_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_code_object_code_interpreter.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_code_object_code_interpreter_outputs_inner.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_code_output_image_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_code_output_image_object_image.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_code_output_logs_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_function_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_function_object_function.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_object_tool_calls_inner.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_delta_step_details_tool_calls_retrieval_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_message_creation_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_message_creation_object_message_creation.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_code_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_code_object_code_interpreter.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_code_object_code_interpreter_outputs_inner.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_code_output_image_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_code_output_image_object_image.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_code_output_logs_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_function_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_function_object_function.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_object_tool_calls_inner.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_details_tool_calls_retrieval_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_object_last_error.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_object_step_details.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_stream_event.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_stream_event_one_of.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_stream_event_one_of1.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_stream_event_one_of2.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_stream_event_one_of3.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_stream_event_one_of4.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_stream_event_one_of5.py
+Comment: 
+
+Filename: openapiopenai/models/run_step_stream_event_one_of6.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event_one_of.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event_one_of1.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event_one_of2.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event_one_of3.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event_one_of4.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event_one_of5.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event_one_of6.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event_one_of7.py
+Comment: 
+
+Filename: openapiopenai/models/run_stream_event_one_of8.py
+Comment: 
+
+Filename: openapiopenai/models/run_tool_call_object.py
+Comment: 
+
+Filename: openapiopenai/models/run_tool_call_object_function.py
+Comment: 
+
+Filename: openapiopenai/models/submit_tool_outputs_run_request.py
+Comment: 
+
+Filename: openapiopenai/models/submit_tool_outputs_run_request_tool_outputs_inner.py
+Comment: 
+
+Filename: openapiopenai/models/thread_object.py
+Comment: 
+
+Filename: openapiopenai/models/thread_stream_event.py
+Comment: 
+
+Filename: openapiopenai/models/thread_stream_event_one_of.py
+Comment: 
+
+Filename: openapiopenai/models/transcription_segment.py
+Comment: 
+
+Filename: openapiopenai/models/transcription_word.py
+Comment: 
+
+Filename: openapiopenai/models/truncation_object.py
+Comment: 
+
+Filename: openapiopenai-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: openapiopenai-1.0.0.dist-info/WHEEL
+Filename: openapiopenai-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: openapiopenai-1.0.0.dist-info/top_level.txt
+Filename: openapiopenai-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: openapiopenai-1.0.0.dist-info/RECORD
+Filename: openapiopenai-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openapiopenai/__init__.py

```diff
@@ -1,93 +1,283 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 # import apis into sdk package
-from openapiopenai.api.open_ai_api import OpenAIApi
+from openapiopenai.api.assistants_api import AssistantsApi
+from openapiopenai.api.audio_api import AudioApi
+from openapiopenai.api.chat_api import ChatApi
+from openapiopenai.api.completions_api import CompletionsApi
+from openapiopenai.api.embeddings_api import EmbeddingsApi
+from openapiopenai.api.files_api import FilesApi
+from openapiopenai.api.fine_tuning_api import FineTuningApi
+from openapiopenai.api.images_api import ImagesApi
+from openapiopenai.api.models_api import ModelsApi
+from openapiopenai.api.moderations_api import ModerationsApi
 
 # import ApiClient
 from openapiopenai.api_response import ApiResponse
 from openapiopenai.api_client import ApiClient
 from openapiopenai.configuration import Configuration
 from openapiopenai.exceptions import OpenApiException
 from openapiopenai.exceptions import ApiTypeError
 from openapiopenai.exceptions import ApiValueError
 from openapiopenai.exceptions import ApiKeyError
 from openapiopenai.exceptions import ApiAttributeError
 from openapiopenai.exceptions import ApiException
 
 # import models into sdk package
+from openapiopenai.models.assistant_file_object import AssistantFileObject
+from openapiopenai.models.assistant_object import AssistantObject
+from openapiopenai.models.assistant_object_tools_inner import AssistantObjectToolsInner
+from openapiopenai.models.assistant_stream_event import AssistantStreamEvent
+from openapiopenai.models.assistant_tools_code import AssistantToolsCode
+from openapiopenai.models.assistant_tools_function import AssistantToolsFunction
+from openapiopenai.models.assistant_tools_retrieval import AssistantToolsRetrieval
+from openapiopenai.models.assistants_api_named_tool_choice import AssistantsApiNamedToolChoice
+from openapiopenai.models.assistants_api_response_format import AssistantsApiResponseFormat
+from openapiopenai.models.assistants_api_response_format_option import AssistantsApiResponseFormatOption
+from openapiopenai.models.assistants_api_tool_choice_option import AssistantsApiToolChoiceOption
+from openapiopenai.models.chat_completion_function_call_option import ChatCompletionFunctionCallOption
 from openapiopenai.models.chat_completion_functions import ChatCompletionFunctions
+from openapiopenai.models.chat_completion_message_tool_call import ChatCompletionMessageToolCall
+from openapiopenai.models.chat_completion_message_tool_call_chunk import ChatCompletionMessageToolCallChunk
+from openapiopenai.models.chat_completion_message_tool_call_chunk_function import ChatCompletionMessageToolCallChunkFunction
+from openapiopenai.models.chat_completion_message_tool_call_function import ChatCompletionMessageToolCallFunction
+from openapiopenai.models.chat_completion_named_tool_choice import ChatCompletionNamedToolChoice
+from openapiopenai.models.chat_completion_named_tool_choice_function import ChatCompletionNamedToolChoiceFunction
+from openapiopenai.models.chat_completion_request_assistant_message import ChatCompletionRequestAssistantMessage
+from openapiopenai.models.chat_completion_request_assistant_message_function_call import ChatCompletionRequestAssistantMessageFunctionCall
+from openapiopenai.models.chat_completion_request_function_message import ChatCompletionRequestFunctionMessage
 from openapiopenai.models.chat_completion_request_message import ChatCompletionRequestMessage
-from openapiopenai.models.chat_completion_request_message_function_call import ChatCompletionRequestMessageFunctionCall
+from openapiopenai.models.chat_completion_request_message_content_part import ChatCompletionRequestMessageContentPart
+from openapiopenai.models.chat_completion_request_message_content_part_image import ChatCompletionRequestMessageContentPartImage
+from openapiopenai.models.chat_completion_request_message_content_part_image_image_url import ChatCompletionRequestMessageContentPartImageImageUrl
+from openapiopenai.models.chat_completion_request_message_content_part_text import ChatCompletionRequestMessageContentPartText
+from openapiopenai.models.chat_completion_request_system_message import ChatCompletionRequestSystemMessage
+from openapiopenai.models.chat_completion_request_tool_message import ChatCompletionRequestToolMessage
+from openapiopenai.models.chat_completion_request_user_message import ChatCompletionRequestUserMessage
+from openapiopenai.models.chat_completion_request_user_message_content import ChatCompletionRequestUserMessageContent
 from openapiopenai.models.chat_completion_response_message import ChatCompletionResponseMessage
+from openapiopenai.models.chat_completion_role import ChatCompletionRole
 from openapiopenai.models.chat_completion_stream_response_delta import ChatCompletionStreamResponseDelta
+from openapiopenai.models.chat_completion_stream_response_delta_function_call import ChatCompletionStreamResponseDeltaFunctionCall
+from openapiopenai.models.chat_completion_token_logprob import ChatCompletionTokenLogprob
+from openapiopenai.models.chat_completion_token_logprob_top_logprobs_inner import ChatCompletionTokenLogprobTopLogprobsInner
+from openapiopenai.models.chat_completion_tool import ChatCompletionTool
+from openapiopenai.models.chat_completion_tool_choice_option import ChatCompletionToolChoiceOption
+from openapiopenai.models.completion_usage import CompletionUsage
+from openapiopenai.models.create_assistant_file_request import CreateAssistantFileRequest
+from openapiopenai.models.create_assistant_request import CreateAssistantRequest
+from openapiopenai.models.create_assistant_request_model import CreateAssistantRequestModel
+from openapiopenai.models.create_chat_completion_function_response import CreateChatCompletionFunctionResponse
+from openapiopenai.models.create_chat_completion_function_response_choices_inner import CreateChatCompletionFunctionResponseChoicesInner
 from openapiopenai.models.create_chat_completion_request import CreateChatCompletionRequest
 from openapiopenai.models.create_chat_completion_request_function_call import CreateChatCompletionRequestFunctionCall
-from openapiopenai.models.create_chat_completion_request_function_call_one_of import CreateChatCompletionRequestFunctionCallOneOf
 from openapiopenai.models.create_chat_completion_request_model import CreateChatCompletionRequestModel
+from openapiopenai.models.create_chat_completion_request_response_format import CreateChatCompletionRequestResponseFormat
 from openapiopenai.models.create_chat_completion_request_stop import CreateChatCompletionRequestStop
 from openapiopenai.models.create_chat_completion_response import CreateChatCompletionResponse
 from openapiopenai.models.create_chat_completion_response_choices_inner import CreateChatCompletionResponseChoicesInner
+from openapiopenai.models.create_chat_completion_response_choices_inner_logprobs import CreateChatCompletionResponseChoicesInnerLogprobs
 from openapiopenai.models.create_chat_completion_stream_response import CreateChatCompletionStreamResponse
 from openapiopenai.models.create_chat_completion_stream_response_choices_inner import CreateChatCompletionStreamResponseChoicesInner
 from openapiopenai.models.create_completion_request import CreateCompletionRequest
 from openapiopenai.models.create_completion_request_model import CreateCompletionRequestModel
 from openapiopenai.models.create_completion_request_prompt import CreateCompletionRequestPrompt
 from openapiopenai.models.create_completion_request_stop import CreateCompletionRequestStop
 from openapiopenai.models.create_completion_response import CreateCompletionResponse
 from openapiopenai.models.create_completion_response_choices_inner import CreateCompletionResponseChoicesInner
 from openapiopenai.models.create_completion_response_choices_inner_logprobs import CreateCompletionResponseChoicesInnerLogprobs
-from openapiopenai.models.create_completion_response_usage import CreateCompletionResponseUsage
-from openapiopenai.models.create_edit_request import CreateEditRequest
-from openapiopenai.models.create_edit_request_model import CreateEditRequestModel
-from openapiopenai.models.create_edit_response import CreateEditResponse
-from openapiopenai.models.create_edit_response_choices_inner import CreateEditResponseChoicesInner
 from openapiopenai.models.create_embedding_request import CreateEmbeddingRequest
 from openapiopenai.models.create_embedding_request_input import CreateEmbeddingRequestInput
 from openapiopenai.models.create_embedding_request_model import CreateEmbeddingRequestModel
 from openapiopenai.models.create_embedding_response import CreateEmbeddingResponse
-from openapiopenai.models.create_embedding_response_data_inner import CreateEmbeddingResponseDataInner
 from openapiopenai.models.create_embedding_response_usage import CreateEmbeddingResponseUsage
-from openapiopenai.models.create_fine_tune_request import CreateFineTuneRequest
-from openapiopenai.models.create_fine_tune_request_model import CreateFineTuneRequestModel
+from openapiopenai.models.create_fine_tuning_job_request import CreateFineTuningJobRequest
+from openapiopenai.models.create_fine_tuning_job_request_hyperparameters import CreateFineTuningJobRequestHyperparameters
+from openapiopenai.models.create_fine_tuning_job_request_hyperparameters_batch_size import CreateFineTuningJobRequestHyperparametersBatchSize
+from openapiopenai.models.create_fine_tuning_job_request_hyperparameters_learning_rate_multiplier import CreateFineTuningJobRequestHyperparametersLearningRateMultiplier
+from openapiopenai.models.create_fine_tuning_job_request_hyperparameters_n_epochs import CreateFineTuningJobRequestHyperparametersNEpochs
+from openapiopenai.models.create_fine_tuning_job_request_integrations_inner import CreateFineTuningJobRequestIntegrationsInner
+from openapiopenai.models.create_fine_tuning_job_request_integrations_inner_type import CreateFineTuningJobRequestIntegrationsInnerType
+from openapiopenai.models.create_fine_tuning_job_request_integrations_inner_wandb import CreateFineTuningJobRequestIntegrationsInnerWandb
+from openapiopenai.models.create_fine_tuning_job_request_model import CreateFineTuningJobRequestModel
+from openapiopenai.models.create_image_edit_request_model import CreateImageEditRequestModel
 from openapiopenai.models.create_image_request import CreateImageRequest
+from openapiopenai.models.create_image_request_model import CreateImageRequestModel
+from openapiopenai.models.create_message_request import CreateMessageRequest
 from openapiopenai.models.create_moderation_request import CreateModerationRequest
 from openapiopenai.models.create_moderation_request_input import CreateModerationRequestInput
 from openapiopenai.models.create_moderation_request_model import CreateModerationRequestModel
 from openapiopenai.models.create_moderation_response import CreateModerationResponse
 from openapiopenai.models.create_moderation_response_results_inner import CreateModerationResponseResultsInner
 from openapiopenai.models.create_moderation_response_results_inner_categories import CreateModerationResponseResultsInnerCategories
 from openapiopenai.models.create_moderation_response_results_inner_category_scores import CreateModerationResponseResultsInnerCategoryScores
+from openapiopenai.models.create_run_request import CreateRunRequest
+from openapiopenai.models.create_run_request_model import CreateRunRequestModel
+from openapiopenai.models.create_speech_request import CreateSpeechRequest
+from openapiopenai.models.create_speech_request_model import CreateSpeechRequestModel
+from openapiopenai.models.create_thread_and_run_request import CreateThreadAndRunRequest
+from openapiopenai.models.create_thread_and_run_request_tools_inner import CreateThreadAndRunRequestToolsInner
+from openapiopenai.models.create_thread_request import CreateThreadRequest
+from openapiopenai.models.create_transcription200_response import CreateTranscription200Response
 from openapiopenai.models.create_transcription_request_model import CreateTranscriptionRequestModel
-from openapiopenai.models.create_transcription_response import CreateTranscriptionResponse
-from openapiopenai.models.create_translation_response import CreateTranslationResponse
+from openapiopenai.models.create_transcription_response_json import CreateTranscriptionResponseJson
+from openapiopenai.models.create_transcription_response_verbose_json import CreateTranscriptionResponseVerboseJson
+from openapiopenai.models.create_translation200_response import CreateTranslation200Response
+from openapiopenai.models.create_translation_response_json import CreateTranslationResponseJson
+from openapiopenai.models.create_translation_response_verbose_json import CreateTranslationResponseVerboseJson
+from openapiopenai.models.delete_assistant_file_response import DeleteAssistantFileResponse
+from openapiopenai.models.delete_assistant_response import DeleteAssistantResponse
 from openapiopenai.models.delete_file_response import DeleteFileResponse
+from openapiopenai.models.delete_message_response import DeleteMessageResponse
 from openapiopenai.models.delete_model_response import DeleteModelResponse
+from openapiopenai.models.delete_thread_response import DeleteThreadResponse
+from openapiopenai.models.done_event import DoneEvent
+from openapiopenai.models.embedding import Embedding
 from openapiopenai.models.error import Error
+from openapiopenai.models.error_event import ErrorEvent
 from openapiopenai.models.error_response import ErrorResponse
-from openapiopenai.models.fine_tune import FineTune
-from openapiopenai.models.fine_tune_event import FineTuneEvent
+from openapiopenai.models.fine_tuning_integration import FineTuningIntegration
+from openapiopenai.models.fine_tuning_job import FineTuningJob
+from openapiopenai.models.fine_tuning_job_checkpoint import FineTuningJobCheckpoint
+from openapiopenai.models.fine_tuning_job_checkpoint_metrics import FineTuningJobCheckpointMetrics
+from openapiopenai.models.fine_tuning_job_error import FineTuningJobError
+from openapiopenai.models.fine_tuning_job_event import FineTuningJobEvent
+from openapiopenai.models.fine_tuning_job_hyperparameters import FineTuningJobHyperparameters
+from openapiopenai.models.fine_tuning_job_hyperparameters_n_epochs import FineTuningJobHyperparametersNEpochs
+from openapiopenai.models.fine_tuning_job_integrations_inner import FineTuningJobIntegrationsInner
+from openapiopenai.models.function_object import FunctionObject
+from openapiopenai.models.image import Image
 from openapiopenai.models.images_response import ImagesResponse
-from openapiopenai.models.images_response_data_inner import ImagesResponseDataInner
+from openapiopenai.models.list_assistant_files_response import ListAssistantFilesResponse
+from openapiopenai.models.list_assistants_response import ListAssistantsResponse
 from openapiopenai.models.list_files_response import ListFilesResponse
-from openapiopenai.models.list_fine_tune_events_response import ListFineTuneEventsResponse
-from openapiopenai.models.list_fine_tunes_response import ListFineTunesResponse
+from openapiopenai.models.list_fine_tuning_job_checkpoints_response import ListFineTuningJobCheckpointsResponse
+from openapiopenai.models.list_fine_tuning_job_events_response import ListFineTuningJobEventsResponse
+from openapiopenai.models.list_message_files_response import ListMessageFilesResponse
+from openapiopenai.models.list_messages_response import ListMessagesResponse
 from openapiopenai.models.list_models_response import ListModelsResponse
+from openapiopenai.models.list_paginated_fine_tuning_jobs_response import ListPaginatedFineTuningJobsResponse
+from openapiopenai.models.list_run_steps_response import ListRunStepsResponse
+from openapiopenai.models.list_runs_response import ListRunsResponse
+from openapiopenai.models.list_threads_response import ListThreadsResponse
+from openapiopenai.models.message_content_image_file_object import MessageContentImageFileObject
+from openapiopenai.models.message_content_image_file_object_image_file import MessageContentImageFileObjectImageFile
+from openapiopenai.models.message_content_text_annotations_file_citation_object import MessageContentTextAnnotationsFileCitationObject
+from openapiopenai.models.message_content_text_annotations_file_citation_object_file_citation import MessageContentTextAnnotationsFileCitationObjectFileCitation
+from openapiopenai.models.message_content_text_annotations_file_path_object import MessageContentTextAnnotationsFilePathObject
+from openapiopenai.models.message_content_text_annotations_file_path_object_file_path import MessageContentTextAnnotationsFilePathObjectFilePath
+from openapiopenai.models.message_content_text_object import MessageContentTextObject
+from openapiopenai.models.message_content_text_object_text import MessageContentTextObjectText
+from openapiopenai.models.message_content_text_object_text_annotations_inner import MessageContentTextObjectTextAnnotationsInner
+from openapiopenai.models.message_delta_content_image_file_object import MessageDeltaContentImageFileObject
+from openapiopenai.models.message_delta_content_image_file_object_image_file import MessageDeltaContentImageFileObjectImageFile
+from openapiopenai.models.message_delta_content_text_annotations_file_citation_object import MessageDeltaContentTextAnnotationsFileCitationObject
+from openapiopenai.models.message_delta_content_text_annotations_file_citation_object_file_citation import MessageDeltaContentTextAnnotationsFileCitationObjectFileCitation
+from openapiopenai.models.message_delta_content_text_annotations_file_path_object import MessageDeltaContentTextAnnotationsFilePathObject
+from openapiopenai.models.message_delta_content_text_annotations_file_path_object_file_path import MessageDeltaContentTextAnnotationsFilePathObjectFilePath
+from openapiopenai.models.message_delta_content_text_object import MessageDeltaContentTextObject
+from openapiopenai.models.message_delta_content_text_object_text import MessageDeltaContentTextObjectText
+from openapiopenai.models.message_delta_content_text_object_text_annotations_inner import MessageDeltaContentTextObjectTextAnnotationsInner
+from openapiopenai.models.message_delta_object import MessageDeltaObject
+from openapiopenai.models.message_delta_object_delta import MessageDeltaObjectDelta
+from openapiopenai.models.message_delta_object_delta_content_inner import MessageDeltaObjectDeltaContentInner
+from openapiopenai.models.message_file_object import MessageFileObject
+from openapiopenai.models.message_object import MessageObject
+from openapiopenai.models.message_object_content_inner import MessageObjectContentInner
+from openapiopenai.models.message_object_incomplete_details import MessageObjectIncompleteDetails
+from openapiopenai.models.message_stream_event import MessageStreamEvent
+from openapiopenai.models.message_stream_event_one_of import MessageStreamEventOneOf
+from openapiopenai.models.message_stream_event_one_of1 import MessageStreamEventOneOf1
+from openapiopenai.models.message_stream_event_one_of2 import MessageStreamEventOneOf2
+from openapiopenai.models.message_stream_event_one_of3 import MessageStreamEventOneOf3
+from openapiopenai.models.message_stream_event_one_of4 import MessageStreamEventOneOf4
 from openapiopenai.models.model import Model
+from openapiopenai.models.modify_assistant_request import ModifyAssistantRequest
+from openapiopenai.models.modify_message_request import ModifyMessageRequest
+from openapiopenai.models.modify_run_request import ModifyRunRequest
+from openapiopenai.models.modify_thread_request import ModifyThreadRequest
 from openapiopenai.models.open_ai_file import OpenAIFile
+from openapiopenai.models.run_completion_usage import RunCompletionUsage
+from openapiopenai.models.run_object import RunObject
+from openapiopenai.models.run_object_incomplete_details import RunObjectIncompleteDetails
+from openapiopenai.models.run_object_last_error import RunObjectLastError
+from openapiopenai.models.run_object_required_action import RunObjectRequiredAction
+from openapiopenai.models.run_object_required_action_submit_tool_outputs import RunObjectRequiredActionSubmitToolOutputs
+from openapiopenai.models.run_step_completion_usage import RunStepCompletionUsage
+from openapiopenai.models.run_step_delta_object import RunStepDeltaObject
+from openapiopenai.models.run_step_delta_object_delta import RunStepDeltaObjectDelta
+from openapiopenai.models.run_step_delta_object_delta_step_details import RunStepDeltaObjectDeltaStepDetails
+from openapiopenai.models.run_step_delta_step_details_message_creation_object import RunStepDeltaStepDetailsMessageCreationObject
+from openapiopenai.models.run_step_delta_step_details_message_creation_object_message_creation import RunStepDeltaStepDetailsMessageCreationObjectMessageCreation
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_object import RunStepDeltaStepDetailsToolCallsCodeObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_object_code_interpreter import RunStepDeltaStepDetailsToolCallsCodeObjectCodeInterpreter
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_object_code_interpreter_outputs_inner import RunStepDeltaStepDetailsToolCallsCodeObjectCodeInterpreterOutputsInner
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_output_image_object import RunStepDeltaStepDetailsToolCallsCodeOutputImageObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_output_image_object_image import RunStepDeltaStepDetailsToolCallsCodeOutputImageObjectImage
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_output_logs_object import RunStepDeltaStepDetailsToolCallsCodeOutputLogsObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_function_object import RunStepDeltaStepDetailsToolCallsFunctionObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_function_object_function import RunStepDeltaStepDetailsToolCallsFunctionObjectFunction
+from openapiopenai.models.run_step_delta_step_details_tool_calls_object import RunStepDeltaStepDetailsToolCallsObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_object_tool_calls_inner import RunStepDeltaStepDetailsToolCallsObjectToolCallsInner
+from openapiopenai.models.run_step_delta_step_details_tool_calls_retrieval_object import RunStepDeltaStepDetailsToolCallsRetrievalObject
+from openapiopenai.models.run_step_details_message_creation_object import RunStepDetailsMessageCreationObject
+from openapiopenai.models.run_step_details_message_creation_object_message_creation import RunStepDetailsMessageCreationObjectMessageCreation
+from openapiopenai.models.run_step_details_tool_calls_code_object import RunStepDetailsToolCallsCodeObject
+from openapiopenai.models.run_step_details_tool_calls_code_object_code_interpreter import RunStepDetailsToolCallsCodeObjectCodeInterpreter
+from openapiopenai.models.run_step_details_tool_calls_code_object_code_interpreter_outputs_inner import RunStepDetailsToolCallsCodeObjectCodeInterpreterOutputsInner
+from openapiopenai.models.run_step_details_tool_calls_code_output_image_object import RunStepDetailsToolCallsCodeOutputImageObject
+from openapiopenai.models.run_step_details_tool_calls_code_output_image_object_image import RunStepDetailsToolCallsCodeOutputImageObjectImage
+from openapiopenai.models.run_step_details_tool_calls_code_output_logs_object import RunStepDetailsToolCallsCodeOutputLogsObject
+from openapiopenai.models.run_step_details_tool_calls_function_object import RunStepDetailsToolCallsFunctionObject
+from openapiopenai.models.run_step_details_tool_calls_function_object_function import RunStepDetailsToolCallsFunctionObjectFunction
+from openapiopenai.models.run_step_details_tool_calls_object import RunStepDetailsToolCallsObject
+from openapiopenai.models.run_step_details_tool_calls_object_tool_calls_inner import RunStepDetailsToolCallsObjectToolCallsInner
+from openapiopenai.models.run_step_details_tool_calls_retrieval_object import RunStepDetailsToolCallsRetrievalObject
+from openapiopenai.models.run_step_object import RunStepObject
+from openapiopenai.models.run_step_object_last_error import RunStepObjectLastError
+from openapiopenai.models.run_step_object_step_details import RunStepObjectStepDetails
+from openapiopenai.models.run_step_stream_event import RunStepStreamEvent
+from openapiopenai.models.run_step_stream_event_one_of import RunStepStreamEventOneOf
+from openapiopenai.models.run_step_stream_event_one_of1 import RunStepStreamEventOneOf1
+from openapiopenai.models.run_step_stream_event_one_of2 import RunStepStreamEventOneOf2
+from openapiopenai.models.run_step_stream_event_one_of3 import RunStepStreamEventOneOf3
+from openapiopenai.models.run_step_stream_event_one_of4 import RunStepStreamEventOneOf4
+from openapiopenai.models.run_step_stream_event_one_of5 import RunStepStreamEventOneOf5
+from openapiopenai.models.run_step_stream_event_one_of6 import RunStepStreamEventOneOf6
+from openapiopenai.models.run_stream_event import RunStreamEvent
+from openapiopenai.models.run_stream_event_one_of import RunStreamEventOneOf
+from openapiopenai.models.run_stream_event_one_of1 import RunStreamEventOneOf1
+from openapiopenai.models.run_stream_event_one_of2 import RunStreamEventOneOf2
+from openapiopenai.models.run_stream_event_one_of3 import RunStreamEventOneOf3
+from openapiopenai.models.run_stream_event_one_of4 import RunStreamEventOneOf4
+from openapiopenai.models.run_stream_event_one_of5 import RunStreamEventOneOf5
+from openapiopenai.models.run_stream_event_one_of6 import RunStreamEventOneOf6
+from openapiopenai.models.run_stream_event_one_of7 import RunStreamEventOneOf7
+from openapiopenai.models.run_stream_event_one_of8 import RunStreamEventOneOf8
+from openapiopenai.models.run_tool_call_object import RunToolCallObject
+from openapiopenai.models.run_tool_call_object_function import RunToolCallObjectFunction
+from openapiopenai.models.submit_tool_outputs_run_request import SubmitToolOutputsRunRequest
+from openapiopenai.models.submit_tool_outputs_run_request_tool_outputs_inner import SubmitToolOutputsRunRequestToolOutputsInner
+from openapiopenai.models.thread_object import ThreadObject
+from openapiopenai.models.thread_stream_event import ThreadStreamEvent
+from openapiopenai.models.thread_stream_event_one_of import ThreadStreamEventOneOf
+from openapiopenai.models.transcription_segment import TranscriptionSegment
+from openapiopenai.models.transcription_word import TranscriptionWord
+from openapiopenai.models.truncation_object import TruncationObject
```

## openapiopenai/api_client.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.1.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

## openapiopenai/configuration.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -52,14 +52,15 @@
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum
       values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
       in PEM format.
 
+    :Example:
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
@@ -356,26 +357,33 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
+        if self.access_token is not None:
+            auth['ApiKeyAuth'] = {
+                'type': 'bearer',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': 'Bearer ' + self.access_token
+            }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2.0.0\n"\
-               "SDK Package Version: 1.0.0".\
+               "SDK Package Version: 1.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

## openapiopenai/exceptions.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## openapiopenai/rest.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## openapiopenai/api/__init__.py

```diff
@@ -1,5 +1,14 @@
 # flake8: noqa
 
 # import apis into api package
-from openapiopenai.api.open_ai_api import OpenAIApi
+from openapiopenai.api.assistants_api import AssistantsApi
+from openapiopenai.api.audio_api import AudioApi
+from openapiopenai.api.chat_api import ChatApi
+from openapiopenai.api.completions_api import CompletionsApi
+from openapiopenai.api.embeddings_api import EmbeddingsApi
+from openapiopenai.api.files_api import FilesApi
+from openapiopenai.api.fine_tuning_api import FineTuningApi
+from openapiopenai.api.images_api import ImagesApi
+from openapiopenai.api.models_api import ModelsApi
+from openapiopenai.api.moderations_api import ModerationsApi
```

## openapiopenai/models/__init__.py

```diff
@@ -1,76 +1,257 @@
 # coding: utf-8
 
 # flake8: noqa
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
+from openapiopenai.models.assistant_file_object import AssistantFileObject
+from openapiopenai.models.assistant_object import AssistantObject
+from openapiopenai.models.assistant_object_tools_inner import AssistantObjectToolsInner
+from openapiopenai.models.assistant_stream_event import AssistantStreamEvent
+from openapiopenai.models.assistant_tools_code import AssistantToolsCode
+from openapiopenai.models.assistant_tools_function import AssistantToolsFunction
+from openapiopenai.models.assistant_tools_retrieval import AssistantToolsRetrieval
+from openapiopenai.models.assistants_api_named_tool_choice import AssistantsApiNamedToolChoice
+from openapiopenai.models.assistants_api_response_format import AssistantsApiResponseFormat
+from openapiopenai.models.assistants_api_response_format_option import AssistantsApiResponseFormatOption
+from openapiopenai.models.assistants_api_tool_choice_option import AssistantsApiToolChoiceOption
+from openapiopenai.models.chat_completion_function_call_option import ChatCompletionFunctionCallOption
 from openapiopenai.models.chat_completion_functions import ChatCompletionFunctions
+from openapiopenai.models.chat_completion_message_tool_call import ChatCompletionMessageToolCall
+from openapiopenai.models.chat_completion_message_tool_call_chunk import ChatCompletionMessageToolCallChunk
+from openapiopenai.models.chat_completion_message_tool_call_chunk_function import ChatCompletionMessageToolCallChunkFunction
+from openapiopenai.models.chat_completion_message_tool_call_function import ChatCompletionMessageToolCallFunction
+from openapiopenai.models.chat_completion_named_tool_choice import ChatCompletionNamedToolChoice
+from openapiopenai.models.chat_completion_named_tool_choice_function import ChatCompletionNamedToolChoiceFunction
+from openapiopenai.models.chat_completion_request_assistant_message import ChatCompletionRequestAssistantMessage
+from openapiopenai.models.chat_completion_request_assistant_message_function_call import ChatCompletionRequestAssistantMessageFunctionCall
+from openapiopenai.models.chat_completion_request_function_message import ChatCompletionRequestFunctionMessage
 from openapiopenai.models.chat_completion_request_message import ChatCompletionRequestMessage
-from openapiopenai.models.chat_completion_request_message_function_call import ChatCompletionRequestMessageFunctionCall
+from openapiopenai.models.chat_completion_request_message_content_part import ChatCompletionRequestMessageContentPart
+from openapiopenai.models.chat_completion_request_message_content_part_image import ChatCompletionRequestMessageContentPartImage
+from openapiopenai.models.chat_completion_request_message_content_part_image_image_url import ChatCompletionRequestMessageContentPartImageImageUrl
+from openapiopenai.models.chat_completion_request_message_content_part_text import ChatCompletionRequestMessageContentPartText
+from openapiopenai.models.chat_completion_request_system_message import ChatCompletionRequestSystemMessage
+from openapiopenai.models.chat_completion_request_tool_message import ChatCompletionRequestToolMessage
+from openapiopenai.models.chat_completion_request_user_message import ChatCompletionRequestUserMessage
+from openapiopenai.models.chat_completion_request_user_message_content import ChatCompletionRequestUserMessageContent
 from openapiopenai.models.chat_completion_response_message import ChatCompletionResponseMessage
+from openapiopenai.models.chat_completion_role import ChatCompletionRole
 from openapiopenai.models.chat_completion_stream_response_delta import ChatCompletionStreamResponseDelta
+from openapiopenai.models.chat_completion_stream_response_delta_function_call import ChatCompletionStreamResponseDeltaFunctionCall
+from openapiopenai.models.chat_completion_token_logprob import ChatCompletionTokenLogprob
+from openapiopenai.models.chat_completion_token_logprob_top_logprobs_inner import ChatCompletionTokenLogprobTopLogprobsInner
+from openapiopenai.models.chat_completion_tool import ChatCompletionTool
+from openapiopenai.models.chat_completion_tool_choice_option import ChatCompletionToolChoiceOption
+from openapiopenai.models.completion_usage import CompletionUsage
+from openapiopenai.models.create_assistant_file_request import CreateAssistantFileRequest
+from openapiopenai.models.create_assistant_request import CreateAssistantRequest
+from openapiopenai.models.create_assistant_request_model import CreateAssistantRequestModel
+from openapiopenai.models.create_chat_completion_function_response import CreateChatCompletionFunctionResponse
+from openapiopenai.models.create_chat_completion_function_response_choices_inner import CreateChatCompletionFunctionResponseChoicesInner
 from openapiopenai.models.create_chat_completion_request import CreateChatCompletionRequest
 from openapiopenai.models.create_chat_completion_request_function_call import CreateChatCompletionRequestFunctionCall
-from openapiopenai.models.create_chat_completion_request_function_call_one_of import CreateChatCompletionRequestFunctionCallOneOf
 from openapiopenai.models.create_chat_completion_request_model import CreateChatCompletionRequestModel
+from openapiopenai.models.create_chat_completion_request_response_format import CreateChatCompletionRequestResponseFormat
 from openapiopenai.models.create_chat_completion_request_stop import CreateChatCompletionRequestStop
 from openapiopenai.models.create_chat_completion_response import CreateChatCompletionResponse
 from openapiopenai.models.create_chat_completion_response_choices_inner import CreateChatCompletionResponseChoicesInner
+from openapiopenai.models.create_chat_completion_response_choices_inner_logprobs import CreateChatCompletionResponseChoicesInnerLogprobs
 from openapiopenai.models.create_chat_completion_stream_response import CreateChatCompletionStreamResponse
 from openapiopenai.models.create_chat_completion_stream_response_choices_inner import CreateChatCompletionStreamResponseChoicesInner
 from openapiopenai.models.create_completion_request import CreateCompletionRequest
 from openapiopenai.models.create_completion_request_model import CreateCompletionRequestModel
 from openapiopenai.models.create_completion_request_prompt import CreateCompletionRequestPrompt
 from openapiopenai.models.create_completion_request_stop import CreateCompletionRequestStop
 from openapiopenai.models.create_completion_response import CreateCompletionResponse
 from openapiopenai.models.create_completion_response_choices_inner import CreateCompletionResponseChoicesInner
 from openapiopenai.models.create_completion_response_choices_inner_logprobs import CreateCompletionResponseChoicesInnerLogprobs
-from openapiopenai.models.create_completion_response_usage import CreateCompletionResponseUsage
-from openapiopenai.models.create_edit_request import CreateEditRequest
-from openapiopenai.models.create_edit_request_model import CreateEditRequestModel
-from openapiopenai.models.create_edit_response import CreateEditResponse
-from openapiopenai.models.create_edit_response_choices_inner import CreateEditResponseChoicesInner
 from openapiopenai.models.create_embedding_request import CreateEmbeddingRequest
 from openapiopenai.models.create_embedding_request_input import CreateEmbeddingRequestInput
 from openapiopenai.models.create_embedding_request_model import CreateEmbeddingRequestModel
 from openapiopenai.models.create_embedding_response import CreateEmbeddingResponse
-from openapiopenai.models.create_embedding_response_data_inner import CreateEmbeddingResponseDataInner
 from openapiopenai.models.create_embedding_response_usage import CreateEmbeddingResponseUsage
-from openapiopenai.models.create_fine_tune_request import CreateFineTuneRequest
-from openapiopenai.models.create_fine_tune_request_model import CreateFineTuneRequestModel
+from openapiopenai.models.create_fine_tuning_job_request import CreateFineTuningJobRequest
+from openapiopenai.models.create_fine_tuning_job_request_hyperparameters import CreateFineTuningJobRequestHyperparameters
+from openapiopenai.models.create_fine_tuning_job_request_hyperparameters_batch_size import CreateFineTuningJobRequestHyperparametersBatchSize
+from openapiopenai.models.create_fine_tuning_job_request_hyperparameters_learning_rate_multiplier import CreateFineTuningJobRequestHyperparametersLearningRateMultiplier
+from openapiopenai.models.create_fine_tuning_job_request_hyperparameters_n_epochs import CreateFineTuningJobRequestHyperparametersNEpochs
+from openapiopenai.models.create_fine_tuning_job_request_integrations_inner import CreateFineTuningJobRequestIntegrationsInner
+from openapiopenai.models.create_fine_tuning_job_request_integrations_inner_type import CreateFineTuningJobRequestIntegrationsInnerType
+from openapiopenai.models.create_fine_tuning_job_request_integrations_inner_wandb import CreateFineTuningJobRequestIntegrationsInnerWandb
+from openapiopenai.models.create_fine_tuning_job_request_model import CreateFineTuningJobRequestModel
+from openapiopenai.models.create_image_edit_request_model import CreateImageEditRequestModel
 from openapiopenai.models.create_image_request import CreateImageRequest
+from openapiopenai.models.create_image_request_model import CreateImageRequestModel
+from openapiopenai.models.create_message_request import CreateMessageRequest
 from openapiopenai.models.create_moderation_request import CreateModerationRequest
 from openapiopenai.models.create_moderation_request_input import CreateModerationRequestInput
 from openapiopenai.models.create_moderation_request_model import CreateModerationRequestModel
 from openapiopenai.models.create_moderation_response import CreateModerationResponse
 from openapiopenai.models.create_moderation_response_results_inner import CreateModerationResponseResultsInner
 from openapiopenai.models.create_moderation_response_results_inner_categories import CreateModerationResponseResultsInnerCategories
 from openapiopenai.models.create_moderation_response_results_inner_category_scores import CreateModerationResponseResultsInnerCategoryScores
+from openapiopenai.models.create_run_request import CreateRunRequest
+from openapiopenai.models.create_run_request_model import CreateRunRequestModel
+from openapiopenai.models.create_speech_request import CreateSpeechRequest
+from openapiopenai.models.create_speech_request_model import CreateSpeechRequestModel
+from openapiopenai.models.create_thread_and_run_request import CreateThreadAndRunRequest
+from openapiopenai.models.create_thread_and_run_request_tools_inner import CreateThreadAndRunRequestToolsInner
+from openapiopenai.models.create_thread_request import CreateThreadRequest
+from openapiopenai.models.create_transcription200_response import CreateTranscription200Response
 from openapiopenai.models.create_transcription_request_model import CreateTranscriptionRequestModel
-from openapiopenai.models.create_transcription_response import CreateTranscriptionResponse
-from openapiopenai.models.create_translation_response import CreateTranslationResponse
+from openapiopenai.models.create_transcription_response_json import CreateTranscriptionResponseJson
+from openapiopenai.models.create_transcription_response_verbose_json import CreateTranscriptionResponseVerboseJson
+from openapiopenai.models.create_translation200_response import CreateTranslation200Response
+from openapiopenai.models.create_translation_response_json import CreateTranslationResponseJson
+from openapiopenai.models.create_translation_response_verbose_json import CreateTranslationResponseVerboseJson
+from openapiopenai.models.delete_assistant_file_response import DeleteAssistantFileResponse
+from openapiopenai.models.delete_assistant_response import DeleteAssistantResponse
 from openapiopenai.models.delete_file_response import DeleteFileResponse
+from openapiopenai.models.delete_message_response import DeleteMessageResponse
 from openapiopenai.models.delete_model_response import DeleteModelResponse
+from openapiopenai.models.delete_thread_response import DeleteThreadResponse
+from openapiopenai.models.done_event import DoneEvent
+from openapiopenai.models.embedding import Embedding
 from openapiopenai.models.error import Error
+from openapiopenai.models.error_event import ErrorEvent
 from openapiopenai.models.error_response import ErrorResponse
-from openapiopenai.models.fine_tune import FineTune
-from openapiopenai.models.fine_tune_event import FineTuneEvent
+from openapiopenai.models.fine_tuning_integration import FineTuningIntegration
+from openapiopenai.models.fine_tuning_job import FineTuningJob
+from openapiopenai.models.fine_tuning_job_checkpoint import FineTuningJobCheckpoint
+from openapiopenai.models.fine_tuning_job_checkpoint_metrics import FineTuningJobCheckpointMetrics
+from openapiopenai.models.fine_tuning_job_error import FineTuningJobError
+from openapiopenai.models.fine_tuning_job_event import FineTuningJobEvent
+from openapiopenai.models.fine_tuning_job_hyperparameters import FineTuningJobHyperparameters
+from openapiopenai.models.fine_tuning_job_hyperparameters_n_epochs import FineTuningJobHyperparametersNEpochs
+from openapiopenai.models.fine_tuning_job_integrations_inner import FineTuningJobIntegrationsInner
+from openapiopenai.models.function_object import FunctionObject
+from openapiopenai.models.image import Image
 from openapiopenai.models.images_response import ImagesResponse
-from openapiopenai.models.images_response_data_inner import ImagesResponseDataInner
+from openapiopenai.models.list_assistant_files_response import ListAssistantFilesResponse
+from openapiopenai.models.list_assistants_response import ListAssistantsResponse
 from openapiopenai.models.list_files_response import ListFilesResponse
-from openapiopenai.models.list_fine_tune_events_response import ListFineTuneEventsResponse
-from openapiopenai.models.list_fine_tunes_response import ListFineTunesResponse
+from openapiopenai.models.list_fine_tuning_job_checkpoints_response import ListFineTuningJobCheckpointsResponse
+from openapiopenai.models.list_fine_tuning_job_events_response import ListFineTuningJobEventsResponse
+from openapiopenai.models.list_message_files_response import ListMessageFilesResponse
+from openapiopenai.models.list_messages_response import ListMessagesResponse
 from openapiopenai.models.list_models_response import ListModelsResponse
+from openapiopenai.models.list_paginated_fine_tuning_jobs_response import ListPaginatedFineTuningJobsResponse
+from openapiopenai.models.list_run_steps_response import ListRunStepsResponse
+from openapiopenai.models.list_runs_response import ListRunsResponse
+from openapiopenai.models.list_threads_response import ListThreadsResponse
+from openapiopenai.models.message_content_image_file_object import MessageContentImageFileObject
+from openapiopenai.models.message_content_image_file_object_image_file import MessageContentImageFileObjectImageFile
+from openapiopenai.models.message_content_text_annotations_file_citation_object import MessageContentTextAnnotationsFileCitationObject
+from openapiopenai.models.message_content_text_annotations_file_citation_object_file_citation import MessageContentTextAnnotationsFileCitationObjectFileCitation
+from openapiopenai.models.message_content_text_annotations_file_path_object import MessageContentTextAnnotationsFilePathObject
+from openapiopenai.models.message_content_text_annotations_file_path_object_file_path import MessageContentTextAnnotationsFilePathObjectFilePath
+from openapiopenai.models.message_content_text_object import MessageContentTextObject
+from openapiopenai.models.message_content_text_object_text import MessageContentTextObjectText
+from openapiopenai.models.message_content_text_object_text_annotations_inner import MessageContentTextObjectTextAnnotationsInner
+from openapiopenai.models.message_delta_content_image_file_object import MessageDeltaContentImageFileObject
+from openapiopenai.models.message_delta_content_image_file_object_image_file import MessageDeltaContentImageFileObjectImageFile
+from openapiopenai.models.message_delta_content_text_annotations_file_citation_object import MessageDeltaContentTextAnnotationsFileCitationObject
+from openapiopenai.models.message_delta_content_text_annotations_file_citation_object_file_citation import MessageDeltaContentTextAnnotationsFileCitationObjectFileCitation
+from openapiopenai.models.message_delta_content_text_annotations_file_path_object import MessageDeltaContentTextAnnotationsFilePathObject
+from openapiopenai.models.message_delta_content_text_annotations_file_path_object_file_path import MessageDeltaContentTextAnnotationsFilePathObjectFilePath
+from openapiopenai.models.message_delta_content_text_object import MessageDeltaContentTextObject
+from openapiopenai.models.message_delta_content_text_object_text import MessageDeltaContentTextObjectText
+from openapiopenai.models.message_delta_content_text_object_text_annotations_inner import MessageDeltaContentTextObjectTextAnnotationsInner
+from openapiopenai.models.message_delta_object import MessageDeltaObject
+from openapiopenai.models.message_delta_object_delta import MessageDeltaObjectDelta
+from openapiopenai.models.message_delta_object_delta_content_inner import MessageDeltaObjectDeltaContentInner
+from openapiopenai.models.message_file_object import MessageFileObject
+from openapiopenai.models.message_object import MessageObject
+from openapiopenai.models.message_object_content_inner import MessageObjectContentInner
+from openapiopenai.models.message_object_incomplete_details import MessageObjectIncompleteDetails
+from openapiopenai.models.message_stream_event import MessageStreamEvent
+from openapiopenai.models.message_stream_event_one_of import MessageStreamEventOneOf
+from openapiopenai.models.message_stream_event_one_of1 import MessageStreamEventOneOf1
+from openapiopenai.models.message_stream_event_one_of2 import MessageStreamEventOneOf2
+from openapiopenai.models.message_stream_event_one_of3 import MessageStreamEventOneOf3
+from openapiopenai.models.message_stream_event_one_of4 import MessageStreamEventOneOf4
 from openapiopenai.models.model import Model
+from openapiopenai.models.modify_assistant_request import ModifyAssistantRequest
+from openapiopenai.models.modify_message_request import ModifyMessageRequest
+from openapiopenai.models.modify_run_request import ModifyRunRequest
+from openapiopenai.models.modify_thread_request import ModifyThreadRequest
 from openapiopenai.models.open_ai_file import OpenAIFile
+from openapiopenai.models.run_completion_usage import RunCompletionUsage
+from openapiopenai.models.run_object import RunObject
+from openapiopenai.models.run_object_incomplete_details import RunObjectIncompleteDetails
+from openapiopenai.models.run_object_last_error import RunObjectLastError
+from openapiopenai.models.run_object_required_action import RunObjectRequiredAction
+from openapiopenai.models.run_object_required_action_submit_tool_outputs import RunObjectRequiredActionSubmitToolOutputs
+from openapiopenai.models.run_step_completion_usage import RunStepCompletionUsage
+from openapiopenai.models.run_step_delta_object import RunStepDeltaObject
+from openapiopenai.models.run_step_delta_object_delta import RunStepDeltaObjectDelta
+from openapiopenai.models.run_step_delta_object_delta_step_details import RunStepDeltaObjectDeltaStepDetails
+from openapiopenai.models.run_step_delta_step_details_message_creation_object import RunStepDeltaStepDetailsMessageCreationObject
+from openapiopenai.models.run_step_delta_step_details_message_creation_object_message_creation import RunStepDeltaStepDetailsMessageCreationObjectMessageCreation
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_object import RunStepDeltaStepDetailsToolCallsCodeObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_object_code_interpreter import RunStepDeltaStepDetailsToolCallsCodeObjectCodeInterpreter
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_object_code_interpreter_outputs_inner import RunStepDeltaStepDetailsToolCallsCodeObjectCodeInterpreterOutputsInner
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_output_image_object import RunStepDeltaStepDetailsToolCallsCodeOutputImageObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_output_image_object_image import RunStepDeltaStepDetailsToolCallsCodeOutputImageObjectImage
+from openapiopenai.models.run_step_delta_step_details_tool_calls_code_output_logs_object import RunStepDeltaStepDetailsToolCallsCodeOutputLogsObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_function_object import RunStepDeltaStepDetailsToolCallsFunctionObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_function_object_function import RunStepDeltaStepDetailsToolCallsFunctionObjectFunction
+from openapiopenai.models.run_step_delta_step_details_tool_calls_object import RunStepDeltaStepDetailsToolCallsObject
+from openapiopenai.models.run_step_delta_step_details_tool_calls_object_tool_calls_inner import RunStepDeltaStepDetailsToolCallsObjectToolCallsInner
+from openapiopenai.models.run_step_delta_step_details_tool_calls_retrieval_object import RunStepDeltaStepDetailsToolCallsRetrievalObject
+from openapiopenai.models.run_step_details_message_creation_object import RunStepDetailsMessageCreationObject
+from openapiopenai.models.run_step_details_message_creation_object_message_creation import RunStepDetailsMessageCreationObjectMessageCreation
+from openapiopenai.models.run_step_details_tool_calls_code_object import RunStepDetailsToolCallsCodeObject
+from openapiopenai.models.run_step_details_tool_calls_code_object_code_interpreter import RunStepDetailsToolCallsCodeObjectCodeInterpreter
+from openapiopenai.models.run_step_details_tool_calls_code_object_code_interpreter_outputs_inner import RunStepDetailsToolCallsCodeObjectCodeInterpreterOutputsInner
+from openapiopenai.models.run_step_details_tool_calls_code_output_image_object import RunStepDetailsToolCallsCodeOutputImageObject
+from openapiopenai.models.run_step_details_tool_calls_code_output_image_object_image import RunStepDetailsToolCallsCodeOutputImageObjectImage
+from openapiopenai.models.run_step_details_tool_calls_code_output_logs_object import RunStepDetailsToolCallsCodeOutputLogsObject
+from openapiopenai.models.run_step_details_tool_calls_function_object import RunStepDetailsToolCallsFunctionObject
+from openapiopenai.models.run_step_details_tool_calls_function_object_function import RunStepDetailsToolCallsFunctionObjectFunction
+from openapiopenai.models.run_step_details_tool_calls_object import RunStepDetailsToolCallsObject
+from openapiopenai.models.run_step_details_tool_calls_object_tool_calls_inner import RunStepDetailsToolCallsObjectToolCallsInner
+from openapiopenai.models.run_step_details_tool_calls_retrieval_object import RunStepDetailsToolCallsRetrievalObject
+from openapiopenai.models.run_step_object import RunStepObject
+from openapiopenai.models.run_step_object_last_error import RunStepObjectLastError
+from openapiopenai.models.run_step_object_step_details import RunStepObjectStepDetails
+from openapiopenai.models.run_step_stream_event import RunStepStreamEvent
+from openapiopenai.models.run_step_stream_event_one_of import RunStepStreamEventOneOf
+from openapiopenai.models.run_step_stream_event_one_of1 import RunStepStreamEventOneOf1
+from openapiopenai.models.run_step_stream_event_one_of2 import RunStepStreamEventOneOf2
+from openapiopenai.models.run_step_stream_event_one_of3 import RunStepStreamEventOneOf3
+from openapiopenai.models.run_step_stream_event_one_of4 import RunStepStreamEventOneOf4
+from openapiopenai.models.run_step_stream_event_one_of5 import RunStepStreamEventOneOf5
+from openapiopenai.models.run_step_stream_event_one_of6 import RunStepStreamEventOneOf6
+from openapiopenai.models.run_stream_event import RunStreamEvent
+from openapiopenai.models.run_stream_event_one_of import RunStreamEventOneOf
+from openapiopenai.models.run_stream_event_one_of1 import RunStreamEventOneOf1
+from openapiopenai.models.run_stream_event_one_of2 import RunStreamEventOneOf2
+from openapiopenai.models.run_stream_event_one_of3 import RunStreamEventOneOf3
+from openapiopenai.models.run_stream_event_one_of4 import RunStreamEventOneOf4
+from openapiopenai.models.run_stream_event_one_of5 import RunStreamEventOneOf5
+from openapiopenai.models.run_stream_event_one_of6 import RunStreamEventOneOf6
+from openapiopenai.models.run_stream_event_one_of7 import RunStreamEventOneOf7
+from openapiopenai.models.run_stream_event_one_of8 import RunStreamEventOneOf8
+from openapiopenai.models.run_tool_call_object import RunToolCallObject
+from openapiopenai.models.run_tool_call_object_function import RunToolCallObjectFunction
+from openapiopenai.models.submit_tool_outputs_run_request import SubmitToolOutputsRunRequest
+from openapiopenai.models.submit_tool_outputs_run_request_tool_outputs_inner import SubmitToolOutputsRunRequestToolOutputsInner
+from openapiopenai.models.thread_object import ThreadObject
+from openapiopenai.models.thread_stream_event import ThreadStreamEvent
+from openapiopenai.models.thread_stream_event_one_of import ThreadStreamEventOneOf
+from openapiopenai.models.transcription_segment import TranscriptionSegment
+from openapiopenai.models.transcription_word import TranscriptionWord
+from openapiopenai.models.truncation_object import TruncationObject
```

## openapiopenai/models/chat_completion_functions.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -23,18 +23,18 @@
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ChatCompletionFunctions(BaseModel):
     """
     ChatCompletionFunctions
     """ # noqa: E501
+    description: Optional[StrictStr] = Field(default=None, description="A description of what the function does, used by the model to choose when and how to call the function.")
     name: StrictStr = Field(description="The name of the function to be called. Must be a-z, A-Z, 0-9, or contain underscores and dashes, with a maximum length of 64.")
-    description: Optional[StrictStr] = Field(default=None, description="The description of what the function does.")
-    parameters: Optional[Dict[str, Any]] = Field(default=None, description="The parameters the functions accepts, described as a JSON Schema object. See the [guide](/docs/guides/gpt/function-calling) for examples, and the [JSON Schema reference](https://json-schema.org/understanding-json-schema/) for documentation about the format.")
-    __properties: ClassVar[List[str]] = ["name", "description", "parameters"]
+    parameters: Optional[Dict[str, Any]] = Field(default=None, description="The parameters the functions accepts, described as a JSON Schema object. See the [guide](/docs/guides/text-generation/function-calling) for examples, and the [JSON Schema reference](https://json-schema.org/understanding-json-schema/) for documentation about the format.   Omitting `parameters` defines a function with an empty parameter list.")
+    __properties: ClassVar[List[str]] = ["description", "name", "parameters"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -79,14 +79,14 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
             "description": obj.get("description"),
+            "name": obj.get("name"),
             "parameters": obj.get("parameters")
         })
         return _obj
```

## openapiopenai/models/chat_completion_request_message.py

```diff
@@ -1,105 +1,180 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
-import pprint
-import re  # noqa: F401
 import json
+import pprint
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
+from typing import Any, List, Optional
+from openapiopenai.models.chat_completion_request_assistant_message import ChatCompletionRequestAssistantMessage
+from openapiopenai.models.chat_completion_request_function_message import ChatCompletionRequestFunctionMessage
+from openapiopenai.models.chat_completion_request_system_message import ChatCompletionRequestSystemMessage
+from openapiopenai.models.chat_completion_request_tool_message import ChatCompletionRequestToolMessage
+from openapiopenai.models.chat_completion_request_user_message import ChatCompletionRequestUserMessage
+from pydantic import StrictStr, Field
+from typing import Union, List, Optional, Dict
+from typing_extensions import Literal, Self
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List, Optional
-from openapiopenai.models.chat_completion_request_message_function_call import ChatCompletionRequestMessageFunctionCall
-from typing import Optional, Set
-from typing_extensions import Self
+CHATCOMPLETIONREQUESTMESSAGE_ONE_OF_SCHEMAS = ["ChatCompletionRequestAssistantMessage", "ChatCompletionRequestFunctionMessage", "ChatCompletionRequestSystemMessage", "ChatCompletionRequestToolMessage", "ChatCompletionRequestUserMessage"]
 
 class ChatCompletionRequestMessage(BaseModel):
     """
     ChatCompletionRequestMessage
-    """ # noqa: E501
-    role: StrictStr = Field(description="The role of the messages author. One of `system`, `user`, `assistant`, or `function`.")
-    content: Optional[StrictStr] = Field(default=None, description="The contents of the message. `content` is required for all messages except assistant messages with function calls.")
-    name: Optional[StrictStr] = Field(default=None, description="The name of the author of this message. `name` is required if role is `function`, and it should be the name of the function whose response is in the `content`. May contain a-z, A-Z, 0-9, and underscores, with a maximum length of 64 characters.")
-    function_call: Optional[ChatCompletionRequestMessageFunctionCall] = None
-    __properties: ClassVar[List[str]] = ["role", "content", "name", "function_call"]
-
-    @field_validator('role')
-    def role_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in set(['system', 'user', 'assistant', 'function']):
-            raise ValueError("must be one of enum values ('system', 'user', 'assistant', 'function')")
-        return value
+    """
+    # data type: ChatCompletionRequestSystemMessage
+    oneof_schema_1_validator: Optional[ChatCompletionRequestSystemMessage] = None
+    # data type: ChatCompletionRequestUserMessage
+    oneof_schema_2_validator: Optional[ChatCompletionRequestUserMessage] = None
+    # data type: ChatCompletionRequestAssistantMessage
+    oneof_schema_3_validator: Optional[ChatCompletionRequestAssistantMessage] = None
+    # data type: ChatCompletionRequestToolMessage
+    oneof_schema_4_validator: Optional[ChatCompletionRequestToolMessage] = None
+    # data type: ChatCompletionRequestFunctionMessage
+    oneof_schema_5_validator: Optional[ChatCompletionRequestFunctionMessage] = None
+    actual_instance: Optional[Union[ChatCompletionRequestAssistantMessage, ChatCompletionRequestFunctionMessage, ChatCompletionRequestSystemMessage, ChatCompletionRequestToolMessage, ChatCompletionRequestUserMessage]] = None
+    one_of_schemas: List[str] = Field(default=Literal["ChatCompletionRequestAssistantMessage", "ChatCompletionRequestFunctionMessage", "ChatCompletionRequestSystemMessage", "ChatCompletionRequestToolMessage", "ChatCompletionRequestUserMessage"])
 
     model_config = ConfigDict(
-        populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
 
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
+    def __init__(self, *args, **kwargs) -> None:
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
+    @field_validator('actual_instance')
+    def actual_instance_must_validate_oneof(cls, v):
+        instance = ChatCompletionRequestMessage.model_construct()
+        error_messages = []
+        match = 0
+        # validate data type: ChatCompletionRequestSystemMessage
+        if not isinstance(v, ChatCompletionRequestSystemMessage):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ChatCompletionRequestSystemMessage`")
+        else:
+            match += 1
+        # validate data type: ChatCompletionRequestUserMessage
+        if not isinstance(v, ChatCompletionRequestUserMessage):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ChatCompletionRequestUserMessage`")
+        else:
+            match += 1
+        # validate data type: ChatCompletionRequestAssistantMessage
+        if not isinstance(v, ChatCompletionRequestAssistantMessage):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ChatCompletionRequestAssistantMessage`")
+        else:
+            match += 1
+        # validate data type: ChatCompletionRequestToolMessage
+        if not isinstance(v, ChatCompletionRequestToolMessage):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ChatCompletionRequestToolMessage`")
+        else:
+            match += 1
+        # validate data type: ChatCompletionRequestFunctionMessage
+        if not isinstance(v, ChatCompletionRequestFunctionMessage):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ChatCompletionRequestFunctionMessage`")
+        else:
+            match += 1
+        if match > 1:
+            # more than 1 match
+            raise ValueError("Multiple matches found when setting `actual_instance` in ChatCompletionRequestMessage with oneOf schemas: ChatCompletionRequestAssistantMessage, ChatCompletionRequestFunctionMessage, ChatCompletionRequestSystemMessage, ChatCompletionRequestToolMessage, ChatCompletionRequestUserMessage. Details: " + ", ".join(error_messages))
+        elif match == 0:
+            # no match
+            raise ValueError("No match found when setting `actual_instance` in ChatCompletionRequestMessage with oneOf schemas: ChatCompletionRequestAssistantMessage, ChatCompletionRequestFunctionMessage, ChatCompletionRequestSystemMessage, ChatCompletionRequestToolMessage, ChatCompletionRequestUserMessage. Details: " + ", ".join(error_messages))
+        else:
+            return v
 
     @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ChatCompletionRequestMessage from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
-
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
-        )
-        # override the default output from pydantic by calling `to_dict()` of function_call
-        if self.function_call:
-            _dict['function_call'] = self.function_call.to_dict()
-        return _dict
+    def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
+        return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ChatCompletionRequestMessage from a dict"""
-        if obj is None:
+    def from_json(cls, json_str: str) -> Self:
+        """Returns the object represented by the json string"""
+        instance = cls.model_construct()
+        error_messages = []
+        match = 0
+
+        # deserialize data into ChatCompletionRequestSystemMessage
+        try:
+            instance.actual_instance = ChatCompletionRequestSystemMessage.from_json(json_str)
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+        # deserialize data into ChatCompletionRequestUserMessage
+        try:
+            instance.actual_instance = ChatCompletionRequestUserMessage.from_json(json_str)
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+        # deserialize data into ChatCompletionRequestAssistantMessage
+        try:
+            instance.actual_instance = ChatCompletionRequestAssistantMessage.from_json(json_str)
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+        # deserialize data into ChatCompletionRequestToolMessage
+        try:
+            instance.actual_instance = ChatCompletionRequestToolMessage.from_json(json_str)
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+        # deserialize data into ChatCompletionRequestFunctionMessage
+        try:
+            instance.actual_instance = ChatCompletionRequestFunctionMessage.from_json(json_str)
+            match += 1
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+
+        if match > 1:
+            # more than 1 match
+            raise ValueError("Multiple matches found when deserializing the JSON string into ChatCompletionRequestMessage with oneOf schemas: ChatCompletionRequestAssistantMessage, ChatCompletionRequestFunctionMessage, ChatCompletionRequestSystemMessage, ChatCompletionRequestToolMessage, ChatCompletionRequestUserMessage. Details: " + ", ".join(error_messages))
+        elif match == 0:
+            # no match
+            raise ValueError("No match found when deserializing the JSON string into ChatCompletionRequestMessage with oneOf schemas: ChatCompletionRequestAssistantMessage, ChatCompletionRequestFunctionMessage, ChatCompletionRequestSystemMessage, ChatCompletionRequestToolMessage, ChatCompletionRequestUserMessage. Details: " + ", ".join(error_messages))
+        else:
+            return instance
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the actual instance"""
+        if self.actual_instance is None:
+            return "null"
+
+        if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
+            return self.actual_instance.to_json()
+        else:
+            return json.dumps(self.actual_instance)
+
+    def to_dict(self) -> Optional[Union[Dict[str, Any], ChatCompletionRequestAssistantMessage, ChatCompletionRequestFunctionMessage, ChatCompletionRequestSystemMessage, ChatCompletionRequestToolMessage, ChatCompletionRequestUserMessage]]:
+        """Returns the dict representation of the actual instance"""
+        if self.actual_instance is None:
             return None
 
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
+        if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
+            return self.actual_instance.to_dict()
+        else:
+            # primitive type
+            return self.actual_instance
 
-        _obj = cls.model_validate({
-            "role": obj.get("role"),
-            "content": obj.get("content"),
-            "name": obj.get("name"),
-            "function_call": ChatCompletionRequestMessageFunctionCall.from_dict(obj["function_call"]) if obj.get("function_call") is not None else None
-        })
-        return _obj
+    def to_str(self) -> str:
+        """Returns the string representation of the actual instance"""
+        return pprint.pformat(self.model_dump())
```

## openapiopenai/models/chat_completion_response_message.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -16,32 +16,34 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from openapiopenai.models.chat_completion_request_message_function_call import ChatCompletionRequestMessageFunctionCall
+from openapiopenai.models.chat_completion_message_tool_call import ChatCompletionMessageToolCall
+from openapiopenai.models.chat_completion_request_assistant_message_function_call import ChatCompletionRequestAssistantMessageFunctionCall
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ChatCompletionResponseMessage(BaseModel):
     """
-    ChatCompletionResponseMessage
+    A chat completion message generated by the model.
     """ # noqa: E501
+    content: Optional[StrictStr] = Field(description="The contents of the message.")
+    tool_calls: Optional[List[ChatCompletionMessageToolCall]] = Field(default=None, description="The tool calls generated by the model, such as function calls.")
     role: StrictStr = Field(description="The role of the author of this message.")
-    content: Optional[StrictStr] = Field(default=None, description="The contents of the message.")
-    function_call: Optional[ChatCompletionRequestMessageFunctionCall] = None
-    __properties: ClassVar[List[str]] = ["role", "content", "function_call"]
+    function_call: Optional[ChatCompletionRequestAssistantMessageFunctionCall] = None
+    __properties: ClassVar[List[str]] = ["content", "tool_calls", "role", "function_call"]
 
     @field_validator('role')
     def role_validate_enum(cls, value):
         """Validates the enum"""
-        if value not in set(['system', 'user', 'assistant', 'function']):
-            raise ValueError("must be one of enum values ('system', 'user', 'assistant', 'function')")
+        if value not in set(['assistant']):
+            raise ValueError("must be one of enum values ('assistant')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -75,14 +77,21 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in tool_calls (list)
+        _items = []
+        if self.tool_calls:
+            for _item in self.tool_calls:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tool_calls'] = _items
         # override the default output from pydantic by calling `to_dict()` of function_call
         if self.function_call:
             _dict['function_call'] = self.function_call.to_dict()
         # set to None if content (nullable) is None
         # and model_fields_set contains the field
         if self.content is None and "content" in self.model_fields_set:
             _dict['content'] = None
@@ -95,14 +104,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "role": obj.get("role"),
             "content": obj.get("content"),
-            "function_call": ChatCompletionRequestMessageFunctionCall.from_dict(obj["function_call"]) if obj.get("function_call") is not None else None
+            "tool_calls": [ChatCompletionMessageToolCall.from_dict(_item) for _item in obj["tool_calls"]] if obj.get("tool_calls") is not None else None,
+            "role": obj.get("role"),
+            "function_call": ChatCompletionRequestAssistantMessageFunctionCall.from_dict(obj["function_call"]) if obj.get("function_call") is not None else None
         })
         return _obj
```

## openapiopenai/models/chat_completion_stream_response_delta.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -16,35 +16,37 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from openapiopenai.models.chat_completion_request_message_function_call import ChatCompletionRequestMessageFunctionCall
+from openapiopenai.models.chat_completion_message_tool_call_chunk import ChatCompletionMessageToolCallChunk
+from openapiopenai.models.chat_completion_stream_response_delta_function_call import ChatCompletionStreamResponseDeltaFunctionCall
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ChatCompletionStreamResponseDelta(BaseModel):
     """
-    ChatCompletionStreamResponseDelta
+    A chat completion delta generated by streamed model responses.
     """ # noqa: E501
-    role: Optional[StrictStr] = Field(default=None, description="The role of the author of this message.")
     content: Optional[StrictStr] = Field(default=None, description="The contents of the chunk message.")
-    function_call: Optional[ChatCompletionRequestMessageFunctionCall] = None
-    __properties: ClassVar[List[str]] = ["role", "content", "function_call"]
+    function_call: Optional[ChatCompletionStreamResponseDeltaFunctionCall] = None
+    tool_calls: Optional[List[ChatCompletionMessageToolCallChunk]] = None
+    role: Optional[StrictStr] = Field(default=None, description="The role of the author of this message.")
+    __properties: ClassVar[List[str]] = ["content", "function_call", "tool_calls", "role"]
 
     @field_validator('role')
     def role_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['system', 'user', 'assistant', 'function']):
-            raise ValueError("must be one of enum values ('system', 'user', 'assistant', 'function')")
+        if value not in set(['system', 'user', 'assistant', 'tool']):
+            raise ValueError("must be one of enum values ('system', 'user', 'assistant', 'tool')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -81,14 +83,21 @@
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of function_call
         if self.function_call:
             _dict['function_call'] = self.function_call.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in tool_calls (list)
+        _items = []
+        if self.tool_calls:
+            for _item in self.tool_calls:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tool_calls'] = _items
         # set to None if content (nullable) is None
         # and model_fields_set contains the field
         if self.content is None and "content" in self.model_fields_set:
             _dict['content'] = None
 
         return _dict
 
@@ -98,14 +107,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "role": obj.get("role"),
             "content": obj.get("content"),
-            "function_call": ChatCompletionRequestMessageFunctionCall.from_dict(obj["function_call"]) if obj.get("function_call") is not None else None
+            "function_call": ChatCompletionStreamResponseDeltaFunctionCall.from_dict(obj["function_call"]) if obj.get("function_call") is not None else None,
+            "tool_calls": [ChatCompletionMessageToolCallChunk.from_dict(_item) for _item in obj["tool_calls"]] if obj.get("tool_calls") is not None else None,
+            "role": obj.get("role")
         })
         return _obj
```

## openapiopenai/models/create_chat_completion_request.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -19,39 +19,48 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing_extensions import Annotated
 from openapiopenai.models.chat_completion_functions import ChatCompletionFunctions
 from openapiopenai.models.chat_completion_request_message import ChatCompletionRequestMessage
+from openapiopenai.models.chat_completion_tool import ChatCompletionTool
+from openapiopenai.models.chat_completion_tool_choice_option import ChatCompletionToolChoiceOption
 from openapiopenai.models.create_chat_completion_request_function_call import CreateChatCompletionRequestFunctionCall
 from openapiopenai.models.create_chat_completion_request_model import CreateChatCompletionRequestModel
+from openapiopenai.models.create_chat_completion_request_response_format import CreateChatCompletionRequestResponseFormat
 from openapiopenai.models.create_chat_completion_request_stop import CreateChatCompletionRequestStop
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateChatCompletionRequest(BaseModel):
     """
     CreateChatCompletionRequest
     """ # noqa: E501
+    messages: Annotated[List[ChatCompletionRequestMessage], Field(min_length=1)] = Field(description="A list of messages comprising the conversation so far. [Example Python code](https://cookbook.openai.com/examples/how_to_format_inputs_to_chatgpt_models).")
     model: CreateChatCompletionRequestModel
-    messages: Annotated[List[ChatCompletionRequestMessage], Field(min_length=1)] = Field(description="A list of messages comprising the conversation so far. [Example Python code](https://github.com/openai/openai-cookbook/blob/main/examples/How_to_format_inputs_to_ChatGPT_models.ipynb).")
-    functions: Optional[Annotated[List[ChatCompletionFunctions], Field(min_length=1)]] = Field(default=None, description="A list of functions the model may generate JSON inputs for.")
-    function_call: Optional[CreateChatCompletionRequestFunctionCall] = None
+    frequency_penalty: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=-2)], Annotated[int, Field(le=2, strict=True, ge=-2)]]] = Field(default=0, description="Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim.  [See more information about frequency and presence penalties.](/docs/guides/text-generation/parameter-details) ")
+    logit_bias: Optional[Dict[str, StrictInt]] = Field(default=None, description="Modify the likelihood of specified tokens appearing in the completion.  Accepts a JSON object that maps tokens (specified by their token ID in the tokenizer) to an associated bias value from -100 to 100. Mathematically, the bias is added to the logits generated by the model prior to sampling. The exact effect will vary per model, but values between -1 and 1 should decrease or increase likelihood of selection; values like -100 or 100 should result in a ban or exclusive selection of the relevant token. ")
+    logprobs: Optional[StrictBool] = Field(default=False, description="Whether to return log probabilities of the output tokens or not. If true, returns the log probabilities of each output token returned in the `content` of `message`.")
+    top_logprobs: Optional[Annotated[int, Field(le=20, strict=True, ge=0)]] = Field(default=None, description="An integer between 0 and 20 specifying the number of most likely tokens to return at each token position, each with an associated log probability. `logprobs` must be set to `true` if this parameter is used.")
+    max_tokens: Optional[StrictInt] = Field(default=None, description="The maximum number of [tokens](/tokenizer) that can be generated in the chat completion.  The total length of input tokens and generated tokens is limited by the model's context length. [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken) for counting tokens. ")
+    n: Optional[Annotated[int, Field(le=128, strict=True, ge=1)]] = Field(default=1, description="How many chat completion choices to generate for each input message. Note that you will be charged based on the number of generated tokens across all of the choices. Keep `n` as `1` to minimize costs.")
+    presence_penalty: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=-2)], Annotated[int, Field(le=2, strict=True, ge=-2)]]] = Field(default=0, description="Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far, increasing the model's likelihood to talk about new topics.  [See more information about frequency and presence penalties.](/docs/guides/text-generation/parameter-details) ")
+    response_format: Optional[CreateChatCompletionRequestResponseFormat] = None
+    seed: Optional[Annotated[int, Field(le=9223372036854775807, strict=True, ge=-9223372036854775808)]] = Field(default=None, description="This feature is in Beta. If specified, our system will make a best effort to sample deterministically, such that repeated requests with the same `seed` and parameters should return the same result. Determinism is not guaranteed, and you should refer to the `system_fingerprint` response parameter to monitor changes in the backend. ")
+    stop: Optional[CreateChatCompletionRequestStop] = None
+    stream: Optional[StrictBool] = Field(default=False, description="If set, partial message deltas will be sent, like in ChatGPT. Tokens will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available, with the stream terminated by a `data: [DONE]` message. [Example Python code](https://cookbook.openai.com/examples/how_to_stream_completions). ")
     temperature: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=0)], Annotated[int, Field(le=2, strict=True, ge=0)]]] = Field(default=1, description="What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.  We generally recommend altering this or `top_p` but not both. ")
     top_p: Optional[Union[Annotated[float, Field(le=1, strict=True, ge=0)], Annotated[int, Field(le=1, strict=True, ge=0)]]] = Field(default=1, description="An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens comprising the top 10% probability mass are considered.  We generally recommend altering this or `temperature` but not both. ")
-    n: Optional[Annotated[int, Field(le=128, strict=True, ge=1)]] = Field(default=1, description="How many chat completion choices to generate for each input message.")
-    stream: Optional[StrictBool] = Field(default=False, description="If set, partial message deltas will be sent, like in ChatGPT. Tokens will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available, with the stream terminated by a `data: [DONE]` message. [Example Python code](https://github.com/openai/openai-cookbook/blob/main/examples/How_to_stream_completions.ipynb). ")
-    stop: Optional[CreateChatCompletionRequestStop] = None
-    max_tokens: Optional[StrictInt] = Field(default=None, description="The maximum number of [tokens](/tokenizer) to generate in the chat completion.  The total length of input tokens and generated tokens is limited by the model's context length. [Example Python code](https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb) for counting tokens. ")
-    presence_penalty: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=-2)], Annotated[int, Field(le=2, strict=True, ge=-2)]]] = Field(default=0, description="Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far, increasing the model's likelihood to talk about new topics.  [See more information about frequency and presence penalties.](/docs/api-reference/parameter-details) ")
-    frequency_penalty: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=-2)], Annotated[int, Field(le=2, strict=True, ge=-2)]]] = Field(default=0, description="Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim.  [See more information about frequency and presence penalties.](/docs/api-reference/parameter-details) ")
-    logit_bias: Optional[Dict[str, Any]] = Field(default=None, description="Modify the likelihood of specified tokens appearing in the completion.  Accepts a json object that maps tokens (specified by their token ID in the tokenizer) to an associated bias value from -100 to 100. Mathematically, the bias is added to the logits generated by the model prior to sampling. The exact effect will vary per model, but values between -1 and 1 should decrease or increase likelihood of selection; values like -100 or 100 should result in a ban or exclusive selection of the relevant token. ")
+    tools: Optional[List[ChatCompletionTool]] = Field(default=None, description="A list of tools the model may call. Currently, only functions are supported as a tool. Use this to provide a list of functions the model may generate JSON inputs for. A max of 128 functions are supported. ")
+    tool_choice: Optional[ChatCompletionToolChoiceOption] = None
     user: Optional[StrictStr] = Field(default=None, description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")
-    __properties: ClassVar[List[str]] = ["model", "messages", "functions", "function_call", "temperature", "top_p", "n", "stream", "stop", "max_tokens", "presence_penalty", "frequency_penalty", "logit_bias", "user"]
+    function_call: Optional[CreateChatCompletionRequestFunctionCall] = None
+    functions: Optional[Annotated[List[ChatCompletionFunctions], Field(min_length=1, max_length=128)]] = Field(default=None, description="Deprecated in favor of `tools`.  A list of functions the model may generate JSON inputs for. ")
+    __properties: ClassVar[List[str]] = ["messages", "model", "frequency_penalty", "logit_bias", "logprobs", "top_logprobs", "max_tokens", "n", "presence_penalty", "response_format", "seed", "stop", "stream", "temperature", "top_p", "tools", "tool_choice", "user", "function_call", "functions"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -84,95 +93,134 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of model
-        if self.model:
-            _dict['model'] = self.model.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in messages (list)
         _items = []
         if self.messages:
             for _item in self.messages:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['messages'] = _items
+        # override the default output from pydantic by calling `to_dict()` of model
+        if self.model:
+            _dict['model'] = self.model.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of response_format
+        if self.response_format:
+            _dict['response_format'] = self.response_format.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of stop
+        if self.stop:
+            _dict['stop'] = self.stop.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in tools (list)
+        _items = []
+        if self.tools:
+            for _item in self.tools:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tools'] = _items
+        # override the default output from pydantic by calling `to_dict()` of tool_choice
+        if self.tool_choice:
+            _dict['tool_choice'] = self.tool_choice.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of function_call
+        if self.function_call:
+            _dict['function_call'] = self.function_call.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in functions (list)
         _items = []
         if self.functions:
             for _item in self.functions:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['functions'] = _items
-        # override the default output from pydantic by calling `to_dict()` of function_call
-        if self.function_call:
-            _dict['function_call'] = self.function_call.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of stop
-        if self.stop:
-            _dict['stop'] = self.stop.to_dict()
-        # set to None if temperature (nullable) is None
+        # set to None if frequency_penalty (nullable) is None
         # and model_fields_set contains the field
-        if self.temperature is None and "temperature" in self.model_fields_set:
-            _dict['temperature'] = None
+        if self.frequency_penalty is None and "frequency_penalty" in self.model_fields_set:
+            _dict['frequency_penalty'] = None
 
-        # set to None if top_p (nullable) is None
+        # set to None if logit_bias (nullable) is None
         # and model_fields_set contains the field
-        if self.top_p is None and "top_p" in self.model_fields_set:
-            _dict['top_p'] = None
+        if self.logit_bias is None and "logit_bias" in self.model_fields_set:
+            _dict['logit_bias'] = None
+
+        # set to None if logprobs (nullable) is None
+        # and model_fields_set contains the field
+        if self.logprobs is None and "logprobs" in self.model_fields_set:
+            _dict['logprobs'] = None
+
+        # set to None if top_logprobs (nullable) is None
+        # and model_fields_set contains the field
+        if self.top_logprobs is None and "top_logprobs" in self.model_fields_set:
+            _dict['top_logprobs'] = None
+
+        # set to None if max_tokens (nullable) is None
+        # and model_fields_set contains the field
+        if self.max_tokens is None and "max_tokens" in self.model_fields_set:
+            _dict['max_tokens'] = None
 
         # set to None if n (nullable) is None
         # and model_fields_set contains the field
         if self.n is None and "n" in self.model_fields_set:
             _dict['n'] = None
 
-        # set to None if stream (nullable) is None
-        # and model_fields_set contains the field
-        if self.stream is None and "stream" in self.model_fields_set:
-            _dict['stream'] = None
-
         # set to None if presence_penalty (nullable) is None
         # and model_fields_set contains the field
         if self.presence_penalty is None and "presence_penalty" in self.model_fields_set:
             _dict['presence_penalty'] = None
 
-        # set to None if frequency_penalty (nullable) is None
+        # set to None if seed (nullable) is None
         # and model_fields_set contains the field
-        if self.frequency_penalty is None and "frequency_penalty" in self.model_fields_set:
-            _dict['frequency_penalty'] = None
+        if self.seed is None and "seed" in self.model_fields_set:
+            _dict['seed'] = None
 
-        # set to None if logit_bias (nullable) is None
+        # set to None if stream (nullable) is None
         # and model_fields_set contains the field
-        if self.logit_bias is None and "logit_bias" in self.model_fields_set:
-            _dict['logit_bias'] = None
+        if self.stream is None and "stream" in self.model_fields_set:
+            _dict['stream'] = None
+
+        # set to None if temperature (nullable) is None
+        # and model_fields_set contains the field
+        if self.temperature is None and "temperature" in self.model_fields_set:
+            _dict['temperature'] = None
+
+        # set to None if top_p (nullable) is None
+        # and model_fields_set contains the field
+        if self.top_p is None and "top_p" in self.model_fields_set:
+            _dict['top_p'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of CreateChatCompletionRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "model": CreateChatCompletionRequestModel.from_dict(obj["model"]) if obj.get("model") is not None else None,
             "messages": [ChatCompletionRequestMessage.from_dict(_item) for _item in obj["messages"]] if obj.get("messages") is not None else None,
-            "functions": [ChatCompletionFunctions.from_dict(_item) for _item in obj["functions"]] if obj.get("functions") is not None else None,
-            "function_call": CreateChatCompletionRequestFunctionCall.from_dict(obj["function_call"]) if obj.get("function_call") is not None else None,
-            "temperature": obj.get("temperature") if obj.get("temperature") is not None else 1,
-            "top_p": obj.get("top_p") if obj.get("top_p") is not None else 1,
-            "n": obj.get("n") if obj.get("n") is not None else 1,
-            "stream": obj.get("stream") if obj.get("stream") is not None else False,
-            "stop": CreateChatCompletionRequestStop.from_dict(obj["stop"]) if obj.get("stop") is not None else None,
-            "max_tokens": obj.get("max_tokens"),
-            "presence_penalty": obj.get("presence_penalty") if obj.get("presence_penalty") is not None else 0,
+            "model": CreateChatCompletionRequestModel.from_dict(obj["model"]) if obj.get("model") is not None else None,
             "frequency_penalty": obj.get("frequency_penalty") if obj.get("frequency_penalty") is not None else 0,
             "logit_bias": obj.get("logit_bias"),
-            "user": obj.get("user")
+            "logprobs": obj.get("logprobs") if obj.get("logprobs") is not None else False,
+            "top_logprobs": obj.get("top_logprobs"),
+            "max_tokens": obj.get("max_tokens"),
+            "n": obj.get("n") if obj.get("n") is not None else 1,
+            "presence_penalty": obj.get("presence_penalty") if obj.get("presence_penalty") is not None else 0,
+            "response_format": CreateChatCompletionRequestResponseFormat.from_dict(obj["response_format"]) if obj.get("response_format") is not None else None,
+            "seed": obj.get("seed"),
+            "stop": CreateChatCompletionRequestStop.from_dict(obj["stop"]) if obj.get("stop") is not None else None,
+            "stream": obj.get("stream") if obj.get("stream") is not None else False,
+            "temperature": obj.get("temperature") if obj.get("temperature") is not None else 1,
+            "top_p": obj.get("top_p") if obj.get("top_p") is not None else 1,
+            "tools": [ChatCompletionTool.from_dict(_item) for _item in obj["tools"]] if obj.get("tools") is not None else None,
+            "tool_choice": ChatCompletionToolChoiceOption.from_dict(obj["tool_choice"]) if obj.get("tool_choice") is not None else None,
+            "user": obj.get("user"),
+            "function_call": CreateChatCompletionRequestFunctionCall.from_dict(obj["function_call"]) if obj.get("function_call") is not None else None,
+            "functions": [ChatCompletionFunctions.from_dict(_item) for _item in obj["functions"]] if obj.get("functions") is not None else None
         })
         return _obj
```

## openapiopenai/models/create_chat_completion_request_function_call.py

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 import pprint
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
 from typing import Any, List, Optional
-from openapiopenai.models.create_chat_completion_request_function_call_one_of import CreateChatCompletionRequestFunctionCallOneOf
+from openapiopenai.models.chat_completion_function_call_option import ChatCompletionFunctionCallOption
 from pydantic import StrictStr, Field
 from typing import Union, List, Optional, Dict
 from typing_extensions import Literal, Self
 
-CREATECHATCOMPLETIONREQUESTFUNCTIONCALL_ONE_OF_SCHEMAS = ["CreateChatCompletionRequestFunctionCallOneOf", "str"]
+CREATECHATCOMPLETIONREQUESTFUNCTIONCALL_ONE_OF_SCHEMAS = ["ChatCompletionFunctionCallOption", "str"]
 
 class CreateChatCompletionRequestFunctionCall(BaseModel):
     """
-    Controls how the model responds to function calls. \"none\" means the model does not call a function, and responds to the end-user. \"auto\" means the model can pick between an end-user or calling a function.  Specifying a particular function via `{\"name\":\\ \"my_function\"}` forces the model to call that function. \"none\" is the default when no functions are present. \"auto\" is the default if functions are present.
+    Deprecated in favor of `tool_choice`.  Controls which (if any) function is called by the model. `none` means the model will not call a function and instead generates a message. `auto` means the model can pick between generating a message or calling a function. Specifying a particular function via `{\"name\": \"my_function\"}` forces the model to call that function.  `none` is the default when no functions are present. `auto` is the default if functions are present. 
     """
     # data type: str
-    oneof_schema_1_validator: Optional[StrictStr] = None
-    # data type: CreateChatCompletionRequestFunctionCallOneOf
-    oneof_schema_2_validator: Optional[CreateChatCompletionRequestFunctionCallOneOf] = None
-    actual_instance: Optional[Union[CreateChatCompletionRequestFunctionCallOneOf, str]] = None
-    one_of_schemas: List[str] = Field(default=Literal["CreateChatCompletionRequestFunctionCallOneOf", "str"])
+    oneof_schema_1_validator: Optional[StrictStr] = Field(default=None, description="`none` means the model will not call a function and instead generates a message. `auto` means the model can pick between generating a message or calling a function. ")
+    # data type: ChatCompletionFunctionCallOption
+    oneof_schema_2_validator: Optional[ChatCompletionFunctionCallOption] = None
+    actual_instance: Optional[Union[ChatCompletionFunctionCallOption, str]] = None
+    one_of_schemas: List[str] = Field(default=Literal["ChatCompletionFunctionCallOption", "str"])
 
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
     )
 
 
@@ -59,25 +59,25 @@
         match = 0
         # validate data type: str
         try:
             instance.oneof_schema_1_validator = v
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        # validate data type: CreateChatCompletionRequestFunctionCallOneOf
-        if not isinstance(v, CreateChatCompletionRequestFunctionCallOneOf):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `CreateChatCompletionRequestFunctionCallOneOf`")
+        # validate data type: ChatCompletionFunctionCallOption
+        if not isinstance(v, ChatCompletionFunctionCallOption):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ChatCompletionFunctionCallOption`")
         else:
             match += 1
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in CreateChatCompletionRequestFunctionCall with oneOf schemas: CreateChatCompletionRequestFunctionCallOneOf, str. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when setting `actual_instance` in CreateChatCompletionRequestFunctionCall with oneOf schemas: ChatCompletionFunctionCallOption, str. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in CreateChatCompletionRequestFunctionCall with oneOf schemas: CreateChatCompletionRequestFunctionCallOneOf, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting `actual_instance` in CreateChatCompletionRequestFunctionCall with oneOf schemas: ChatCompletionFunctionCallOption, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
         return cls.from_json(json.dumps(obj))
 
@@ -93,41 +93,41 @@
             # validation
             instance.oneof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.oneof_schema_1_validator
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        # deserialize data into CreateChatCompletionRequestFunctionCallOneOf
+        # deserialize data into ChatCompletionFunctionCallOption
         try:
-            instance.actual_instance = CreateChatCompletionRequestFunctionCallOneOf.from_json(json_str)
+            instance.actual_instance = ChatCompletionFunctionCallOption.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into CreateChatCompletionRequestFunctionCall with oneOf schemas: CreateChatCompletionRequestFunctionCallOneOf, str. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when deserializing the JSON string into CreateChatCompletionRequestFunctionCall with oneOf schemas: ChatCompletionFunctionCallOption, str. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into CreateChatCompletionRequestFunctionCall with oneOf schemas: CreateChatCompletionRequestFunctionCallOneOf, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into CreateChatCompletionRequestFunctionCall with oneOf schemas: ChatCompletionFunctionCallOption, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], CreateChatCompletionRequestFunctionCallOneOf, str]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], ChatCompletionFunctionCallOption, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

## openapiopenai/models/create_chat_completion_request_model.py

```diff
@@ -1,122 +1,118 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
+from inspect import getfullargspec
 import json
 import pprint
+import re  # noqa: F401
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
-from typing import Any, List, Optional
-from pydantic import StrictStr, Field
-from typing import Union, List, Optional, Dict
+from typing import Optional
+from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
+from pydantic import Field
 
-CREATECHATCOMPLETIONREQUESTMODEL_ONE_OF_SCHEMAS = ["str"]
+CREATECHATCOMPLETIONREQUESTMODEL_ANY_OF_SCHEMAS = ["str"]
 
 class CreateChatCompletionRequestModel(BaseModel):
     """
     ID of the model to use. See the [model endpoint compatibility](/docs/models/model-endpoint-compatibility) table for details on which models work with the Chat API.
     """
+
     # data type: str
-    oneof_schema_1_validator: Optional[StrictStr] = None
+    anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: str
-    oneof_schema_2_validator: Optional[StrictStr] = None
-    actual_instance: Optional[Union[str]] = None
-    one_of_schemas: List[str] = Field(default=Literal["str"])
-
-    model_config = ConfigDict(
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
-
+    anyof_schema_2_validator: Optional[StrictStr] = None
+    if TYPE_CHECKING:
+        actual_instance: Optional[Union[str]] = None
+    else:
+        actual_instance: Any = None
+    any_of_schemas: List[str] = Field(default=Literal["str"])
+
+    model_config = {
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
                 raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
             if kwargs:
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
+    def actual_instance_must_validate_anyof(cls, v):
         instance = CreateChatCompletionRequestModel.model_construct()
         error_messages = []
-        match = 0
         # validate data type: str
         try:
-            instance.oneof_schema_1_validator = v
-            match += 1
+            instance.anyof_schema_1_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # validate data type: str
         try:
-            instance.oneof_schema_2_validator = v
-            match += 1
+            instance.anyof_schema_2_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in CreateChatCompletionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in CreateChatCompletionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in CreateChatCompletionRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
+    def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        match = 0
-
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_1_validator = json.loads(json_str)
+            instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_1_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_1_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_2_validator = json.loads(json_str)
+            instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_2_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_2_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into CreateChatCompletionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into CreateChatCompletionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into CreateChatCompletionRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
@@ -130,15 +126,14 @@
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
-            # primitive type
             return self.actual_instance
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.model_dump())
```

## openapiopenai/models/create_chat_completion_request_stop.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## openapiopenai/models/create_chat_completion_response.py

```diff
@@ -1,45 +1,53 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
+from openapiopenai.models.completion_usage import CompletionUsage
 from openapiopenai.models.create_chat_completion_response_choices_inner import CreateChatCompletionResponseChoicesInner
-from openapiopenai.models.create_completion_response_usage import CreateCompletionResponseUsage
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateChatCompletionResponse(BaseModel):
     """
-    CreateChatCompletionResponse
+    Represents a chat completion response returned by model, based on the provided input.
     """ # noqa: E501
-    id: StrictStr
-    object: StrictStr
-    created: StrictInt
-    model: StrictStr
-    choices: List[CreateChatCompletionResponseChoicesInner]
-    usage: Optional[CreateCompletionResponseUsage] = None
-    __properties: ClassVar[List[str]] = ["id", "object", "created", "model", "choices", "usage"]
+    id: StrictStr = Field(description="A unique identifier for the chat completion.")
+    choices: List[CreateChatCompletionResponseChoicesInner] = Field(description="A list of chat completion choices. Can be more than one if `n` is greater than 1.")
+    created: StrictInt = Field(description="The Unix timestamp (in seconds) of when the chat completion was created.")
+    model: StrictStr = Field(description="The model used for the chat completion.")
+    system_fingerprint: Optional[StrictStr] = Field(default=None, description="This fingerprint represents the backend configuration that the model runs with.  Can be used in conjunction with the `seed` request parameter to understand when backend changes have been made that might impact determinism. ")
+    object: StrictStr = Field(description="The object type, which is always `chat.completion`.")
+    usage: Optional[CompletionUsage] = None
+    __properties: ClassVar[List[str]] = ["id", "choices", "created", "model", "system_fingerprint", "object", "usage"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['chat.completion']):
+            raise ValueError("must be one of enum values ('chat.completion')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -95,16 +103,17 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "object": obj.get("object"),
+            "choices": [CreateChatCompletionResponseChoicesInner.from_dict(_item) for _item in obj["choices"]] if obj.get("choices") is not None else None,
             "created": obj.get("created"),
             "model": obj.get("model"),
-            "choices": [CreateChatCompletionResponseChoicesInner.from_dict(_item) for _item in obj["choices"]] if obj.get("choices") is not None else None,
-            "usage": CreateCompletionResponseUsage.from_dict(obj["usage"]) if obj.get("usage") is not None else None
+            "system_fingerprint": obj.get("system_fingerprint"),
+            "object": obj.get("object"),
+            "usage": CompletionUsage.from_dict(obj["usage"]) if obj.get("usage") is not None else None
         })
         return _obj
```

## openapiopenai/models/create_chat_completion_response_choices_inner.py

```diff
@@ -1,50 +1,49 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from openapiopenai.models.chat_completion_response_message import ChatCompletionResponseMessage
+from openapiopenai.models.create_chat_completion_response_choices_inner_logprobs import CreateChatCompletionResponseChoicesInnerLogprobs
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateChatCompletionResponseChoicesInner(BaseModel):
     """
     CreateChatCompletionResponseChoicesInner
     """ # noqa: E501
-    index: Optional[StrictInt] = None
-    message: Optional[ChatCompletionResponseMessage] = None
-    finish_reason: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["index", "message", "finish_reason"]
+    finish_reason: StrictStr = Field(description="The reason the model stopped generating tokens. This will be `stop` if the model hit a natural stop point or a provided stop sequence, `length` if the maximum number of tokens specified in the request was reached, `content_filter` if content was omitted due to a flag from our content filters, `tool_calls` if the model called a tool, or `function_call` (deprecated) if the model called a function. ")
+    index: StrictInt = Field(description="The index of the choice in the list of choices.")
+    message: ChatCompletionResponseMessage
+    logprobs: Optional[CreateChatCompletionResponseChoicesInnerLogprobs]
+    __properties: ClassVar[List[str]] = ["finish_reason", "index", "message", "logprobs"]
 
     @field_validator('finish_reason')
     def finish_reason_validate_enum(cls, value):
         """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['stop', 'length', 'function_call']):
-            raise ValueError("must be one of enum values ('stop', 'length', 'function_call')")
+        if value not in set(['stop', 'length', 'tool_calls', 'content_filter', 'function_call']):
+            raise ValueError("must be one of enum values ('stop', 'length', 'tool_calls', 'content_filter', 'function_call')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -81,26 +80,35 @@
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of message
         if self.message:
             _dict['message'] = self.message.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of logprobs
+        if self.logprobs:
+            _dict['logprobs'] = self.logprobs.to_dict()
+        # set to None if logprobs (nullable) is None
+        # and model_fields_set contains the field
+        if self.logprobs is None and "logprobs" in self.model_fields_set:
+            _dict['logprobs'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of CreateChatCompletionResponseChoicesInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "finish_reason": obj.get("finish_reason"),
             "index": obj.get("index"),
             "message": ChatCompletionResponseMessage.from_dict(obj["message"]) if obj.get("message") is not None else None,
-            "finish_reason": obj.get("finish_reason")
+            "logprobs": CreateChatCompletionResponseChoicesInnerLogprobs.from_dict(obj["logprobs"]) if obj.get("logprobs") is not None else None
         })
         return _obj
```

## openapiopenai/models/create_chat_completion_stream_response.py

```diff
@@ -1,43 +1,51 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List, Optional
 from openapiopenai.models.create_chat_completion_stream_response_choices_inner import CreateChatCompletionStreamResponseChoicesInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateChatCompletionStreamResponse(BaseModel):
     """
-    CreateChatCompletionStreamResponse
+    Represents a streamed chunk of a chat completion response returned by model, based on the provided input.
     """ # noqa: E501
-    id: StrictStr
-    object: StrictStr
-    created: StrictInt
-    model: StrictStr
-    choices: List[CreateChatCompletionStreamResponseChoicesInner]
-    __properties: ClassVar[List[str]] = ["id", "object", "created", "model", "choices"]
+    id: StrictStr = Field(description="A unique identifier for the chat completion. Each chunk has the same ID.")
+    choices: List[CreateChatCompletionStreamResponseChoicesInner] = Field(description="A list of chat completion choices. Can be more than one if `n` is greater than 1.")
+    created: StrictInt = Field(description="The Unix timestamp (in seconds) of when the chat completion was created. Each chunk has the same timestamp.")
+    model: StrictStr = Field(description="The model to generate the completion.")
+    system_fingerprint: Optional[StrictStr] = Field(default=None, description="This fingerprint represents the backend configuration that the model runs with. Can be used in conjunction with the `seed` request parameter to understand when backend changes have been made that might impact determinism. ")
+    object: StrictStr = Field(description="The object type, which is always `chat.completion.chunk`.")
+    __properties: ClassVar[List[str]] = ["id", "choices", "created", "model", "system_fingerprint", "object"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['chat.completion.chunk']):
+            raise ValueError("must be one of enum values ('chat.completion.chunk')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -90,15 +98,16 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "object": obj.get("object"),
+            "choices": [CreateChatCompletionStreamResponseChoicesInner.from_dict(_item) for _item in obj["choices"]] if obj.get("choices") is not None else None,
             "created": obj.get("created"),
             "model": obj.get("model"),
-            "choices": [CreateChatCompletionStreamResponseChoicesInner.from_dict(_item) for _item in obj["choices"]] if obj.get("choices") is not None else None
+            "system_fingerprint": obj.get("system_fingerprint"),
+            "object": obj.get("object")
         })
         return _obj
```

## openapiopenai/models/create_chat_completion_stream_response_choices_inner.py

```diff
@@ -1,50 +1,52 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from openapiopenai.models.chat_completion_stream_response_delta import ChatCompletionStreamResponseDelta
+from openapiopenai.models.create_chat_completion_response_choices_inner_logprobs import CreateChatCompletionResponseChoicesInnerLogprobs
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateChatCompletionStreamResponseChoicesInner(BaseModel):
     """
     CreateChatCompletionStreamResponseChoicesInner
     """ # noqa: E501
-    index: Optional[StrictInt] = None
-    delta: Optional[ChatCompletionStreamResponseDelta] = None
-    finish_reason: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["index", "delta", "finish_reason"]
+    delta: ChatCompletionStreamResponseDelta
+    logprobs: Optional[CreateChatCompletionResponseChoicesInnerLogprobs] = None
+    finish_reason: Optional[StrictStr] = Field(description="The reason the model stopped generating tokens. This will be `stop` if the model hit a natural stop point or a provided stop sequence, `length` if the maximum number of tokens specified in the request was reached, `content_filter` if content was omitted due to a flag from our content filters, `tool_calls` if the model called a tool, or `function_call` (deprecated) if the model called a function. ")
+    index: StrictInt = Field(description="The index of the choice in the list of choices.")
+    __properties: ClassVar[List[str]] = ["delta", "logprobs", "finish_reason", "index"]
 
     @field_validator('finish_reason')
     def finish_reason_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['stop', 'length', 'function_call']):
-            raise ValueError("must be one of enum values ('stop', 'length', 'function_call')")
+        if value not in set(['stop', 'length', 'tool_calls', 'content_filter', 'function_call']):
+            raise ValueError("must be one of enum values ('stop', 'length', 'tool_calls', 'content_filter', 'function_call')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -81,26 +83,40 @@
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of delta
         if self.delta:
             _dict['delta'] = self.delta.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of logprobs
+        if self.logprobs:
+            _dict['logprobs'] = self.logprobs.to_dict()
+        # set to None if logprobs (nullable) is None
+        # and model_fields_set contains the field
+        if self.logprobs is None and "logprobs" in self.model_fields_set:
+            _dict['logprobs'] = None
+
+        # set to None if finish_reason (nullable) is None
+        # and model_fields_set contains the field
+        if self.finish_reason is None and "finish_reason" in self.model_fields_set:
+            _dict['finish_reason'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of CreateChatCompletionStreamResponseChoicesInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "index": obj.get("index"),
             "delta": ChatCompletionStreamResponseDelta.from_dict(obj["delta"]) if obj.get("delta") is not None else None,
-            "finish_reason": obj.get("finish_reason")
+            "logprobs": CreateChatCompletionResponseChoicesInnerLogprobs.from_dict(obj["logprobs"]) if obj.get("logprobs") is not None else None,
+            "finish_reason": obj.get("finish_reason"),
+            "index": obj.get("index")
         })
         return _obj
```

## openapiopenai/models/create_completion_request.py

```diff
@@ -1,57 +1,58 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing_extensions import Annotated
 from openapiopenai.models.create_completion_request_model import CreateCompletionRequestModel
 from openapiopenai.models.create_completion_request_prompt import CreateCompletionRequestPrompt
 from openapiopenai.models.create_completion_request_stop import CreateCompletionRequestStop
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateCompletionRequest(BaseModel):
     """
     CreateCompletionRequest
     """ # noqa: E501
     model: CreateCompletionRequestModel
     prompt: Optional[CreateCompletionRequestPrompt]
-    suffix: Optional[StrictStr] = Field(default=None, description="The suffix that comes after a completion of inserted text.")
-    max_tokens: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=16, description="The maximum number of [tokens](/tokenizer) to generate in the completion.  The token count of your prompt plus `max_tokens` cannot exceed the model's context length. [Example Python code](https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb) for counting tokens. ")
-    temperature: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=0)], Annotated[int, Field(le=2, strict=True, ge=0)]]] = Field(default=1, description="What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.  We generally recommend altering this or `top_p` but not both. ")
-    top_p: Optional[Union[Annotated[float, Field(le=1, strict=True, ge=0)], Annotated[int, Field(le=1, strict=True, ge=0)]]] = Field(default=1, description="An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens comprising the top 10% probability mass are considered.  We generally recommend altering this or `temperature` but not both. ")
-    n: Optional[Annotated[int, Field(le=128, strict=True, ge=1)]] = Field(default=1, description="How many completions to generate for each prompt.  **Note:** Because this parameter generates many completions, it can quickly consume your token quota. Use carefully and ensure that you have reasonable settings for `max_tokens` and `stop`. ")
-    stream: Optional[StrictBool] = Field(default=False, description="Whether to stream back partial progress. If set, tokens will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available, with the stream terminated by a `data: [DONE]` message. [Example Python code](https://github.com/openai/openai-cookbook/blob/main/examples/How_to_stream_completions.ipynb). ")
-    logprobs: Optional[Annotated[int, Field(le=5, strict=True, ge=0)]] = Field(default=None, description="Include the log probabilities on the `logprobs` most likely tokens, as well the chosen tokens. For example, if `logprobs` is 5, the API will return a list of the 5 most likely tokens. The API will always return the `logprob` of the sampled token, so there may be up to `logprobs+1` elements in the response.  The maximum value for `logprobs` is 5. ")
+    best_of: Optional[Annotated[int, Field(le=20, strict=True, ge=0)]] = Field(default=1, description="Generates `best_of` completions server-side and returns the \"best\" (the one with the highest log probability per token). Results cannot be streamed.  When used with `n`, `best_of` controls the number of candidate completions and `n` specifies how many to return – `best_of` must be greater than `n`.  **Note:** Because this parameter generates many completions, it can quickly consume your token quota. Use carefully and ensure that you have reasonable settings for `max_tokens` and `stop`. ")
     echo: Optional[StrictBool] = Field(default=False, description="Echo back the prompt in addition to the completion ")
+    frequency_penalty: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=-2)], Annotated[int, Field(le=2, strict=True, ge=-2)]]] = Field(default=0, description="Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim.  [See more information about frequency and presence penalties.](/docs/guides/text-generation/parameter-details) ")
+    logit_bias: Optional[Dict[str, StrictInt]] = Field(default=None, description="Modify the likelihood of specified tokens appearing in the completion.  Accepts a JSON object that maps tokens (specified by their token ID in the GPT tokenizer) to an associated bias value from -100 to 100. You can use this [tokenizer tool](/tokenizer?view=bpe) to convert text to token IDs. Mathematically, the bias is added to the logits generated by the model prior to sampling. The exact effect will vary per model, but values between -1 and 1 should decrease or increase likelihood of selection; values like -100 or 100 should result in a ban or exclusive selection of the relevant token.  As an example, you can pass `{\"50256\": -100}` to prevent the <|endoftext|> token from being generated. ")
+    logprobs: Optional[Annotated[int, Field(le=5, strict=True, ge=0)]] = Field(default=None, description="Include the log probabilities on the `logprobs` most likely output tokens, as well the chosen tokens. For example, if `logprobs` is 5, the API will return a list of the 5 most likely tokens. The API will always return the `logprob` of the sampled token, so there may be up to `logprobs+1` elements in the response.  The maximum value for `logprobs` is 5. ")
+    max_tokens: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(default=16, description="The maximum number of [tokens](/tokenizer) that can be generated in the completion.  The token count of your prompt plus `max_tokens` cannot exceed the model's context length. [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken) for counting tokens. ")
+    n: Optional[Annotated[int, Field(le=128, strict=True, ge=1)]] = Field(default=1, description="How many completions to generate for each prompt.  **Note:** Because this parameter generates many completions, it can quickly consume your token quota. Use carefully and ensure that you have reasonable settings for `max_tokens` and `stop`. ")
+    presence_penalty: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=-2)], Annotated[int, Field(le=2, strict=True, ge=-2)]]] = Field(default=0, description="Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far, increasing the model's likelihood to talk about new topics.  [See more information about frequency and presence penalties.](/docs/guides/text-generation/parameter-details) ")
+    seed: Optional[Annotated[int, Field(le=9223372036854775807, strict=True, ge=-9223372036854775808)]] = Field(default=None, description="If specified, our system will make a best effort to sample deterministically, such that repeated requests with the same `seed` and parameters should return the same result.  Determinism is not guaranteed, and you should refer to the `system_fingerprint` response parameter to monitor changes in the backend. ")
     stop: Optional[CreateCompletionRequestStop] = None
-    presence_penalty: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=-2)], Annotated[int, Field(le=2, strict=True, ge=-2)]]] = Field(default=0, description="Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far, increasing the model's likelihood to talk about new topics.  [See more information about frequency and presence penalties.](/docs/api-reference/parameter-details) ")
-    frequency_penalty: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=-2)], Annotated[int, Field(le=2, strict=True, ge=-2)]]] = Field(default=0, description="Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim.  [See more information about frequency and presence penalties.](/docs/api-reference/parameter-details) ")
-    best_of: Optional[Annotated[int, Field(le=20, strict=True, ge=0)]] = Field(default=1, description="Generates `best_of` completions server-side and returns the \"best\" (the one with the highest log probability per token). Results cannot be streamed.  When used with `n`, `best_of` controls the number of candidate completions and `n` specifies how many to return – `best_of` must be greater than `n`.  **Note:** Because this parameter generates many completions, it can quickly consume your token quota. Use carefully and ensure that you have reasonable settings for `max_tokens` and `stop`. ")
-    logit_bias: Optional[Dict[str, Any]] = Field(default=None, description="Modify the likelihood of specified tokens appearing in the completion.  Accepts a json object that maps tokens (specified by their token ID in the GPT tokenizer) to an associated bias value from -100 to 100. You can use this [tokenizer tool](/tokenizer?view=bpe) (which works for both GPT-2 and GPT-3) to convert text to token IDs. Mathematically, the bias is added to the logits generated by the model prior to sampling. The exact effect will vary per model, but values between -1 and 1 should decrease or increase likelihood of selection; values like -100 or 100 should result in a ban or exclusive selection of the relevant token.  As an example, you can pass `{\"50256\": -100}` to prevent the <|endoftext|> token from being generated. ")
+    stream: Optional[StrictBool] = Field(default=False, description="Whether to stream back partial progress. If set, tokens will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available, with the stream terminated by a `data: [DONE]` message. [Example Python code](https://cookbook.openai.com/examples/how_to_stream_completions). ")
+    suffix: Optional[StrictStr] = Field(default=None, description="The suffix that comes after a completion of inserted text.  This parameter is only supported for `gpt-3.5-turbo-instruct`. ")
+    temperature: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=0)], Annotated[int, Field(le=2, strict=True, ge=0)]]] = Field(default=1, description="What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.  We generally recommend altering this or `top_p` but not both. ")
+    top_p: Optional[Union[Annotated[float, Field(le=1, strict=True, ge=0)], Annotated[int, Field(le=1, strict=True, ge=0)]]] = Field(default=1, description="An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens comprising the top 10% probability mass are considered.  We generally recommend altering this or `temperature` but not both. ")
     user: Optional[StrictStr] = Field(default=None, description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")
-    __properties: ClassVar[List[str]] = ["model", "prompt", "suffix", "max_tokens", "temperature", "top_p", "n", "stream", "logprobs", "echo", "stop", "presence_penalty", "frequency_penalty", "best_of", "logit_bias", "user"]
+    __properties: ClassVar[List[str]] = ["model", "prompt", "best_of", "echo", "frequency_penalty", "logit_bias", "logprobs", "max_tokens", "n", "presence_penalty", "seed", "stop", "stream", "suffix", "temperature", "top_p", "user"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -98,78 +99,83 @@
         if self.stop:
             _dict['stop'] = self.stop.to_dict()
         # set to None if prompt (nullable) is None
         # and model_fields_set contains the field
         if self.prompt is None and "prompt" in self.model_fields_set:
             _dict['prompt'] = None
 
-        # set to None if suffix (nullable) is None
+        # set to None if best_of (nullable) is None
         # and model_fields_set contains the field
-        if self.suffix is None and "suffix" in self.model_fields_set:
-            _dict['suffix'] = None
+        if self.best_of is None and "best_of" in self.model_fields_set:
+            _dict['best_of'] = None
 
-        # set to None if max_tokens (nullable) is None
+        # set to None if echo (nullable) is None
         # and model_fields_set contains the field
-        if self.max_tokens is None and "max_tokens" in self.model_fields_set:
-            _dict['max_tokens'] = None
+        if self.echo is None and "echo" in self.model_fields_set:
+            _dict['echo'] = None
 
-        # set to None if temperature (nullable) is None
+        # set to None if frequency_penalty (nullable) is None
         # and model_fields_set contains the field
-        if self.temperature is None and "temperature" in self.model_fields_set:
-            _dict['temperature'] = None
+        if self.frequency_penalty is None and "frequency_penalty" in self.model_fields_set:
+            _dict['frequency_penalty'] = None
 
-        # set to None if top_p (nullable) is None
+        # set to None if logit_bias (nullable) is None
         # and model_fields_set contains the field
-        if self.top_p is None and "top_p" in self.model_fields_set:
-            _dict['top_p'] = None
+        if self.logit_bias is None and "logit_bias" in self.model_fields_set:
+            _dict['logit_bias'] = None
+
+        # set to None if logprobs (nullable) is None
+        # and model_fields_set contains the field
+        if self.logprobs is None and "logprobs" in self.model_fields_set:
+            _dict['logprobs'] = None
+
+        # set to None if max_tokens (nullable) is None
+        # and model_fields_set contains the field
+        if self.max_tokens is None and "max_tokens" in self.model_fields_set:
+            _dict['max_tokens'] = None
 
         # set to None if n (nullable) is None
         # and model_fields_set contains the field
         if self.n is None and "n" in self.model_fields_set:
             _dict['n'] = None
 
-        # set to None if stream (nullable) is None
-        # and model_fields_set contains the field
-        if self.stream is None and "stream" in self.model_fields_set:
-            _dict['stream'] = None
-
-        # set to None if logprobs (nullable) is None
+        # set to None if presence_penalty (nullable) is None
         # and model_fields_set contains the field
-        if self.logprobs is None and "logprobs" in self.model_fields_set:
-            _dict['logprobs'] = None
+        if self.presence_penalty is None and "presence_penalty" in self.model_fields_set:
+            _dict['presence_penalty'] = None
 
-        # set to None if echo (nullable) is None
+        # set to None if seed (nullable) is None
         # and model_fields_set contains the field
-        if self.echo is None and "echo" in self.model_fields_set:
-            _dict['echo'] = None
+        if self.seed is None and "seed" in self.model_fields_set:
+            _dict['seed'] = None
 
         # set to None if stop (nullable) is None
         # and model_fields_set contains the field
         if self.stop is None and "stop" in self.model_fields_set:
             _dict['stop'] = None
 
-        # set to None if presence_penalty (nullable) is None
+        # set to None if stream (nullable) is None
         # and model_fields_set contains the field
-        if self.presence_penalty is None and "presence_penalty" in self.model_fields_set:
-            _dict['presence_penalty'] = None
+        if self.stream is None and "stream" in self.model_fields_set:
+            _dict['stream'] = None
 
-        # set to None if frequency_penalty (nullable) is None
+        # set to None if suffix (nullable) is None
         # and model_fields_set contains the field
-        if self.frequency_penalty is None and "frequency_penalty" in self.model_fields_set:
-            _dict['frequency_penalty'] = None
+        if self.suffix is None and "suffix" in self.model_fields_set:
+            _dict['suffix'] = None
 
-        # set to None if best_of (nullable) is None
+        # set to None if temperature (nullable) is None
         # and model_fields_set contains the field
-        if self.best_of is None and "best_of" in self.model_fields_set:
-            _dict['best_of'] = None
+        if self.temperature is None and "temperature" in self.model_fields_set:
+            _dict['temperature'] = None
 
-        # set to None if logit_bias (nullable) is None
+        # set to None if top_p (nullable) is None
         # and model_fields_set contains the field
-        if self.logit_bias is None and "logit_bias" in self.model_fields_set:
-            _dict['logit_bias'] = None
+        if self.top_p is None and "top_p" in self.model_fields_set:
+            _dict['top_p'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of CreateCompletionRequest from a dict"""
         if obj is None:
@@ -177,25 +183,26 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "model": CreateCompletionRequestModel.from_dict(obj["model"]) if obj.get("model") is not None else None,
             "prompt": CreateCompletionRequestPrompt.from_dict(obj["prompt"]) if obj.get("prompt") is not None else None,
-            "suffix": obj.get("suffix"),
-            "max_tokens": obj.get("max_tokens") if obj.get("max_tokens") is not None else 16,
-            "temperature": obj.get("temperature") if obj.get("temperature") is not None else 1,
-            "top_p": obj.get("top_p") if obj.get("top_p") is not None else 1,
-            "n": obj.get("n") if obj.get("n") is not None else 1,
-            "stream": obj.get("stream") if obj.get("stream") is not None else False,
-            "logprobs": obj.get("logprobs"),
+            "best_of": obj.get("best_of") if obj.get("best_of") is not None else 1,
             "echo": obj.get("echo") if obj.get("echo") is not None else False,
-            "stop": CreateCompletionRequestStop.from_dict(obj["stop"]) if obj.get("stop") is not None else None,
-            "presence_penalty": obj.get("presence_penalty") if obj.get("presence_penalty") is not None else 0,
             "frequency_penalty": obj.get("frequency_penalty") if obj.get("frequency_penalty") is not None else 0,
-            "best_of": obj.get("best_of") if obj.get("best_of") is not None else 1,
             "logit_bias": obj.get("logit_bias"),
+            "logprobs": obj.get("logprobs"),
+            "max_tokens": obj.get("max_tokens") if obj.get("max_tokens") is not None else 16,
+            "n": obj.get("n") if obj.get("n") is not None else 1,
+            "presence_penalty": obj.get("presence_penalty") if obj.get("presence_penalty") is not None else 0,
+            "seed": obj.get("seed"),
+            "stop": CreateCompletionRequestStop.from_dict(obj["stop"]) if obj.get("stop") is not None else None,
+            "stream": obj.get("stream") if obj.get("stream") is not None else False,
+            "suffix": obj.get("suffix"),
+            "temperature": obj.get("temperature") if obj.get("temperature") is not None else 1,
+            "top_p": obj.get("top_p") if obj.get("top_p") is not None else 1,
             "user": obj.get("user")
         })
         return _obj
```

## openapiopenai/models/create_completion_request_model.py

```diff
@@ -1,122 +1,118 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
+from inspect import getfullargspec
 import json
 import pprint
+import re  # noqa: F401
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
-from typing import Any, List, Optional
-from pydantic import StrictStr, Field
-from typing import Union, List, Optional, Dict
+from typing import Optional
+from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
+from pydantic import Field
 
-CREATECOMPLETIONREQUESTMODEL_ONE_OF_SCHEMAS = ["str"]
+CREATECOMPLETIONREQUESTMODEL_ANY_OF_SCHEMAS = ["str"]
 
 class CreateCompletionRequestModel(BaseModel):
     """
     ID of the model to use. You can use the [List models](/docs/api-reference/models/list) API to see all of your available models, or see our [Model overview](/docs/models/overview) for descriptions of them. 
     """
+
     # data type: str
-    oneof_schema_1_validator: Optional[StrictStr] = None
+    anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: str
-    oneof_schema_2_validator: Optional[StrictStr] = None
-    actual_instance: Optional[Union[str]] = None
-    one_of_schemas: List[str] = Field(default=Literal["str"])
-
-    model_config = ConfigDict(
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
-
+    anyof_schema_2_validator: Optional[StrictStr] = None
+    if TYPE_CHECKING:
+        actual_instance: Optional[Union[str]] = None
+    else:
+        actual_instance: Any = None
+    any_of_schemas: List[str] = Field(default=Literal["str"])
+
+    model_config = {
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
                 raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
             if kwargs:
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
+    def actual_instance_must_validate_anyof(cls, v):
         instance = CreateCompletionRequestModel.model_construct()
         error_messages = []
-        match = 0
         # validate data type: str
         try:
-            instance.oneof_schema_1_validator = v
-            match += 1
+            instance.anyof_schema_1_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # validate data type: str
         try:
-            instance.oneof_schema_2_validator = v
-            match += 1
+            instance.anyof_schema_2_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in CreateCompletionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in CreateCompletionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in CreateCompletionRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
+    def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        match = 0
-
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_1_validator = json.loads(json_str)
+            instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_1_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_1_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_2_validator = json.loads(json_str)
+            instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_2_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_2_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into CreateCompletionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into CreateCompletionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into CreateCompletionRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
@@ -130,15 +126,14 @@
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
-            # primitive type
             return self.actual_instance
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.model_dump())
```

## openapiopenai/models/create_completion_request_prompt.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## openapiopenai/models/create_completion_request_stop.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## openapiopenai/models/create_completion_response.py

```diff
@@ -1,45 +1,53 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
+from openapiopenai.models.completion_usage import CompletionUsage
 from openapiopenai.models.create_completion_response_choices_inner import CreateCompletionResponseChoicesInner
-from openapiopenai.models.create_completion_response_usage import CreateCompletionResponseUsage
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateCompletionResponse(BaseModel):
     """
-    CreateCompletionResponse
+    Represents a completion response from the API. Note: both the streamed and non-streamed response objects share the same shape (unlike the chat endpoint). 
     """ # noqa: E501
-    id: StrictStr
-    object: StrictStr
-    created: StrictInt
-    model: StrictStr
-    choices: List[CreateCompletionResponseChoicesInner]
-    usage: Optional[CreateCompletionResponseUsage] = None
-    __properties: ClassVar[List[str]] = ["id", "object", "created", "model", "choices", "usage"]
+    id: StrictStr = Field(description="A unique identifier for the completion.")
+    choices: List[CreateCompletionResponseChoicesInner] = Field(description="The list of completion choices the model generated for the input prompt.")
+    created: StrictInt = Field(description="The Unix timestamp (in seconds) of when the completion was created.")
+    model: StrictStr = Field(description="The model used for completion.")
+    system_fingerprint: Optional[StrictStr] = Field(default=None, description="This fingerprint represents the backend configuration that the model runs with.  Can be used in conjunction with the `seed` request parameter to understand when backend changes have been made that might impact determinism. ")
+    object: StrictStr = Field(description="The object type, which is always \"text_completion\"")
+    usage: Optional[CompletionUsage] = None
+    __properties: ClassVar[List[str]] = ["id", "choices", "created", "model", "system_fingerprint", "object", "usage"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['text_completion']):
+            raise ValueError("must be one of enum values ('text_completion')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -95,16 +103,17 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "object": obj.get("object"),
+            "choices": [CreateCompletionResponseChoicesInner.from_dict(_item) for _item in obj["choices"]] if obj.get("choices") is not None else None,
             "created": obj.get("created"),
             "model": obj.get("model"),
-            "choices": [CreateCompletionResponseChoicesInner.from_dict(_item) for _item in obj["choices"]] if obj.get("choices") is not None else None,
-            "usage": CreateCompletionResponseUsage.from_dict(obj["usage"]) if obj.get("usage") is not None else None
+            "system_fingerprint": obj.get("system_fingerprint"),
+            "object": obj.get("object"),
+            "usage": CompletionUsage.from_dict(obj["usage"]) if obj.get("usage") is not None else None
         })
         return _obj
```

## openapiopenai/models/create_completion_response_choices_inner.py

```diff
@@ -1,48 +1,48 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from openapiopenai.models.create_completion_response_choices_inner_logprobs import CreateCompletionResponseChoicesInnerLogprobs
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateCompletionResponseChoicesInner(BaseModel):
     """
     CreateCompletionResponseChoicesInner
     """ # noqa: E501
-    text: StrictStr
+    finish_reason: StrictStr = Field(description="The reason the model stopped generating tokens. This will be `stop` if the model hit a natural stop point or a provided stop sequence, `length` if the maximum number of tokens specified in the request was reached, or `content_filter` if content was omitted due to a flag from our content filters. ")
     index: StrictInt
     logprobs: Optional[CreateCompletionResponseChoicesInnerLogprobs]
-    finish_reason: StrictStr
-    __properties: ClassVar[List[str]] = ["text", "index", "logprobs", "finish_reason"]
+    text: StrictStr
+    __properties: ClassVar[List[str]] = ["finish_reason", "index", "logprobs", "text"]
 
     @field_validator('finish_reason')
     def finish_reason_validate_enum(cls, value):
         """Validates the enum"""
-        if value not in set(['stop', 'length']):
-            raise ValueError("must be one of enum values ('stop', 'length')")
+        if value not in set(['stop', 'length', 'content_filter']):
+            raise ValueError("must be one of enum values ('stop', 'length', 'content_filter')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -96,15 +96,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "text": obj.get("text"),
+            "finish_reason": obj.get("finish_reason"),
             "index": obj.get("index"),
             "logprobs": CreateCompletionResponseChoicesInnerLogprobs.from_dict(obj["logprobs"]) if obj.get("logprobs") is not None else None,
-            "finish_reason": obj.get("finish_reason")
+            "text": obj.get("text")
         })
         return _obj
```

## openapiopenai/models/create_completion_response_choices_inner_logprobs.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -23,19 +23,19 @@
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateCompletionResponseChoicesInnerLogprobs(BaseModel):
     """
     CreateCompletionResponseChoicesInnerLogprobs
     """ # noqa: E501
-    tokens: Optional[List[StrictStr]] = None
-    token_logprobs: Optional[List[Union[StrictFloat, StrictInt]]] = None
-    top_logprobs: Optional[List[Dict[str, Any]]] = None
     text_offset: Optional[List[StrictInt]] = None
-    __properties: ClassVar[List[str]] = ["tokens", "token_logprobs", "top_logprobs", "text_offset"]
+    token_logprobs: Optional[List[Union[StrictFloat, StrictInt]]] = None
+    tokens: Optional[List[StrictStr]] = None
+    top_logprobs: Optional[List[Dict[str, Union[StrictFloat, StrictInt]]]] = None
+    __properties: ClassVar[List[str]] = ["text_offset", "token_logprobs", "tokens", "top_logprobs"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -80,15 +80,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "tokens": obj.get("tokens"),
+            "text_offset": obj.get("text_offset"),
             "token_logprobs": obj.get("token_logprobs"),
-            "top_logprobs": obj.get("top_logprobs"),
-            "text_offset": obj.get("text_offset")
+            "tokens": obj.get("tokens"),
+            "top_logprobs": obj.get("top_logprobs")
         })
         return _obj
```

## openapiopenai/models/create_embedding_request.py

```diff
@@ -1,42 +1,55 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
+from typing_extensions import Annotated
 from openapiopenai.models.create_embedding_request_input import CreateEmbeddingRequestInput
 from openapiopenai.models.create_embedding_request_model import CreateEmbeddingRequestModel
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateEmbeddingRequest(BaseModel):
     """
     CreateEmbeddingRequest
     """ # noqa: E501
-    model: CreateEmbeddingRequestModel
     input: CreateEmbeddingRequestInput
+    model: CreateEmbeddingRequestModel
+    encoding_format: Optional[StrictStr] = Field(default='float', description="The format to return the embeddings in. Can be either `float` or [`base64`](https://pypi.org/project/pybase64/).")
+    dimensions: Optional[Annotated[int, Field(strict=True, ge=1)]] = Field(default=None, description="The number of dimensions the resulting output embeddings should have. Only supported in `text-embedding-3` and later models. ")
     user: Optional[StrictStr] = Field(default=None, description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")
-    __properties: ClassVar[List[str]] = ["model", "input", "user"]
+    __properties: ClassVar[List[str]] = ["input", "model", "encoding_format", "dimensions", "user"]
+
+    @field_validator('encoding_format')
+    def encoding_format_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['float', 'base64']):
+            raise ValueError("must be one of enum values ('float', 'base64')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -69,32 +82,34 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of model
-        if self.model:
-            _dict['model'] = self.model.to_dict()
         # override the default output from pydantic by calling `to_dict()` of input
         if self.input:
             _dict['input'] = self.input.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of model
+        if self.model:
+            _dict['model'] = self.model.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of CreateEmbeddingRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "model": CreateEmbeddingRequestModel.from_dict(obj["model"]) if obj.get("model") is not None else None,
             "input": CreateEmbeddingRequestInput.from_dict(obj["input"]) if obj.get("input") is not None else None,
+            "model": CreateEmbeddingRequestModel.from_dict(obj["model"]) if obj.get("model") is not None else None,
+            "encoding_format": obj.get("encoding_format") if obj.get("encoding_format") is not None else 'float',
+            "dimensions": obj.get("dimensions"),
             "user": obj.get("user")
         })
         return _obj
```

## openapiopenai/models/create_embedding_request_input.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -23,24 +23,24 @@
 from typing import Union, List, Optional, Dict
 from typing_extensions import Literal, Self
 
 CREATEEMBEDDINGREQUESTINPUT_ONE_OF_SCHEMAS = ["List[List[int]]", "List[int]", "List[str]", "str"]
 
 class CreateEmbeddingRequestInput(BaseModel):
     """
-    Input text to embed, encoded as a string or array of tokens. To embed multiple inputs in a single request, pass an array of strings or array of token arrays. Each input must not exceed the max input tokens for the model (8191 tokens for `text-embedding-ada-002`). [Example Python code](https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb) for counting tokens. 
+    Input text to embed, encoded as a string or array of tokens. To embed multiple inputs in a single request, pass an array of strings or array of token arrays. The input must not exceed the max input tokens for the model (8192 tokens for `text-embedding-ada-002`), cannot be an empty string, and any array must be 2048 dimensions or less. [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken) for counting tokens. 
     """
     # data type: str
-    oneof_schema_1_validator: Optional[StrictStr] = ''
+    oneof_schema_1_validator: Optional[StrictStr] = Field(default='', description="The string that will be turned into an embedding.")
     # data type: List[str]
-    oneof_schema_2_validator: Optional[List[StrictStr]] = None
+    oneof_schema_2_validator: Optional[Annotated[List[StrictStr], Field(min_length=1, max_length=2048)]] = Field(default=None, description="The array of strings that will be turned into an embedding.")
     # data type: List[int]
-    oneof_schema_3_validator: Optional[Annotated[List[StrictInt], Field(min_length=1)]] = None
+    oneof_schema_3_validator: Optional[Annotated[List[StrictInt], Field(min_length=1, max_length=2048)]] = Field(default=None, description="The array of integers that will be turned into an embedding.")
     # data type: List[List[int]]
-    oneof_schema_4_validator: Optional[Annotated[List[Annotated[List[StrictInt], Field(min_length=1)]], Field(min_length=1)]] = None
+    oneof_schema_4_validator: Optional[Annotated[List[Annotated[List[StrictInt], Field(min_length=1)]], Field(min_length=1, max_length=2048)]] = Field(default=None, description="The array of arrays containing integers that will be turned into an embedding.")
     actual_instance: Optional[Union[List[List[int]], List[int], List[str], str]] = None
     one_of_schemas: List[str] = Field(default=Literal["List[List[int]]", "List[int]", "List[str]", "str"])
 
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
     )
```

## openapiopenai/models/create_embedding_request_model.py

```diff
@@ -1,122 +1,118 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
+from inspect import getfullargspec
 import json
 import pprint
+import re  # noqa: F401
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
-from typing import Any, List, Optional
-from pydantic import StrictStr, Field
-from typing import Union, List, Optional, Dict
+from typing import Optional
+from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
+from pydantic import Field
 
-CREATEEMBEDDINGREQUESTMODEL_ONE_OF_SCHEMAS = ["str"]
+CREATEEMBEDDINGREQUESTMODEL_ANY_OF_SCHEMAS = ["str"]
 
 class CreateEmbeddingRequestModel(BaseModel):
     """
     ID of the model to use. You can use the [List models](/docs/api-reference/models/list) API to see all of your available models, or see our [Model overview](/docs/models/overview) for descriptions of them. 
     """
+
     # data type: str
-    oneof_schema_1_validator: Optional[StrictStr] = None
+    anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: str
-    oneof_schema_2_validator: Optional[StrictStr] = None
-    actual_instance: Optional[Union[str]] = None
-    one_of_schemas: List[str] = Field(default=Literal["str"])
-
-    model_config = ConfigDict(
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
-
+    anyof_schema_2_validator: Optional[StrictStr] = None
+    if TYPE_CHECKING:
+        actual_instance: Optional[Union[str]] = None
+    else:
+        actual_instance: Any = None
+    any_of_schemas: List[str] = Field(default=Literal["str"])
+
+    model_config = {
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
                 raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
             if kwargs:
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
+    def actual_instance_must_validate_anyof(cls, v):
         instance = CreateEmbeddingRequestModel.model_construct()
         error_messages = []
-        match = 0
         # validate data type: str
         try:
-            instance.oneof_schema_1_validator = v
-            match += 1
+            instance.anyof_schema_1_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # validate data type: str
         try:
-            instance.oneof_schema_2_validator = v
-            match += 1
+            instance.anyof_schema_2_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in CreateEmbeddingRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in CreateEmbeddingRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in CreateEmbeddingRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
+    def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        match = 0
-
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_1_validator = json.loads(json_str)
+            instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_1_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_1_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_2_validator = json.loads(json_str)
+            instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_2_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_2_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into CreateEmbeddingRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into CreateEmbeddingRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into CreateEmbeddingRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
@@ -130,15 +126,14 @@
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
-            # primitive type
             return self.actual_instance
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.model_dump())
```

## openapiopenai/models/create_embedding_response.py

```diff
@@ -1,43 +1,50 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
-from openapiopenai.models.create_embedding_response_data_inner import CreateEmbeddingResponseDataInner
 from openapiopenai.models.create_embedding_response_usage import CreateEmbeddingResponseUsage
+from openapiopenai.models.embedding import Embedding
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateEmbeddingResponse(BaseModel):
     """
     CreateEmbeddingResponse
     """ # noqa: E501
-    object: StrictStr
-    model: StrictStr
-    data: List[CreateEmbeddingResponseDataInner]
+    data: List[Embedding] = Field(description="The list of embeddings generated by the model.")
+    model: StrictStr = Field(description="The name of the model used to generate the embedding.")
+    object: StrictStr = Field(description="The object type, which is always \"list\".")
     usage: CreateEmbeddingResponseUsage
-    __properties: ClassVar[List[str]] = ["object", "model", "data", "usage"]
+    __properties: ClassVar[List[str]] = ["data", "model", "object", "usage"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['list']):
+            raise ValueError("must be one of enum values ('list')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -92,15 +99,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "object": obj.get("object"),
+            "data": [Embedding.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
             "model": obj.get("model"),
-            "data": [CreateEmbeddingResponseDataInner.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
+            "object": obj.get("object"),
             "usage": CreateEmbeddingResponseUsage.from_dict(obj["usage"]) if obj.get("usage") is not None else None
         })
         return _obj
```

## openapiopenai/models/create_embedding_response_usage.py

```diff
@@ -1,38 +1,38 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateEmbeddingResponseUsage(BaseModel):
     """
-    CreateEmbeddingResponseUsage
+    The usage information for the request.
     """ # noqa: E501
-    prompt_tokens: StrictInt
-    total_tokens: StrictInt
+    prompt_tokens: StrictInt = Field(description="The number of tokens used by the prompt.")
+    total_tokens: StrictInt = Field(description="The total number of tokens used by the request.")
     __properties: ClassVar[List[str]] = ["prompt_tokens", "total_tokens"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
```

## openapiopenai/models/create_image_request.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -17,48 +17,72 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
+from openapiopenai.models.create_image_request_model import CreateImageRequestModel
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateImageRequest(BaseModel):
     """
     CreateImageRequest
     """ # noqa: E501
-    prompt: StrictStr = Field(description="A text description of the desired image(s). The maximum length is 1000 characters.")
-    n: Optional[Annotated[int, Field(le=10, strict=True, ge=1)]] = Field(default=1, description="The number of images to generate. Must be between 1 and 10.")
-    size: Optional[StrictStr] = Field(default='1024x1024', description="The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.")
-    response_format: Optional[StrictStr] = Field(default='url', description="The format in which the generated images are returned. Must be one of `url` or `b64_json`.")
+    prompt: StrictStr = Field(description="A text description of the desired image(s). The maximum length is 1000 characters for `dall-e-2` and 4000 characters for `dall-e-3`.")
+    model: Optional[CreateImageRequestModel] = None
+    n: Optional[Annotated[int, Field(le=10, strict=True, ge=1)]] = Field(default=1, description="The number of images to generate. Must be between 1 and 10. For `dall-e-3`, only `n=1` is supported.")
+    quality: Optional[StrictStr] = Field(default='standard', description="The quality of the image that will be generated. `hd` creates images with finer details and greater consistency across the image. This param is only supported for `dall-e-3`.")
+    response_format: Optional[StrictStr] = Field(default='url', description="The format in which the generated images are returned. Must be one of `url` or `b64_json`. URLs are only valid for 60 minutes after the image has been generated.")
+    size: Optional[StrictStr] = Field(default='1024x1024', description="The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024` for `dall-e-2`. Must be one of `1024x1024`, `1792x1024`, or `1024x1792` for `dall-e-3` models.")
+    style: Optional[StrictStr] = Field(default='vivid', description="The style of the generated images. Must be one of `vivid` or `natural`. Vivid causes the model to lean towards generating hyper-real and dramatic images. Natural causes the model to produce more natural, less hyper-real looking images. This param is only supported for `dall-e-3`.")
     user: Optional[StrictStr] = Field(default=None, description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")
-    __properties: ClassVar[List[str]] = ["prompt", "n", "size", "response_format", "user"]
+    __properties: ClassVar[List[str]] = ["prompt", "model", "n", "quality", "response_format", "size", "style", "user"]
 
-    @field_validator('size')
-    def size_validate_enum(cls, value):
+    @field_validator('quality')
+    def quality_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['256x256', '512x512', '1024x1024']):
-            raise ValueError("must be one of enum values ('256x256', '512x512', '1024x1024')")
+        if value not in set(['standard', 'hd']):
+            raise ValueError("must be one of enum values ('standard', 'hd')")
         return value
 
     @field_validator('response_format')
     def response_format_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
         if value not in set(['url', 'b64_json']):
             raise ValueError("must be one of enum values ('url', 'b64_json')")
         return value
 
+    @field_validator('size')
+    def size_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['256x256', '512x512', '1024x1024', '1792x1024', '1024x1792']):
+            raise ValueError("must be one of enum values ('256x256', '512x512', '1024x1024', '1792x1024', '1024x1792')")
+        return value
+
+    @field_validator('style')
+    def style_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['vivid', 'natural']):
+            raise ValueError("must be one of enum values ('vivid', 'natural')")
+        return value
+
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
 
@@ -90,43 +114,59 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of model
+        if self.model:
+            _dict['model'] = self.model.to_dict()
+        # set to None if model (nullable) is None
+        # and model_fields_set contains the field
+        if self.model is None and "model" in self.model_fields_set:
+            _dict['model'] = None
+
         # set to None if n (nullable) is None
         # and model_fields_set contains the field
         if self.n is None and "n" in self.model_fields_set:
             _dict['n'] = None
 
+        # set to None if response_format (nullable) is None
+        # and model_fields_set contains the field
+        if self.response_format is None and "response_format" in self.model_fields_set:
+            _dict['response_format'] = None
+
         # set to None if size (nullable) is None
         # and model_fields_set contains the field
         if self.size is None and "size" in self.model_fields_set:
             _dict['size'] = None
 
-        # set to None if response_format (nullable) is None
+        # set to None if style (nullable) is None
         # and model_fields_set contains the field
-        if self.response_format is None and "response_format" in self.model_fields_set:
-            _dict['response_format'] = None
+        if self.style is None and "style" in self.model_fields_set:
+            _dict['style'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of CreateImageRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "prompt": obj.get("prompt"),
+            "model": CreateImageRequestModel.from_dict(obj["model"]) if obj.get("model") is not None else None,
             "n": obj.get("n") if obj.get("n") is not None else 1,
-            "size": obj.get("size") if obj.get("size") is not None else '1024x1024',
+            "quality": obj.get("quality") if obj.get("quality") is not None else 'standard',
             "response_format": obj.get("response_format") if obj.get("response_format") is not None else 'url',
+            "size": obj.get("size") if obj.get("size") is not None else '1024x1024',
+            "style": obj.get("style") if obj.get("style") is not None else 'vivid',
             "user": obj.get("user")
         })
         return _obj
```

## openapiopenai/models/create_moderation_request.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## openapiopenai/models/create_moderation_request_input.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## openapiopenai/models/create_moderation_request_model.py

```diff
@@ -1,122 +1,118 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
+from inspect import getfullargspec
 import json
 import pprint
+import re  # noqa: F401
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
-from typing import Any, List, Optional
-from pydantic import StrictStr, Field
-from typing import Union, List, Optional, Dict
+from typing import Optional
+from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
+from pydantic import Field
 
-CREATEMODERATIONREQUESTMODEL_ONE_OF_SCHEMAS = ["str"]
+CREATEMODERATIONREQUESTMODEL_ANY_OF_SCHEMAS = ["str"]
 
 class CreateModerationRequestModel(BaseModel):
     """
     Two content moderations models are available: `text-moderation-stable` and `text-moderation-latest`.  The default is `text-moderation-latest` which will be automatically upgraded over time. This ensures you are always using our most accurate model. If you use `text-moderation-stable`, we will provide advanced notice before updating the model. Accuracy of `text-moderation-stable` may be slightly lower than for `text-moderation-latest`. 
     """
+
     # data type: str
-    oneof_schema_1_validator: Optional[StrictStr] = None
+    anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: str
-    oneof_schema_2_validator: Optional[StrictStr] = None
-    actual_instance: Optional[Union[str]] = None
-    one_of_schemas: List[str] = Field(default=Literal["str"])
-
-    model_config = ConfigDict(
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
-
+    anyof_schema_2_validator: Optional[StrictStr] = None
+    if TYPE_CHECKING:
+        actual_instance: Optional[Union[str]] = None
+    else:
+        actual_instance: Any = None
+    any_of_schemas: List[str] = Field(default=Literal["str"])
+
+    model_config = {
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
                 raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
             if kwargs:
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
+    def actual_instance_must_validate_anyof(cls, v):
         instance = CreateModerationRequestModel.model_construct()
         error_messages = []
-        match = 0
         # validate data type: str
         try:
-            instance.oneof_schema_1_validator = v
-            match += 1
+            instance.anyof_schema_1_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # validate data type: str
         try:
-            instance.oneof_schema_2_validator = v
-            match += 1
+            instance.anyof_schema_2_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in CreateModerationRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in CreateModerationRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in CreateModerationRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
+    def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        match = 0
-
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_1_validator = json.loads(json_str)
+            instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_1_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_1_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_2_validator = json.loads(json_str)
+            instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_2_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_2_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into CreateModerationRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into CreateModerationRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into CreateModerationRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
@@ -130,15 +126,14 @@
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
-            # primitive type
             return self.actual_instance
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.model_dump())
```

## openapiopenai/models/create_moderation_response.py

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
 from openapiopenai.models.create_moderation_response_results_inner import CreateModerationResponseResultsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateModerationResponse(BaseModel):
     """
-    CreateModerationResponse
+    Represents if a given text input is potentially harmful.
     """ # noqa: E501
-    id: StrictStr
-    model: StrictStr
-    results: List[CreateModerationResponseResultsInner]
+    id: StrictStr = Field(description="The unique identifier for the moderation request.")
+    model: StrictStr = Field(description="The model used to generate the moderation results.")
+    results: List[CreateModerationResponseResultsInner] = Field(description="A list of moderation objects.")
     __properties: ClassVar[List[str]] = ["id", "model", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
```

## openapiopenai/models/create_moderation_response_results_inner.py

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool
+from pydantic import BaseModel, ConfigDict, Field, StrictBool
 from typing import Any, ClassVar, Dict, List
 from openapiopenai.models.create_moderation_response_results_inner_categories import CreateModerationResponseResultsInnerCategories
 from openapiopenai.models.create_moderation_response_results_inner_category_scores import CreateModerationResponseResultsInnerCategoryScores
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateModerationResponseResultsInner(BaseModel):
     """
     CreateModerationResponseResultsInner
     """ # noqa: E501
-    flagged: StrictBool
+    flagged: StrictBool = Field(description="Whether any of the below categories are flagged.")
     categories: CreateModerationResponseResultsInnerCategories
     category_scores: CreateModerationResponseResultsInnerCategoryScores
     __properties: ClassVar[List[str]] = ["flagged", "categories", "category_scores"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
```

## openapiopenai/models/create_moderation_response_results_inner_categories.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -21,24 +21,28 @@
 from pydantic import BaseModel, ConfigDict, Field, StrictBool
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateModerationResponseResultsInnerCategories(BaseModel):
     """
-    CreateModerationResponseResultsInnerCategories
+    A list of the categories, and whether they are flagged or not.
     """ # noqa: E501
-    hate: StrictBool
-    hate_threatening: StrictBool = Field(alias="hate/threatening")
-    self_harm: StrictBool = Field(alias="self-harm")
-    sexual: StrictBool
-    sexual_minors: StrictBool = Field(alias="sexual/minors")
-    violence: StrictBool
-    violence_graphic: StrictBool = Field(alias="violence/graphic")
-    __properties: ClassVar[List[str]] = ["hate", "hate/threatening", "self-harm", "sexual", "sexual/minors", "violence", "violence/graphic"]
+    hate: StrictBool = Field(description="Content that expresses, incites, or promotes hate based on race, gender, ethnicity, religion, nationality, sexual orientation, disability status, or caste. Hateful content aimed at non-protected groups (e.g., chess players) is harassment.")
+    hate_threatening: StrictBool = Field(description="Hateful content that also includes violence or serious harm towards the targeted group based on race, gender, ethnicity, religion, nationality, sexual orientation, disability status, or caste.", alias="hate/threatening")
+    harassment: StrictBool = Field(description="Content that expresses, incites, or promotes harassing language towards any target.")
+    harassment_threatening: StrictBool = Field(description="Harassment content that also includes violence or serious harm towards any target.", alias="harassment/threatening")
+    self_harm: StrictBool = Field(description="Content that promotes, encourages, or depicts acts of self-harm, such as suicide, cutting, and eating disorders.", alias="self-harm")
+    self_harm_intent: StrictBool = Field(description="Content where the speaker expresses that they are engaging or intend to engage in acts of self-harm, such as suicide, cutting, and eating disorders.", alias="self-harm/intent")
+    self_harm_instructions: StrictBool = Field(description="Content that encourages performing acts of self-harm, such as suicide, cutting, and eating disorders, or that gives instructions or advice on how to commit such acts.", alias="self-harm/instructions")
+    sexual: StrictBool = Field(description="Content meant to arouse sexual excitement, such as the description of sexual activity, or that promotes sexual services (excluding sex education and wellness).")
+    sexual_minors: StrictBool = Field(description="Sexual content that includes an individual who is under 18 years old.", alias="sexual/minors")
+    violence: StrictBool = Field(description="Content that depicts death, violence, or physical injury.")
+    violence_graphic: StrictBool = Field(description="Content that depicts death, violence, or physical injury in graphic detail.", alias="violence/graphic")
+    __properties: ClassVar[List[str]] = ["hate", "hate/threatening", "harassment", "harassment/threatening", "self-harm", "self-harm/intent", "self-harm/instructions", "sexual", "sexual/minors", "violence", "violence/graphic"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -85,15 +89,19 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "hate": obj.get("hate"),
             "hate/threatening": obj.get("hate/threatening"),
+            "harassment": obj.get("harassment"),
+            "harassment/threatening": obj.get("harassment/threatening"),
             "self-harm": obj.get("self-harm"),
+            "self-harm/intent": obj.get("self-harm/intent"),
+            "self-harm/instructions": obj.get("self-harm/instructions"),
             "sexual": obj.get("sexual"),
             "sexual/minors": obj.get("sexual/minors"),
             "violence": obj.get("violence"),
             "violence/graphic": obj.get("violence/graphic")
         })
         return _obj
```

## openapiopenai/models/create_moderation_response_results_inner_category_scores.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -21,24 +21,28 @@
 from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt
 from typing import Any, ClassVar, Dict, List, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateModerationResponseResultsInnerCategoryScores(BaseModel):
     """
-    CreateModerationResponseResultsInnerCategoryScores
+    A list of the categories along with their scores as predicted by model.
     """ # noqa: E501
-    hate: Union[StrictFloat, StrictInt]
-    hate_threatening: Union[StrictFloat, StrictInt] = Field(alias="hate/threatening")
-    self_harm: Union[StrictFloat, StrictInt] = Field(alias="self-harm")
-    sexual: Union[StrictFloat, StrictInt]
-    sexual_minors: Union[StrictFloat, StrictInt] = Field(alias="sexual/minors")
-    violence: Union[StrictFloat, StrictInt]
-    violence_graphic: Union[StrictFloat, StrictInt] = Field(alias="violence/graphic")
-    __properties: ClassVar[List[str]] = ["hate", "hate/threatening", "self-harm", "sexual", "sexual/minors", "violence", "violence/graphic"]
+    hate: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'hate'.")
+    hate_threatening: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'hate/threatening'.", alias="hate/threatening")
+    harassment: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'harassment'.")
+    harassment_threatening: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'harassment/threatening'.", alias="harassment/threatening")
+    self_harm: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'self-harm'.", alias="self-harm")
+    self_harm_intent: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'self-harm/intent'.", alias="self-harm/intent")
+    self_harm_instructions: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'self-harm/instructions'.", alias="self-harm/instructions")
+    sexual: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'sexual'.")
+    sexual_minors: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'sexual/minors'.", alias="sexual/minors")
+    violence: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'violence'.")
+    violence_graphic: Union[StrictFloat, StrictInt] = Field(description="The score for the category 'violence/graphic'.", alias="violence/graphic")
+    __properties: ClassVar[List[str]] = ["hate", "hate/threatening", "harassment", "harassment/threatening", "self-harm", "self-harm/intent", "self-harm/instructions", "sexual", "sexual/minors", "violence", "violence/graphic"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -85,15 +89,19 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "hate": obj.get("hate"),
             "hate/threatening": obj.get("hate/threatening"),
+            "harassment": obj.get("harassment"),
+            "harassment/threatening": obj.get("harassment/threatening"),
             "self-harm": obj.get("self-harm"),
+            "self-harm/intent": obj.get("self-harm/intent"),
+            "self-harm/instructions": obj.get("self-harm/instructions"),
             "sexual": obj.get("sexual"),
             "sexual/minors": obj.get("sexual/minors"),
             "violence": obj.get("violence"),
             "violence/graphic": obj.get("violence/graphic")
         })
         return _obj
```

## openapiopenai/models/create_transcription_request_model.py

```diff
@@ -1,122 +1,118 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
+from inspect import getfullargspec
 import json
 import pprint
+import re  # noqa: F401
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
-from typing import Any, List, Optional
-from pydantic import StrictStr, Field
-from typing import Union, List, Optional, Dict
+from typing import Optional
+from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
+from pydantic import Field
 
-CREATETRANSCRIPTIONREQUESTMODEL_ONE_OF_SCHEMAS = ["str"]
+CREATETRANSCRIPTIONREQUESTMODEL_ANY_OF_SCHEMAS = ["str"]
 
 class CreateTranscriptionRequestModel(BaseModel):
     """
-    ID of the model to use. Only `whisper-1` is currently available. 
+    ID of the model to use. Only `whisper-1` (which is powered by our open source Whisper V2 model) is currently available. 
     """
+
     # data type: str
-    oneof_schema_1_validator: Optional[StrictStr] = None
+    anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: str
-    oneof_schema_2_validator: Optional[StrictStr] = None
-    actual_instance: Optional[Union[str]] = None
-    one_of_schemas: List[str] = Field(default=Literal["str"])
-
-    model_config = ConfigDict(
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
-
+    anyof_schema_2_validator: Optional[StrictStr] = None
+    if TYPE_CHECKING:
+        actual_instance: Optional[Union[str]] = None
+    else:
+        actual_instance: Any = None
+    any_of_schemas: List[str] = Field(default=Literal["str"])
+
+    model_config = {
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
     def __init__(self, *args, **kwargs) -> None:
         if args:
             if len(args) > 1:
                 raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
             if kwargs:
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
+    def actual_instance_must_validate_anyof(cls, v):
         instance = CreateTranscriptionRequestModel.model_construct()
         error_messages = []
-        match = 0
         # validate data type: str
         try:
-            instance.oneof_schema_1_validator = v
-            match += 1
+            instance.anyof_schema_1_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # validate data type: str
         try:
-            instance.oneof_schema_2_validator = v
-            match += 1
+            instance.anyof_schema_2_validator = v
+            return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in CreateTranscriptionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in CreateTranscriptionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in CreateTranscriptionRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
+    def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        match = 0
-
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_1_validator = json.loads(json_str)
+            instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_1_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_1_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # deserialize data into str
         try:
             # validation
-            instance.oneof_schema_2_validator = json.loads(json_str)
+            instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_2_validator
-            match += 1
+            instance.actual_instance = instance.anyof_schema_2_validator
+            return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into CreateTranscriptionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into CreateTranscriptionRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into CreateTranscriptionRequestModel with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
@@ -130,15 +126,14 @@
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
-            # primitive type
             return self.actual_instance
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.model_dump())
```

## openapiopenai/models/delete_file_response.py

```diff
@@ -1,41 +1,48 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DeleteFileResponse(BaseModel):
     """
     DeleteFileResponse
     """ # noqa: E501
     id: StrictStr
     object: StrictStr
     deleted: StrictBool
     __properties: ClassVar[List[str]] = ["id", "object", "deleted"]
 
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['file']):
+            raise ValueError("must be one of enum values ('file')")
+        return value
+
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
```

## openapiopenai/models/delete_model_response.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -24,17 +24,17 @@
 from typing_extensions import Self
 
 class DeleteModelResponse(BaseModel):
     """
     DeleteModelResponse
     """ # noqa: E501
     id: StrictStr
-    object: StrictStr
     deleted: StrictBool
-    __properties: ClassVar[List[str]] = ["id", "object", "deleted"]
+    object: StrictStr
+    __properties: ClassVar[List[str]] = ["id", "deleted", "object"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -80,13 +80,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "object": obj.get("object"),
-            "deleted": obj.get("deleted")
+            "deleted": obj.get("deleted"),
+            "object": obj.get("object")
         })
         return _obj
```

## openapiopenai/models/error.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -23,19 +23,19 @@
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Error(BaseModel):
     """
     Error
     """ # noqa: E501
-    type: StrictStr
+    code: Optional[StrictStr]
     message: StrictStr
     param: Optional[StrictStr]
-    code: Optional[StrictStr]
-    __properties: ClassVar[List[str]] = ["type", "message", "param", "code"]
+    type: StrictStr
+    __properties: ClassVar[List[str]] = ["code", "message", "param", "type"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -68,37 +68,37 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if param (nullable) is None
-        # and model_fields_set contains the field
-        if self.param is None and "param" in self.model_fields_set:
-            _dict['param'] = None
-
         # set to None if code (nullable) is None
         # and model_fields_set contains the field
         if self.code is None and "code" in self.model_fields_set:
             _dict['code'] = None
 
+        # set to None if param (nullable) is None
+        # and model_fields_set contains the field
+        if self.param is None and "param" in self.model_fields_set:
+            _dict['param'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of Error from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "type": obj.get("type"),
+            "code": obj.get("code"),
             "message": obj.get("message"),
             "param": obj.get("param"),
-            "code": obj.get("code")
+            "type": obj.get("type")
         })
         return _obj
```

## openapiopenai/models/error_response.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

## openapiopenai/models/images_response.py

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -16,24 +16,24 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
-from openapiopenai.models.images_response_data_inner import ImagesResponseDataInner
+from openapiopenai.models.image import Image
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ImagesResponse(BaseModel):
     """
     ImagesResponse
     """ # noqa: E501
     created: StrictInt
-    data: List[ImagesResponseDataInner]
+    data: List[Image]
     __properties: ClassVar[List[str]] = ["created", "data"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -87,12 +87,12 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "created": obj.get("created"),
-            "data": [ImagesResponseDataInner.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None
+            "data": [Image.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None
         })
         return _obj
```

## openapiopenai/models/list_files_response.py

```diff
@@ -1,40 +1,47 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
 from openapiopenai.models.open_ai_file import OpenAIFile
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ListFilesResponse(BaseModel):
     """
     ListFilesResponse
     """ # noqa: E501
-    object: StrictStr
     data: List[OpenAIFile]
-    __properties: ClassVar[List[str]] = ["object", "data"]
+    object: StrictStr
+    __properties: ClassVar[List[str]] = ["data", "object"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['list']):
+            raise ValueError("must be one of enum values ('list')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -86,13 +93,13 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "object": obj.get("object"),
-            "data": [OpenAIFile.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None
+            "data": [OpenAIFile.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
+            "object": obj.get("object")
         })
         return _obj
```

## openapiopenai/models/list_models_response.py

```diff
@@ -1,41 +1,48 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
 from openapiopenai.models.model import Model
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ListModelsResponse(BaseModel):
     """
     ListModelsResponse
     """ # noqa: E501
     object: StrictStr
     data: List[Model]
     __properties: ClassVar[List[str]] = ["object", "data"]
 
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['list']):
+            raise ValueError("must be one of enum values ('list')")
+        return value
+
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
```

## openapiopenai/models/model.py

```diff
@@ -1,41 +1,48 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Model(BaseModel):
     """
-    Model
+    Describes an OpenAI model offering that can be used with the API.
     """ # noqa: E501
-    id: StrictStr
-    object: StrictStr
-    created: StrictInt
-    owned_by: StrictStr
-    __properties: ClassVar[List[str]] = ["id", "object", "created", "owned_by"]
+    id: StrictStr = Field(description="The model identifier, which can be referenced in the API endpoints.")
+    created: StrictInt = Field(description="The Unix timestamp (in seconds) when the model was created.")
+    object: StrictStr = Field(description="The object type, which is always \"model\".")
+    owned_by: StrictStr = Field(description="The organization that owns the model.")
+    __properties: ClassVar[List[str]] = ["id", "created", "object", "owned_by"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['model']):
+            raise ValueError("must be one of enum values ('model')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -81,14 +88,14 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "object": obj.get("object"),
             "created": obj.get("created"),
+            "object": obj.get("object"),
             "owned_by": obj.get("owned_by")
         })
         return _obj
```

## openapiopenai/models/open_ai_file.py

```diff
@@ -1,45 +1,66 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class OpenAIFile(BaseModel):
     """
-    OpenAIFile
+    The `File` object represents a document that has been uploaded to OpenAI.
     """ # noqa: E501
-    id: StrictStr
-    object: StrictStr
-    bytes: StrictInt
-    created_at: StrictInt
-    filename: StrictStr
-    purpose: StrictStr
-    status: Optional[StrictStr] = None
-    status_details: Optional[Dict[str, Any]] = None
-    __properties: ClassVar[List[str]] = ["id", "object", "bytes", "created_at", "filename", "purpose", "status", "status_details"]
+    id: StrictStr = Field(description="The file identifier, which can be referenced in the API endpoints.")
+    bytes: StrictInt = Field(description="The size of the file, in bytes.")
+    created_at: StrictInt = Field(description="The Unix timestamp (in seconds) for when the file was created.")
+    filename: StrictStr = Field(description="The name of the file.")
+    object: StrictStr = Field(description="The object type, which is always `file`.")
+    purpose: StrictStr = Field(description="The intended purpose of the file. Supported values are `fine-tune`, `fine-tune-results`, `assistants`, and `assistants_output`.")
+    status: StrictStr = Field(description="Deprecated. The current status of the file, which can be either `uploaded`, `processed`, or `error`.")
+    status_details: Optional[StrictStr] = Field(default=None, description="Deprecated. For details on why a fine-tuning training file failed validation, see the `error` field on `fine_tuning.job`.")
+    __properties: ClassVar[List[str]] = ["id", "bytes", "created_at", "filename", "object", "purpose", "status", "status_details"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['file']):
+            raise ValueError("must be one of enum values ('file')")
+        return value
+
+    @field_validator('purpose')
+    def purpose_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['fine-tune', 'fine-tune-results', 'assistants', 'assistants_output']):
+            raise ValueError("must be one of enum values ('fine-tune', 'fine-tune-results', 'assistants', 'assistants_output')")
+        return value
+
+    @field_validator('status')
+    def status_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['uploaded', 'processed', 'error']):
+            raise ValueError("must be one of enum values ('uploaded', 'processed', 'error')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -72,36 +93,31 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if status_details (nullable) is None
-        # and model_fields_set contains the field
-        if self.status_details is None and "status_details" in self.model_fields_set:
-            _dict['status_details'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of OpenAIFile from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "object": obj.get("object"),
             "bytes": obj.get("bytes"),
             "created_at": obj.get("created_at"),
             "filename": obj.get("filename"),
+            "object": obj.get("object"),
             "purpose": obj.get("purpose"),
             "status": obj.get("status"),
             "status_details": obj.get("status_details")
         })
         return _obj
```

## Comparing `openapiopenai/api/open_ai_api.py` & `openapiopenai/api/assistants_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,100 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictBool, StrictBytes, StrictFloat, StrictInt, StrictStr, field_validator
-from typing import Optional, Union
+from pydantic import Field, StrictInt, StrictStr, field_validator
+from typing import Optional
 from typing_extensions import Annotated
-from openapiopenai.models.create_chat_completion_request import CreateChatCompletionRequest
-from openapiopenai.models.create_chat_completion_response import CreateChatCompletionResponse
-from openapiopenai.models.create_completion_request import CreateCompletionRequest
-from openapiopenai.models.create_completion_response import CreateCompletionResponse
-from openapiopenai.models.create_edit_request import CreateEditRequest
-from openapiopenai.models.create_edit_response import CreateEditResponse
-from openapiopenai.models.create_embedding_request import CreateEmbeddingRequest
-from openapiopenai.models.create_embedding_response import CreateEmbeddingResponse
-from openapiopenai.models.create_fine_tune_request import CreateFineTuneRequest
-from openapiopenai.models.create_image_request import CreateImageRequest
-from openapiopenai.models.create_moderation_request import CreateModerationRequest
-from openapiopenai.models.create_moderation_response import CreateModerationResponse
-from openapiopenai.models.create_transcription_request_model import CreateTranscriptionRequestModel
-from openapiopenai.models.create_transcription_response import CreateTranscriptionResponse
-from openapiopenai.models.create_translation_response import CreateTranslationResponse
-from openapiopenai.models.delete_file_response import DeleteFileResponse
-from openapiopenai.models.delete_model_response import DeleteModelResponse
-from openapiopenai.models.fine_tune import FineTune
-from openapiopenai.models.images_response import ImagesResponse
-from openapiopenai.models.list_files_response import ListFilesResponse
-from openapiopenai.models.list_fine_tune_events_response import ListFineTuneEventsResponse
-from openapiopenai.models.list_fine_tunes_response import ListFineTunesResponse
-from openapiopenai.models.list_models_response import ListModelsResponse
-from openapiopenai.models.model import Model
-from openapiopenai.models.open_ai_file import OpenAIFile
+from openapiopenai.models.assistant_file_object import AssistantFileObject
+from openapiopenai.models.assistant_object import AssistantObject
+from openapiopenai.models.create_assistant_file_request import CreateAssistantFileRequest
+from openapiopenai.models.create_assistant_request import CreateAssistantRequest
+from openapiopenai.models.create_message_request import CreateMessageRequest
+from openapiopenai.models.create_run_request import CreateRunRequest
+from openapiopenai.models.create_thread_and_run_request import CreateThreadAndRunRequest
+from openapiopenai.models.create_thread_request import CreateThreadRequest
+from openapiopenai.models.delete_assistant_file_response import DeleteAssistantFileResponse
+from openapiopenai.models.delete_assistant_response import DeleteAssistantResponse
+from openapiopenai.models.delete_thread_response import DeleteThreadResponse
+from openapiopenai.models.list_assistant_files_response import ListAssistantFilesResponse
+from openapiopenai.models.list_assistants_response import ListAssistantsResponse
+from openapiopenai.models.list_message_files_response import ListMessageFilesResponse
+from openapiopenai.models.list_messages_response import ListMessagesResponse
+from openapiopenai.models.list_run_steps_response import ListRunStepsResponse
+from openapiopenai.models.list_runs_response import ListRunsResponse
+from openapiopenai.models.message_file_object import MessageFileObject
+from openapiopenai.models.message_object import MessageObject
+from openapiopenai.models.modify_assistant_request import ModifyAssistantRequest
+from openapiopenai.models.modify_message_request import ModifyMessageRequest
+from openapiopenai.models.modify_run_request import ModifyRunRequest
+from openapiopenai.models.modify_thread_request import ModifyThreadRequest
+from openapiopenai.models.run_object import RunObject
+from openapiopenai.models.run_step_object import RunStepObject
+from openapiopenai.models.submit_tool_outputs_run_request import SubmitToolOutputsRunRequest
+from openapiopenai.models.thread_object import ThreadObject
 
 from openapiopenai.api_client import ApiClient, RequestSerialized
 from openapiopenai.api_response import ApiResponse
 from openapiopenai.rest import RESTResponseType
 
 
-class OpenAIApi:
+class AssistantsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def cancel_fine_tune(
+    def cancel_run(
         self,
-        fine_tune_id: Annotated[StrictStr, Field(description="The ID of the fine-tune job to cancel ")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which this run belongs.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to cancel.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> FineTune:
-        """Immediately cancel a fine-tune job. 
+    ) -> RunObject:
+        """Cancels a run that is `in_progress`.
 
 
-        :param fine_tune_id: The ID of the fine-tune job to cancel  (required)
-        :type fine_tune_id: str
+        :param thread_id: The ID of the thread to which this run belongs. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to cancel. (required)
+        :type run_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -104,58 +109,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._cancel_fine_tune_serialize(
-            fine_tune_id=fine_tune_id,
+        _param = self._cancel_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FineTune",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def cancel_fine_tune_with_http_info(
+    def cancel_run_with_http_info(
         self,
-        fine_tune_id: Annotated[StrictStr, Field(description="The ID of the fine-tune job to cancel ")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which this run belongs.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to cancel.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[FineTune]:
-        """Immediately cancel a fine-tune job. 
+    ) -> ApiResponse[RunObject]:
+        """Cancels a run that is `in_progress`.
 
 
-        :param fine_tune_id: The ID of the fine-tune job to cancel  (required)
-        :type fine_tune_id: str
+        :param thread_id: The ID of the thread to which this run belongs. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to cancel. (required)
+        :type run_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -170,58 +179,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._cancel_fine_tune_serialize(
-            fine_tune_id=fine_tune_id,
+        _param = self._cancel_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FineTune",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def cancel_fine_tune_without_preload_content(
+    def cancel_run_without_preload_content(
         self,
-        fine_tune_id: Annotated[StrictStr, Field(description="The ID of the fine-tune job to cancel ")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which this run belongs.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to cancel.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Immediately cancel a fine-tune job. 
+        """Cancels a run that is `in_progress`.
 
 
-        :param fine_tune_id: The ID of the fine-tune job to cancel  (required)
-        :type fine_tune_id: str
+        :param thread_id: The ID of the thread to which this run belongs. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to cancel. (required)
+        :type run_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -236,35 +249,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._cancel_fine_tune_serialize(
-            fine_tune_id=fine_tune_id,
+        _param = self._cancel_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FineTune",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _cancel_fine_tune_serialize(
+    def _cancel_run_serialize(
         self,
-        fine_tune_id,
+        thread_id,
+        run_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -276,16 +291,18 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if fine_tune_id is not None:
-            _path_params['fine_tune_id'] = fine_tune_id
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if run_id is not None:
+            _path_params['run_id'] = run_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -294,19 +311,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/fine-tunes/{fine_tune_id}/cancel',
+            resource_path='/threads/{thread_id}/runs/{run_id}/cancel',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -315,35 +333,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_chat_completion(
+    def create_assistant(
         self,
-        create_chat_completion_request: CreateChatCompletionRequest,
+        create_assistant_request: CreateAssistantRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateChatCompletionResponse:
-        """Creates a model response for the given chat conversation.
+    ) -> AssistantObject:
+        """Create an assistant with a model and instructions.
 
 
-        :param create_chat_completion_request: (required)
-        :type create_chat_completion_request: CreateChatCompletionRequest
+        :param create_assistant_request: (required)
+        :type create_assistant_request: CreateAssistantRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -358,58 +376,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_chat_completion_serialize(
-            create_chat_completion_request=create_chat_completion_request,
+        _param = self._create_assistant_serialize(
+            create_assistant_request=create_assistant_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateChatCompletionResponse",
+            '200': "AssistantObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_chat_completion_with_http_info(
+    def create_assistant_with_http_info(
         self,
-        create_chat_completion_request: CreateChatCompletionRequest,
+        create_assistant_request: CreateAssistantRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateChatCompletionResponse]:
-        """Creates a model response for the given chat conversation.
+    ) -> ApiResponse[AssistantObject]:
+        """Create an assistant with a model and instructions.
 
 
-        :param create_chat_completion_request: (required)
-        :type create_chat_completion_request: CreateChatCompletionRequest
+        :param create_assistant_request: (required)
+        :type create_assistant_request: CreateAssistantRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -424,58 +442,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_chat_completion_serialize(
-            create_chat_completion_request=create_chat_completion_request,
+        _param = self._create_assistant_serialize(
+            create_assistant_request=create_assistant_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateChatCompletionResponse",
+            '200': "AssistantObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_chat_completion_without_preload_content(
+    def create_assistant_without_preload_content(
         self,
-        create_chat_completion_request: CreateChatCompletionRequest,
+        create_assistant_request: CreateAssistantRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Creates a model response for the given chat conversation.
+        """Create an assistant with a model and instructions.
 
 
-        :param create_chat_completion_request: (required)
-        :type create_chat_completion_request: CreateChatCompletionRequest
+        :param create_assistant_request: (required)
+        :type create_assistant_request: CreateAssistantRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -490,35 +508,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_chat_completion_serialize(
-            create_chat_completion_request=create_chat_completion_request,
+        _param = self._create_assistant_serialize(
+            create_assistant_request=create_assistant_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateChatCompletionResponse",
+            '200': "AssistantObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_chat_completion_serialize(
+    def _create_assistant_serialize(
         self,
-        create_chat_completion_request,
+        create_assistant_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -534,16 +552,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_chat_completion_request is not None:
-            _body_params = create_chat_completion_request
+        if create_assistant_request is not None:
+            _body_params = create_assistant_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -561,19 +579,20 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/chat/completions',
+            resource_path='/assistants',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -582,35 +601,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_completion(
+    def create_assistant_file(
         self,
-        create_completion_request: CreateCompletionRequest,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant for which to create a File. ")],
+        create_assistant_file_request: CreateAssistantFileRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateCompletionResponse:
-        """Creates a completion for the provided prompt and parameters.
+    ) -> AssistantFileObject:
+        """Create an assistant file by attaching a [File](/docs/api-reference/files) to an [assistant](/docs/api-reference/assistants).
 
 
-        :param create_completion_request: (required)
-        :type create_completion_request: CreateCompletionRequest
+        :param assistant_id: The ID of the assistant for which to create a File.  (required)
+        :type assistant_id: str
+        :param create_assistant_file_request: (required)
+        :type create_assistant_file_request: CreateAssistantFileRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -625,58 +647,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_completion_serialize(
-            create_completion_request=create_completion_request,
+        _param = self._create_assistant_file_serialize(
+            assistant_id=assistant_id,
+            create_assistant_file_request=create_assistant_file_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateCompletionResponse",
+            '200': "AssistantFileObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_completion_with_http_info(
+    def create_assistant_file_with_http_info(
         self,
-        create_completion_request: CreateCompletionRequest,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant for which to create a File. ")],
+        create_assistant_file_request: CreateAssistantFileRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateCompletionResponse]:
-        """Creates a completion for the provided prompt and parameters.
+    ) -> ApiResponse[AssistantFileObject]:
+        """Create an assistant file by attaching a [File](/docs/api-reference/files) to an [assistant](/docs/api-reference/assistants).
 
 
-        :param create_completion_request: (required)
-        :type create_completion_request: CreateCompletionRequest
+        :param assistant_id: The ID of the assistant for which to create a File.  (required)
+        :type assistant_id: str
+        :param create_assistant_file_request: (required)
+        :type create_assistant_file_request: CreateAssistantFileRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -691,58 +717,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_completion_serialize(
-            create_completion_request=create_completion_request,
+        _param = self._create_assistant_file_serialize(
+            assistant_id=assistant_id,
+            create_assistant_file_request=create_assistant_file_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateCompletionResponse",
+            '200': "AssistantFileObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_completion_without_preload_content(
+    def create_assistant_file_without_preload_content(
         self,
-        create_completion_request: CreateCompletionRequest,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant for which to create a File. ")],
+        create_assistant_file_request: CreateAssistantFileRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Creates a completion for the provided prompt and parameters.
+        """Create an assistant file by attaching a [File](/docs/api-reference/files) to an [assistant](/docs/api-reference/assistants).
 
 
-        :param create_completion_request: (required)
-        :type create_completion_request: CreateCompletionRequest
+        :param assistant_id: The ID of the assistant for which to create a File.  (required)
+        :type assistant_id: str
+        :param create_assistant_file_request: (required)
+        :type create_assistant_file_request: CreateAssistantFileRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -757,35 +787,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_completion_serialize(
-            create_completion_request=create_completion_request,
+        _param = self._create_assistant_file_serialize(
+            assistant_id=assistant_id,
+            create_assistant_file_request=create_assistant_file_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateCompletionResponse",
+            '200': "AssistantFileObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_completion_serialize(
+    def _create_assistant_file_serialize(
         self,
-        create_completion_request,
+        assistant_id,
+        create_assistant_file_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -797,20 +829,22 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if assistant_id is not None:
+            _path_params['assistant_id'] = assistant_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_completion_request is not None:
-            _body_params = create_completion_request
+        if create_assistant_file_request is not None:
+            _body_params = create_assistant_file_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -828,19 +862,20 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/completions',
+            resource_path='/assistants/{assistant_id}/files',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -849,35 +884,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_edit(
+    def create_message(
         self,
-        create_edit_request: CreateEditRequest,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) to create a message for.")],
+        create_message_request: CreateMessageRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateEditResponse:
-        """Creates a new edit for the provided input, instruction, and parameters.
+    ) -> MessageObject:
+        """Create a message.
 
 
-        :param create_edit_request: (required)
-        :type create_edit_request: CreateEditRequest
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) to create a message for. (required)
+        :type thread_id: str
+        :param create_message_request: (required)
+        :type create_message_request: CreateMessageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -892,58 +930,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_edit_serialize(
-            create_edit_request=create_edit_request,
+        _param = self._create_message_serialize(
+            thread_id=thread_id,
+            create_message_request=create_message_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateEditResponse",
+            '200': "MessageObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_edit_with_http_info(
+    def create_message_with_http_info(
         self,
-        create_edit_request: CreateEditRequest,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) to create a message for.")],
+        create_message_request: CreateMessageRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateEditResponse]:
-        """Creates a new edit for the provided input, instruction, and parameters.
+    ) -> ApiResponse[MessageObject]:
+        """Create a message.
 
 
-        :param create_edit_request: (required)
-        :type create_edit_request: CreateEditRequest
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) to create a message for. (required)
+        :type thread_id: str
+        :param create_message_request: (required)
+        :type create_message_request: CreateMessageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -958,58 +1000,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_edit_serialize(
-            create_edit_request=create_edit_request,
+        _param = self._create_message_serialize(
+            thread_id=thread_id,
+            create_message_request=create_message_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateEditResponse",
+            '200': "MessageObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_edit_without_preload_content(
+    def create_message_without_preload_content(
         self,
-        create_edit_request: CreateEditRequest,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) to create a message for.")],
+        create_message_request: CreateMessageRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Creates a new edit for the provided input, instruction, and parameters.
+        """Create a message.
 
 
-        :param create_edit_request: (required)
-        :type create_edit_request: CreateEditRequest
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) to create a message for. (required)
+        :type thread_id: str
+        :param create_message_request: (required)
+        :type create_message_request: CreateMessageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1024,35 +1070,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_edit_serialize(
-            create_edit_request=create_edit_request,
+        _param = self._create_message_serialize(
+            thread_id=thread_id,
+            create_message_request=create_message_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateEditResponse",
+            '200': "MessageObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_edit_serialize(
+    def _create_message_serialize(
         self,
-        create_edit_request,
+        thread_id,
+        create_message_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1064,20 +1112,22 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_edit_request is not None:
-            _body_params = create_edit_request
+        if create_message_request is not None:
+            _body_params = create_message_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1095,19 +1145,20 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/edits',
+            resource_path='/threads/{thread_id}/messages',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1116,35 +1167,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_embedding(
+    def create_run(
         self,
-        create_embedding_request: CreateEmbeddingRequest,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to run.")],
+        create_run_request: CreateRunRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateEmbeddingResponse:
-        """Creates an embedding vector representing the input text.
+    ) -> RunObject:
+        """Create a run.
 
 
-        :param create_embedding_request: (required)
-        :type create_embedding_request: CreateEmbeddingRequest
+        :param thread_id: The ID of the thread to run. (required)
+        :type thread_id: str
+        :param create_run_request: (required)
+        :type create_run_request: CreateRunRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1159,58 +1213,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_embedding_serialize(
-            create_embedding_request=create_embedding_request,
+        _param = self._create_run_serialize(
+            thread_id=thread_id,
+            create_run_request=create_run_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateEmbeddingResponse",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_embedding_with_http_info(
+    def create_run_with_http_info(
         self,
-        create_embedding_request: CreateEmbeddingRequest,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to run.")],
+        create_run_request: CreateRunRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateEmbeddingResponse]:
-        """Creates an embedding vector representing the input text.
+    ) -> ApiResponse[RunObject]:
+        """Create a run.
 
 
-        :param create_embedding_request: (required)
-        :type create_embedding_request: CreateEmbeddingRequest
+        :param thread_id: The ID of the thread to run. (required)
+        :type thread_id: str
+        :param create_run_request: (required)
+        :type create_run_request: CreateRunRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1225,58 +1283,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_embedding_serialize(
-            create_embedding_request=create_embedding_request,
+        _param = self._create_run_serialize(
+            thread_id=thread_id,
+            create_run_request=create_run_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateEmbeddingResponse",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_embedding_without_preload_content(
+    def create_run_without_preload_content(
         self,
-        create_embedding_request: CreateEmbeddingRequest,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to run.")],
+        create_run_request: CreateRunRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Creates an embedding vector representing the input text.
+        """Create a run.
 
 
-        :param create_embedding_request: (required)
-        :type create_embedding_request: CreateEmbeddingRequest
+        :param thread_id: The ID of the thread to run. (required)
+        :type thread_id: str
+        :param create_run_request: (required)
+        :type create_run_request: CreateRunRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1291,35 +1353,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_embedding_serialize(
-            create_embedding_request=create_embedding_request,
+        _param = self._create_run_serialize(
+            thread_id=thread_id,
+            create_run_request=create_run_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateEmbeddingResponse",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_embedding_serialize(
+    def _create_run_serialize(
         self,
-        create_embedding_request,
+        thread_id,
+        create_run_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1331,20 +1395,22 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_embedding_request is not None:
-            _body_params = create_embedding_request
+        if create_run_request is not None:
+            _body_params = create_run_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1362,19 +1428,20 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/embeddings',
+            resource_path='/threads/{thread_id}/runs',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1383,38 +1450,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_file(
+    def create_thread(
         self,
-        file: Annotated[Union[StrictBytes, StrictStr], Field(description="Name of the [JSON Lines](https://jsonlines.readthedocs.io/en/latest/) file to be uploaded.  If the `purpose` is set to \\\"fine-tune\\\", each line is a JSON record with \\\"prompt\\\" and \\\"completion\\\" fields representing your [training examples](/docs/guides/fine-tuning/prepare-training-data). ")],
-        purpose: Annotated[StrictStr, Field(description="The intended purpose of the uploaded documents.  Use \\\"fine-tune\\\" for [Fine-tuning](/docs/api-reference/fine-tunes). This allows us to validate the format of the uploaded file. ")],
+        create_thread_request: Optional[CreateThreadRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> OpenAIFile:
-        """Upload a file that contains document(s) to be used across various endpoints/features. Currently, the size of all the files uploaded by one organization can be up to 1 GB. Please contact us if you need to increase the storage limit. 
+    ) -> ThreadObject:
+        """Create a thread.
 
 
-        :param file: Name of the [JSON Lines](https://jsonlines.readthedocs.io/en/latest/) file to be uploaded.  If the `purpose` is set to \\\"fine-tune\\\", each line is a JSON record with \\\"prompt\\\" and \\\"completion\\\" fields representing your [training examples](/docs/guides/fine-tuning/prepare-training-data).  (required)
-        :type file: bytearray
-        :param purpose: The intended purpose of the uploaded documents.  Use \\\"fine-tune\\\" for [Fine-tuning](/docs/api-reference/fine-tunes). This allows us to validate the format of the uploaded file.  (required)
-        :type purpose: str
+        :param create_thread_request:
+        :type create_thread_request: CreateThreadRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1429,62 +1493,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_file_serialize(
-            file=file,
-            purpose=purpose,
+        _param = self._create_thread_serialize(
+            create_thread_request=create_thread_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "OpenAIFile",
+            '200': "ThreadObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_file_with_http_info(
+    def create_thread_with_http_info(
         self,
-        file: Annotated[Union[StrictBytes, StrictStr], Field(description="Name of the [JSON Lines](https://jsonlines.readthedocs.io/en/latest/) file to be uploaded.  If the `purpose` is set to \\\"fine-tune\\\", each line is a JSON record with \\\"prompt\\\" and \\\"completion\\\" fields representing your [training examples](/docs/guides/fine-tuning/prepare-training-data). ")],
-        purpose: Annotated[StrictStr, Field(description="The intended purpose of the uploaded documents.  Use \\\"fine-tune\\\" for [Fine-tuning](/docs/api-reference/fine-tunes). This allows us to validate the format of the uploaded file. ")],
+        create_thread_request: Optional[CreateThreadRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[OpenAIFile]:
-        """Upload a file that contains document(s) to be used across various endpoints/features. Currently, the size of all the files uploaded by one organization can be up to 1 GB. Please contact us if you need to increase the storage limit. 
+    ) -> ApiResponse[ThreadObject]:
+        """Create a thread.
 
 
-        :param file: Name of the [JSON Lines](https://jsonlines.readthedocs.io/en/latest/) file to be uploaded.  If the `purpose` is set to \\\"fine-tune\\\", each line is a JSON record with \\\"prompt\\\" and \\\"completion\\\" fields representing your [training examples](/docs/guides/fine-tuning/prepare-training-data).  (required)
-        :type file: bytearray
-        :param purpose: The intended purpose of the uploaded documents.  Use \\\"fine-tune\\\" for [Fine-tuning](/docs/api-reference/fine-tunes). This allows us to validate the format of the uploaded file.  (required)
-        :type purpose: str
+        :param create_thread_request:
+        :type create_thread_request: CreateThreadRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1499,62 +1559,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_file_serialize(
-            file=file,
-            purpose=purpose,
+        _param = self._create_thread_serialize(
+            create_thread_request=create_thread_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "OpenAIFile",
+            '200': "ThreadObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_file_without_preload_content(
+    def create_thread_without_preload_content(
         self,
-        file: Annotated[Union[StrictBytes, StrictStr], Field(description="Name of the [JSON Lines](https://jsonlines.readthedocs.io/en/latest/) file to be uploaded.  If the `purpose` is set to \\\"fine-tune\\\", each line is a JSON record with \\\"prompt\\\" and \\\"completion\\\" fields representing your [training examples](/docs/guides/fine-tuning/prepare-training-data). ")],
-        purpose: Annotated[StrictStr, Field(description="The intended purpose of the uploaded documents.  Use \\\"fine-tune\\\" for [Fine-tuning](/docs/api-reference/fine-tunes). This allows us to validate the format of the uploaded file. ")],
+        create_thread_request: Optional[CreateThreadRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Upload a file that contains document(s) to be used across various endpoints/features. Currently, the size of all the files uploaded by one organization can be up to 1 GB. Please contact us if you need to increase the storage limit. 
+        """Create a thread.
 
 
-        :param file: Name of the [JSON Lines](https://jsonlines.readthedocs.io/en/latest/) file to be uploaded.  If the `purpose` is set to \\\"fine-tune\\\", each line is a JSON record with \\\"prompt\\\" and \\\"completion\\\" fields representing your [training examples](/docs/guides/fine-tuning/prepare-training-data).  (required)
-        :type file: bytearray
-        :param purpose: The intended purpose of the uploaded documents.  Use \\\"fine-tune\\\" for [Fine-tuning](/docs/api-reference/fine-tunes). This allows us to validate the format of the uploaded file.  (required)
-        :type purpose: str
+        :param create_thread_request:
+        :type create_thread_request: CreateThreadRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1569,37 +1625,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_file_serialize(
-            file=file,
-            purpose=purpose,
+        _param = self._create_thread_serialize(
+            create_thread_request=create_thread_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "OpenAIFile",
+            '200': "ThreadObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_file_serialize(
+    def _create_thread_serialize(
         self,
-        file,
-        purpose,
+        create_thread_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1614,19 +1668,17 @@
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
-        if file is not None:
-            _files['file'] = file
-        if purpose is not None:
-            _form_params.append(('purpose', purpose))
         # process the body parameter
+        if create_thread_request is not None:
+            _body_params = create_thread_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1635,28 +1687,29 @@
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
             _default_content_type = (
                 self.api_client.select_header_content_type(
                     [
-                        'multipart/form-data'
+                        'application/json'
                     ]
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/files',
+            resource_path='/threads',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1665,35 +1718,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_fine_tune(
+    def create_thread_and_run(
         self,
-        create_fine_tune_request: CreateFineTuneRequest,
+        create_thread_and_run_request: CreateThreadAndRunRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> FineTune:
-        """Creates a job that fine-tunes a specified model from a given dataset.  Response includes details of the enqueued job including job status and the name of the fine-tuned models once complete.  [Learn more about Fine-tuning](/docs/guides/fine-tuning) 
+    ) -> RunObject:
+        """Create a thread and run it in one request.
 
 
-        :param create_fine_tune_request: (required)
-        :type create_fine_tune_request: CreateFineTuneRequest
+        :param create_thread_and_run_request: (required)
+        :type create_thread_and_run_request: CreateThreadAndRunRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1708,58 +1761,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_fine_tune_serialize(
-            create_fine_tune_request=create_fine_tune_request,
+        _param = self._create_thread_and_run_serialize(
+            create_thread_and_run_request=create_thread_and_run_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FineTune",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_fine_tune_with_http_info(
+    def create_thread_and_run_with_http_info(
         self,
-        create_fine_tune_request: CreateFineTuneRequest,
+        create_thread_and_run_request: CreateThreadAndRunRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[FineTune]:
-        """Creates a job that fine-tunes a specified model from a given dataset.  Response includes details of the enqueued job including job status and the name of the fine-tuned models once complete.  [Learn more about Fine-tuning](/docs/guides/fine-tuning) 
+    ) -> ApiResponse[RunObject]:
+        """Create a thread and run it in one request.
 
 
-        :param create_fine_tune_request: (required)
-        :type create_fine_tune_request: CreateFineTuneRequest
+        :param create_thread_and_run_request: (required)
+        :type create_thread_and_run_request: CreateThreadAndRunRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1774,58 +1827,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_fine_tune_serialize(
-            create_fine_tune_request=create_fine_tune_request,
+        _param = self._create_thread_and_run_serialize(
+            create_thread_and_run_request=create_thread_and_run_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FineTune",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_fine_tune_without_preload_content(
+    def create_thread_and_run_without_preload_content(
         self,
-        create_fine_tune_request: CreateFineTuneRequest,
+        create_thread_and_run_request: CreateThreadAndRunRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Creates a job that fine-tunes a specified model from a given dataset.  Response includes details of the enqueued job including job status and the name of the fine-tuned models once complete.  [Learn more about Fine-tuning](/docs/guides/fine-tuning) 
+        """Create a thread and run it in one request.
 
 
-        :param create_fine_tune_request: (required)
-        :type create_fine_tune_request: CreateFineTuneRequest
+        :param create_thread_and_run_request: (required)
+        :type create_thread_and_run_request: CreateThreadAndRunRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1840,35 +1893,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_fine_tune_serialize(
-            create_fine_tune_request=create_fine_tune_request,
+        _param = self._create_thread_and_run_serialize(
+            create_thread_and_run_request=create_thread_and_run_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FineTune",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_fine_tune_serialize(
+    def _create_thread_and_run_serialize(
         self,
-        create_fine_tune_request,
+        create_thread_and_run_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1884,16 +1937,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_fine_tune_request is not None:
-            _body_params = create_fine_tune_request
+        if create_thread_and_run_request is not None:
+            _body_params = create_thread_and_run_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1911,19 +1964,20 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/fine-tunes',
+            resource_path='/threads/runs',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1932,35 +1986,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_image(
+    def delete_assistant(
         self,
-        create_image_request: CreateImageRequest,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ImagesResponse:
-        """Creates an image given a prompt.
+    ) -> DeleteAssistantResponse:
+        """Delete an assistant.
 
 
-        :param create_image_request: (required)
-        :type create_image_request: CreateImageRequest
+        :param assistant_id: The ID of the assistant to delete. (required)
+        :type assistant_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1975,58 +2029,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_image_serialize(
-            create_image_request=create_image_request,
+        _param = self._delete_assistant_serialize(
+            assistant_id=assistant_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImagesResponse",
+            '200': "DeleteAssistantResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_image_with_http_info(
+    def delete_assistant_with_http_info(
         self,
-        create_image_request: CreateImageRequest,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ImagesResponse]:
-        """Creates an image given a prompt.
+    ) -> ApiResponse[DeleteAssistantResponse]:
+        """Delete an assistant.
 
 
-        :param create_image_request: (required)
-        :type create_image_request: CreateImageRequest
+        :param assistant_id: The ID of the assistant to delete. (required)
+        :type assistant_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2041,58 +2095,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_image_serialize(
-            create_image_request=create_image_request,
+        _param = self._delete_assistant_serialize(
+            assistant_id=assistant_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImagesResponse",
+            '200': "DeleteAssistantResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_image_without_preload_content(
+    def delete_assistant_without_preload_content(
         self,
-        create_image_request: CreateImageRequest,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Creates an image given a prompt.
+        """Delete an assistant.
 
 
-        :param create_image_request: (required)
-        :type create_image_request: CreateImageRequest
+        :param assistant_id: The ID of the assistant to delete. (required)
+        :type assistant_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2107,35 +2161,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_image_serialize(
-            create_image_request=create_image_request,
+        _param = self._delete_assistant_serialize(
+            assistant_id=assistant_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImagesResponse",
+            '200': "DeleteAssistantResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_image_serialize(
+    def _delete_assistant_serialize(
         self,
-        create_image_request,
+        assistant_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -2147,50 +2201,38 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if assistant_id is not None:
+            _path_params['assistant_id'] = assistant_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_image_request is not None:
-            _body_params = create_image_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/images/generations',
+            method='DELETE',
+            resource_path='/assistants/{assistant_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2199,53 +2241,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_image_edit(
+    def delete_assistant_file(
         self,
-        image: Annotated[Union[StrictBytes, StrictStr], Field(description="The image to edit. Must be a valid PNG file, less than 4MB, and square. If mask is not provided, image must have transparency, which will be used as the mask.")],
-        prompt: Annotated[StrictStr, Field(description="A text description of the desired image(s). The maximum length is 1000 characters.")],
-        mask: Annotated[Optional[Union[StrictBytes, StrictStr]], Field(description="An additional image whose fully transparent areas (e.g. where alpha is zero) indicate where `image` should be edited. Must be a valid PNG file, less than 4MB, and have the same dimensions as `image`.")] = None,
-        n: Annotated[Optional[Annotated[int, Field(le=10, strict=True, ge=1)]], Field(description="The number of images to generate. Must be between 1 and 10.")] = None,
-        size: Annotated[Optional[StrictStr], Field(description="The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format in which the generated images are returned. Must be one of `url` or `b64_json`.")] = None,
-        user: Annotated[Optional[StrictStr], Field(description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")] = None,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant that the file belongs to.")],
+        file_id: Annotated[StrictStr, Field(description="The ID of the file to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ImagesResponse:
-        """Creates an edited or extended image given an original image and a prompt.
+    ) -> DeleteAssistantFileResponse:
+        """Delete an assistant file.
 
 
-        :param image: The image to edit. Must be a valid PNG file, less than 4MB, and square. If mask is not provided, image must have transparency, which will be used as the mask. (required)
-        :type image: bytearray
-        :param prompt: A text description of the desired image(s). The maximum length is 1000 characters. (required)
-        :type prompt: str
-        :param mask: An additional image whose fully transparent areas (e.g. where alpha is zero) indicate where `image` should be edited. Must be a valid PNG file, less than 4MB, and have the same dimensions as `image`.
-        :type mask: bytearray
-        :param n: The number of images to generate. Must be between 1 and 10.
-        :type n: int
-        :param size: The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.
-        :type size: str
-        :param response_format: The format in which the generated images are returned. Must be one of `url` or `b64_json`.
-        :type response_format: str
-        :param user: A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). 
-        :type user: str
+        :param assistant_id: The ID of the assistant that the file belongs to. (required)
+        :type assistant_id: str
+        :param file_id: The ID of the file to delete. (required)
+        :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2260,82 +2287,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_image_edit_serialize(
-            image=image,
-            prompt=prompt,
-            mask=mask,
-            n=n,
-            size=size,
-            response_format=response_format,
-            user=user,
+        _param = self._delete_assistant_file_serialize(
+            assistant_id=assistant_id,
+            file_id=file_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImagesResponse",
+            '200': "DeleteAssistantFileResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_image_edit_with_http_info(
+    def delete_assistant_file_with_http_info(
         self,
-        image: Annotated[Union[StrictBytes, StrictStr], Field(description="The image to edit. Must be a valid PNG file, less than 4MB, and square. If mask is not provided, image must have transparency, which will be used as the mask.")],
-        prompt: Annotated[StrictStr, Field(description="A text description of the desired image(s). The maximum length is 1000 characters.")],
-        mask: Annotated[Optional[Union[StrictBytes, StrictStr]], Field(description="An additional image whose fully transparent areas (e.g. where alpha is zero) indicate where `image` should be edited. Must be a valid PNG file, less than 4MB, and have the same dimensions as `image`.")] = None,
-        n: Annotated[Optional[Annotated[int, Field(le=10, strict=True, ge=1)]], Field(description="The number of images to generate. Must be between 1 and 10.")] = None,
-        size: Annotated[Optional[StrictStr], Field(description="The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format in which the generated images are returned. Must be one of `url` or `b64_json`.")] = None,
-        user: Annotated[Optional[StrictStr], Field(description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")] = None,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant that the file belongs to.")],
+        file_id: Annotated[StrictStr, Field(description="The ID of the file to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ImagesResponse]:
-        """Creates an edited or extended image given an original image and a prompt.
+    ) -> ApiResponse[DeleteAssistantFileResponse]:
+        """Delete an assistant file.
 
 
-        :param image: The image to edit. Must be a valid PNG file, less than 4MB, and square. If mask is not provided, image must have transparency, which will be used as the mask. (required)
-        :type image: bytearray
-        :param prompt: A text description of the desired image(s). The maximum length is 1000 characters. (required)
-        :type prompt: str
-        :param mask: An additional image whose fully transparent areas (e.g. where alpha is zero) indicate where `image` should be edited. Must be a valid PNG file, less than 4MB, and have the same dimensions as `image`.
-        :type mask: bytearray
-        :param n: The number of images to generate. Must be between 1 and 10.
-        :type n: int
-        :param size: The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.
-        :type size: str
-        :param response_format: The format in which the generated images are returned. Must be one of `url` or `b64_json`.
-        :type response_format: str
-        :param user: A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). 
-        :type user: str
+        :param assistant_id: The ID of the assistant that the file belongs to. (required)
+        :type assistant_id: str
+        :param file_id: The ID of the file to delete. (required)
+        :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2350,82 +2357,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_image_edit_serialize(
-            image=image,
-            prompt=prompt,
-            mask=mask,
-            n=n,
-            size=size,
-            response_format=response_format,
-            user=user,
+        _param = self._delete_assistant_file_serialize(
+            assistant_id=assistant_id,
+            file_id=file_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImagesResponse",
+            '200': "DeleteAssistantFileResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_image_edit_without_preload_content(
+    def delete_assistant_file_without_preload_content(
         self,
-        image: Annotated[Union[StrictBytes, StrictStr], Field(description="The image to edit. Must be a valid PNG file, less than 4MB, and square. If mask is not provided, image must have transparency, which will be used as the mask.")],
-        prompt: Annotated[StrictStr, Field(description="A text description of the desired image(s). The maximum length is 1000 characters.")],
-        mask: Annotated[Optional[Union[StrictBytes, StrictStr]], Field(description="An additional image whose fully transparent areas (e.g. where alpha is zero) indicate where `image` should be edited. Must be a valid PNG file, less than 4MB, and have the same dimensions as `image`.")] = None,
-        n: Annotated[Optional[Annotated[int, Field(le=10, strict=True, ge=1)]], Field(description="The number of images to generate. Must be between 1 and 10.")] = None,
-        size: Annotated[Optional[StrictStr], Field(description="The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format in which the generated images are returned. Must be one of `url` or `b64_json`.")] = None,
-        user: Annotated[Optional[StrictStr], Field(description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")] = None,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant that the file belongs to.")],
+        file_id: Annotated[StrictStr, Field(description="The ID of the file to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Creates an edited or extended image given an original image and a prompt.
+        """Delete an assistant file.
 
 
-        :param image: The image to edit. Must be a valid PNG file, less than 4MB, and square. If mask is not provided, image must have transparency, which will be used as the mask. (required)
-        :type image: bytearray
-        :param prompt: A text description of the desired image(s). The maximum length is 1000 characters. (required)
-        :type prompt: str
-        :param mask: An additional image whose fully transparent areas (e.g. where alpha is zero) indicate where `image` should be edited. Must be a valid PNG file, less than 4MB, and have the same dimensions as `image`.
-        :type mask: bytearray
-        :param n: The number of images to generate. Must be between 1 and 10.
-        :type n: int
-        :param size: The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.
-        :type size: str
-        :param response_format: The format in which the generated images are returned. Must be one of `url` or `b64_json`.
-        :type response_format: str
-        :param user: A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). 
-        :type user: str
+        :param assistant_id: The ID of the assistant that the file belongs to. (required)
+        :type assistant_id: str
+        :param file_id: The ID of the file to delete. (required)
+        :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2440,47 +2427,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_image_edit_serialize(
-            image=image,
-            prompt=prompt,
-            mask=mask,
-            n=n,
-            size=size,
-            response_format=response_format,
-            user=user,
+        _param = self._delete_assistant_file_serialize(
+            assistant_id=assistant_id,
+            file_id=file_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImagesResponse",
+            '200': "DeleteAssistantFileResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_image_edit_serialize(
+    def _delete_assistant_file_serialize(
         self,
-        image,
-        prompt,
-        mask,
-        n,
-        size,
-        response_format,
-        user,
+        assistant_id,
+        file_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -2492,62 +2469,40 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if assistant_id is not None:
+            _path_params['assistant_id'] = assistant_id
+        if file_id is not None:
+            _path_params['file_id'] = file_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
-        if image is not None:
-            _files['image'] = image
-        if mask is not None:
-            _files['mask'] = mask
-        if prompt is not None:
-            _form_params.append(('prompt', prompt))
-        if n is not None:
-            _form_params.append(('n', n))
-        if size is not None:
-            _form_params.append(('size', size))
-        if response_format is not None:
-            _form_params.append(('response_format', response_format))
-        if user is not None:
-            _form_params.append(('user', user))
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'multipart/form-data'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/images/edits',
+            method='DELETE',
+            resource_path='/assistants/{assistant_id}/files/{file_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2556,47 +2511,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_image_variation(
+    def delete_thread(
         self,
-        image: Annotated[Union[StrictBytes, StrictStr], Field(description="The image to use as the basis for the variation(s). Must be a valid PNG file, less than 4MB, and square.")],
-        n: Annotated[Optional[Annotated[int, Field(le=10, strict=True, ge=1)]], Field(description="The number of images to generate. Must be between 1 and 10.")] = None,
-        size: Annotated[Optional[StrictStr], Field(description="The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format in which the generated images are returned. Must be one of `url` or `b64_json`.")] = None,
-        user: Annotated[Optional[StrictStr], Field(description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")] = None,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ImagesResponse:
-        """Creates a variation of a given image.
+    ) -> DeleteThreadResponse:
+        """Delete a thread.
 
 
-        :param image: The image to use as the basis for the variation(s). Must be a valid PNG file, less than 4MB, and square. (required)
-        :type image: bytearray
-        :param n: The number of images to generate. Must be between 1 and 10.
-        :type n: int
-        :param size: The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.
-        :type size: str
-        :param response_format: The format in which the generated images are returned. Must be one of `url` or `b64_json`.
-        :type response_format: str
-        :param user: A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). 
-        :type user: str
+        :param thread_id: The ID of the thread to delete. (required)
+        :type thread_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2611,74 +2554,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_image_variation_serialize(
-            image=image,
-            n=n,
-            size=size,
-            response_format=response_format,
-            user=user,
+        _param = self._delete_thread_serialize(
+            thread_id=thread_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImagesResponse",
+            '200': "DeleteThreadResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_image_variation_with_http_info(
+    def delete_thread_with_http_info(
         self,
-        image: Annotated[Union[StrictBytes, StrictStr], Field(description="The image to use as the basis for the variation(s). Must be a valid PNG file, less than 4MB, and square.")],
-        n: Annotated[Optional[Annotated[int, Field(le=10, strict=True, ge=1)]], Field(description="The number of images to generate. Must be between 1 and 10.")] = None,
-        size: Annotated[Optional[StrictStr], Field(description="The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format in which the generated images are returned. Must be one of `url` or `b64_json`.")] = None,
-        user: Annotated[Optional[StrictStr], Field(description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")] = None,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ImagesResponse]:
-        """Creates a variation of a given image.
+    ) -> ApiResponse[DeleteThreadResponse]:
+        """Delete a thread.
 
 
-        :param image: The image to use as the basis for the variation(s). Must be a valid PNG file, less than 4MB, and square. (required)
-        :type image: bytearray
-        :param n: The number of images to generate. Must be between 1 and 10.
-        :type n: int
-        :param size: The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.
-        :type size: str
-        :param response_format: The format in which the generated images are returned. Must be one of `url` or `b64_json`.
-        :type response_format: str
-        :param user: A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). 
-        :type user: str
+        :param thread_id: The ID of the thread to delete. (required)
+        :type thread_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2693,74 +2620,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_image_variation_serialize(
-            image=image,
-            n=n,
-            size=size,
-            response_format=response_format,
-            user=user,
+        _param = self._delete_thread_serialize(
+            thread_id=thread_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImagesResponse",
+            '200': "DeleteThreadResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_image_variation_without_preload_content(
+    def delete_thread_without_preload_content(
         self,
-        image: Annotated[Union[StrictBytes, StrictStr], Field(description="The image to use as the basis for the variation(s). Must be a valid PNG file, less than 4MB, and square.")],
-        n: Annotated[Optional[Annotated[int, Field(le=10, strict=True, ge=1)]], Field(description="The number of images to generate. Must be between 1 and 10.")] = None,
-        size: Annotated[Optional[StrictStr], Field(description="The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format in which the generated images are returned. Must be one of `url` or `b64_json`.")] = None,
-        user: Annotated[Optional[StrictStr], Field(description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). ")] = None,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to delete.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Creates a variation of a given image.
+        """Delete a thread.
 
 
-        :param image: The image to use as the basis for the variation(s). Must be a valid PNG file, less than 4MB, and square. (required)
-        :type image: bytearray
-        :param n: The number of images to generate. Must be between 1 and 10.
-        :type n: int
-        :param size: The size of the generated images. Must be one of `256x256`, `512x512`, or `1024x1024`.
-        :type size: str
-        :param response_format: The format in which the generated images are returned. Must be one of `url` or `b64_json`.
-        :type response_format: str
-        :param user: A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. [Learn more](/docs/guides/safety-best-practices/end-user-ids). 
-        :type user: str
+        :param thread_id: The ID of the thread to delete. (required)
+        :type thread_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2775,43 +2686,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_image_variation_serialize(
-            image=image,
-            n=n,
-            size=size,
-            response_format=response_format,
-            user=user,
+        _param = self._delete_thread_serialize(
+            thread_id=thread_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImagesResponse",
+            '200': "DeleteThreadResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_image_variation_serialize(
+    def _delete_thread_serialize(
         self,
-        image,
-        n,
-        size,
-        response_format,
-        user,
+        thread_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -2823,58 +2726,38 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
-        if image is not None:
-            _files['image'] = image
-        if n is not None:
-            _form_params.append(('n', n))
-        if size is not None:
-            _form_params.append(('size', size))
-        if response_format is not None:
-            _form_params.append(('response_format', response_format))
-        if user is not None:
-            _form_params.append(('user', user))
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'multipart/form-data'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/images/variations',
+            method='DELETE',
+            resource_path='/threads/{thread_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2883,35 +2766,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_moderation(
+    def get_assistant(
         self,
-        create_moderation_request: CreateModerationRequest,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateModerationResponse:
-        """Classifies if text violates OpenAI's Content Policy
+    ) -> AssistantObject:
+        """Retrieves an assistant.
 
 
-        :param create_moderation_request: (required)
-        :type create_moderation_request: CreateModerationRequest
+        :param assistant_id: The ID of the assistant to retrieve. (required)
+        :type assistant_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2926,58 +2809,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_moderation_serialize(
-            create_moderation_request=create_moderation_request,
+        _param = self._get_assistant_serialize(
+            assistant_id=assistant_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateModerationResponse",
+            '200': "AssistantObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_moderation_with_http_info(
+    def get_assistant_with_http_info(
         self,
-        create_moderation_request: CreateModerationRequest,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateModerationResponse]:
-        """Classifies if text violates OpenAI's Content Policy
+    ) -> ApiResponse[AssistantObject]:
+        """Retrieves an assistant.
 
 
-        :param create_moderation_request: (required)
-        :type create_moderation_request: CreateModerationRequest
+        :param assistant_id: The ID of the assistant to retrieve. (required)
+        :type assistant_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2992,58 +2875,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_moderation_serialize(
-            create_moderation_request=create_moderation_request,
+        _param = self._get_assistant_serialize(
+            assistant_id=assistant_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateModerationResponse",
+            '200': "AssistantObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_moderation_without_preload_content(
+    def get_assistant_without_preload_content(
         self,
-        create_moderation_request: CreateModerationRequest,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Classifies if text violates OpenAI's Content Policy
+        """Retrieves an assistant.
 
 
-        :param create_moderation_request: (required)
-        :type create_moderation_request: CreateModerationRequest
+        :param assistant_id: The ID of the assistant to retrieve. (required)
+        :type assistant_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3058,35 +2941,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_moderation_serialize(
-            create_moderation_request=create_moderation_request,
+        _param = self._get_assistant_serialize(
+            assistant_id=assistant_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateModerationResponse",
+            '200': "AssistantObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_moderation_serialize(
+    def _get_assistant_serialize(
         self,
-        create_moderation_request,
+        assistant_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -3098,50 +2981,38 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if assistant_id is not None:
+            _path_params['assistant_id'] = assistant_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_moderation_request is not None:
-            _body_params = create_moderation_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/moderations',
+            method='GET',
+            resource_path='/assistants/{assistant_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -3150,50 +3021,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_transcription(
+    def get_assistant_file(
         self,
-        file: Annotated[Union[StrictBytes, StrictStr], Field(description="The audio file object (not file name) to transcribe, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm. ")],
-        model: CreateTranscriptionRequestModel,
-        prompt: Annotated[Optional[StrictStr], Field(description="An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should match the audio language. ")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. ")] = None,
-        temperature: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. ")] = None,
-        language: Annotated[Optional[StrictStr], Field(description="The language of the input audio. Supplying the input language in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format will improve accuracy and latency. ")] = None,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant who the file belongs to.")],
+        file_id: Annotated[StrictStr, Field(description="The ID of the file we're getting.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateTranscriptionResponse:
-        """Transcribes audio into the input language.
+    ) -> AssistantFileObject:
+        """Retrieves an AssistantFile.
 
 
-        :param file: The audio file object (not file name) to transcribe, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm.  (required)
-        :type file: bytearray
-        :param model: (required)
-        :type model: CreateTranscriptionRequestModel
-        :param prompt: An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should match the audio language. 
-        :type prompt: str
-        :param response_format: The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. 
-        :type response_format: str
-        :param temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. 
-        :type temperature: float
-        :param language: The language of the input audio. Supplying the input language in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format will improve accuracy and latency. 
-        :type language: str
+        :param assistant_id: The ID of the assistant who the file belongs to. (required)
+        :type assistant_id: str
+        :param file_id: The ID of the file we're getting. (required)
+        :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3208,78 +3067,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_transcription_serialize(
-            file=file,
-            model=model,
-            prompt=prompt,
-            response_format=response_format,
-            temperature=temperature,
-            language=language,
+        _param = self._get_assistant_file_serialize(
+            assistant_id=assistant_id,
+            file_id=file_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateTranscriptionResponse",
+            '200': "AssistantFileObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_transcription_with_http_info(
+    def get_assistant_file_with_http_info(
         self,
-        file: Annotated[Union[StrictBytes, StrictStr], Field(description="The audio file object (not file name) to transcribe, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm. ")],
-        model: CreateTranscriptionRequestModel,
-        prompt: Annotated[Optional[StrictStr], Field(description="An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should match the audio language. ")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. ")] = None,
-        temperature: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. ")] = None,
-        language: Annotated[Optional[StrictStr], Field(description="The language of the input audio. Supplying the input language in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format will improve accuracy and latency. ")] = None,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant who the file belongs to.")],
+        file_id: Annotated[StrictStr, Field(description="The ID of the file we're getting.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateTranscriptionResponse]:
-        """Transcribes audio into the input language.
+    ) -> ApiResponse[AssistantFileObject]:
+        """Retrieves an AssistantFile.
 
 
-        :param file: The audio file object (not file name) to transcribe, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm.  (required)
-        :type file: bytearray
-        :param model: (required)
-        :type model: CreateTranscriptionRequestModel
-        :param prompt: An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should match the audio language. 
-        :type prompt: str
-        :param response_format: The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. 
-        :type response_format: str
-        :param temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. 
-        :type temperature: float
-        :param language: The language of the input audio. Supplying the input language in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format will improve accuracy and latency. 
-        :type language: str
+        :param assistant_id: The ID of the assistant who the file belongs to. (required)
+        :type assistant_id: str
+        :param file_id: The ID of the file we're getting. (required)
+        :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3294,78 +3137,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_transcription_serialize(
-            file=file,
-            model=model,
-            prompt=prompt,
-            response_format=response_format,
-            temperature=temperature,
-            language=language,
+        _param = self._get_assistant_file_serialize(
+            assistant_id=assistant_id,
+            file_id=file_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateTranscriptionResponse",
+            '200': "AssistantFileObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_transcription_without_preload_content(
+    def get_assistant_file_without_preload_content(
         self,
-        file: Annotated[Union[StrictBytes, StrictStr], Field(description="The audio file object (not file name) to transcribe, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm. ")],
-        model: CreateTranscriptionRequestModel,
-        prompt: Annotated[Optional[StrictStr], Field(description="An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should match the audio language. ")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. ")] = None,
-        temperature: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. ")] = None,
-        language: Annotated[Optional[StrictStr], Field(description="The language of the input audio. Supplying the input language in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format will improve accuracy and latency. ")] = None,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant who the file belongs to.")],
+        file_id: Annotated[StrictStr, Field(description="The ID of the file we're getting.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Transcribes audio into the input language.
+        """Retrieves an AssistantFile.
 
 
-        :param file: The audio file object (not file name) to transcribe, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm.  (required)
-        :type file: bytearray
-        :param model: (required)
-        :type model: CreateTranscriptionRequestModel
-        :param prompt: An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should match the audio language. 
-        :type prompt: str
-        :param response_format: The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. 
-        :type response_format: str
-        :param temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. 
-        :type temperature: float
-        :param language: The language of the input audio. Supplying the input language in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format will improve accuracy and latency. 
-        :type language: str
+        :param assistant_id: The ID of the assistant who the file belongs to. (required)
+        :type assistant_id: str
+        :param file_id: The ID of the file we're getting. (required)
+        :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3380,45 +3207,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_transcription_serialize(
-            file=file,
-            model=model,
-            prompt=prompt,
-            response_format=response_format,
-            temperature=temperature,
-            language=language,
+        _param = self._get_assistant_file_serialize(
+            assistant_id=assistant_id,
+            file_id=file_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateTranscriptionResponse",
+            '200': "AssistantFileObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_transcription_serialize(
+    def _get_assistant_file_serialize(
         self,
-        file,
-        model,
-        prompt,
-        response_format,
-        temperature,
-        language,
+        assistant_id,
+        file_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -3430,60 +3249,40 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if assistant_id is not None:
+            _path_params['assistant_id'] = assistant_id
+        if file_id is not None:
+            _path_params['file_id'] = file_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
-        if file is not None:
-            _files['file'] = file
-        if model is not None:
-            _form_params.append(('model', model))
-        if prompt is not None:
-            _form_params.append(('prompt', prompt))
-        if response_format is not None:
-            _form_params.append(('response_format', response_format))
-        if temperature is not None:
-            _form_params.append(('temperature', temperature))
-        if language is not None:
-            _form_params.append(('language', language))
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'multipart/form-data'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/audio/transcriptions',
+            method='GET',
+            resource_path='/assistants/{assistant_id}/files/{file_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -3492,47 +3291,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_translation(
+    def get_message(
         self,
-        file: Annotated[Union[StrictBytes, StrictStr], Field(description="The audio file object (not file name) translate, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm. ")],
-        model: CreateTranscriptionRequestModel,
-        prompt: Annotated[Optional[StrictStr], Field(description="An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should be in English. ")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. ")] = None,
-        temperature: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. ")] = None,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) to which this message belongs.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateTranslationResponse:
-        """Translates audio into English.
+    ) -> MessageObject:
+        """Retrieve a message.
 
 
-        :param file: The audio file object (not file name) translate, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm.  (required)
-        :type file: bytearray
-        :param model: (required)
-        :type model: CreateTranscriptionRequestModel
-        :param prompt: An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should be in English. 
-        :type prompt: str
-        :param response_format: The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. 
-        :type response_format: str
-        :param temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. 
-        :type temperature: float
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) to which this message belongs. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message to retrieve. (required)
+        :type message_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3547,74 +3337,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_translation_serialize(
-            file=file,
-            model=model,
-            prompt=prompt,
-            response_format=response_format,
-            temperature=temperature,
+        _param = self._get_message_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateTranslationResponse",
+            '200': "MessageObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_translation_with_http_info(
+    def get_message_with_http_info(
         self,
-        file: Annotated[Union[StrictBytes, StrictStr], Field(description="The audio file object (not file name) translate, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm. ")],
-        model: CreateTranscriptionRequestModel,
-        prompt: Annotated[Optional[StrictStr], Field(description="An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should be in English. ")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. ")] = None,
-        temperature: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. ")] = None,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) to which this message belongs.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateTranslationResponse]:
-        """Translates audio into English.
+    ) -> ApiResponse[MessageObject]:
+        """Retrieve a message.
 
 
-        :param file: The audio file object (not file name) translate, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm.  (required)
-        :type file: bytearray
-        :param model: (required)
-        :type model: CreateTranscriptionRequestModel
-        :param prompt: An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should be in English. 
-        :type prompt: str
-        :param response_format: The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. 
-        :type response_format: str
-        :param temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. 
-        :type temperature: float
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) to which this message belongs. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message to retrieve. (required)
+        :type message_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3629,74 +3407,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_translation_serialize(
-            file=file,
-            model=model,
-            prompt=prompt,
-            response_format=response_format,
-            temperature=temperature,
+        _param = self._get_message_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateTranslationResponse",
+            '200': "MessageObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_translation_without_preload_content(
+    def get_message_without_preload_content(
         self,
-        file: Annotated[Union[StrictBytes, StrictStr], Field(description="The audio file object (not file name) translate, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm. ")],
-        model: CreateTranscriptionRequestModel,
-        prompt: Annotated[Optional[StrictStr], Field(description="An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should be in English. ")] = None,
-        response_format: Annotated[Optional[StrictStr], Field(description="The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. ")] = None,
-        temperature: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. ")] = None,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) to which this message belongs.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Translates audio into English.
+        """Retrieve a message.
 
 
-        :param file: The audio file object (not file name) translate, in one of these formats: mp3, mp4, mpeg, mpga, m4a, wav, or webm.  (required)
-        :type file: bytearray
-        :param model: (required)
-        :type model: CreateTranscriptionRequestModel
-        :param prompt: An optional text to guide the model's style or continue a previous audio segment. The [prompt](/docs/guides/speech-to-text/prompting) should be in English. 
-        :type prompt: str
-        :param response_format: The format of the transcript output, in one of these options: json, text, srt, verbose_json, or vtt. 
-        :type response_format: str
-        :param temperature: The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use [log probability](https://en.wikipedia.org/wiki/Log_probability) to automatically increase the temperature until certain thresholds are hit. 
-        :type temperature: float
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) to which this message belongs. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message to retrieve. (required)
+        :type message_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3711,43 +3477,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_translation_serialize(
-            file=file,
-            model=model,
-            prompt=prompt,
-            response_format=response_format,
-            temperature=temperature,
+        _param = self._get_message_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateTranslationResponse",
+            '200': "MessageObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_translation_serialize(
+    def _get_message_serialize(
         self,
-        file,
-        model,
-        prompt,
-        response_format,
-        temperature,
+        thread_id,
+        message_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -3759,58 +3519,40 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if message_id is not None:
+            _path_params['message_id'] = message_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
-        if file is not None:
-            _files['file'] = file
-        if model is not None:
-            _form_params.append(('model', model))
-        if prompt is not None:
-            _form_params.append(('prompt', prompt))
-        if response_format is not None:
-            _form_params.append(('response_format', response_format))
-        if temperature is not None:
-            _form_params.append(('temperature', temperature))
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'multipart/form-data'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/audio/translations',
+            method='GET',
+            resource_path='/threads/{thread_id}/messages/{message_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -3819,34 +3561,40 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def delete_file(
+    def get_message_file(
         self,
-        file_id: Annotated[StrictStr, Field(description="The ID of the file to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which the message and File belong.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message the file belongs to.")],
+        file_id: Annotated[StrictStr, Field(description="The ID of the file being retrieved.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> DeleteFileResponse:
-        """Delete a file.
+    ) -> MessageFileObject:
+        """Retrieves a message file.
 
 
-        :param file_id: The ID of the file to use for this request (required)
+        :param thread_id: The ID of the thread to which the message and File belong. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message the file belongs to. (required)
+        :type message_id: str
+        :param file_id: The ID of the file being retrieved. (required)
         :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -3862,57 +3610,65 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_file_serialize(
+        _param = self._get_message_file_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
             file_id=file_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "DeleteFileResponse",
+            '200': "MessageFileObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def delete_file_with_http_info(
+    def get_message_file_with_http_info(
         self,
-        file_id: Annotated[StrictStr, Field(description="The ID of the file to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which the message and File belong.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message the file belongs to.")],
+        file_id: Annotated[StrictStr, Field(description="The ID of the file being retrieved.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[DeleteFileResponse]:
-        """Delete a file.
+    ) -> ApiResponse[MessageFileObject]:
+        """Retrieves a message file.
 
 
-        :param file_id: The ID of the file to use for this request (required)
+        :param thread_id: The ID of the thread to which the message and File belong. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message the file belongs to. (required)
+        :type message_id: str
+        :param file_id: The ID of the file being retrieved. (required)
         :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -3928,57 +3684,65 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_file_serialize(
+        _param = self._get_message_file_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
             file_id=file_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "DeleteFileResponse",
+            '200': "MessageFileObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def delete_file_without_preload_content(
+    def get_message_file_without_preload_content(
         self,
-        file_id: Annotated[StrictStr, Field(description="The ID of the file to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which the message and File belong.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message the file belongs to.")],
+        file_id: Annotated[StrictStr, Field(description="The ID of the file being retrieved.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a file.
+        """Retrieves a message file.
 
 
-        :param file_id: The ID of the file to use for this request (required)
+        :param thread_id: The ID of the thread to which the message and File belong. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message the file belongs to. (required)
+        :type message_id: str
+        :param file_id: The ID of the file being retrieved. (required)
         :type file_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -3994,34 +3758,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_file_serialize(
+        _param = self._get_message_file_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
             file_id=file_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "DeleteFileResponse",
+            '200': "MessageFileObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _delete_file_serialize(
+    def _get_message_file_serialize(
         self,
+        thread_id,
+        message_id,
         file_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
@@ -4034,14 +3802,18 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if message_id is not None:
+            _path_params['message_id'] = message_id
         if file_id is not None:
             _path_params['file_id'] = file_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
@@ -4052,19 +3824,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='DELETE',
-            resource_path='/files/{file_id}',
+            method='GET',
+            resource_path='/threads/{thread_id}/messages/{message_id}/files/{file_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -4073,35 +3846,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def delete_model(
+    def get_run(
         self,
-        model: Annotated[StrictStr, Field(description="The model to delete")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) that was run.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> DeleteModelResponse:
-        """Delete a fine-tuned model. You must have the Owner role in your organization.
+    ) -> RunObject:
+        """Retrieves a run.
 
 
-        :param model: The model to delete (required)
-        :type model: str
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) that was run. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to retrieve. (required)
+        :type run_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4116,58 +3892,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_model_serialize(
-            model=model,
+        _param = self._get_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "DeleteModelResponse",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def delete_model_with_http_info(
+    def get_run_with_http_info(
         self,
-        model: Annotated[StrictStr, Field(description="The model to delete")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) that was run.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[DeleteModelResponse]:
-        """Delete a fine-tuned model. You must have the Owner role in your organization.
+    ) -> ApiResponse[RunObject]:
+        """Retrieves a run.
 
 
-        :param model: The model to delete (required)
-        :type model: str
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) that was run. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to retrieve. (required)
+        :type run_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4182,58 +3962,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_model_serialize(
-            model=model,
+        _param = self._get_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "DeleteModelResponse",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def delete_model_without_preload_content(
+    def get_run_without_preload_content(
         self,
-        model: Annotated[StrictStr, Field(description="The model to delete")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) that was run.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a fine-tuned model. You must have the Owner role in your organization.
+        """Retrieves a run.
 
 
-        :param model: The model to delete (required)
-        :type model: str
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) that was run. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to retrieve. (required)
+        :type run_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4248,35 +4032,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_model_serialize(
-            model=model,
+        _param = self._get_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "DeleteModelResponse",
+            '200': "RunObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _delete_model_serialize(
+    def _get_run_serialize(
         self,
-        model,
+        thread_id,
+        run_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -4288,16 +4074,18 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if model is not None:
-            _path_params['model'] = model
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if run_id is not None:
+            _path_params['run_id'] = run_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -4306,19 +4094,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='DELETE',
-            resource_path='/models/{model}',
+            method='GET',
+            resource_path='/threads/{thread_id}/runs/{run_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -4327,35 +4116,41 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def download_file(
+    def get_run_step(
         self,
-        file_id: Annotated[StrictStr, Field(description="The ID of the file to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which the run and run step belongs.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to which the run step belongs.")],
+        step_id: Annotated[StrictStr, Field(description="The ID of the run step to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> str:
-        """Returns the contents of the specified file
+    ) -> RunStepObject:
+        """Retrieves a run step.
 
 
-        :param file_id: The ID of the file to use for this request (required)
-        :type file_id: str
+        :param thread_id: The ID of the thread to which the run and run step belongs. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to which the run step belongs. (required)
+        :type run_id: str
+        :param step_id: The ID of the run step to retrieve. (required)
+        :type step_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4370,58 +4165,66 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._download_file_serialize(
-            file_id=file_id,
+        _param = self._get_run_step_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            step_id=step_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "str",
+            '200': "RunStepObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def download_file_with_http_info(
+    def get_run_step_with_http_info(
         self,
-        file_id: Annotated[StrictStr, Field(description="The ID of the file to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which the run and run step belongs.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to which the run step belongs.")],
+        step_id: Annotated[StrictStr, Field(description="The ID of the run step to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[str]:
-        """Returns the contents of the specified file
+    ) -> ApiResponse[RunStepObject]:
+        """Retrieves a run step.
 
 
-        :param file_id: The ID of the file to use for this request (required)
-        :type file_id: str
+        :param thread_id: The ID of the thread to which the run and run step belongs. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to which the run step belongs. (required)
+        :type run_id: str
+        :param step_id: The ID of the run step to retrieve. (required)
+        :type step_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4436,58 +4239,66 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._download_file_serialize(
-            file_id=file_id,
+        _param = self._get_run_step_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            step_id=step_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "str",
+            '200': "RunStepObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def download_file_without_preload_content(
+    def get_run_step_without_preload_content(
         self,
-        file_id: Annotated[StrictStr, Field(description="The ID of the file to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which the run and run step belongs.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to which the run step belongs.")],
+        step_id: Annotated[StrictStr, Field(description="The ID of the run step to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Returns the contents of the specified file
+        """Retrieves a run step.
 
 
-        :param file_id: The ID of the file to use for this request (required)
-        :type file_id: str
+        :param thread_id: The ID of the thread to which the run and run step belongs. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to which the run step belongs. (required)
+        :type run_id: str
+        :param step_id: The ID of the run step to retrieve. (required)
+        :type step_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4502,35 +4313,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._download_file_serialize(
-            file_id=file_id,
+        _param = self._get_run_step_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            step_id=step_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "str",
+            '200': "RunStepObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _download_file_serialize(
+    def _get_run_step_serialize(
         self,
-        file_id,
+        thread_id,
+        run_id,
+        step_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -4542,16 +4357,20 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if file_id is not None:
-            _path_params['file_id'] = file_id
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if run_id is not None:
+            _path_params['run_id'] = run_id
+        if step_id is not None:
+            _path_params['step_id'] = step_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -4560,19 +4379,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/files/{file_id}/content',
+            resource_path='/threads/{thread_id}/runs/{run_id}/steps/{step_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -4581,32 +4401,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_files(
+    def get_thread(
         self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ListFilesResponse:
-        """Returns a list of files that belong to the user's organization.
+    ) -> ThreadObject:
+        """Retrieves a thread.
 
 
+        :param thread_id: The ID of the thread to retrieve. (required)
+        :type thread_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4621,54 +4444,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_files_serialize(
+        _param = self._get_thread_serialize(
+            thread_id=thread_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListFilesResponse",
+            '200': "ThreadObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_files_with_http_info(
+    def get_thread_with_http_info(
         self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ListFilesResponse]:
-        """Returns a list of files that belong to the user's organization.
+    ) -> ApiResponse[ThreadObject]:
+        """Retrieves a thread.
 
 
+        :param thread_id: The ID of the thread to retrieve. (required)
+        :type thread_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4683,54 +4510,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_files_serialize(
+        _param = self._get_thread_serialize(
+            thread_id=thread_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListFilesResponse",
+            '200': "ThreadObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_files_without_preload_content(
+    def get_thread_without_preload_content(
         self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to retrieve.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Returns a list of files that belong to the user's organization.
+        """Retrieves a thread.
 
 
+        :param thread_id: The ID of the thread to retrieve. (required)
+        :type thread_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4745,33 +4576,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_files_serialize(
+        _param = self._get_thread_serialize(
+            thread_id=thread_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListFilesResponse",
+            '200': "ThreadObject",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_files_serialize(
+    def _get_thread_serialize(
         self,
+        thread_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -4783,14 +4616,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -4799,19 +4634,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/files',
+            resource_path='/threads/{thread_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -4820,38 +4656,47 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_fine_tune_events(
+    def list_assistant_files(
         self,
-        fine_tune_id: Annotated[StrictStr, Field(description="The ID of the fine-tune job to get events for. ")],
-        stream: Annotated[Optional[StrictBool], Field(description="Whether to stream events for the fine-tune job. If set to true, events will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available. The stream will terminate with a `data: [DONE]` message when the job is finished (succeeded, cancelled, or failed).  If set to false, only events generated so far will be returned. ")] = None,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant the file belongs to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ListFineTuneEventsResponse:
-        """Get fine-grained status updates for a fine-tune job. 
+    ) -> ListAssistantFilesResponse:
+        """Returns a list of assistant files.
 
 
-        :param fine_tune_id: The ID of the fine-tune job to get events for.  (required)
-        :type fine_tune_id: str
-        :param stream: Whether to stream events for the fine-tune job. If set to true, events will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available. The stream will terminate with a `data: [DONE]` message when the job is finished (succeeded, cancelled, or failed).  If set to false, only events generated so far will be returned. 
-        :type stream: bool
+        :param assistant_id: The ID of the assistant the file belongs to. (required)
+        :type assistant_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4866,62 +4711,74 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_fine_tune_events_serialize(
-            fine_tune_id=fine_tune_id,
-            stream=stream,
+        _param = self._list_assistant_files_serialize(
+            assistant_id=assistant_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListFineTuneEventsResponse",
+            '200': "ListAssistantFilesResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_fine_tune_events_with_http_info(
+    def list_assistant_files_with_http_info(
         self,
-        fine_tune_id: Annotated[StrictStr, Field(description="The ID of the fine-tune job to get events for. ")],
-        stream: Annotated[Optional[StrictBool], Field(description="Whether to stream events for the fine-tune job. If set to true, events will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available. The stream will terminate with a `data: [DONE]` message when the job is finished (succeeded, cancelled, or failed).  If set to false, only events generated so far will be returned. ")] = None,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant the file belongs to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ListFineTuneEventsResponse]:
-        """Get fine-grained status updates for a fine-tune job. 
+    ) -> ApiResponse[ListAssistantFilesResponse]:
+        """Returns a list of assistant files.
 
 
-        :param fine_tune_id: The ID of the fine-tune job to get events for.  (required)
-        :type fine_tune_id: str
-        :param stream: Whether to stream events for the fine-tune job. If set to true, events will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available. The stream will terminate with a `data: [DONE]` message when the job is finished (succeeded, cancelled, or failed).  If set to false, only events generated so far will be returned. 
-        :type stream: bool
+        :param assistant_id: The ID of the assistant the file belongs to. (required)
+        :type assistant_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4936,62 +4793,74 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_fine_tune_events_serialize(
-            fine_tune_id=fine_tune_id,
-            stream=stream,
+        _param = self._list_assistant_files_serialize(
+            assistant_id=assistant_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListFineTuneEventsResponse",
+            '200': "ListAssistantFilesResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_fine_tune_events_without_preload_content(
+    def list_assistant_files_without_preload_content(
         self,
-        fine_tune_id: Annotated[StrictStr, Field(description="The ID of the fine-tune job to get events for. ")],
-        stream: Annotated[Optional[StrictBool], Field(description="Whether to stream events for the fine-tune job. If set to true, events will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available. The stream will terminate with a `data: [DONE]` message when the job is finished (succeeded, cancelled, or failed).  If set to false, only events generated so far will be returned. ")] = None,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant the file belongs to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get fine-grained status updates for a fine-tune job. 
+        """Returns a list of assistant files.
 
 
-        :param fine_tune_id: The ID of the fine-tune job to get events for.  (required)
-        :type fine_tune_id: str
-        :param stream: Whether to stream events for the fine-tune job. If set to true, events will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format) as they become available. The stream will terminate with a `data: [DONE]` message when the job is finished (succeeded, cancelled, or failed).  If set to false, only events generated so far will be returned. 
-        :type stream: bool
+        :param assistant_id: The ID of the assistant the file belongs to. (required)
+        :type assistant_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5006,37 +4875,43 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_fine_tune_events_serialize(
-            fine_tune_id=fine_tune_id,
-            stream=stream,
+        _param = self._list_assistant_files_serialize(
+            assistant_id=assistant_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListFineTuneEventsResponse",
+            '200': "ListAssistantFilesResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_fine_tune_events_serialize(
+    def _list_assistant_files_serialize(
         self,
-        fine_tune_id,
-        stream,
+        assistant_id,
+        limit,
+        order,
+        after,
+        before,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -5048,20 +4923,32 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if fine_tune_id is not None:
-            _path_params['fine_tune_id'] = fine_tune_id
+        if assistant_id is not None:
+            _path_params['assistant_id'] = assistant_id
         # process the query parameters
-        if stream is not None:
+        if limit is not None:
             
-            _query_params.append(('stream', stream))
+            _query_params.append(('limit', limit))
+            
+        if order is not None:
+            
+            _query_params.append(('order', order))
+            
+        if after is not None:
+            
+            _query_params.append(('after', after))
+            
+        if before is not None:
+            
+            _query_params.append(('before', before))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -5070,19 +4957,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/fine-tunes/{fine_tune_id}/events',
+            resource_path='/assistants/{assistant_id}/files',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -5091,32 +4979,44 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_fine_tunes(
+    def list_assistants(
         self,
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ListFineTunesResponse:
-        """List your organization's fine-tuning jobs 
+    ) -> ListAssistantsResponse:
+        """Returns a list of assistants.
 
 
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5131,54 +5031,70 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_fine_tunes_serialize(
+        _param = self._list_assistants_serialize(
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListFineTunesResponse",
+            '200': "ListAssistantsResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_fine_tunes_with_http_info(
+    def list_assistants_with_http_info(
         self,
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ListFineTunesResponse]:
-        """List your organization's fine-tuning jobs 
+    ) -> ApiResponse[ListAssistantsResponse]:
+        """Returns a list of assistants.
 
 
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5193,54 +5109,70 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_fine_tunes_serialize(
+        _param = self._list_assistants_serialize(
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListFineTunesResponse",
+            '200': "ListAssistantsResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_fine_tunes_without_preload_content(
+    def list_assistants_without_preload_content(
         self,
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """List your organization's fine-tuning jobs 
+        """Returns a list of assistants.
 
 
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5255,33 +5187,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_fine_tunes_serialize(
+        _param = self._list_assistants_serialize(
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListFineTunesResponse",
+            '200': "ListAssistantsResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_fine_tunes_serialize(
+    def _list_assistants_serialize(
         self,
+        limit,
+        order,
+        after,
+        before,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -5294,14 +5234,30 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
+        if order is not None:
+            
+            _query_params.append(('order', order))
+            
+        if after is not None:
+            
+            _query_params.append(('after', after))
+            
+        if before is not None:
+            
+            _query_params.append(('before', before))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -5309,19 +5265,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/fine-tunes',
+            resource_path='/assistants',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -5330,32 +5287,50 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_models(
+    def list_message_files(
         self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread that the message and files belong to.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message that the files belongs to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ListModelsResponse:
-        """Lists the currently available models, and provides basic information about each one such as the owner and availability.
+    ) -> ListMessageFilesResponse:
+        """Returns a list of message files.
 
 
+        :param thread_id: The ID of the thread that the message and files belong to. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message that the files belongs to. (required)
+        :type message_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5370,54 +5345,78 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_models_serialize(
+        _param = self._list_message_files_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListModelsResponse",
+            '200': "ListMessageFilesResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_models_with_http_info(
+    def list_message_files_with_http_info(
         self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread that the message and files belong to.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message that the files belongs to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ListModelsResponse]:
-        """Lists the currently available models, and provides basic information about each one such as the owner and availability.
+    ) -> ApiResponse[ListMessageFilesResponse]:
+        """Returns a list of message files.
 
 
+        :param thread_id: The ID of the thread that the message and files belong to. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message that the files belongs to. (required)
+        :type message_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5432,54 +5431,78 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_models_serialize(
+        _param = self._list_message_files_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListModelsResponse",
+            '200': "ListMessageFilesResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_models_without_preload_content(
+    def list_message_files_without_preload_content(
         self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread that the message and files belong to.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message that the files belongs to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Lists the currently available models, and provides basic information about each one such as the owner and availability.
+        """Returns a list of message files.
 
 
+        :param thread_id: The ID of the thread that the message and files belong to. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message that the files belongs to. (required)
+        :type message_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5494,33 +5517,45 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_models_serialize(
+        _param = self._list_message_files_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListModelsResponse",
+            '200': "ListMessageFilesResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_models_serialize(
+    def _list_message_files_serialize(
         self,
+        thread_id,
+        message_id,
+        limit,
+        order,
+        after,
+        before,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -5532,15 +5567,35 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if message_id is not None:
+            _path_params['message_id'] = message_id
         # process the query parameters
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
+        if order is not None:
+            
+            _query_params.append(('order', order))
+            
+        if after is not None:
+            
+            _query_params.append(('after', after))
+            
+        if before is not None:
+            
+            _query_params.append(('before', before))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -5548,19 +5603,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/models',
+            resource_path='/threads/{thread_id}/messages/{message_id}/files',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -5569,35 +5625,50 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def retrieve_file(
+    def list_messages(
         self,
-        file_id: Annotated[StrictStr, Field(description="The ID of the file to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) the messages belong to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
+        run_id: Annotated[Optional[StrictStr], Field(description="Filter messages by the run ID that generated them. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> OpenAIFile:
-        """Returns information about a specific file.
+    ) -> ListMessagesResponse:
+        """Returns a list of messages for a given thread.
 
 
-        :param file_id: The ID of the file to use for this request (required)
-        :type file_id: str
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) the messages belong to. (required)
+        :type thread_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
+        :param run_id: Filter messages by the run ID that generated them. 
+        :type run_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5612,58 +5683,78 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._retrieve_file_serialize(
-            file_id=file_id,
+        _param = self._list_messages_serialize(
+            thread_id=thread_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
+            run_id=run_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "OpenAIFile",
+            '200': "ListMessagesResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def retrieve_file_with_http_info(
+    def list_messages_with_http_info(
         self,
-        file_id: Annotated[StrictStr, Field(description="The ID of the file to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) the messages belong to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
+        run_id: Annotated[Optional[StrictStr], Field(description="Filter messages by the run ID that generated them. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[OpenAIFile]:
-        """Returns information about a specific file.
+    ) -> ApiResponse[ListMessagesResponse]:
+        """Returns a list of messages for a given thread.
 
 
-        :param file_id: The ID of the file to use for this request (required)
-        :type file_id: str
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) the messages belong to. (required)
+        :type thread_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
+        :param run_id: Filter messages by the run ID that generated them. 
+        :type run_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5678,58 +5769,78 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._retrieve_file_serialize(
-            file_id=file_id,
+        _param = self._list_messages_serialize(
+            thread_id=thread_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
+            run_id=run_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "OpenAIFile",
+            '200': "ListMessagesResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def retrieve_file_without_preload_content(
+    def list_messages_without_preload_content(
         self,
-        file_id: Annotated[StrictStr, Field(description="The ID of the file to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) the messages belong to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
+        run_id: Annotated[Optional[StrictStr], Field(description="Filter messages by the run ID that generated them. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Returns information about a specific file.
+        """Returns a list of messages for a given thread.
 
 
-        :param file_id: The ID of the file to use for this request (required)
-        :type file_id: str
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) the messages belong to. (required)
+        :type thread_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
+        :param run_id: Filter messages by the run ID that generated them. 
+        :type run_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5744,35 +5855,45 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._retrieve_file_serialize(
-            file_id=file_id,
+        _param = self._list_messages_serialize(
+            thread_id=thread_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
+            run_id=run_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "OpenAIFile",
+            '200': "ListMessagesResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _retrieve_file_serialize(
+    def _list_messages_serialize(
         self,
-        file_id,
+        thread_id,
+        limit,
+        order,
+        after,
+        before,
+        run_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -5784,17 +5905,37 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if file_id is not None:
-            _path_params['file_id'] = file_id
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
         # process the query parameters
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
+        if order is not None:
+            
+            _query_params.append(('order', order))
+            
+        if after is not None:
+            
+            _query_params.append(('after', after))
+            
+        if before is not None:
+            
+            _query_params.append(('before', before))
+            
+        if run_id is not None:
+            
+            _query_params.append(('run_id', run_id))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -5802,19 +5943,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/files/{file_id}',
+            resource_path='/threads/{thread_id}/messages',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -5823,35 +5965,50 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def retrieve_fine_tune(
+    def list_run_steps(
         self,
-        fine_tune_id: Annotated[StrictStr, Field(description="The ID of the fine-tune job ")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread the run and run steps belong to.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run the run steps belong to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> FineTune:
-        """Gets info about the fine-tune job.  [Learn more about Fine-tuning](/docs/guides/fine-tuning) 
+    ) -> ListRunStepsResponse:
+        """Returns a list of run steps belonging to a run.
 
 
-        :param fine_tune_id: The ID of the fine-tune job  (required)
-        :type fine_tune_id: str
+        :param thread_id: The ID of the thread the run and run steps belong to. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run the run steps belong to. (required)
+        :type run_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5866,58 +6023,78 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._retrieve_fine_tune_serialize(
-            fine_tune_id=fine_tune_id,
+        _param = self._list_run_steps_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FineTune",
+            '200': "ListRunStepsResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def retrieve_fine_tune_with_http_info(
+    def list_run_steps_with_http_info(
         self,
-        fine_tune_id: Annotated[StrictStr, Field(description="The ID of the fine-tune job ")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread the run and run steps belong to.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run the run steps belong to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[FineTune]:
-        """Gets info about the fine-tune job.  [Learn more about Fine-tuning](/docs/guides/fine-tuning) 
+    ) -> ApiResponse[ListRunStepsResponse]:
+        """Returns a list of run steps belonging to a run.
 
 
-        :param fine_tune_id: The ID of the fine-tune job  (required)
-        :type fine_tune_id: str
+        :param thread_id: The ID of the thread the run and run steps belong to. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run the run steps belong to. (required)
+        :type run_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5932,58 +6109,78 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._retrieve_fine_tune_serialize(
-            fine_tune_id=fine_tune_id,
+        _param = self._list_run_steps_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FineTune",
+            '200': "ListRunStepsResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def retrieve_fine_tune_without_preload_content(
+    def list_run_steps_without_preload_content(
         self,
-        fine_tune_id: Annotated[StrictStr, Field(description="The ID of the fine-tune job ")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread the run and run steps belong to.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run the run steps belong to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Gets info about the fine-tune job.  [Learn more about Fine-tuning](/docs/guides/fine-tuning) 
+        """Returns a list of run steps belonging to a run.
 
 
-        :param fine_tune_id: The ID of the fine-tune job  (required)
-        :type fine_tune_id: str
+        :param thread_id: The ID of the thread the run and run steps belong to. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run the run steps belong to. (required)
+        :type run_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5998,35 +6195,45 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._retrieve_fine_tune_serialize(
-            fine_tune_id=fine_tune_id,
+        _param = self._list_run_steps_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FineTune",
+            '200': "ListRunStepsResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _retrieve_fine_tune_serialize(
+    def _list_run_steps_serialize(
         self,
-        fine_tune_id,
+        thread_id,
+        run_id,
+        limit,
+        order,
+        after,
+        before,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -6038,17 +6245,35 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if fine_tune_id is not None:
-            _path_params['fine_tune_id'] = fine_tune_id
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if run_id is not None:
+            _path_params['run_id'] = run_id
         # process the query parameters
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
+        if order is not None:
+            
+            _query_params.append(('order', order))
+            
+        if after is not None:
+            
+            _query_params.append(('after', after))
+            
+        if before is not None:
+            
+            _query_params.append(('before', before))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -6056,19 +6281,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/fine-tunes/{fine_tune_id}',
+            resource_path='/threads/{thread_id}/runs/{run_id}/steps',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -6077,35 +6303,47 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def retrieve_model(
+    def list_runs(
         self,
-        model: Annotated[StrictStr, Field(description="The ID of the model to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread the run belongs to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Model:
-        """Retrieves a model instance, providing basic information about the model such as the owner and permissioning.
+    ) -> ListRunsResponse:
+        """Returns a list of runs belonging to a thread.
 
 
-        :param model: The ID of the model to use for this request (required)
-        :type model: str
+        :param thread_id: The ID of the thread the run belongs to. (required)
+        :type thread_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -6120,58 +6358,74 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._retrieve_model_serialize(
-            model=model,
+        _param = self._list_runs_serialize(
+            thread_id=thread_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Model",
+            '200': "ListRunsResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def retrieve_model_with_http_info(
+    def list_runs_with_http_info(
         self,
-        model: Annotated[StrictStr, Field(description="The ID of the model to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread the run belongs to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Model]:
-        """Retrieves a model instance, providing basic information about the model such as the owner and permissioning.
+    ) -> ApiResponse[ListRunsResponse]:
+        """Returns a list of runs belonging to a thread.
 
 
-        :param model: The ID of the model to use for this request (required)
-        :type model: str
+        :param thread_id: The ID of the thread the run belongs to. (required)
+        :type thread_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -6186,58 +6440,74 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._retrieve_model_serialize(
-            model=model,
+        _param = self._list_runs_serialize(
+            thread_id=thread_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Model",
+            '200': "ListRunsResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def retrieve_model_without_preload_content(
+    def list_runs_without_preload_content(
         self,
-        model: Annotated[StrictStr, Field(description="The ID of the model to use for this request")],
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread the run belongs to.")],
+        limit: Annotated[Optional[StrictInt], Field(description="A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. ")] = None,
+        order: Annotated[Optional[StrictStr], Field(description="Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. ")] = None,
+        after: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. ")] = None,
+        before: Annotated[Optional[StrictStr], Field(description="A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. ")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Retrieves a model instance, providing basic information about the model such as the owner and permissioning.
+        """Returns a list of runs belonging to a thread.
 
 
-        :param model: The ID of the model to use for this request (required)
-        :type model: str
+        :param thread_id: The ID of the thread the run belongs to. (required)
+        :type thread_id: str
+        :param limit: A limit on the number of objects to be returned. Limit can range between 1 and 100, and the default is 20. 
+        :type limit: int
+        :param order: Sort order by the `created_at` timestamp of the objects. `asc` for ascending order and `desc` for descending order. 
+        :type order: str
+        :param after: A cursor for use in pagination. `after` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include after=obj_foo in order to fetch the next page of the list. 
+        :type after: str
+        :param before: A cursor for use in pagination. `before` is an object ID that defines your place in the list. For instance, if you make a list request and receive 100 objects, ending with obj_foo, your subsequent call can include before=obj_foo in order to fetch the previous page of the list. 
+        :type before: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -6252,35 +6522,43 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._retrieve_model_serialize(
-            model=model,
+        _param = self._list_runs_serialize(
+            thread_id=thread_id,
+            limit=limit,
+            order=order,
+            after=after,
+            before=before,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Model",
+            '200': "ListRunsResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _retrieve_model_serialize(
+    def _list_runs_serialize(
         self,
-        model,
+        thread_id,
+        limit,
+        order,
+        after,
+        before,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -6292,17 +6570,33 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if model is not None:
-            _path_params['model'] = model
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
         # process the query parameters
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
+        if order is not None:
+            
+            _query_params.append(('order', order))
+            
+        if after is not None:
+            
+            _query_params.append(('after', after))
+            
+        if before is not None:
+            
+            _query_params.append(('before', before))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -6310,19 +6604,1480 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/models/{model}',
+            resource_path='/threads/{thread_id}/runs',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def modify_assistant(
+        self,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant to modify.")],
+        modify_assistant_request: ModifyAssistantRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> AssistantObject:
+        """Modifies an assistant.
+
+
+        :param assistant_id: The ID of the assistant to modify. (required)
+        :type assistant_id: str
+        :param modify_assistant_request: (required)
+        :type modify_assistant_request: ModifyAssistantRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_assistant_serialize(
+            assistant_id=assistant_id,
+            modify_assistant_request=modify_assistant_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "AssistantObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def modify_assistant_with_http_info(
+        self,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant to modify.")],
+        modify_assistant_request: ModifyAssistantRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[AssistantObject]:
+        """Modifies an assistant.
+
+
+        :param assistant_id: The ID of the assistant to modify. (required)
+        :type assistant_id: str
+        :param modify_assistant_request: (required)
+        :type modify_assistant_request: ModifyAssistantRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_assistant_serialize(
+            assistant_id=assistant_id,
+            modify_assistant_request=modify_assistant_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "AssistantObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def modify_assistant_without_preload_content(
+        self,
+        assistant_id: Annotated[StrictStr, Field(description="The ID of the assistant to modify.")],
+        modify_assistant_request: ModifyAssistantRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Modifies an assistant.
+
+
+        :param assistant_id: The ID of the assistant to modify. (required)
+        :type assistant_id: str
+        :param modify_assistant_request: (required)
+        :type modify_assistant_request: ModifyAssistantRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_assistant_serialize(
+            assistant_id=assistant_id,
+            modify_assistant_request=modify_assistant_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "AssistantObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _modify_assistant_serialize(
+        self,
+        assistant_id,
+        modify_assistant_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if assistant_id is not None:
+            _path_params['assistant_id'] = assistant_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if modify_assistant_request is not None:
+            _body_params = modify_assistant_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/assistants/{assistant_id}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def modify_message(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which this message belongs.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message to modify.")],
+        modify_message_request: ModifyMessageRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> MessageObject:
+        """Modifies a message.
+
+
+        :param thread_id: The ID of the thread to which this message belongs. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message to modify. (required)
+        :type message_id: str
+        :param modify_message_request: (required)
+        :type modify_message_request: ModifyMessageRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_message_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
+            modify_message_request=modify_message_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "MessageObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def modify_message_with_http_info(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which this message belongs.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message to modify.")],
+        modify_message_request: ModifyMessageRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[MessageObject]:
+        """Modifies a message.
+
+
+        :param thread_id: The ID of the thread to which this message belongs. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message to modify. (required)
+        :type message_id: str
+        :param modify_message_request: (required)
+        :type modify_message_request: ModifyMessageRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_message_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
+            modify_message_request=modify_message_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "MessageObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def modify_message_without_preload_content(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to which this message belongs.")],
+        message_id: Annotated[StrictStr, Field(description="The ID of the message to modify.")],
+        modify_message_request: ModifyMessageRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Modifies a message.
+
+
+        :param thread_id: The ID of the thread to which this message belongs. (required)
+        :type thread_id: str
+        :param message_id: The ID of the message to modify. (required)
+        :type message_id: str
+        :param modify_message_request: (required)
+        :type modify_message_request: ModifyMessageRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_message_serialize(
+            thread_id=thread_id,
+            message_id=message_id,
+            modify_message_request=modify_message_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "MessageObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _modify_message_serialize(
+        self,
+        thread_id,
+        message_id,
+        modify_message_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if message_id is not None:
+            _path_params['message_id'] = message_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if modify_message_request is not None:
+            _body_params = modify_message_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/threads/{thread_id}/messages/{message_id}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def modify_run(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) that was run.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to modify.")],
+        modify_run_request: ModifyRunRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RunObject:
+        """Modifies a run.
+
+
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) that was run. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to modify. (required)
+        :type run_id: str
+        :param modify_run_request: (required)
+        :type modify_run_request: ModifyRunRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            modify_run_request=modify_run_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "RunObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def modify_run_with_http_info(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) that was run.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to modify.")],
+        modify_run_request: ModifyRunRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[RunObject]:
+        """Modifies a run.
+
+
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) that was run. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to modify. (required)
+        :type run_id: str
+        :param modify_run_request: (required)
+        :type modify_run_request: ModifyRunRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            modify_run_request=modify_run_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "RunObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def modify_run_without_preload_content(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) that was run.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run to modify.")],
+        modify_run_request: ModifyRunRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Modifies a run.
+
+
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) that was run. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run to modify. (required)
+        :type run_id: str
+        :param modify_run_request: (required)
+        :type modify_run_request: ModifyRunRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            modify_run_request=modify_run_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "RunObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _modify_run_serialize(
+        self,
+        thread_id,
+        run_id,
+        modify_run_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if run_id is not None:
+            _path_params['run_id'] = run_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if modify_run_request is not None:
+            _body_params = modify_run_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/threads/{thread_id}/runs/{run_id}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def modify_thread(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to modify. Only the `metadata` can be modified.")],
+        modify_thread_request: ModifyThreadRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ThreadObject:
+        """Modifies a thread.
+
+
+        :param thread_id: The ID of the thread to modify. Only the `metadata` can be modified. (required)
+        :type thread_id: str
+        :param modify_thread_request: (required)
+        :type modify_thread_request: ModifyThreadRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_thread_serialize(
+            thread_id=thread_id,
+            modify_thread_request=modify_thread_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ThreadObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def modify_thread_with_http_info(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to modify. Only the `metadata` can be modified.")],
+        modify_thread_request: ModifyThreadRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[ThreadObject]:
+        """Modifies a thread.
+
+
+        :param thread_id: The ID of the thread to modify. Only the `metadata` can be modified. (required)
+        :type thread_id: str
+        :param modify_thread_request: (required)
+        :type modify_thread_request: ModifyThreadRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_thread_serialize(
+            thread_id=thread_id,
+            modify_thread_request=modify_thread_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ThreadObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def modify_thread_without_preload_content(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the thread to modify. Only the `metadata` can be modified.")],
+        modify_thread_request: ModifyThreadRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Modifies a thread.
+
+
+        :param thread_id: The ID of the thread to modify. Only the `metadata` can be modified. (required)
+        :type thread_id: str
+        :param modify_thread_request: (required)
+        :type modify_thread_request: ModifyThreadRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_thread_serialize(
+            thread_id=thread_id,
+            modify_thread_request=modify_thread_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ThreadObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _modify_thread_serialize(
+        self,
+        thread_id,
+        modify_thread_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if modify_thread_request is not None:
+            _body_params = modify_thread_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/threads/{thread_id}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def submit_tool_ouputs_to_run(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) to which this run belongs.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run that requires the tool output submission.")],
+        submit_tool_outputs_run_request: SubmitToolOutputsRunRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RunObject:
+        """When a run has the `status: \"requires_action\"` and `required_action.type` is `submit_tool_outputs`, this endpoint can be used to submit the outputs from the tool calls once they're all completed. All outputs must be submitted in a single request. 
+
+
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) to which this run belongs. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run that requires the tool output submission. (required)
+        :type run_id: str
+        :param submit_tool_outputs_run_request: (required)
+        :type submit_tool_outputs_run_request: SubmitToolOutputsRunRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._submit_tool_ouputs_to_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            submit_tool_outputs_run_request=submit_tool_outputs_run_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "RunObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def submit_tool_ouputs_to_run_with_http_info(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) to which this run belongs.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run that requires the tool output submission.")],
+        submit_tool_outputs_run_request: SubmitToolOutputsRunRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[RunObject]:
+        """When a run has the `status: \"requires_action\"` and `required_action.type` is `submit_tool_outputs`, this endpoint can be used to submit the outputs from the tool calls once they're all completed. All outputs must be submitted in a single request. 
+
+
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) to which this run belongs. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run that requires the tool output submission. (required)
+        :type run_id: str
+        :param submit_tool_outputs_run_request: (required)
+        :type submit_tool_outputs_run_request: SubmitToolOutputsRunRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._submit_tool_ouputs_to_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            submit_tool_outputs_run_request=submit_tool_outputs_run_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "RunObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def submit_tool_ouputs_to_run_without_preload_content(
+        self,
+        thread_id: Annotated[StrictStr, Field(description="The ID of the [thread](/docs/api-reference/threads) to which this run belongs.")],
+        run_id: Annotated[StrictStr, Field(description="The ID of the run that requires the tool output submission.")],
+        submit_tool_outputs_run_request: SubmitToolOutputsRunRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """When a run has the `status: \"requires_action\"` and `required_action.type` is `submit_tool_outputs`, this endpoint can be used to submit the outputs from the tool calls once they're all completed. All outputs must be submitted in a single request. 
+
+
+        :param thread_id: The ID of the [thread](/docs/api-reference/threads) to which this run belongs. (required)
+        :type thread_id: str
+        :param run_id: The ID of the run that requires the tool output submission. (required)
+        :type run_id: str
+        :param submit_tool_outputs_run_request: (required)
+        :type submit_tool_outputs_run_request: SubmitToolOutputsRunRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._submit_tool_ouputs_to_run_serialize(
+            thread_id=thread_id,
+            run_id=run_id,
+            submit_tool_outputs_run_request=submit_tool_outputs_run_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "RunObject",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _submit_tool_ouputs_to_run_serialize(
+        self,
+        thread_id,
+        run_id,
+        submit_tool_outputs_run_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if thread_id is not None:
+            _path_params['thread_id'] = thread_id
+        if run_id is not None:
+            _path_params['run_id'] = run_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if submit_tool_outputs_run_request is not None:
+            _body_params = submit_tool_outputs_run_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/threads/{thread_id}/runs/{run_id}/submit_tool_outputs',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

## Comparing `openapiopenai/models/chat_completion_request_message_function_call.py` & `openapiopenai/models/chat_completion_function_call_option.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -15,25 +15,24 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ChatCompletionRequestMessageFunctionCall(BaseModel):
+class ChatCompletionFunctionCallOption(BaseModel):
     """
-    The name and arguments of a function that should be called, as generated by the model.
+    Specifying a particular function via `{\"name\": \"my_function\"}` forces the model to call that function. 
     """ # noqa: E501
-    name: Optional[StrictStr] = Field(default=None, description="The name of the function to call.")
-    arguments: Optional[StrictStr] = Field(default=None, description="The arguments to call the function with, as generated by the model in JSON format. Note that the model does not always generate valid JSON, and may hallucinate parameters not defined by your function schema. Validate the arguments in your code before calling your function.")
-    __properties: ClassVar[List[str]] = ["name", "arguments"]
+    name: StrictStr = Field(description="The name of the function to call.")
+    __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ChatCompletionRequestMessageFunctionCall from a JSON string"""
+        """Create an instance of ChatCompletionFunctionCallOption from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ChatCompletionRequestMessageFunctionCall from a dict"""
+        """Create an instance of ChatCompletionFunctionCallOption from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "arguments": obj.get("arguments")
+            "name": obj.get("name")
         })
         return _obj
```

## Comparing `openapiopenai/models/create_chat_completion_request_function_call_one_of.py` & `openapiopenai/models/chat_completion_named_tool_choice_function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -19,17 +19,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateChatCompletionRequestFunctionCallOneOf(BaseModel):
+class ChatCompletionNamedToolChoiceFunction(BaseModel):
     """
-    CreateChatCompletionRequestFunctionCallOneOf
+    ChatCompletionNamedToolChoiceFunction
     """ # noqa: E501
     name: StrictStr = Field(description="The name of the function to call.")
     __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateChatCompletionRequestFunctionCallOneOf from a JSON string"""
+        """Create an instance of ChatCompletionNamedToolChoiceFunction from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,15 +69,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateChatCompletionRequestFunctionCallOneOf from a dict"""
+        """Create an instance of ChatCompletionNamedToolChoiceFunction from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

## Comparing `openapiopenai/models/create_completion_response_usage.py` & `openapiopenai/models/run_step_completion_usage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateCompletionResponseUsage(BaseModel):
+class RunStepCompletionUsage(BaseModel):
     """
-    CreateCompletionResponseUsage
+    Usage statistics related to the run step. This value will be `null` while the run step's status is `in_progress`.
     """ # noqa: E501
-    prompt_tokens: StrictInt
-    completion_tokens: StrictInt
-    total_tokens: StrictInt
-    __properties: ClassVar[List[str]] = ["prompt_tokens", "completion_tokens", "total_tokens"]
+    completion_tokens: StrictInt = Field(description="Number of completion tokens used over the course of the run step.")
+    prompt_tokens: StrictInt = Field(description="Number of prompt tokens used over the course of the run step.")
+    total_tokens: StrictInt = Field(description="Total number of tokens used (prompt + completion).")
+    __properties: ClassVar[List[str]] = ["completion_tokens", "prompt_tokens", "total_tokens"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateCompletionResponseUsage from a JSON string"""
+        """Create an instance of RunStepCompletionUsage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,22 +71,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateCompletionResponseUsage from a dict"""
+        """Create an instance of RunStepCompletionUsage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "prompt_tokens": obj.get("prompt_tokens"),
             "completion_tokens": obj.get("completion_tokens"),
+            "prompt_tokens": obj.get("prompt_tokens"),
             "total_tokens": obj.get("total_tokens")
         })
         return _obj
```

## Comparing `openapiopenai/models/create_edit_request.py` & `openapiopenai/models/create_chat_completion_function_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from typing_extensions import Annotated
-from openapiopenai.models.create_edit_request_model import CreateEditRequestModel
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List, Optional
+from openapiopenai.models.completion_usage import CompletionUsage
+from openapiopenai.models.create_chat_completion_function_response_choices_inner import CreateChatCompletionFunctionResponseChoicesInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateEditRequest(BaseModel):
+class CreateChatCompletionFunctionResponse(BaseModel):
     """
-    CreateEditRequest
+    Represents a chat completion response returned by model, based on the provided input.
     """ # noqa: E501
-    model: CreateEditRequestModel
-    input: Optional[StrictStr] = Field(default='', description="The input text to use as a starting point for the edit.")
-    instruction: StrictStr = Field(description="The instruction that tells the model how to edit the prompt.")
-    n: Optional[Annotated[int, Field(le=20, strict=True, ge=1)]] = Field(default=1, description="How many edits to generate for the input and instruction.")
-    temperature: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=0)], Annotated[int, Field(le=2, strict=True, ge=0)]]] = Field(default=1, description="What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.  We generally recommend altering this or `top_p` but not both. ")
-    top_p: Optional[Union[Annotated[float, Field(le=1, strict=True, ge=0)], Annotated[int, Field(le=1, strict=True, ge=0)]]] = Field(default=1, description="An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens comprising the top 10% probability mass are considered.  We generally recommend altering this or `temperature` but not both. ")
-    __properties: ClassVar[List[str]] = ["model", "input", "instruction", "n", "temperature", "top_p"]
+    id: StrictStr = Field(description="A unique identifier for the chat completion.")
+    choices: List[CreateChatCompletionFunctionResponseChoicesInner] = Field(description="A list of chat completion choices. Can be more than one if `n` is greater than 1.")
+    created: StrictInt = Field(description="The Unix timestamp (in seconds) of when the chat completion was created.")
+    model: StrictStr = Field(description="The model used for the chat completion.")
+    system_fingerprint: Optional[StrictStr] = Field(default=None, description="This fingerprint represents the backend configuration that the model runs with.  Can be used in conjunction with the `seed` request parameter to understand when backend changes have been made that might impact determinism. ")
+    object: StrictStr = Field(description="The object type, which is always `chat.completion`.")
+    usage: Optional[CompletionUsage] = None
+    __properties: ClassVar[List[str]] = ["id", "choices", "created", "model", "system_fingerprint", "object", "usage"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['chat.completion']):
+            raise ValueError("must be one of enum values ('chat.completion')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -51,15 +59,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateEditRequest from a JSON string"""
+        """Create an instance of CreateChatCompletionFunctionResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,52 +80,40 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of model
-        if self.model:
-            _dict['model'] = self.model.to_dict()
-        # set to None if input (nullable) is None
-        # and model_fields_set contains the field
-        if self.input is None and "input" in self.model_fields_set:
-            _dict['input'] = None
-
-        # set to None if n (nullable) is None
-        # and model_fields_set contains the field
-        if self.n is None and "n" in self.model_fields_set:
-            _dict['n'] = None
-
-        # set to None if temperature (nullable) is None
-        # and model_fields_set contains the field
-        if self.temperature is None and "temperature" in self.model_fields_set:
-            _dict['temperature'] = None
-
-        # set to None if top_p (nullable) is None
-        # and model_fields_set contains the field
-        if self.top_p is None and "top_p" in self.model_fields_set:
-            _dict['top_p'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of each item in choices (list)
+        _items = []
+        if self.choices:
+            for _item in self.choices:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['choices'] = _items
+        # override the default output from pydantic by calling `to_dict()` of usage
+        if self.usage:
+            _dict['usage'] = self.usage.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateEditRequest from a dict"""
+        """Create an instance of CreateChatCompletionFunctionResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "model": CreateEditRequestModel.from_dict(obj["model"]) if obj.get("model") is not None else None,
-            "input": obj.get("input") if obj.get("input") is not None else '',
-            "instruction": obj.get("instruction"),
-            "n": obj.get("n") if obj.get("n") is not None else 1,
-            "temperature": obj.get("temperature") if obj.get("temperature") is not None else 1,
-            "top_p": obj.get("top_p") if obj.get("top_p") is not None else 1
+            "id": obj.get("id"),
+            "choices": [CreateChatCompletionFunctionResponseChoicesInner.from_dict(_item) for _item in obj["choices"]] if obj.get("choices") is not None else None,
+            "created": obj.get("created"),
+            "model": obj.get("model"),
+            "system_fingerprint": obj.get("system_fingerprint"),
+            "object": obj.get("object"),
+            "usage": CompletionUsage.from_dict(obj["usage"]) if obj.get("usage") is not None else None
         })
         return _obj
```

## Comparing `openapiopenai/models/create_edit_request_model.py` & `openapiopenai/models/fine_tuning_job_hyperparameters_n_epochs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 import pprint
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
 from typing import Any, List, Optional
+from typing_extensions import Annotated
 from pydantic import StrictStr, Field
 from typing import Union, List, Optional, Dict
 from typing_extensions import Literal, Self
 
-CREATEEDITREQUESTMODEL_ONE_OF_SCHEMAS = ["str"]
+FINETUNINGJOBHYPERPARAMETERSNEPOCHS_ONE_OF_SCHEMAS = ["int", "str"]
 
-class CreateEditRequestModel(BaseModel):
+class FineTuningJobHyperparametersNEpochs(BaseModel):
     """
-    ID of the model to use. You can use the `text-davinci-edit-001` or `code-davinci-edit-001` model with this endpoint.
+    The number of epochs to train the model for. An epoch refers to one full cycle through the training dataset. \"auto\" decides the optimal number of epochs based on the size of the dataset. If setting the number manually, we support any number between 1 and 50 epochs.
     """
     # data type: str
     oneof_schema_1_validator: Optional[StrictStr] = None
-    # data type: str
-    oneof_schema_2_validator: Optional[StrictStr] = None
-    actual_instance: Optional[Union[str]] = None
-    one_of_schemas: List[str] = Field(default=Literal["str"])
+    # data type: int
+    oneof_schema_2_validator: Optional[Annotated[int, Field(le=50, strict=True, ge=1)]] = None
+    actual_instance: Optional[Union[int, str]] = None
+    one_of_schemas: List[str] = Field(default=Literal["int", "str"])
 
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
     )
 
 
@@ -49,35 +50,35 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_oneof(cls, v):
-        instance = CreateEditRequestModel.model_construct()
+        instance = FineTuningJobHyperparametersNEpochs.model_construct()
         error_messages = []
         match = 0
         # validate data type: str
         try:
             instance.oneof_schema_1_validator = v
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        # validate data type: str
+        # validate data type: int
         try:
             instance.oneof_schema_2_validator = v
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in CreateEditRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when setting `actual_instance` in FineTuningJobHyperparametersNEpochs with oneOf schemas: int, str. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in CreateEditRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting `actual_instance` in FineTuningJobHyperparametersNEpochs with oneOf schemas: int, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
         return cls.from_json(json.dumps(obj))
 
@@ -93,44 +94,44 @@
             # validation
             instance.oneof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.oneof_schema_1_validator
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        # deserialize data into str
+        # deserialize data into int
         try:
             # validation
             instance.oneof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.oneof_schema_2_validator
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into CreateEditRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when deserializing the JSON string into FineTuningJobHyperparametersNEpochs with oneOf schemas: int, str. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into CreateEditRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into FineTuningJobHyperparametersNEpochs with oneOf schemas: int, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], str]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], int, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

## Comparing `openapiopenai/models/create_edit_response.py` & `openapiopenai/models/create_chat_completion_function_response_choices_inner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
-from openapiopenai.models.create_completion_response_usage import CreateCompletionResponseUsage
-from openapiopenai.models.create_edit_response_choices_inner import CreateEditResponseChoicesInner
+from openapiopenai.models.chat_completion_response_message import ChatCompletionResponseMessage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateEditResponse(BaseModel):
+class CreateChatCompletionFunctionResponseChoicesInner(BaseModel):
     """
-    CreateEditResponse
+    CreateChatCompletionFunctionResponseChoicesInner
     """ # noqa: E501
-    object: StrictStr
-    created: StrictInt
-    choices: List[CreateEditResponseChoicesInner]
-    usage: CreateCompletionResponseUsage
-    __properties: ClassVar[List[str]] = ["object", "created", "choices", "usage"]
+    finish_reason: StrictStr = Field(description="The reason the model stopped generating tokens. This will be `stop` if the model hit a natural stop point or a provided stop sequence, `length` if the maximum number of tokens specified in the request was reached, `content_filter` if content was omitted due to a flag from our content filters, or `function_call` if the model called a function. ")
+    index: StrictInt = Field(description="The index of the choice in the list of choices.")
+    message: ChatCompletionResponseMessage
+    __properties: ClassVar[List[str]] = ["finish_reason", "index", "message"]
+
+    @field_validator('finish_reason')
+    def finish_reason_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['stop', 'length', 'function_call', 'content_filter']):
+            raise ValueError("must be one of enum values ('stop', 'length', 'function_call', 'content_filter')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateEditResponse from a JSON string"""
+        """Create an instance of CreateChatCompletionFunctionResponseChoicesInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,37 +75,29 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in choices (list)
-        _items = []
-        if self.choices:
-            for _item in self.choices:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['choices'] = _items
-        # override the default output from pydantic by calling `to_dict()` of usage
-        if self.usage:
-            _dict['usage'] = self.usage.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of message
+        if self.message:
+            _dict['message'] = self.message.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateEditResponse from a dict"""
+        """Create an instance of CreateChatCompletionFunctionResponseChoicesInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "object": obj.get("object"),
-            "created": obj.get("created"),
-            "choices": [CreateEditResponseChoicesInner.from_dict(_item) for _item in obj["choices"]] if obj.get("choices") is not None else None,
-            "usage": CreateCompletionResponseUsage.from_dict(obj["usage"]) if obj.get("usage") is not None else None
+            "finish_reason": obj.get("finish_reason"),
+            "index": obj.get("index"),
+            "message": ChatCompletionResponseMessage.from_dict(obj["message"]) if obj.get("message") is not None else None
         })
         return _obj
```

## Comparing `openapiopenai/models/create_edit_response_choices_inner.py` & `openapiopenai/models/create_chat_completion_request_response_format.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from openapiopenai.models.create_completion_response_choices_inner_logprobs import CreateCompletionResponseChoicesInnerLogprobs
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateEditResponseChoicesInner(BaseModel):
+class CreateChatCompletionRequestResponseFormat(BaseModel):
     """
-    CreateEditResponseChoicesInner
+    An object specifying the format that the model must output. Compatible with [GPT-4 Turbo](/docs/models/gpt-4-and-gpt-4-turbo) and all GPT-3.5 Turbo models newer than `gpt-3.5-turbo-1106`.  Setting to `{ \"type\": \"json_object\" }` enables JSON mode, which guarantees the message the model generates is valid JSON.  **Important:** when using JSON mode, you **must** also instruct the model to produce JSON yourself via a system or user message. Without this, the model may generate an unending stream of whitespace until the generation reaches the token limit, resulting in a long-running and seemingly \"stuck\" request. Also note that the message content may be partially cut off if `finish_reason=\"length\"`, which indicates the generation exceeded `max_tokens` or the conversation exceeded the max context length. 
     """ # noqa: E501
-    text: Optional[StrictStr] = None
-    index: Optional[StrictInt] = None
-    logprobs: Optional[CreateCompletionResponseChoicesInnerLogprobs] = None
-    finish_reason: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["text", "index", "logprobs", "finish_reason"]
+    type: Optional[StrictStr] = Field(default='text', description="Must be one of `text` or `json_object`.")
+    __properties: ClassVar[List[str]] = ["type"]
 
-    @field_validator('finish_reason')
-    def finish_reason_validate_enum(cls, value):
+    @field_validator('type')
+    def type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['stop', 'length']):
-            raise ValueError("must be one of enum values ('stop', 'length')")
+        if value not in set(['text', 'json_object']):
+            raise ValueError("must be one of enum values ('text', 'json_object')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -58,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateEditResponseChoicesInner from a JSON string"""
+        """Create an instance of CreateChatCompletionRequestResponseFormat from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,35 +75,24 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of logprobs
-        if self.logprobs:
-            _dict['logprobs'] = self.logprobs.to_dict()
-        # set to None if logprobs (nullable) is None
-        # and model_fields_set contains the field
-        if self.logprobs is None and "logprobs" in self.model_fields_set:
-            _dict['logprobs'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateEditResponseChoicesInner from a dict"""
+        """Create an instance of CreateChatCompletionRequestResponseFormat from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "text": obj.get("text"),
-            "index": obj.get("index"),
-            "logprobs": CreateCompletionResponseChoicesInnerLogprobs.from_dict(obj["logprobs"]) if obj.get("logprobs") is not None else None,
-            "finish_reason": obj.get("finish_reason")
+            "type": obj.get("type") if obj.get("type") is not None else 'text'
         })
         return _obj
```

## Comparing `openapiopenai/models/create_embedding_response_data_inner.py` & `openapiopenai/models/assistant_tools_code.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Union
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateEmbeddingResponseDataInner(BaseModel):
+class AssistantToolsCode(BaseModel):
     """
-    CreateEmbeddingResponseDataInner
+    AssistantToolsCode
     """ # noqa: E501
-    index: StrictInt
-    object: StrictStr
-    embedding: List[Union[StrictFloat, StrictInt]]
-    __properties: ClassVar[List[str]] = ["index", "object", "embedding"]
+    type: StrictStr = Field(description="The type of tool being defined: `code_interpreter`")
+    __properties: ClassVar[List[str]] = ["type"]
+
+    @field_validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['code_interpreter']):
+            raise ValueError("must be one of enum values ('code_interpreter')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +51,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateEmbeddingResponseDataInner from a JSON string"""
+        """Create an instance of AssistantToolsCode from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,22 +76,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateEmbeddingResponseDataInner from a dict"""
+        """Create an instance of AssistantToolsCode from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "index": obj.get("index"),
-            "object": obj.get("object"),
-            "embedding": obj.get("embedding")
+            "type": obj.get("type")
         })
         return _obj
```

## Comparing `openapiopenai/models/create_fine_tune_request.py` & `openapiopenai/models/create_run_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing_extensions import Annotated
-from openapiopenai.models.create_fine_tune_request_model import CreateFineTuneRequestModel
+from openapiopenai.models.assistant_object_tools_inner import AssistantObjectToolsInner
+from openapiopenai.models.assistants_api_response_format_option import AssistantsApiResponseFormatOption
+from openapiopenai.models.assistants_api_tool_choice_option import AssistantsApiToolChoiceOption
+from openapiopenai.models.create_message_request import CreateMessageRequest
+from openapiopenai.models.create_run_request_model import CreateRunRequestModel
+from openapiopenai.models.truncation_object import TruncationObject
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateFineTuneRequest(BaseModel):
+class CreateRunRequest(BaseModel):
     """
-    CreateFineTuneRequest
+    CreateRunRequest
     """ # noqa: E501
-    training_file: StrictStr = Field(description="The ID of an uploaded file that contains training data.  See [upload file](/docs/api-reference/files/upload) for how to upload a file.  Your dataset must be formatted as a JSONL file, where each training example is a JSON object with the keys \"prompt\" and \"completion\". Additionally, you must upload your file with the purpose `fine-tune`.  See the [fine-tuning guide](/docs/guides/fine-tuning/creating-training-data) for more details. ")
-    validation_file: Optional[StrictStr] = Field(default=None, description="The ID of an uploaded file that contains validation data.  If you provide this file, the data is used to generate validation metrics periodically during fine-tuning. These metrics can be viewed in the [fine-tuning results file](/docs/guides/fine-tuning/analyzing-your-fine-tuned-model). Your train and validation data should be mutually exclusive.  Your dataset must be formatted as a JSONL file, where each validation example is a JSON object with the keys \"prompt\" and \"completion\". Additionally, you must upload your file with the purpose `fine-tune`.  See the [fine-tuning guide](/docs/guides/fine-tuning/creating-training-data) for more details. ")
-    model: Optional[CreateFineTuneRequestModel] = None
-    n_epochs: Optional[StrictInt] = Field(default=4, description="The number of epochs to train the model for. An epoch refers to one full cycle through the training dataset. ")
-    batch_size: Optional[StrictInt] = Field(default=None, description="The batch size to use for training. The batch size is the number of training examples used to train a single forward and backward pass.  By default, the batch size will be dynamically configured to be ~0.2% of the number of examples in the training set, capped at 256 - in general, we've found that larger batch sizes tend to work better for larger datasets. ")
-    learning_rate_multiplier: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="The learning rate multiplier to use for training. The fine-tuning learning rate is the original learning rate used for pretraining multiplied by this value.  By default, the learning rate multiplier is the 0.05, 0.1, or 0.2 depending on final `batch_size` (larger learning rates tend to perform better with larger batch sizes). We recommend experimenting with values in the range 0.02 to 0.2 to see what produces the best results. ")
-    prompt_loss_weight: Optional[Union[StrictFloat, StrictInt]] = Field(default=0.01, description="The weight to use for loss on the prompt tokens. This controls how much the model tries to learn to generate the prompt (as compared to the completion which always has a weight of 1.0), and can add a stabilizing effect to training when completions are short.  If prompts are extremely long (relative to completions), it may make sense to reduce this weight so as to avoid over-prioritizing learning the prompt. ")
-    compute_classification_metrics: Optional[StrictBool] = Field(default=False, description="If set, we calculate classification-specific metrics such as accuracy and F-1 score using the validation set at the end of every epoch. These metrics can be viewed in the [results file](/docs/guides/fine-tuning/analyzing-your-fine-tuned-model).  In order to compute classification metrics, you must provide a `validation_file`. Additionally, you must specify `classification_n_classes` for multiclass classification or `classification_positive_class` for binary classification. ")
-    classification_n_classes: Optional[StrictInt] = Field(default=None, description="The number of classes in a classification task.  This parameter is required for multiclass classification. ")
-    classification_positive_class: Optional[StrictStr] = Field(default=None, description="The positive class in binary classification.  This parameter is needed to generate precision, recall, and F1 metrics when doing binary classification. ")
-    classification_betas: Optional[List[Union[StrictFloat, StrictInt]]] = Field(default=None, description="If this is provided, we calculate F-beta scores at the specified beta values. The F-beta score is a generalization of F-1 score. This is only used for binary classification.  With a beta of 1 (i.e. the F-1 score), precision and recall are given the same weight. A larger beta score puts more weight on recall and less on precision. A smaller beta score puts more weight on precision and less on recall. ")
-    suffix: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=40)]] = Field(default=None, description="A string of up to 40 characters that will be added to your fine-tuned model name.  For example, a `suffix` of \"custom-model-name\" would produce a model name like `ada:ft-your-org:custom-model-name-2022-02-15-04-21-04`. ")
-    __properties: ClassVar[List[str]] = ["training_file", "validation_file", "model", "n_epochs", "batch_size", "learning_rate_multiplier", "prompt_loss_weight", "compute_classification_metrics", "classification_n_classes", "classification_positive_class", "classification_betas", "suffix"]
+    assistant_id: StrictStr = Field(description="The ID of the [assistant](/docs/api-reference/assistants) to use to execute this run.")
+    model: Optional[CreateRunRequestModel] = None
+    instructions: Optional[StrictStr] = Field(default=None, description="Overrides the [instructions](/docs/api-reference/assistants/createAssistant) of the assistant. This is useful for modifying the behavior on a per-run basis.")
+    additional_instructions: Optional[StrictStr] = Field(default=None, description="Appends additional instructions at the end of the instructions for the run. This is useful for modifying the behavior on a per-run basis without overriding other instructions.")
+    additional_messages: Optional[List[CreateMessageRequest]] = Field(default=None, description="Adds additional messages to the thread before creating the run.")
+    tools: Optional[Annotated[List[AssistantObjectToolsInner], Field(max_length=20)]] = Field(default=None, description="Override the tools the assistant can use for this run. This is useful for modifying the behavior on a per-run basis.")
+    metadata: Optional[Dict[str, Any]] = Field(default=None, description="Set of 16 key-value pairs that can be attached to an object. This can be useful for storing additional information about the object in a structured format. Keys can be a maximum of 64 characters long and values can be a maxium of 512 characters long. ")
+    temperature: Optional[Union[Annotated[float, Field(le=2, strict=True, ge=0)], Annotated[int, Field(le=2, strict=True, ge=0)]]] = Field(default=1, description="What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. ")
+    stream: Optional[StrictBool] = Field(default=None, description="If `true`, returns a stream of events that happen during the Run as server-sent events, terminating when the Run enters a terminal state with a `data: [DONE]` message. ")
+    max_prompt_tokens: Optional[Annotated[int, Field(strict=True, ge=256)]] = Field(default=None, description="The maximum number of prompt tokens that may be used over the course of the run. The run will make a best effort to use only the number of prompt tokens specified, across multiple turns of the run. If the run exceeds the number of prompt tokens specified, the run will end with status `complete`. See `incomplete_details` for more info. ")
+    max_completion_tokens: Optional[Annotated[int, Field(strict=True, ge=256)]] = Field(default=None, description="The maximum number of completion tokens that may be used over the course of the run. The run will make a best effort to use only the number of completion tokens specified, across multiple turns of the run. If the run exceeds the number of completion tokens specified, the run will end with status `complete`. See `incomplete_details` for more info. ")
+    truncation_strategy: Optional[TruncationObject] = None
+    tool_choice: Optional[AssistantsApiToolChoiceOption] = None
+    response_format: Optional[AssistantsApiResponseFormatOption] = None
+    __properties: ClassVar[List[str]] = ["assistant_id", "model", "instructions", "additional_instructions", "additional_messages", "tools", "metadata", "temperature", "stream", "max_prompt_tokens", "max_completion_tokens", "truncation_strategy", "tool_choice", "response_format"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -57,15 +64,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateFineTuneRequest from a JSON string"""
+        """Create an instance of CreateRunRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -81,90 +88,110 @@
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of model
         if self.model:
             _dict['model'] = self.model.to_dict()
-        # set to None if validation_file (nullable) is None
-        # and model_fields_set contains the field
-        if self.validation_file is None and "validation_file" in self.model_fields_set:
-            _dict['validation_file'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of each item in additional_messages (list)
+        _items = []
+        if self.additional_messages:
+            for _item in self.additional_messages:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['additional_messages'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in tools (list)
+        _items = []
+        if self.tools:
+            for _item in self.tools:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tools'] = _items
+        # override the default output from pydantic by calling `to_dict()` of truncation_strategy
+        if self.truncation_strategy:
+            _dict['truncation_strategy'] = self.truncation_strategy.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of tool_choice
+        if self.tool_choice:
+            _dict['tool_choice'] = self.tool_choice.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of response_format
+        if self.response_format:
+            _dict['response_format'] = self.response_format.to_dict()
         # set to None if model (nullable) is None
         # and model_fields_set contains the field
         if self.model is None and "model" in self.model_fields_set:
             _dict['model'] = None
 
-        # set to None if n_epochs (nullable) is None
+        # set to None if instructions (nullable) is None
         # and model_fields_set contains the field
-        if self.n_epochs is None and "n_epochs" in self.model_fields_set:
-            _dict['n_epochs'] = None
+        if self.instructions is None and "instructions" in self.model_fields_set:
+            _dict['instructions'] = None
 
-        # set to None if batch_size (nullable) is None
+        # set to None if additional_instructions (nullable) is None
         # and model_fields_set contains the field
-        if self.batch_size is None and "batch_size" in self.model_fields_set:
-            _dict['batch_size'] = None
+        if self.additional_instructions is None and "additional_instructions" in self.model_fields_set:
+            _dict['additional_instructions'] = None
 
-        # set to None if learning_rate_multiplier (nullable) is None
+        # set to None if additional_messages (nullable) is None
         # and model_fields_set contains the field
-        if self.learning_rate_multiplier is None and "learning_rate_multiplier" in self.model_fields_set:
-            _dict['learning_rate_multiplier'] = None
+        if self.additional_messages is None and "additional_messages" in self.model_fields_set:
+            _dict['additional_messages'] = None
 
-        # set to None if prompt_loss_weight (nullable) is None
+        # set to None if tools (nullable) is None
         # and model_fields_set contains the field
-        if self.prompt_loss_weight is None and "prompt_loss_weight" in self.model_fields_set:
-            _dict['prompt_loss_weight'] = None
+        if self.tools is None and "tools" in self.model_fields_set:
+            _dict['tools'] = None
 
-        # set to None if compute_classification_metrics (nullable) is None
+        # set to None if metadata (nullable) is None
         # and model_fields_set contains the field
-        if self.compute_classification_metrics is None and "compute_classification_metrics" in self.model_fields_set:
-            _dict['compute_classification_metrics'] = None
+        if self.metadata is None and "metadata" in self.model_fields_set:
+            _dict['metadata'] = None
 
-        # set to None if classification_n_classes (nullable) is None
+        # set to None if temperature (nullable) is None
         # and model_fields_set contains the field
-        if self.classification_n_classes is None and "classification_n_classes" in self.model_fields_set:
-            _dict['classification_n_classes'] = None
+        if self.temperature is None and "temperature" in self.model_fields_set:
+            _dict['temperature'] = None
 
-        # set to None if classification_positive_class (nullable) is None
+        # set to None if stream (nullable) is None
         # and model_fields_set contains the field
-        if self.classification_positive_class is None and "classification_positive_class" in self.model_fields_set:
-            _dict['classification_positive_class'] = None
+        if self.stream is None and "stream" in self.model_fields_set:
+            _dict['stream'] = None
 
-        # set to None if classification_betas (nullable) is None
+        # set to None if max_prompt_tokens (nullable) is None
         # and model_fields_set contains the field
-        if self.classification_betas is None and "classification_betas" in self.model_fields_set:
-            _dict['classification_betas'] = None
+        if self.max_prompt_tokens is None and "max_prompt_tokens" in self.model_fields_set:
+            _dict['max_prompt_tokens'] = None
 
-        # set to None if suffix (nullable) is None
+        # set to None if max_completion_tokens (nullable) is None
         # and model_fields_set contains the field
-        if self.suffix is None and "suffix" in self.model_fields_set:
-            _dict['suffix'] = None
+        if self.max_completion_tokens is None and "max_completion_tokens" in self.model_fields_set:
+            _dict['max_completion_tokens'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateFineTuneRequest from a dict"""
+        """Create an instance of CreateRunRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "training_file": obj.get("training_file"),
-            "validation_file": obj.get("validation_file"),
-            "model": CreateFineTuneRequestModel.from_dict(obj["model"]) if obj.get("model") is not None else None,
-            "n_epochs": obj.get("n_epochs") if obj.get("n_epochs") is not None else 4,
-            "batch_size": obj.get("batch_size"),
-            "learning_rate_multiplier": obj.get("learning_rate_multiplier"),
-            "prompt_loss_weight": obj.get("prompt_loss_weight") if obj.get("prompt_loss_weight") is not None else 0.01,
-            "compute_classification_metrics": obj.get("compute_classification_metrics") if obj.get("compute_classification_metrics") is not None else False,
-            "classification_n_classes": obj.get("classification_n_classes"),
-            "classification_positive_class": obj.get("classification_positive_class"),
-            "classification_betas": obj.get("classification_betas"),
-            "suffix": obj.get("suffix")
+            "assistant_id": obj.get("assistant_id"),
+            "model": CreateRunRequestModel.from_dict(obj["model"]) if obj.get("model") is not None else None,
+            "instructions": obj.get("instructions"),
+            "additional_instructions": obj.get("additional_instructions"),
+            "additional_messages": [CreateMessageRequest.from_dict(_item) for _item in obj["additional_messages"]] if obj.get("additional_messages") is not None else None,
+            "tools": [AssistantObjectToolsInner.from_dict(_item) for _item in obj["tools"]] if obj.get("tools") is not None else None,
+            "metadata": obj.get("metadata"),
+            "temperature": obj.get("temperature") if obj.get("temperature") is not None else 1,
+            "stream": obj.get("stream"),
+            "max_prompt_tokens": obj.get("max_prompt_tokens"),
+            "max_completion_tokens": obj.get("max_completion_tokens"),
+            "truncation_strategy": TruncationObject.from_dict(obj["truncation_strategy"]) if obj.get("truncation_strategy") is not None else None,
+            "tool_choice": AssistantsApiToolChoiceOption.from_dict(obj["tool_choice"]) if obj.get("tool_choice") is not None else None,
+            "response_format": AssistantsApiResponseFormatOption.from_dict(obj["response_format"]) if obj.get("response_format") is not None else None
         })
         return _obj
```

## Comparing `openapiopenai/models/create_fine_tune_request_model.py` & `openapiopenai/models/assistants_api_tool_choice_option.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 import pprint
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
 from typing import Any, List, Optional
+from openapiopenai.models.assistants_api_named_tool_choice import AssistantsApiNamedToolChoice
 from pydantic import StrictStr, Field
 from typing import Union, List, Optional, Dict
 from typing_extensions import Literal, Self
 
-CREATEFINETUNEREQUESTMODEL_ONE_OF_SCHEMAS = ["str"]
+ASSISTANTSAPITOOLCHOICEOPTION_ONE_OF_SCHEMAS = ["AssistantsApiNamedToolChoice", "str"]
 
-class CreateFineTuneRequestModel(BaseModel):
+class AssistantsApiToolChoiceOption(BaseModel):
     """
-    The name of the base model to fine-tune. You can select one of \"ada\", \"babbage\", \"curie\", \"davinci\", or a fine-tuned model created after 2022-04-21. To learn more about these models, see the [Models](https://platform.openai.com/docs/models) documentation. 
+    Controls which (if any) tool is called by the model. `none` means the model will not call any tools and instead generates a message. `auto` is the default value and means the model can pick between generating a message or calling a tool. Specifying a particular tool like `{\"type\": \"TOOL_TYPE\"}` or `{\"type\": \"function\", \"function\": {\"name\": \"my_function\"}}` forces the model to call that tool. 
     """
     # data type: str
-    oneof_schema_1_validator: Optional[StrictStr] = None
-    # data type: str
-    oneof_schema_2_validator: Optional[StrictStr] = None
-    actual_instance: Optional[Union[str]] = None
-    one_of_schemas: List[str] = Field(default=Literal["str"])
+    oneof_schema_1_validator: Optional[StrictStr] = Field(default=None, description="`none` means the model will not call a function and instead generates a message. `auto` means the model can pick between generating a message or calling a function. ")
+    # data type: AssistantsApiNamedToolChoice
+    oneof_schema_2_validator: Optional[AssistantsApiNamedToolChoice] = None
+    actual_instance: Optional[Union[AssistantsApiNamedToolChoice, str]] = None
+    one_of_schemas: List[str] = Field(default=Literal["AssistantsApiNamedToolChoice", "str"])
 
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
     )
 
 
@@ -49,94 +50,84 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_oneof(cls, v):
-        if v is None:
-            return v
-
-        instance = CreateFineTuneRequestModel.model_construct()
+        instance = AssistantsApiToolChoiceOption.model_construct()
         error_messages = []
         match = 0
         # validate data type: str
         try:
             instance.oneof_schema_1_validator = v
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        # validate data type: str
-        try:
-            instance.oneof_schema_2_validator = v
+        # validate data type: AssistantsApiNamedToolChoice
+        if not isinstance(v, AssistantsApiNamedToolChoice):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `AssistantsApiNamedToolChoice`")
+        else:
             match += 1
-        except (ValidationError, ValueError) as e:
-            error_messages.append(str(e))
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when setting `actual_instance` in CreateFineTuneRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when setting `actual_instance` in AssistantsApiToolChoiceOption with oneOf schemas: AssistantsApiNamedToolChoice, str. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when setting `actual_instance` in CreateFineTuneRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting `actual_instance` in AssistantsApiToolChoiceOption with oneOf schemas: AssistantsApiNamedToolChoice, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Union[str, Dict[str, Any]]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: Optional[str]) -> Self:
+    def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
-        if json_str is None:
-            return instance
-
         error_messages = []
         match = 0
 
         # deserialize data into str
         try:
             # validation
             instance.oneof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.oneof_schema_1_validator
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        # deserialize data into str
+        # deserialize data into AssistantsApiNamedToolChoice
         try:
-            # validation
-            instance.oneof_schema_2_validator = json.loads(json_str)
-            # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_2_validator
+            instance.actual_instance = AssistantsApiNamedToolChoice.from_json(json_str)
             match += 1
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if match > 1:
             # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into CreateFineTuneRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("Multiple matches found when deserializing the JSON string into AssistantsApiToolChoiceOption with oneOf schemas: AssistantsApiNamedToolChoice, str. Details: " + ", ".join(error_messages))
         elif match == 0:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into CreateFineTuneRequestModel with oneOf schemas: str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into AssistantsApiToolChoiceOption with oneOf schemas: AssistantsApiNamedToolChoice, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], str]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], AssistantsApiNamedToolChoice, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

## Comparing `openapiopenai/models/create_transcription_response.py` & `openapiopenai/models/run_step_object_last_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateTranscriptionResponse(BaseModel):
+class RunStepObjectLastError(BaseModel):
     """
-    CreateTranscriptionResponse
+    The last error associated with this run step. Will be `null` if there are no errors.
     """ # noqa: E501
-    text: StrictStr
-    __properties: ClassVar[List[str]] = ["text"]
+    code: StrictStr = Field(description="One of `server_error` or `rate_limit_exceeded`.")
+    message: StrictStr = Field(description="A human-readable description of the error.")
+    __properties: ClassVar[List[str]] = ["code", "message"]
+
+    @field_validator('code')
+    def code_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['server_error', 'rate_limit_exceeded']):
+            raise ValueError("must be one of enum values ('server_error', 'rate_limit_exceeded')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +52,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateTranscriptionResponse from a JSON string"""
+        """Create an instance of RunStepObjectLastError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +77,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateTranscriptionResponse from a dict"""
+        """Create an instance of RunStepObjectLastError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "text": obj.get("text")
+            "code": obj.get("code"),
+            "message": obj.get("message")
         })
         return _obj
```

## Comparing `openapiopenai/models/create_translation_response.py` & `openapiopenai/models/create_translation_response_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
@@ -19,17 +19,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateTranslationResponse(BaseModel):
+class CreateTranslationResponseJson(BaseModel):
     """
-    CreateTranslationResponse
+    CreateTranslationResponseJson
     """ # noqa: E501
     text: StrictStr
     __properties: ClassVar[List[str]] = ["text"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateTranslationResponse from a JSON string"""
+        """Create an instance of CreateTranslationResponseJson from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,15 +69,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateTranslationResponse from a dict"""
+        """Create an instance of CreateTranslationResponseJson from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

## Comparing `openapiopenai/models/fine_tune.py` & `openapiopenai/models/assistant_object.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from openapiopenai.models.fine_tune_event import FineTuneEvent
-from openapiopenai.models.open_ai_file import OpenAIFile
+from typing_extensions import Annotated
+from openapiopenai.models.assistant_object_tools_inner import AssistantObjectToolsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FineTune(BaseModel):
+class AssistantObject(BaseModel):
     """
-    FineTune
+    Represents an `assistant` that can call the model and use tools.
     """ # noqa: E501
-    id: StrictStr
-    object: StrictStr
-    created_at: StrictInt
-    updated_at: StrictInt
-    model: StrictStr
-    fine_tuned_model: Optional[StrictStr]
-    organization_id: StrictStr
-    status: StrictStr
-    hyperparams: Dict[str, Any]
-    training_files: List[OpenAIFile]
-    validation_files: List[OpenAIFile]
-    result_files: List[OpenAIFile]
-    events: Optional[List[FineTuneEvent]] = None
-    __properties: ClassVar[List[str]] = ["id", "object", "created_at", "updated_at", "model", "fine_tuned_model", "organization_id", "status", "hyperparams", "training_files", "validation_files", "result_files", "events"]
+    id: StrictStr = Field(description="The identifier, which can be referenced in API endpoints.")
+    object: StrictStr = Field(description="The object type, which is always `assistant`.")
+    created_at: StrictInt = Field(description="The Unix timestamp (in seconds) for when the assistant was created.")
+    name: Optional[Annotated[str, Field(strict=True, max_length=256)]] = Field(description="The name of the assistant. The maximum length is 256 characters. ")
+    description: Optional[Annotated[str, Field(strict=True, max_length=512)]] = Field(description="The description of the assistant. The maximum length is 512 characters. ")
+    model: StrictStr = Field(description="ID of the model to use. You can use the [List models](/docs/api-reference/models/list) API to see all of your available models, or see our [Model overview](/docs/models/overview) for descriptions of them. ")
+    instructions: Optional[Annotated[str, Field(strict=True, max_length=256000)]] = Field(description="The system instructions that the assistant uses. The maximum length is 256,000 characters. ")
+    tools: Annotated[List[AssistantObjectToolsInner], Field(max_length=128)] = Field(description="A list of tool enabled on the assistant. There can be a maximum of 128 tools per assistant. Tools can be of types `code_interpreter`, `retrieval`, or `function`. ")
+    file_ids: Annotated[List[StrictStr], Field(max_length=20)] = Field(description="A list of [file](/docs/api-reference/files) IDs attached to this assistant. There can be a maximum of 20 files attached to the assistant. Files are ordered by their creation date in ascending order. ")
+    metadata: Optional[Dict[str, Any]] = Field(description="Set of 16 key-value pairs that can be attached to an object. This can be useful for storing additional information about the object in a structured format. Keys can be a maximum of 64 characters long and values can be a maxium of 512 characters long. ")
+    __properties: ClassVar[List[str]] = ["id", "object", "created_at", "name", "description", "model", "instructions", "tools", "file_ids", "metadata"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['assistant']):
+            raise ValueError("must be one of enum values ('assistant')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -58,15 +62,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FineTune from a JSON string"""
+        """Create an instance of AssistantObject from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,69 +83,60 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in training_files (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in tools (list)
         _items = []
-        if self.training_files:
-            for _item in self.training_files:
+        if self.tools:
+            for _item in self.tools:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['training_files'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in validation_files (list)
-        _items = []
-        if self.validation_files:
-            for _item in self.validation_files:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['validation_files'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in result_files (list)
-        _items = []
-        if self.result_files:
-            for _item in self.result_files:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['result_files'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in events (list)
-        _items = []
-        if self.events:
-            for _item in self.events:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['events'] = _items
-        # set to None if fine_tuned_model (nullable) is None
+            _dict['tools'] = _items
+        # set to None if name (nullable) is None
+        # and model_fields_set contains the field
+        if self.name is None and "name" in self.model_fields_set:
+            _dict['name'] = None
+
+        # set to None if description (nullable) is None
+        # and model_fields_set contains the field
+        if self.description is None and "description" in self.model_fields_set:
+            _dict['description'] = None
+
+        # set to None if instructions (nullable) is None
+        # and model_fields_set contains the field
+        if self.instructions is None and "instructions" in self.model_fields_set:
+            _dict['instructions'] = None
+
+        # set to None if metadata (nullable) is None
         # and model_fields_set contains the field
-        if self.fine_tuned_model is None and "fine_tuned_model" in self.model_fields_set:
-            _dict['fine_tuned_model'] = None
+        if self.metadata is None and "metadata" in self.model_fields_set:
+            _dict['metadata'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FineTune from a dict"""
+        """Create an instance of AssistantObject from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
             "object": obj.get("object"),
             "created_at": obj.get("created_at"),
-            "updated_at": obj.get("updated_at"),
+            "name": obj.get("name"),
+            "description": obj.get("description"),
             "model": obj.get("model"),
-            "fine_tuned_model": obj.get("fine_tuned_model"),
-            "organization_id": obj.get("organization_id"),
-            "status": obj.get("status"),
-            "hyperparams": obj.get("hyperparams"),
-            "training_files": [OpenAIFile.from_dict(_item) for _item in obj["training_files"]] if obj.get("training_files") is not None else None,
-            "validation_files": [OpenAIFile.from_dict(_item) for _item in obj["validation_files"]] if obj.get("validation_files") is not None else None,
-            "result_files": [OpenAIFile.from_dict(_item) for _item in obj["result_files"]] if obj.get("result_files") is not None else None,
-            "events": [FineTuneEvent.from_dict(_item) for _item in obj["events"]] if obj.get("events") is not None else None
+            "instructions": obj.get("instructions"),
+            "tools": [AssistantObjectToolsInner.from_dict(_item) for _item in obj["tools"]] if obj.get("tools") is not None else None,
+            "file_ids": obj.get("file_ids"),
+            "metadata": obj.get("metadata")
         })
         return _obj
```

## Comparing `openapiopenai/models/fine_tune_event.py` & `openapiopenai/models/assistant_tools_retrieval.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FineTuneEvent(BaseModel):
+class AssistantToolsRetrieval(BaseModel):
     """
-    FineTuneEvent
+    AssistantToolsRetrieval
     """ # noqa: E501
-    object: StrictStr
-    created_at: StrictInt
-    level: StrictStr
-    message: StrictStr
-    __properties: ClassVar[List[str]] = ["object", "created_at", "level", "message"]
+    type: StrictStr = Field(description="The type of tool being defined: `retrieval`")
+    __properties: ClassVar[List[str]] = ["type"]
+
+    @field_validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['retrieval']):
+            raise ValueError("must be one of enum values ('retrieval')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +51,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FineTuneEvent from a JSON string"""
+        """Create an instance of AssistantToolsRetrieval from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,23 +76,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FineTuneEvent from a dict"""
+        """Create an instance of AssistantToolsRetrieval from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "object": obj.get("object"),
-            "created_at": obj.get("created_at"),
-            "level": obj.get("level"),
-            "message": obj.get("message")
+            "type": obj.get("type")
         })
         return _obj
```

## Comparing `openapiopenai/models/images_response_data_inner.py` & `openapiopenai/models/assistants_api_response_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ImagesResponseDataInner(BaseModel):
+class AssistantsApiResponseFormat(BaseModel):
     """
-    ImagesResponseDataInner
+    An object describing the expected output of the model. If `json_object` only `function` type `tools` are allowed to be passed to the Run. If `text` the model can return text or any value needed. 
     """ # noqa: E501
-    url: Optional[StrictStr] = None
-    b64_json: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["url", "b64_json"]
+    type: Optional[StrictStr] = Field(default='text', description="Must be one of `text` or `json_object`.")
+    __properties: ClassVar[List[str]] = ["type"]
+
+    @field_validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['text', 'json_object']):
+            raise ValueError("must be one of enum values ('text', 'json_object')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ImagesResponseDataInner from a JSON string"""
+        """Create an instance of AssistantsApiResponseFormat from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +79,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ImagesResponseDataInner from a dict"""
+        """Create an instance of AssistantsApiResponseFormat from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "url": obj.get("url"),
-            "b64_json": obj.get("b64_json")
+            "type": obj.get("type") if obj.get("type") is not None else 'text'
         })
         return _obj
```

## Comparing `openapiopenai/models/list_fine_tune_events_response.py` & `openapiopenai/models/list_fine_tuning_job_events_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
-from openapiopenai.models.fine_tune_event import FineTuneEvent
+from openapiopenai.models.fine_tuning_job_event import FineTuningJobEvent
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ListFineTuneEventsResponse(BaseModel):
+class ListFineTuningJobEventsResponse(BaseModel):
     """
-    ListFineTuneEventsResponse
+    ListFineTuningJobEventsResponse
     """ # noqa: E501
+    data: List[FineTuningJobEvent]
     object: StrictStr
-    data: List[FineTuneEvent]
-    __properties: ClassVar[List[str]] = ["object", "data"]
+    __properties: ClassVar[List[str]] = ["data", "object"]
+
+    @field_validator('object')
+    def object_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['list']):
+            raise ValueError("must be one of enum values ('list')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +53,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ListFineTuneEventsResponse from a JSON string"""
+        """Create an instance of ListFineTuningJobEventsResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,21 +85,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['data'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ListFineTuneEventsResponse from a dict"""
+        """Create an instance of ListFineTuningJobEventsResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "object": obj.get("object"),
-            "data": [FineTuneEvent.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None
+            "data": [FineTuningJobEvent.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
+            "object": obj.get("object")
         })
         return _obj
```

## Comparing `openapiopenai/models/list_fine_tunes_response.py` & `openapiopenai/models/run_stream_event_one_of7.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 # coding: utf-8
 
 """
     OpenAI API
 
-    APIs for sampling from and fine-tuning language models
+    The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
 
     The version of the OpenAPI document: 2.0.0
     Contact: blah+oapicf@cliffano.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
-from openapiopenai.models.fine_tune import FineTune
+from openapiopenai.models.run_object import RunObject
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ListFineTunesResponse(BaseModel):
+class RunStreamEventOneOf7(BaseModel):
     """
-    ListFineTunesResponse
+    Occurs when a [run](/docs/api-reference/runs/object) is cancelled.
     """ # noqa: E501
-    object: StrictStr
-    data: List[FineTune]
-    __properties: ClassVar[List[str]] = ["object", "data"]
+    event: StrictStr
+    data: RunObject
+    __properties: ClassVar[List[str]] = ["event", "data"]
+
+    @field_validator('event')
+    def event_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['thread.run.cancelled']):
+            raise ValueError("must be one of enum values ('thread.run.cancelled')")
+        return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +53,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ListFineTunesResponse from a JSON string"""
+        """Create an instance of RunStreamEventOneOf7 from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,32 +74,28 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ListFineTunesResponse from a dict"""
+        """Create an instance of RunStreamEventOneOf7 from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "object": obj.get("object"),
-            "data": [FineTune.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None
+            "event": obj.get("event"),
+            "data": RunObject.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
```

## Comparing `openapiopenai-1.0.0.dist-info/METADATA` & `openapiopenai-1.1.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: openapiopenai
-Version: 1.0.0
+Version: 1.1.0
 Summary: OpenAI API
 Home-page: https://github.com/oapicf/openapi-openai
 Author: Cliffano Subagio
 Author-email: blah+oapicf@cliffano.com
-License: UNKNOWN
+License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,OpenAI API
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic (>=2)
 Requires-Dist: python-dateutil
 Requires-Dist: typing-extensions (>=4.7.1)
 Requires-Dist: urllib3 (<2.1.0,>=1.25.3)
 
-APIs for sampling from and fine-tuning language models
+The OpenAI REST API. Please see https://platform.openai.com/docs/api-reference for more details.
```

