# Comparing `tmp/sweepai-2.0.0.dev1.tar.gz` & `tmp/sweepai-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-2.0.0.dev1.tar", last modified: Wed Apr  3 16:53:31 2024, max compression
+gzip compressed data, was "sweepai-2.0.1.tar", last modified: Mon Apr 15 19:29:17 2024, max compression
```

## Comparing `sweepai-2.0.0.dev1.tar` & `sweepai-2.0.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/
--rw-r--r--   0 root         (0) root         (0)    34523 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48133 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6420 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.004885 sweepai-2.0.0.dev1/eval/
--rw-r--r--   0 root         (0) root         (0)    10167 2024-04-02 00:22:38.000000 sweepai-2.0.0.dev1/eval/swe_bench.py
--rw-r--r--   0 root         (0) root         (0)    10513 2024-04-02 00:22:38.000000 sweepai-2.0.0.dev1/eval/swe_bench_utils.py
--rw-r--r--   0 root         (0) root         (0)     2009 2024-04-03 16:53:23.000000 sweepai-2.0.0.dev1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.004885 sweepai-2.0.0.dev1/sweepai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.008885 sweepai-2.0.0.dev1/sweepai/agents/
--rw-r--r--   0 root         (0) root         (0)     1185 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/agent_utils.py
--rw-r--r--   0 root         (0) root         (0)    53205 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_function_modify.py
--rw-r--r--   0 root         (0) root         (0)     4691 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_functions.py
--rw-r--r--   0 root         (0) root         (0)    12576 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_planning.py
--rw-r--r--   0 root         (0) root         (0)    18975 2024-04-01 21:54:50.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     4052 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/assistant_wrapper_test.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/complete_code.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/complete_code_test.py
--rw-r--r--   0 root         (0) root         (0)     2448 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/distill_issue.py
--rw-r--r--   0 root         (0) root         (0)    27333 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev1/sweepai/agents/modify_bot.py
--rw-r--r--   0 root         (0) root         (0)     5367 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev1/sweepai/agents/modify_file.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/pr_description_bot.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/agents/prune_modify_snippets.py
--rw-r--r--   0 root         (0) root         (0)    52353 2024-04-01 21:54:50.000000 sweepai-2.0.0.dev1/sweepai/api.py
--rw-r--r--   0 root         (0) root         (0)      753 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/api_test.py
--rw-r--r--   0 root         (0) root         (0)    13534 2024-04-02 23:14:46.000000 sweepai-2.0.0.dev1/sweepai/cli.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/cli_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.008885 sweepai-2.0.0.dev1/sweepai/config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12598 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/config/client.py
--rw-r--r--   0 root         (0) root         (0)     9564 2024-04-02 22:54:02.000000 sweepai-2.0.0.dev1/sweepai/config/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.008885 sweepai-2.0.0.dev1/sweepai/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15920 2024-04-02 23:51:20.000000 sweepai-2.0.0.dev1/sweepai/core/chat.py
--rw-r--r--   0 root         (0) root         (0)    42278 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/core/context_pruning.py
--rw-r--r--   0 root         (0) root         (0)    17833 2024-03-26 17:32:09.000000 sweepai-2.0.0.dev1/sweepai/core/entities.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/core/external_searcher.py
--rw-r--r--   0 root         (0) root         (0)    10630 2024-04-02 18:54:07.000000 sweepai-2.0.0.dev1/sweepai/core/lexical_search.py
--rw-r--r--   0 root         (0) root         (0)     5826 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/core/post_merge.py
--rw-r--r--   0 root         (0) root         (0)     4345 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/core/pr_reader.py
--rw-r--r--   0 root         (0) root         (0)    36545 2024-03-29 19:15:49.000000 sweepai-2.0.0.dev1/sweepai/core/prompts.py
--rw-r--r--   0 root         (0) root         (0)    13688 2024-03-31 22:18:38.000000 sweepai-2.0.0.dev1/sweepai/core/reflection_utils.py
--rw-r--r--   0 root         (0) root         (0)     5377 2024-04-02 00:22:38.000000 sweepai-2.0.0.dev1/sweepai/core/repo_parsing_utils.py
--rw-r--r--   0 root         (0) root         (0)    52641 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/core/sweep_bot.py
--rw-r--r--   0 root         (0) root         (0)     5758 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/core/update_prompts.py
--rw-r--r--   0 root         (0) root         (0)     9561 2024-04-02 23:24:36.000000 sweepai-2.0.0.dev1/sweepai/core/vector_db.py
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/global_threads.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.012885 sweepai-2.0.0.dev1/sweepai/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15582 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/create_pr.py
--rw-r--r--   0 root         (0) root         (0)     5670 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_button_click.py
--rw-r--r--   0 root         (0) root         (0)     1569 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_button_click_test.py
--rw-r--r--   0 root         (0) root         (0)     5247 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_check_suite.py
--rw-r--r--   0 root         (0) root         (0)    18961 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_comment.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_merge.py
--rw-r--r--   0 root         (0) root         (0)    13160 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_merge_conflict.py
--rw-r--r--   0 root         (0) root         (0)      722 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_review.py
--rw-r--r--   0 root         (0) root         (0)    86721 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev1/sweepai/handlers/on_ticket.py
--rw-r--r--   0 root         (0) root         (0)     5262 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/pr_utils.py
--rw-r--r--   0 root         (0) root         (0)    10042 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/stack_pr.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/handlers/stack_pr_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.012885 sweepai-2.0.0.dev1/sweepai/logn/
--rw-r--r--   0 root         (0) root         (0)       44 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/logn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5942 2024-03-26 17:31:09.000000 sweepai-2.0.0.dev1/sweepai/logn/cache.py
--rw-r--r--   0 root         (0) root         (0)    11758 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/logn/logn.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/logn/trace_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/sweepai/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3152 2024-04-02 23:52:56.000000 sweepai-2.0.0.dev1/sweepai/utils/anthropic_client.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/autoimport.py
--rw-r--r--   0 root         (0) root         (0)     3047 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/buttons.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/buttons_test.py
--rw-r--r--   0 root         (0) root         (0)     7850 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/chat_logger.py
--rw-r--r--   0 root         (0) root         (0)     7882 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/code_tree.py
--rw-r--r--   0 root         (0) root         (0)      716 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/code_tree_test.py
--rw-r--r--   0 root         (0) root         (0)      616 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/comment_utils.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/comment_utils_test.py
--rw-r--r--   0 root         (0) root         (0)     5817 2024-03-30 01:11:28.000000 sweepai-2.0.0.dev1/sweepai/utils/convert_openai_anthropic.py
--rw-r--r--   0 root         (0) root         (0)    12918 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/diff.py
--rw-r--r--   0 root         (0) root         (0)     2902 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/diff_test.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)      392 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/docker_utils_test.py
--rw-r--r--   0 root         (0) root         (0)     2637 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/event_logger.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     6767 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/fuzzy_diff.py
--rw-r--r--   0 root         (0) root         (0)     2709 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/fuzzy_diff_test.py
--rw-r--r--   0 root         (0) root         (0)    24266 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/utils/github_utils.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/github_utils_test.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/hash.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/html_extractor.py
--rw-r--r--   0 root         (0) root         (0)     3115 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/utils/modify_utils.py
--rw-r--r--   0 root         (0) root         (0)     5802 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/utils/multi_query.py
--rw-r--r--   0 root         (0) root         (0)    21464 2024-03-31 22:18:38.000000 sweepai-2.0.0.dev1/sweepai/utils/openai_listwise_reranker.py
--rw-r--r--   0 root         (0) root         (0)    11068 2024-03-26 22:42:55.000000 sweepai-2.0.0.dev1/sweepai/utils/openai_proxy.py
--rw-r--r--   0 root         (0) root         (0)     4220 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/openai_proxy_test.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/patch_utils.py
--rw-r--r--   0 root         (0) root         (0)     9641 2024-03-28 21:42:33.000000 sweepai-2.0.0.dev1/sweepai/utils/progress.py
--rw-r--r--   0 root         (0) root         (0)      384 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/progress_test.py
--rw-r--r--   0 root         (0) root         (0)     8711 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/prompt_constructor.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/regex_utils.py
--rw-r--r--   0 root         (0) root         (0)      841 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/safe_pqueue.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/scorer.py
--rw-r--r--   0 root         (0) root         (0)      791 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/scorer_test.py
--rw-r--r--   0 root         (0) root         (0)    13788 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/search_and_replace.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/search_and_replace_test.py
--rw-r--r--   0 root         (0) root         (0)     4596 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/str_utils.py
--rw-r--r--   0 root         (0) root         (0)    12066 2024-04-03 05:54:24.000000 sweepai-2.0.0.dev1/sweepai/utils/ticket_utils.py
--rw-r--r--   0 root         (0) root         (0)      606 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/timer.py
--rw-r--r--   0 root         (0) root         (0)     7346 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/tree_utils.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/user_settings.py
--rw-r--r--   0 root         (0) root         (0)    21346 2024-04-02 01:55:11.000000 sweepai-2.0.0.dev1/sweepai/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)      586 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/utils/utils_test.py
--rw-r--r--   0 root         (0) root         (0)     3989 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/sweepai/web/
--rw-r--r--   0 root         (0) root         (0)     4588 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/web/events.py
--rw-r--r--   0 root         (0) root         (0)     1945 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/web/health.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/sweepai/web/health_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/sweepai.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48133 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3296 2024-04-03 16:53:31.000000 sweepai-2.0.0.dev1/sweepai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-03 16:53:30.000000 sweepai-2.0.0.dev1/sweepai.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:53:31.020885 sweepai-2.0.0.dev1/tests/
--rw-r--r--   0 root         (0) root         (0)      314 2024-03-26 02:10:48.000000 sweepai-2.0.0.dev1/tests/test_watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)     2615 2024-04-10 22:25:21.000000 sweepai-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10746 2024-04-15 19:29:17.151241 sweepai-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6058 2024-04-05 22:26:32.000000 sweepai-2.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     2041 2024-04-15 19:29:01.000000 sweepai-2.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 19:29:17.151241 sweepai-2.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.135241 sweepai-2.0.1/sweepai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.139241 sweepai-2.0.1/sweepai/agents/
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/agent_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/assistant_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3525 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/agents/assistant_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/assistant_wrapper_test.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/complete_code.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/complete_code_test.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/distill_issue.py
+-rw-r--r--   0 root         (0) root         (0)    43756 2024-04-15 19:13:53.000000 sweepai-2.0.1/sweepai/agents/modify.py
+-rw-r--r--   0 root         (0) root         (0)    23096 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/agents/modify_bot.py
+-rw-r--r--   0 root         (0) root         (0)     3515 2024-04-10 19:41:10.000000 sweepai-2.0.1/sweepai/agents/modify_file.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/pr_description_bot.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/prune_modify_snippets.py
+-rw-r--r--   0 root         (0) root         (0)    52254 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/api.py
+-rw-r--r--   0 root         (0) root         (0)      753 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/api_test.py
+-rw-r--r--   0 root         (0) root         (0)    13441 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/cli_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.139241 sweepai-2.0.1/sweepai/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12573 2024-04-09 21:46:59.000000 sweepai-2.0.1/sweepai/config/client.py
+-rw-r--r--   0 root         (0) root         (0)     9845 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/config/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.143241 sweepai-2.0.1/sweepai/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19770 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/core/chat.py
+-rw-r--r--   0 root         (0) root         (0)    47834 2024-04-14 04:26:32.000000 sweepai-2.0.1/sweepai/core/context_pruning.py
+-rw-r--r--   0 root         (0) root         (0)    17807 2024-04-14 22:35:21.000000 sweepai-2.0.1/sweepai/core/entities.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/core/external_searcher.py
+-rw-r--r--   0 root         (0) root         (0)    10786 2024-04-04 06:39:36.000000 sweepai-2.0.1/sweepai/core/lexical_search.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/core/post_merge.py
+-rw-r--r--   0 root         (0) root         (0)     4345 2024-04-04 06:39:36.000000 sweepai-2.0.1/sweepai/core/pr_reader.py
+-rw-r--r--   0 root         (0) root         (0)    45522 2024-04-15 19:07:15.000000 sweepai-2.0.1/sweepai/core/prompts.py
+-rw-r--r--   0 root         (0) root         (0)    33698 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/core/reflection_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-04-09 21:46:59.000000 sweepai-2.0.1/sweepai/core/repo_parsing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    33362 2024-04-14 04:26:32.000000 sweepai-2.0.1/sweepai/core/sweep_bot.py
+-rw-r--r--   0 root         (0) root         (0)     5758 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/core/update_prompts.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2024-04-07 23:48:23.000000 sweepai-2.0.1/sweepai/core/vector_db.py
+-rw-r--r--   0 root         (0) root         (0)       19 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/global_threads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.143241 sweepai-2.0.1/sweepai/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15508 2024-04-07 00:49:31.000000 sweepai-2.0.1/sweepai/handlers/create_pr.py
+-rw-r--r--   0 root         (0) root         (0)     5670 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_button_click.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_button_click_test.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-04-09 21:46:59.000000 sweepai-2.0.1/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0 root         (0) root         (0)    18999 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/handlers/on_comment.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/handlers/on_jira_ticket.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_merge.py
+-rw-r--r--   0 root         (0) root         (0)    13160 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_merge_conflict.py
+-rw-r--r--   0 root         (0) root         (0)      722 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_review.py
+-rw-r--r--   0 root         (0) root         (0)    79755 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/handlers/on_ticket.py
+-rw-r--r--   0 root         (0) root         (0)     5168 2024-04-07 00:49:31.000000 sweepai-2.0.1/sweepai/handlers/pr_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/stack_pr.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/stack_pr_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.143241 sweepai-2.0.1/sweepai/logn/
+-rw-r--r--   0 root         (0) root         (0)       44 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/logn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2024-04-11 00:23:29.000000 sweepai-2.0.1/sweepai/logn/cache.py
+-rw-r--r--   0 root         (0) root         (0)    11758 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/logn/logn.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/logn/trace_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/sweepai/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3235 2024-04-09 21:46:59.000000 sweepai-2.0.1/sweepai/utils/anthropic_client.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/autoimport.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/buttons.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/buttons_test.py
+-rw-r--r--   0 root         (0) root         (0)     7850 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/chat_logger.py
+-rw-r--r--   0 root         (0) root         (0)     7882 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/code_tree.py
+-rw-r--r--   0 root         (0) root         (0)      716 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/code_tree_test.py
+-rw-r--r--   0 root         (0) root         (0)      616 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/comment_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/comment_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     6757 2024-04-05 22:26:32.000000 sweepai-2.0.1/sweepai/utils/convert_openai_anthropic.py
+-rw-r--r--   0 root         (0) root         (0)    13400 2024-04-12 22:10:10.000000 sweepai-2.0.1/sweepai/utils/diff.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/diff_test.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)      392 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/docker_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/event_logger.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7115 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/utils/fuzzy_diff.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/fuzzy_diff_test.py
+-rw-r--r--   0 root         (0) root         (0)    24360 2024-04-11 19:33:18.000000 sweepai-2.0.1/sweepai/utils/github_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/github_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/hash.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/html_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2024-04-15 19:07:17.000000 sweepai-2.0.1/sweepai/utils/modify_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5888 2024-04-09 00:20:22.000000 sweepai-2.0.1/sweepai/utils/multi_query.py
+-rw-r--r--   0 root         (0) root         (0)    34644 2024-04-12 22:10:10.000000 sweepai-2.0.1/sweepai/utils/openai_listwise_reranker.py
+-rw-r--r--   0 root         (0) root         (0)    11201 2024-04-10 19:41:10.000000 sweepai-2.0.1/sweepai/utils/openai_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     4220 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/openai_proxy_test.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/patch_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9641 2024-03-28 21:42:33.000000 sweepai-2.0.1/sweepai/utils/progress.py
+-rw-r--r--   0 root         (0) root         (0)      384 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/progress_test.py
+-rw-r--r--   0 root         (0) root         (0)     7557 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/regex_utils.py
+-rw-r--r--   0 root         (0) root         (0)      841 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/safe_pqueue.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/scorer.py
+-rw-r--r--   0 root         (0) root         (0)      791 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/scorer_test.py
+-rw-r--r--   0 root         (0) root         (0)    13788 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/search_and_replace.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/search_and_replace_test.py
+-rw-r--r--   0 root         (0) root         (0)     4991 2024-04-05 22:26:32.000000 sweepai-2.0.1/sweepai/utils/str_utils.py
+-rw-r--r--   0 root         (0) root         (0)    15481 2024-04-14 04:26:32.000000 sweepai-2.0.1/sweepai/utils/ticket_utils.py
+-rw-r--r--   0 root         (0) root         (0)      606 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/timer.py
+-rw-r--r--   0 root         (0) root         (0)     7346 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/tree_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/user_settings.py
+-rw-r--r--   0 root         (0) root         (0)    23680 2024-04-15 19:07:15.000000 sweepai-2.0.1/sweepai/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)      586 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/sweepai/web/
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/web/event_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/web/events.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/web/health.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/web/health_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/sweepai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10746 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3315 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      728 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      573 2024-04-07 00:49:31.000000 sweepai-2.0.1/tests/test_gha_extraction.py
+-rw-r--r--   0 root         (0) root         (0)      381 2024-04-08 20:37:50.000000 sweepai-2.0.1/tests/test_jira_ticket.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-03-26 02:10:48.000000 sweepai-2.0.1/tests/test_watch.py
```

### Comparing `sweepai-2.0.0.dev1/PKG-INFO` & `sweepai-2.0.1/sweepai/core/prompts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,839 +1,1215 @@
-Metadata-Version: 2.1
-Name: sweepai
-Version: 2.0.0.dev1
-Summary: Sweep fixes GitHub issues
-Author-email: Kevin Lu <kevin@sweep.dev>, William Zeng <william@sweep.dev>, Martin Ye <martin@sweep.dev>
-License:                     GNU AFFERO GENERAL PUBLIC LICENSE
-                               Version 3, 19 November 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU Affero General Public License is a free, copyleft license for
-        software and other kinds of works, specifically designed to ensure
-        cooperation with the community in the case of network server software.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        our General Public Licenses are intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          Developers that use our General Public Licenses protect your rights
-        with two steps: (1) assert copyright on the software, and (2) offer
-        you this License which gives you legal permission to copy, distribute
-        and/or modify the software.
-        
-          A secondary benefit of defending all users' freedom is that
-        improvements made in alternate versions of the program, if they
-        receive widespread use, become available for other developers to
-        incorporate.  Many developers of free software are heartened and
-        encouraged by the resulting cooperation.  However, in the case of
-        software used on network servers, this result may fail to come about.
-        The GNU General Public License permits making a modified version and
-        letting the public access it on a server without ever releasing its
-        source code to the public.
-        
-          The GNU Affero General Public License is designed specifically to
-        ensure that, in such cases, the modified source code becomes available
-        to the community.  It requires the operator of a network server to
-        provide the source code of the modified version running there to the
-        users of that server.  Therefore, public use of a modified version, on
-        a publicly accessible server, gives the public access to the source
-        code of the modified version.
-        
-          An older license, called the Affero General Public License and
-        published by Affero, was designed to accomplish similar goals.  This is
-        a different license, not a version of the Affero GPL, but Affero has
-        released a new version of the Affero GPL which permits relicensing under
-        this license.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU Affero General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Remote Network Interaction; Use with the GNU General Public License.
-        
-          Notwithstanding any other provision of this License, if you modify the
-        Program, your modified version must prominently offer all users
-        interacting with it remotely through a computer network (if your version
-        supports such interaction) an opportunity to receive the Corresponding
-        Source of your version by providing access to the Corresponding Source
-        from a network server at no charge, through some standard or customary
-        means of facilitating copying of software.  This Corresponding Source
-        shall include the Corresponding Source for any work covered by version 3
-        of the GNU General Public License that is incorporated pursuant to the
-        following paragraph.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the work with which it is combined will remain governed by version
-        3 of the GNU General Public License.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU Affero General Public License from time to time.  Such new versions
-        will be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU Affero General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU Affero General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU Affero General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Affero General Public License as published
-            by the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU Affero General Public License for more details.
-        
-            You should have received a copy of the GNU Affero General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If your software can interact with users remotely through a computer
-        network, you should also make sure that it provides a way for users to
-        get its source.  For example, if your program is a web application, its
-        interface could display a "Source" link that leads users to an archive
-        of the code.  There are many ways you could offer source, and different
-        solutions will be better for different programs; see section 13 for the
-        specific requirements.
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU AGPL, see
-        <https://www.gnu.org/licenses/>.
-        
-Project-URL: Repository, https://github.com/sweepai/sweep
-Project-URL: Community, https://discord.gg/sweep
-Project-URL: Documentation, https://docs.sweep.dev
-Project-URL: Homepage, https://sweep.dev
-Project-URL: Bug Tracker, https://github.com/sweepai/sweep/issues
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: anthropic==0.21.3
-Requires-Dist: beautifulsoup4==4.12.3
-Requires-Dist: typer==0.10.0
-Requires-Dist: pygithub==2.2.0
-Requires-Dist: loguru==0.7.2
-Requires-Dist: rich==13.7.1
-Requires-Dist: fastapi==0.110.0
-Requires-Dist: prometheus-fastapi-instrumentator==7.0.0
-Requires-Dist: pyyaml==6.0.1
-Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: openai==1.13.3
-Requires-Dist: backoff==2.2.1
-Requires-Dist: pymongo==4.6.2
-Requires-Dist: gitpython==3.1.42
-Requires-Dist: tree-sitter==0.21.0
-Requires-Dist: tree-sitter-languages==1.10.2
-Requires-Dist: rapidfuzz==3.6.2
-Requires-Dist: importmagic==0.1.7
-Requires-Dist: hatchet-sdk==0.18.0
-Requires-Dist: pyflakes==3.2.0
-Requires-Dist: beautifulsoup4==4.12.3
-Requires-Dist: networkx==3.2.1
-Requires-Dist: attrs==23.2.0
-Requires-Dist: pytest==8.1.1
-Requires-Dist: redis==5.0.3
-Requires-Dist: numpy==1.26.4
-Requires-Dist: markdown==3.5.2
-Requires-Dist: yamllint==1.35.1
-Requires-Dist: logtail==1.0.1
-Requires-Dist: tabulate==0.9.0
-Requires-Dist: rapidfuzz==3.6.2
-Requires-Dist: resend==0.8.0
-Requires-Dist: psutil==5.9.8
-Requires-Dist: jinja2==3.1.3
-Requires-Dist: tiktoken==0.6.0
-Requires-Dist: uvicorn==0.29.0
-Requires-Dist: pylint==3.1.0
-Requires-Dist: parea-ai==0.2.114
-Requires-Dist: voyageai==0.2.1
-Requires-Dist: boto3==1.34.70
-Requires-Dist: scipy==1.12.0
-
-<p align="center">
-    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">
-</p>
-<p align="center">
-    <i>Github Issues ⟶&nbsp; Pull Requests! </i>
-</p>
-<p align="center">
-    <a href="https://github.com/apps/sweep-ai">
-        <img alt="Install Sweep Github App" src="https://img.shields.io/badge/Install Sweep-GitHub App-purple?link=https://github.com/apps/sweep-ai">
-    </a>
-    <a href="https://discord.gg/sweep">
-        <img src="https://dcbadge.vercel.app/api/server/sweep?style=flat" />
-    </a>
-    <a href="https://hub.docker.com/r/sweepai/sweep">
-        <img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/sweepai/sweep" />
-    </a>
-    <a href="https://docs.sweep.dev/">
-        <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-red?link=https%3A%2F%2Fdocs.sweep.dev">
-    </a>
-    <a href="https://github.com/sweepai/sweep">
-        <img src="https://img.shields.io/github/commit-activity/m/sweepai/sweep" />
-    </a>
-    <a href="https://pypi.org/project/sweepai">
-        <img src="https://badge.fury.io/py/sweepai.svg" alt="PyPI version" height="18">
-    </a>
-    <a href="https://hub.docker.com/r/sweepai/sweep">
-        <img alt="Self Host Sweep Docker Image" src="https://img.shields.io/badge/Host Sweep-Docker Image-2496ED?link=https://hub.docker.com/r/sweepai/sweep">
-    </a>
-    <a href="https://github.com/sweepai/sweep/actions/workflows/unittest.yml">
-        <img src="https://github.com/sweepai/sweep/actions/workflows/unittest.yml/badge.svg" alt="Python Unit Tests">
-    </a>
-</p>
+"""
+List of common prompts used across the codebase.
+"""
+
+# Following two should be fused
+system_message_prompt = """\
+You are a brilliant and meticulous engineer assigned to write code for the following Github issue. When you write code, the code works on the first try, is syntactically perfect and is fully implemented. You have the utmost care for the code that you write, so you do not make mistakes and every function and class will be fully implemented. When writing tests, you will ensure the tests are fully implemented, very extensive and cover all cases, and you will make up test data as needed. Take into account the current repository's language, frameworks, and dependencies."""
+
+repo_description_prefix_prompt = "\nThis is a description of the repository:"
+
+rules_prefix_prompt = (
+    "\nThese are the user's preferences and instructions. Use them as needed"
+)
+
+human_message_prompt = [
+    {
+        "role": "user",
+        "content": """{relevant_snippets}""",
+        "key": "relevant_snippets",
+    },
+    {
+        "role": "user",
+        "content": """{relevant_directories}""",
+        "key": "relevant_directories",
+    },
+    {
+        "role": "user",
+        "content": """{relevant_commit_history}""",
+        "key": "relevant_commit_history",
+    },
+    {
+        "role": "user",
+        "content": """<repo_tree>
+{tree}
+</repo_tree>""",
+        "key": "relevant_tree",
+    },
+    {
+        "role": "user",
+        "content": """# Repo & Issue Metadata
+Repo: {repo_name}: {repo_description}
+Issue Title: {title}{description}""",
+        "key": "metadata",
+    },
+]
+
+human_message_review_prompt = [
+    {
+        "role": "user",
+        "content": """{relevant_snippets}""",
+    },
+    {
+        "role": "user",
+        "content": """{relevant_directories}""",
+    },
+    {"role": "user", "content": """{plan}"""},
+    {
+        "role": "user",
+        "content": """{diffs}""",
+    },
+]
+
+snippet_replacement_system_message = f"""{system_message_prompt}
+
+You are selecting relevant snippets for this issue. You must only select files that would help you understand the context of this issue.
+
+## Snippet Step
+
+In order to address this issue, what required information do you need about the snippets? Only include relevant code and required file imports that provides you enough detail about the snippets for the problems:
+
+Note: Do not select the entire file. Only select relevant lines from these files. Keep the relevant_snippets as small as possible.
+
+<contextual_thoughts>
+* Thought_1
+* Thought_2
+...
+</contextual_thoughts>
+
+<relevant_snippets>
+folder_1/file_1.py:1-13
+folder_2/file_2.py:42-75
+...
+</relevant_snippets>
+"""
+
+snippet_replacement = """Based on this issue, determine what context is relevant for the file changes. In the relevant_snippets, do not write the entire file lines. Choose only the most important lines.
+
+Complete the Snippet Step."""
+
+diff_section_prompt = """
+<file_diff file="{diff_file_path}">
+{diffs}
+</file_diff>"""
+
+review_prompt = """\
+Repo & Issue Metadata:
+<metadata>
+Repo: {repo_name}: {repo_description}
+Issue Title: {title}
+Issue Description:
+{description}
+</metadata>
+
+The code was written by an inexperienced programmer. Carefully review the code diffs in this pull request. Use the diffs along with the original plan to verify that each step of the plan was implemented correctly.
+
+Check for the following:
+* Missing imports
+* Incorrect functionality
+* Other errors not listed above
+* Incorrect/broken tests
+
+Indicate all breaking changes. Do not point out stylistic issues. Ensure that the code resolves the issue requested by the user and every function and class is fully implemented.
+
+Respond in the following format:c
+<diff_analysis>
+Check each file_diff function by function and confirm whether it was both implemented and implemented correctly.
+...
+</diff_analysis>"""
+
+final_review_prompt = """\
+Given the diff_analysis write a direct and concise GitHub review comment. Be extra careful with unimplemented sections and do not nitpick on formatting.
+If there is additional work to be done before this PR is ready, mention it. If there are no changes required, simply say "No changes required."
+In case changes are required, keep in mind the author is an inexperienced programmer and may need a pointer to the files and specific changes.
+Follow this format:
+<changes_required>
+Write Yes if the changes are required or No if they are not required.
+</changes_required>
+<review_comment>
+Mention any changes that need to be made, using GitHub markdown to format the comment.
+- Change required in file on line x1-x2
+- Change required in file on line y1-y2
+...
+</review_comment>"""
+
+issue_comment_prompt = """
+<comment username="{username}">
+{reply}
+</comment>"""
+
+# Prompt for comments
+human_message_prompt_comment = [
+    {
+        "role": "user",
+        "content": """{relevant_snippets}""",
+    },
+    {
+        "role": "user",
+        "content": """{relevant_directories}""",
+    },
+    {
+        "role": "user",
+        "content": """<repo_tree>
+{tree}
+</repo_tree>""",
+    },
+    {
+        "role": "user",
+        "content": """# Repo & Pull Request Metadata
+This is the repository as well as the original intent of the Pull Request.
+Repo: {repo_name}: {repo_description}
+Pull Request Title: {title}
+Pull Request Description: {description}{relevant_docs}""",
+    },
+    {
+        "role": "user",
+        "content": """These are the previous file changes
+{diff}""",
+    },
+    {
+        "role": "user",
+        "content": """Please handle the user review comment using the snippets, pull request title, pull request description, and the file changes.
+User pull request review: \"{comment}\"""",
+    },
+]
+
+cot_retrieval_prompt = """
+Gather information to solve the problem. Use "finish" when you feel like you have sufficient information.
+"""
+
+files_to_change_abstract_prompt = """Write an abstract minimum plan to address this issue in the least amount of change possible. Try to originate the root causes of this issue. Be clear and concise. 1 paragraph."""
+
+files_to_change_system_prompt = """You are a brilliant and meticulous engineer assigned to plan code changes to solve the following Github issue using the snippets provided from the codebase. You have the utmost care for the plan that you write, so you ensure that all the relevant modules in the file are identified. Take into account the current repository's language, frameworks, and dependencies, as well as the existing modules such as helper functions, utility operations and backend services."""
+
+files_to_change_system_prompt = """You are a brilliant and meticulous engineer assigned to plan code changes to solve the following Github issue using the snippets provided from the codebase. You have the utmost care for the plan that you write, so you ensure that all the relevant modules in the file are identified. Take into account the current repository's language, frameworks, and dependencies, as well as the existing modules such as helper functions, utility operations and backend services."""
+
+files_to_change_system_prompt = """\
+You are a brilliant and meticulous engineer assigned to plan code changes to solve the following Github issue. You have the utmost care for the plan that you write, so you do not make mistakes and every function and class will be fully implemented. Take into account the current repository's language, frameworks, and dependencies."""
+
+
+# put more emphasis on modify
+# TODO: lots of improvements and cleanup needed here
+files_to_change_prompt = """# Task: 
+Analyze the provided code snippets, repository, and GitHub issue to understand the requested change. Propose a complete plan for an intern to fully resolve the user's issue, utilizing the relevant code snippets and utility modules provided. Because the intern is unfamiliar with the codebase, provide clear and detailed instructions for updating the code logic.
+
+You are provided with relevent_snippets, which contain code snippets you may need to modify or import and read_only_snippets, which contain code snippets of utility functions, services and type definitions you likely do not need to modify.
+
+Guidelines:
+* Always include the full file path (e.g. src/utils/strings/regex_utils.py instead of just strings/regex_utils.py or regex_utils.py) and reference the provided snippets.
+* Provide clear, natural language instructions for updating the code logic and specify necessary imports.
+* Be specific and direct in your instructions, avoiding vague terms like "identify" or "ensure." Instead, use actionable phrases like "add", "locate" or "change."
+* Include relevant type definitions, interfaces, and schemas to provide a clear understanding of the entities and their relationships.
+* Avoid using line numbers; instead, reference the locations of the changes using surrounding code or function headers as context.
+* When modifying code, provide detailed instructions and the actual code changes required. Write all code changes in the diff format. Do not leave comments or placeholders for the user to fill in.
+
+Please use the following XML format for your response:
+
+# Issue Analysis:
+<issue_analysis>
+* Identify the root cause of the issue by referencing specific code entities in the relevant files.
+* Outline a plan that completely resolves the user's request, referencing provided code snippets, entity names, and necessary files/directories.
+
+List ALL files we should modify to resolve the issue:
+- File path 1: Outline of instructions for modifying the file
+    - First change to make in the file
+    - Second change to make in the file
+- File path 2: Outline of instructions for modifying the file
+    - First change to make in the file
+    - Second change to make in the file
+[additional files as needed]
+
+List ALL relevant utility modules from the provided set and specify where they can be used, including:
+- Type definitions, interfaces, and schemas
+- Helper functions
+- Frontend components
+- Database services
+- API endpoints
+[additional relevant modules as needed]
+
+* For each <create> or <modify> section in your plan, explain its purpose and how it contributes to resolving the issue.
+* Topologically sort the plan so that changes in low-level modules, such as DB query logic, are made before changes in high-level modules, such as API endpoints.
+[additional analysis as needed]
+</issue_analysis>
+
+# Plan:
+<plan>
+<create file="file_path_1" relevant_files="space-separated list of files containing ALL modules to use when creating file_path_1">
+* Natural language instructions for creating the new file to solve the issue.
+* Reference necessary imports and entity names.
+* Include relevant type definitions, interfaces, and schemas.
+* Provide the actual code to be added, with detailed explanations.
+</create>
+
+[additional creates as needed]
+
+<modify file="file_path_2" relevant_files="space-separated list of files containing ALL modules to use while modifying file_path_2">
+* Detailed natural language instructions for modifying the file to solve the issue.
+* Reference the locations of the changes using surrounding code or function headers, not line numbers.
+* Include relevant type definitions, interfaces, and schemas.
+* Each file should be modified at most once. If multiple changes are needed, separate them into different <modify> blocks.
+</modify>
+
+[additional modifies as needed]
+</plan>
+
+Here's an example of an excellent issue analysis and plan:
+<issue_analysis>
+The root cause of the issue is that the searchProducts method in the ProductService class (product_service.py) does not properly handle searching for products by category, price range, and keyword simultaneously. It should return products that match all the provided criteria.
+
+To completely resolve the user's request, we need to:
+
+Modify the searchProducts method in product_service.py to:
+Add optional parameters for category_id, min_price, max_price, and keyword
+Update the database query to filter products based on the provided criteria
+Update the search_products endpoint in app.py to:
+Extract the new search parameters from the request
+Pass the parameters to the searchProducts method
+Update the ProductSchema in schemas/product_schema.py to include the category_id field
+Relevant files to modify:
+
+src/services/product_service.py - Update searchProducts to handle category, price range, and keyword filtering
+src/app.py - Update search_products endpoint to extract new parameters and pass them to searchProducts
+src/schemas/product_schema.py - Add category_id field to ProductSchema
+Relevant utility modules:
+"""
+
+# TODO: Fix relevant files block
+
+files_to_change_prompt = """# Task: 
+Critically analyze the provided code snippets, repository, and GitHub issue to understand the requested change. Propose a complete plan for an intern to fully resolve the user's issue, utilizing the relevant code snippets and utility modules provided. Because the intern is unfamiliar with the codebase, provide clear and detailed instructions for updating the code logic.
+
+You are provided with relevent_snippets, which contain code snippets you may need to modify or import and read_only_snippets, which contain code snippets of utility functions, services and type definitions you likely do not need to modify.
+
+Guidelines:
+* Always include the full file path and reference the provided snippets.
+* Provide clear, natural language instructions for updating the code logic and specify necessary imports.
+* Be specific and direct in your instructions, avoiding vague terms like "identify" or "ensure." Instead, use actionable phrases like "add", "locate" or "change."
+* Include relevant type definitions, interfaces, and schemas in the relevant_files to provide a clear understanding of the entities and their relationships.
+* Avoid using line numbers; instead, reference the locations of the changes using surrounding code or function headers as context.
+* Be certain that your plan is complete and covers all the necessary changes to fully resolve the issue.
+* Suggest high-quality changes that are completely safe, maintainable, efficient and backwards compatible.
+* Divide the task into smaller steps, where each <create> or <modify> section corresponds to one small code block of change. You may have multiple <modify> blocks for the same file.
+
+Please use the following XML format for your response:
+
+# Issue Analysis:
+<issue_analysis>
+* Identify the root cause of the issue by referencing specific code entities in the relevant files.
+* Outline ALL changes that need to occur for the user's request to be resolved, by referencing provided code snippets, entity names, and necessary files/directories.
+
+List ALL files we should modify to resolve the issue:
+- File path 1: Outline of instructions for modifying the file
+    - First change to make in the file
+    - Second change to make in the file
+- File path 2: Outline of instructions for modifying the file
+    - First change to make in the file
+    - Second change to make in the file
+[additional files as needed]
+
+List ALL relevant read-only utility modules from the provided set and specify where they can be used. These are not files you need to make changes to but files you need to read while making changes in other files, including:
+- Type definitions, interfaces, and schemas
+- Helper functions
+- Frontend components
+- Database services
+- API endpoints
+[additional relevant modules as needed]
+
+* For each <create> or <modify> section in your plan, explain its purpose and how it contributes to resolving the issue.
+[additional analysis as needed]
+</issue_analysis>
+
+# Plan:
+<plan>
+<create file="file_path_1">
+* Natural language instructions for creating the new file to solve the issue.
+* Reference necessary imports and entity names.
+* Include references to relevant type definitions, interfaces, and schemas.
+</create>
+
+[additional creates as needed]
+
+<modify file="file_path_2">
+* Detailed natural language instructions for modifying the file to solve the issue.
+* Reference the locations of the changes using surrounding code or function headers, not line numbers.
+* Include references to relevant type definitions, interfaces, and schemas.
+* Describe code changes, but do not write the actual code.
+* You may modify the same file multiple times. Each <modify> block should contain a single block of code changes from one small section of the file.
+</modify>
+
+[additional modifies as needed]
+</plan>
+
+<relevant_modules>
+[List of all relevant files to use or read while making changes, such as type definitions, interfaces, and schemas, one per line]
+</relevant_modules>
+
+Here's an example of an excellent issue analysis and plan:
+
+<issue_analysis>
+The root cause of the issue is that the `createPost` method in the `PostService` class (post_service.py) does not validate that the user submitting the post has a non-deleted account. It should check the `user.deleted` property and raise an exception if the user's account is deleted.
+
+To completely resolve the user's request, we need to:
+- Modify the `createPost` method in post_service.py to check if the user's account is deleted before creating the post
+- Add a new exception class `DeletedAccountError` in exceptions.py to raise when a deleted user tries to create a post
+- Update the `create_post` endpoint in app.py to catch the new `DeletedAccountError` and return a 403 error response
+
+Relevant files to modify:
+- src/services/post_service.py
+  - Import the `User` entity and `DeletedAccountError` 
+  - Add validation to check if the user's account is deleted in `createPost`
+  - Raise `DeletedAccountError` if the user's account is deleted
+- src/exceptions.py
+  - Define a new exception class `DeletedAccountError`
+- src/app.py
+  - Import the new `DeletedAccountError`
+  - Catch `DeletedAccountError` in the `create_post` endpoint
+  - Return a 403 error response if `DeletedAccountError` is caught
+
+The relevant utility modules are:
+- `User` entity (src/entities/user.py) - to check if user's account is deleted 
+- `Post` entity (src/entities/post.py) - the entity being created in `createPost`
+
+The <create> and <modify> changes work together to fully handle preventing deleted users from creating posts:
+- The new exception class is created first to be used in the other changes
+- The service method is updated to validate the user and raise the new exception 
+- The API endpoint is updated to catch the new exception and return an appropriate error
+</issue_analysis>
+
+<plan>
+<create file="src/exceptions.py">
+* Define a new exception class called `DeletedAccountError`
+* Have it inherit from the base `Exception` class
+* Give it a clear error message indicating that a deleted account tried to perform an action
+</create>
+
+<modify file="src/services/post_service.py">
+At the top of the file:
+* Import the `User` entity from `src/entities/user.py`
+* Import the `DeletedAccountError` from `src/exceptions.py`
+
+In the `createPost` method of the `PostService` class:
+* After getting the `user` by ID, add an if statement to check:
+  - If `user.deleted` is True, raise a `DeletedAccountError`
+  - Otherwise, continue with creating the post as normal
+</modify>
+
+<modify file="src/services/post_service.py">
+In the `createPost` method of the `PostService` class:
+* After the line that creates the new `post` instance, add:
+  - A call to `self.post_repo.save(post)` to save the new post to the database
+  - A call to `self.logger.info(f"User {{user.id}} created a new post with id {{post.id}}")` to log the post creation
+* Return the newly created `post` instance
+</modify>
+
+<modify file="src/app.py">
+At the top of the file: 
+* Import the `DeletedAccountError` from `src/exceptions.py`
+
+In the `create_post` endpoint:
+* Wrap the existing code in a try/except block
+* Catch the `DeletedAccountError` in the except block
+* If caught, return a JSON response with:
+  - A 403 status code
+  - An error message like "Cannot create post with a deleted account"
+</modify>
+</plan>
+
+<relevant_modules>
+src/entities/user.py
+src/entities/post.py
+</relevant_modules>"""
+
+extract_files_to_change_prompt = """\
+# Task:
+Create a plan that resolves the user's query and ONLY the user's query under "Issue Title" and "Issue Description", providing your response in the below format:
+<contextual_request_analysis>
+Review each function of each relevant_snippet and analyze the user request to determine if this change should use the refactor or unit test tools.
+The refactor tool performs code transformations in a single file without making other logical changes. Determine the function(s) that are too long and should have it's individual parts extracted.
+The unit test tool creates or edits unit tests for a given file. Determine all functions that should be unit tested.
+</contextual_request_analysis>
+
+<use_tools>
+True/False
+</use_tools>
+
+If use_tools is True, then generate a plan to use the given tools in this format:
+* Make sure destination_module refers to a python module and not a path.
+
+<refactor file="file_path_1" destination_module="destination_module" relevant_files="space-separated list of ALL files relevant for modifying file_path_1">
+</refactor>
+<test file="file_path_2" source_file="file_path_to_test" relevant_files="space-separated list of ALL files relevant for modifying file_path_2">
+* Unit tests for the file_path_to_test, to be written in file_path_2.
+* Exact and descriptive instructions for the tests to be created or modified.
+...
+</test>"""
+
+refactor_files_to_change_prompt = """\
+Reference and analyze the snippets, repo, and issue to break down the requested change and propose a plan that addresses the user's request.
+
+Provide a plan to solve the issue, following these rules:
+* You may only create new files, extract snippets into functions, relocate functions, or modify existing files.
+* Include the full path (e.g. src/main.py and not just main.py), using the repo_tree for reference.
+* Be concrete with instructions and do not write "identify x" or "ensure y is done". Simply write "add x" or "change y to z".
+
+You MUST follow the following format:
+
+# Contextual Request Analysis:
+<contextual_request_analysis>
+* Outline the ideal plan that solves the user request by referencing the snippets and any other necessary files/directories.
+* Describe each <create>, <modify>, <extract>, and <relocate> section in the following plan and why it will be needed. Make sure the ordering is correct.
+...
+</contextual_request_analysis>
+
+# Plan:
+<plan>
+<create file="file_path_1" relevant_files="space-separated list of ALL files relevant for creating file_path_1">
+* Exact instructions for creating the new file needed to solve the issue
+* Include references to all files, imports and entity names
+...
+</create>
+...
+
+<extract file="file_path_2" relevant_files="space-separated list of ALL files relevant for modifying file_path_2">
+* Extracts lines of code from a function into a new standalone function.
+* Only extract lines that reduce the overall nesting or complexity of the code.
+...
+</extract>
+...
+
+<relocate file="file_path_3" new_file_path="new_file_path" handle_references="True">
+* This will move a function or variable from file_path_3 into another file while automatically resolving everything. If you use this block do not add other modifications related to imports, references, or function calls.
+</relocate>
+...
+
+<modify file="file_path_4" relevant_files="space-separated list of ALL files relevant for modifying file_path_4">
+* Modifies files by making less than 30-line changes. Be exact and mention references to all files, imports and entity names.
+* Use detailed, natural language instructions on what to modify regarding business logic, and reference files to import.
+* Be concrete with instructions and do not write "identify x" or "ensure y is done". Simply write "add x" or "change y to z".
+* You may modify the same file multiple times.
+...
+</modify>
+...
+
+</plan>"""
+
+sandbox_files_to_change_prompt = """\
+Analyze the snippets, repo, and issue to break down the requested problem or feature. Then propose a high-quality plan that completely fixes the CI/CD run.
+
+Provide a list of ALL of the files we should modify, abiding by the following:
+* You may only create and modify files.
+* Including the FULL path, e.g. src/main.py and not just main.py, using the repo_tree for reference.
+* Use detailed, natural language instructions on what to modify regarding business logic, and reference files to import.
+* Be concrete with instructions and do not write "check for x" or "ensure y is done". Simply write "add x" or "change y to z".
+* If the tests fail you should typically fix the tests and not the source code.
+
+You MUST follow the following format with the final output in XML tags:
+
+<analysis_and_plan>
+Whether the change was caused by the user's change or not. If not, then leave the plan empty.
+Otherwise, determine why the CI/CD run failed and the root cause. Determine the MINIMAL amount of changes to fix, with reference to entities, in the following format:
+
+<minimal_changes>
+* Change x: file to make the change
+* Change y: file to make the change
+...
+</minimal_changes>
+</analysis_and_plan>
+
+<plan>
+<create file="file_path_1" relevant_files="space-separated list of ALL files relevant for creating file_path_1">
+Outline of additions in concise natural language of what needs to be implemented in this file, referencing to external and imported libraries and business logic.
+</create>
+
+<modify file="file_path_2" relevant_files="space-separated list of ALL files relevant for modifying file_path_2">
+Outline of modifications in natural language (no code), referencing entities, and what type of patterns to look for, such as all occurrences of a variable or function call.
+Do not make this XML block if no changes are needed.
+</modify>
+...
+
+</plan>"""
+
+subissues_prompt = """
+Think step-by-step to break down the requested problem into sub-issues each of equally sized non-trivial changes. The sub-issue should be a small, self-contained, and independent part of the problem, and should partition the files to be changed.
+You MUST follow the following format with the final output in XML tags:
+
+Root cause:
+Identify the root cause of this issue and a minimum plan to address this issue concisely in two sentences.
+
+
+Step-by-step thoughts with explanations:
+* Concise imperative thoughts
+* No conjunctions
+...
+
+<plan>
+<issue title="title_1">
+* In file_path_1, do a
+* In file_path_1, do b
+...
+* In file_path_2, do c
+* In file_path_2, do d
+...
+</issue>
+
+<issue title="title_2">
+* In file_path_1, do a
+* In file_path_1, do b
+...
+* In file_path_2, do c
+* In file_path_2, do d
+...
+</issue>
+
+...
+</plan>"""
+
+create_file_prompt = """You are creating a file of code as part of a PR to solve the GitHub user's request. You will follow the request under "# Request" and respond based on the format under "# Format".
+
+# Request
+
+file_name: "{filename}"
+
+{instructions}
+
+# Format
+
+You MUST respond in the following XML format:
+
+<contextual_request_analysis>
+Concisely analyze the request and list step-by-step thoughts on what to create in each section, with low-level, detailed references to functions, variables, and imports to create, and what each function does. Be as explicit and specific as possible.
+Maximize information density in this section.
+</contextual_request_analysis>
+
+<new_file>
+The contents of the new file. NEVER write comments. All functions and classes will be fully implemented.
+When writing unit tests, they will be complete, extensive, and cover ALL edge cases. You will make up data for unit tests. Create mocks when necessary.
+</new_file>
+
+Commit message: "feat/fix: the commit message\"""".strip()
+
+"""
+Reply in the format below.
+* You MUST use the new_file XML tags
+* DO NOT write ``` anywhere, unless it's markdown
+* DO NOT write "pass" or "Rest of code"
+* Do not literally write "{{new_file}}".
+* Format:
+"""
+
+chunking_prompt = """
+We are handling this file in chunks. You have been provided a section of the code.
+Any lines that you do not see will be handled, so trust that the imports are managed and any other issues are taken care of.
+If you see code that should be modified, please modify it. The changes may not need to be in this chunk, do not make any changes."""
+
+modify_file_hallucination_prompt = [
+    {
+        "content": """File Name: (non-existent example)
+<old_file>
+example = True
+if example:
+    x = 1 # comment
+    print("hello")
+    x = 2
+
+class Example:
+    foo: int = 1
+
+    def func():
+        a = 3
+
+</old_file>
 
 ---
 
-<b>Sweep</b> is an AI junior developer that turns bugs and feature requests into code changes. Sweep automatically handles devex improvements like adding typehints/improving test coverage. :robot:
+Code Planning:
+Step-by-step thoughts with explanations:
+* Thought 1
+* Thought 2
+...
+
+Commit message: "feat/fix: the commit message"
+
+Detailed plan of modifications:
+* Modification 1
+* Modification 2
+...
+
+Code Generation:
+
+```
+Generate a diff based on the given plan using the search and replace pairs in the format below.
+* Always prefer the least amount of changes possible, but ensure the solution is complete
+* Prefer multiple small changes over a single large change.
+* NEVER write ellipses anywhere in the diffs. Simply write two diff hunks: one for the beginning and another for the end.
+* Always add lines before and after. The ORIGINAL section should be at least 5 lines long.
+
+The format is as follows:
+
+<<<< ORIGINAL
+line_before
+old_code
+line_after
+====
+line_before
+new_code
+line_after
+>>>> UPDATED
+```
+
+Commit message: "the commit message"
+
+Request: "Change hello to goodbye and change 3 to 4". Limit your changes to the request.
+
+Instructions:
+1. Complete the Code Planning step
+2. Complete the Code Generation step""",
+        "role": "user",
+        "key": "modify_file_hallucination",
+    },
+    {
+        "content": """Code Planning:
+Step-by-step thoughts with explanations:
+* We need to print "goodbye" instead of "hello".
+* We need to update the value of the variable a from 3 to 4.
+
+Detailed plan of modifications:
+* Change the output of the print statement from "hello" to "goodbye" as an example modification.
+* I will update the value of a from 3 to 4.
+
+Code Generation:
+```
+<<<< ORIGINAL
+example = True
+if example:
+    x = 1 # comment
+    print("hello")
+    x = 2
+====
+example = True
+if example:
+    x = 1 # comment
+    print("goodbye")
+    x = 2
+>>>> UPDATED
+
+<<<< ORIGINAL
+class Example:
+    foo: int = 1
+
+    def func():
+        a = 3
+====
+class Example:
+    foo: int = 1
+
+    def func():
+        a = 4
+>>>> UPDATED
+```
+
+Commit message: "Changed goodbye to hello and 3 to 4"\
+""",
+        "role": "assistant",
+        "key": "modify_file_hallucination",
+    },
+]
+
+# TODO: IMPORTANT: THIS DEPENDS ON THE ABOVE PROMPT, modify_file_hallucination_prompt
+modify_file_prompt_3 = """\
+File Name: {filename}
+<old_file>
+{code}
+</old_file>
+
+---
 
-[Install Sweep](https://github.com/apps/sweep-ai) and open a Github Issue like: `Sweep: Add typehints to src/utils/github_utils.py` and Sweep will:
-1. Search through your codebase to find the dependencies of github_utils.py
-2. Modify the code to add typehints
-3. **Run and debug your code to write a Pull Request** ⚡
+User's request:
+{instructions}
 
-### Features
-* Turns issues directly into pull requests (without an IDE)
-* Addresses developer replies & comments on its PRs
-* Understands your codebase using the dependency graph, text, and vector search.
-* Runs your unit tests and autoformatters to validate generated code.
-* Stack small fixes into your PR by applying [Sweep Rules](https://docs.sweep.dev/usage/config#tips-for-writing-rules)
+Limit your changes to the request.
 
-[![Sweep Youtube Tutorial](docs/public/assets/youtube_thumbnail.png)](https://www.youtube.com/watch?v=GVEkDZmWw8E)
+Instructions:
+Complete the Code Planning step and Code Modification step.
+Remember to NOT write ellipses, code things out in full, and use multiple small hunks.\
+"""
+
+modify_recreate_file_prompt_3 = """\
+File Name: {filename}
+<old_file>
+{code}
+</old_file>
 
+---
 
-> [!NOTE]
-> ### What makes Sweep Different
-> We've been addressing code modification using LLMs for a while. We found and are fixing a lot of issues.
->  - **Modifying Code** - LLMs like GPT4 don't have a great way to automatically modify code. We heavily experiment on different ways to modify code so you don't have to. We've spent a really long time working on this - check out https://docs.sweep.dev/blogs/gpt-4-modification!
-> - **Planning Code Changes** - Retrieval-Augmented-Generation isn't enough. We wrote a code chunker that's used fairly heavily, and we're constantly improving this: https://docs.sweep.dev/blogs/chunking-improvements
-> -  Sweep runs your **Github Actions**, catching bugs and making sure each line of new code has been properly validated!
-> -  **Sweep** uses it's sandbox to format your code, and uses [Rules](https://docs.sweep.dev/usage/config#tips-for-writing-rules) to perform other changes like adding typehints, or any other small chores!
+User's request:
+{instructions}
 
+Limit your changes to the request.
 
-## Getting Started
+Format:
+```
+<new_file>
+{{new file content}}
+</new_file>
+```
+
+Instructions:
+1. Complete the Code Planning step
+2. Complete the Code Modification step, remembering to NOT write ellipses, write complete functions, and use multiple small hunks where possible."""
+
+modify_file_system_message = """\
+You are a brilliant and meticulous engineer assigned to write code for the file to address a Github issue. When you write code, the code works on the first try and is syntactically perfect and complete. You have the utmost care for your code, so you do not make mistakes and every function and class will be fully implemented. Take into account the current repository's language, frameworks, and dependencies. You always follow up each code planning session with a code modification.
+
+When you modify code:
+* Always prefer the least amount of changes possible, but ensure the solution is complete.
+* Prefer multiple small changes over a single large change.
+* Do not edit the same parts multiple times.
+* Make sure to add additional lines before and after the original and updated code to disambiguate code when replacing repetitive sections.
+* NEVER write ellipses anywhere in the diffs. Simply write two diff hunks: one for the beginning and another for the end.
+
+Respond in the following format. Both the Code Planning and Code Modification steps are required.
+
+### Format ###
+
+## Code Planning:
+
+Thoughts and detailed plan:
+1.
+2.
+3.
+...
+
+Commit message: "feat/fix: the commit message"
+
+## Code Modification:
+
+Generated diff hunks based on the given plan using the search and replace pairs in the format below.
+```
+The first hunk's description
+
+<<<< ORIGINAL
+{exact copy of lines you would like to change}
+====
+{updated lines}
+>>>> UPDATED
+
+The second hunk's description
+
+<<<< ORIGINAL
+second line before
+first line before
+old code
+first line after
+second line after
+====
+second line before
+first line before
+new code
+first line after
+second line after
+>>>> UPDATED
+```"""
+
+RECREATE_LINE_LENGTH = -1
+
+modify_file_prompt_4 = """\
+File Name: {filename}
+
+<file>
+{code}
+</file>
 
-### GitHub App
-Install Sweep by adding the [**Sweep GitHub App**](https://github.com/apps/sweep-ai) to your desired repositories.
+---
 
-* For more details, visit our [installation page](https://docs.sweep.dev/getting-started).
+Modify the file by responding in the following format:
 
-* Note: Sweep only considers issues with the "Sweep:" title on creation and not on update. If you want Sweep to pick up an existing issue, you can add the "Sweep" label to the issue.
+Code Planning:
 
-* We focus on Python but support all languages GPT-4 can write. This includes JS/TS, Rust, Go, Java, C# and C++.
+Step-by-step thoughts with explanations:
+* Thought 1
+* Thought 2
+...
+
+Detailed plan of modifications:
+* Replace x with y
+* Add a foo method to bar
+...
+
+Code Modification:
+
+```
+Generate a diff based on the given instructions using the search and replace pairs in the following format:
+
+<<<< ORIGINAL
+second line before
+first line before
+old code
+first line after
+second line after
+====
+second line before
+first line before
+new code
+first line after
+second line after
+>>>> UPDATED
+```
+
+Commit message: "the commit message"
+
+The user's request is:
+{instructions}
+
+Instructions:
+1. Complete the Code Planning step
+2. Complete the Code Modification step
+"""
+
+rewrite_file_system_prompt = "You are a brilliant and meticulous engineer assigned to write code for the file to address a Github issue. When you write code, the code works on the first try and is syntactically perfect and complete. You have the utmost care for your code, so you do not make mistakes and every function and class will be fully implemented. Take into account the current repository's language, frameworks, and dependencies."
+
+rewrite_file_prompt = """\
+File Name: {filename}
+<old_file>
+{code}
+</old_file>
 
 ---
 
-## Story
+User's request:
+{instructions}
+
+Limit your changes to the request.
 
-We used to work in large, messy repositories, and we noticed how complex the code could get without regular refactors and unit tests. We realized that AI could handle these chores for us, so we built Sweep!
+Rewrite the following section from the old_file to handle this request.
 
-Unlike existing AI solutions, Sweep can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.
+<section>
 
-## Highlights
-[Examine pull requests created by Sweep!](https://docs.sweep.dev/about/examples)
+{section}
 
-## Pricing
-Every user receives unlimited GPT-3.5 tickets and 5 GPT-4 tickets per month. For professionals who want to try unlimited GPT-4 tickets and priority support, you can get a one week free trial of [Sweep Pro](https://buy.stripe.com/00g5npeT71H2gzCfZ8).
+</section>
 
-For more GPT-4 tickets visit <a href='https://buy.stripe.com/00g3fh7qF85q0AE14d'>our payment portal</a>!
+Think step-by-step on what to modify, then wrap the final answer in the brackets <section></section> XML tags. Only rewrite the section and do not close hanging parentheses and tags.\
+"""
 
-You can get enterprise support by [contacting us](https://form.typeform.com/to/wliuvyWE).
+sandbox_code_repair_modify_prompt_2 = """
+File Name: {filename}
+
+<file>
+{code}
+</file>
 
 ---
 
-> [!WARNING]
-> ### Limitations of Sweep
-> * **Gigantic repos**: >5000 files. We have default extensions and directories to exclude but sometimes this doesn't catch them all. You may need to block some directories (see [`blocked_dirs`](https://docs.sweep.dev/usage/config#blocked_dirs))
-    * If Sweep is stuck at 0% for over 30 min and your repo has a few thousand files, let us know.
-> * **Large-scale refactors**: >3 files or >150 lines of code changes
-    * e.g. Refactor the entire codebase from TensorFlow to PyTorch
-    * Sweep works best when pointed to a file, and we're continously improving Sweep's automation!
-> * **Editing images** and other non-text assets
-    * e.g. Use the logo to create favicons for our landing page
+Above is the code that was written by an inexperienced programmer, and contain errors such as syntax errors, linting erors and type-checking errors. The CI pipeline returned the following logs:
+
+stdout:
+```
+{stdout}
+```
+
+stderr
+```
+{stderr}
+```
+
+Respond in the following format:
+
+Code Planning
+
+Determine the following in code planning:
+1. Are there any syntax errors? Look through the file to find all syntax errors.
+2. Are there basic linting errors, like undefined variables, undefined members or type errors?
+3. Are there incorrect imports and exports?
+4. Are there any other errors not listed above?
+
+Determine whether changes are necessary based on the errors (ignore warnings).
+
+Code Modification:
+
+Generate a diff based on the given plan using the search and replace pairs in the format below.
+* Always prefer the least amount of changes possible, but ensure the solution is complete
+* Prefer multiple small changes over a single large change.
+* NEVER write ellipses anywhere in the diffs. Simply write two diff hunks: one for the beginning and another for the end.
+* DO NOT modify the same section multiple times.
+* Always add lines before and after. The ORIGINAL section should be at least 5 lines long.
+* Restrict the changes to fixing the errors from the logs.
+
+The format is as follows:
+
+```
+<<<< ORIGINAL
+second line before
+first line before
+old code of first hunk
+first line after
+second line after
+====
+second line before
+first line before
+new code of first hunk
+first line after
+second line after
+>>>> UPDATED
+
+<<<< ORIGINAL
+second line before
+first line before
+old code of second hunk
+first line after
+second line after
+====
+second line before
+first line before
+new code of second hunk
+first line after
+second line after
+>>>> UPDATED
+```
+
+Commit message: "the commit message"
+
+Instructions:
+1. Complete the Code Planning step
+2. Complete the Code Modification step
+"""
+
+pr_code_prompt = ""  # TODO: deprecate this
+
+pull_request_prompt = """Now, create a PR for your changes. Be concise but cover all of the changes that were made.
+For the pr_content, add two sections, description and summary.
+Use GitHub markdown in the following format:
+
+pr_title = "..."
+branch = "..."
+pr_content = \"\"\"
+...
+...
+\"\"\""""
+
+summarize_system_prompt = """
+You are an engineer assigned to helping summarize code instructions and code changes.
+"""
+
+user_file_change_summarize_prompt = """
+Summarize the given instructions for making changes in a pull request.
+Code Instructions:
+{message_content}
+"""
+
+assistant_file_change_summarize_prompt = """
+Please summarize the following file using the file stubs.
+Be sure to repeat each method signature and docstring. You may also add additional comments to the docstring.
+Do not repeat the code in the file stubs.
+Code Changes:
+{message_content}
+"""
+
+code_repair_check_system_prompt = """\
+You are a genius trained for validating code.
+You will be given two pieces of code marked by xml tags. The code inside <diff></diff> is the changes applied to create user_code, and the code inside <user_code></user_code> is the final product.
+Our goal is to validate if the final code is valid. This means there are no undefined variables, no syntax errors, has no unimplemented functions (e.g. pass's, comments saying "rest of code") and the code runs.
+"""
+
+code_repair_check_prompt = """\
+This is the diff that was applied to create user_code. Only make changes to code in user_code if the code was affected by the diff.
+
+This is the user_code.
+<user_code>
+{user_code}
+</user_code>
+
+Reply in the following format:
+
+Step-by-step thoughts with explanations:
+1. No syntax errors: True/False
+2. No undefined variables: True/False
+3. No unimplemented functions: True/False
+4. Code runs: True/False
+
+<valid>True</valid> or <valid>False</valid>
+"""
+
+code_repair_system_prompt = """\
+You are a genius trained for code stitching.
+You will be given two pieces of code marked by xml tags. The code inside <diff></diff> is the changes applied to create user_code, and the code inside <user_code></user_code> is the final product. The intention was to implement a change described as {feature}.
+Our goal is to return a working version of user_code that follows {feature}. We should follow the instructions and make as few edits as possible.
+"""
+
+code_repair_prompt = """\
+This is the diff that was applied to create user_code. Only make changes to code in user_code if the code was affected by the diff.
+
+This is the user_code.
+<user_code>
+{user_code}
+</user_code>
+
+Instructions:
+* Do not modify comments, docstrings, or whitespace.
+
+The only operations you may perform are:
+1. Indenting or dedenting code in user_code. This code MUST be code that was modified by the diff.
+2. Adding or deduplicating code in user_code. This code MUST be code that was modified by the diff.
+
+Return the working user_code without xml tags. All of the text you return will be placed in the file.
+"""
+
+doc_query_rewriter_system_prompt = """\
+You must rewrite the user's github issue to leverage the docs. In this case we want to look at {package}. It's used for: {description}. Using the github issue, write a search query that searches for the potential answer using the documentation. This query will be sent to a documentation search engine with vector and lexical based indexing. Make this query contain keywords relevant to the {package} documentation.
+"""
+
+doc_query_rewriter_prompt = """\
+This is the issue:
+{issue}
+
+Write a comprehensive search query for the answer.
+"""
+
+should_edit_code_system_prompt = """\
+We are processing a large file and trying to make code changes to it.
+The file is definitely relevant, but the section we observe may not be relevant.
+Your job is to determine whether the instructions are referring to the given section of the file.
+"""
+
+should_edit_code_prompt = """\
+Here are the instructions to change the code in the file:
+{problem_description}
+Here is the code snippet from the file:
+{code_snippet}
+
+To determine whether the instructions are referring to this section of the file, respond in the following format:
+1. Step-by-step thoughts with explanations:
+* Thought 1 - Explanation 1
+* Thought 2 - Explanation 2
+...
+2. Planning:
+* Is the code relevant?
+* If so, what is the relevant part of the code?
+* If not, what is the reason?
+
+3. In the last line of your response, write either <relevant>True</relevant> or <relevant>False</relevant>.
+"""
+
+slow_mode_system_prompt = """You are a brilliant and meticulous software architect. Your job is to take in the user's GitHub issue and the relevant context from their repository to:
+1. Gather more code snippets using a code search engine.
+2. Expand upon the plan to address the issue."""
+
+generate_plan_and_queries_prompt = """Think step-by-step to break down the requested problem or feature, and write up to three queries for the code search engine. These queries should find relevant code that is not already mentioned in the existing snippets. They should all mention different files and subtasks of the initial issue, avoid duplicates.
+Then add more instructions that build on the user's instructions. These instructions should help plan how to solve the issue.
+* The code search engine is based on semantic similarity. Ask questions that involve code snippets, function references, or mention relevant file paths.
+* The user's instructions should be treated as the source of truth, but sometimes the user will not mention the entire context. In that case, you should add the missing context.
+* Gather files that are relevant, including dependencies and similar files in the codebase. For example, if the user asked to write tests, look at similar tests.
+
+You MUST follow the following format delimited with XML tags:
+
+Step-by-step thoughts with explanations:
+* Thought 1 - Explanation 1
+* Thought 2 - Explanation 2
+...
+
+<queries>
+* query 1
+* query 2
+* query 3
+</queries>
+
+<additional_instructions>
+* additional instructions to be appended to the user's instructions
+</additional_instructions>
+"""
+
+external_search_system_prompt = (
+    "You are an expert at summarizing content from pages that are relevant to a query."
+    " You will be given a page and asked to summarize it."
+)
+
+external_search_prompt = """\
+Here is the page metadata:
+```
+{page_metadata}
+```
+
+The user is attempting to solve the following problem:
+\'\'\'
+{problem}
+\'\'\'
+
+Provide a summary of the page relevant to the problem, including all code snippets.
+"""
+
+
+docs_qa_system_prompt = """You are an expert at summarizing documentation for programming-related to help the user solve the problem. You will be given a question and relevant snippets of documentation, and be asked to provide a summary of relevant snippets for solving the problem."""
+docs_qa_user_prompt = """Here are the relevant documentation snippets:
+{snippets}
+
+The user is attempting to solve the following problem:
+{problem}
+"""
+
+linting_new_file_prompt = """
+<new_file>
+{code}
+</new_file>
+"""
+
+linting_modify_prompt = """Code Planning:
+Step-by-step thoughts with explanations:
+* Thought 1
+* Thought 2
+...
+
+Detailed plan of modifications:
+* Modification 1
+* Modification 2
+...
+
+Code Generation:
+
+```
+Generate a diff based on the given plan using the search and replace pairs in the format below.
+* Always prefer the least amount of changes possible
+* Prefer many small edits over few large edits
+* Always add lines before and after. The ORIGINAL section should be at least 5 lines long.
+
+The linter returned the following logs:
+<linter_logs>
+{logs}
+</linter_logs>
+
+Modify your created file. Note if no changes are needed.
+
 ---
 
-## Contributing
+The format is as follows:
+
+<<<< ORIGINAL
+====
+>>>> UPDATED
+
+Instructions:
+1. Complete the Code Planning step
+2. Complete the Code Generation step"""
+
+summarize_snippet_system_prompt = """You are a technical writer. Summarize code for an engineer. Be concise but detailed. Mention all entities implicitly. Never say "the code does x", just say "x". Keep it within 30 lines.
+
+E.g: If `issue_comment` is None, set `issue_comment` to `current_issue.create_comment(first_comment)`, otherwise edit comment via `issue_comment.edit(first_comment)`"""
+
+summarize_snippet_prompt = """# Code
+```
+{code}
+```
+
+# Repo Metadata
+{metadata}
+
+# Issue
+{issue}
+
+# Instructions
+Losslessly summarize the code in a ordered list for an engineer to search for relevant code to solve the above GitHub issue."""
 
-Contributions are welcome and greatly appreciated! To get set up, see [Development](https://github.com/sweepai/sweep#development). For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
+use_chunking_message = """\
+Respond with a list of the MINIMUM sections that should be modified. To insert code after a function, fetch the last few lines of the function."""
 
-<h2 align="center">
-    Contributors
-</h2>
-<p align="center">
-    Thank you for your contribution!
-</p>
-<p align="center">
-    <a href="https://github.com/sweepai/sweep/graphs/contributors">
-      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />
-    </a>
-</p>
-<p align="center">
-    and, of course, Sweep!
-</p>
+dont_use_chunking_message = """\
+Respond with a list of the MINIMUM sections that should be modified. To insert code after a function, fetch the last few lines of the function."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sweepai-2.0.0.dev1/README.md` & `sweepai-2.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -88,20 +88,18 @@
 
 You can get enterprise support by [contacting us](https://form.typeform.com/to/wliuvyWE).
 
 ---
 
 > [!WARNING]
 > ### Limitations of Sweep
-> * **Gigantic repos**: >5000 files. We have default extensions and directories to exclude but sometimes this doesn't catch them all. You may need to block some directories (see [`blocked_dirs`](https://docs.sweep.dev/usage/config#blocked_dirs))
-    * If Sweep is stuck at 0% for over 30 min and your repo has a few thousand files, let us know.
-> * **Large-scale refactors**: >3 files or >150 lines of code changes
+> * **Large-scale refactors**: > 10 files or > 400 lines of code changes
     * e.g. Refactor the entire codebase from TensorFlow to PyTorch
-    * Sweep works best when pointed to a file, and we're continously improving Sweep's automation!
-> * **Editing images** and other non-text assets
+    * If this is a use case you're looking forward to, let us know!
+> * **Reading or editing images** and other non-text assets
     * e.g. Use the logo to create favicons for our landing page
 ---
 
 ## Contributing
 
 Contributions are welcome and greatly appreciated! To get set up, see [Development](https://github.com/sweepai/sweep#development). For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

#### html2text {}

```diff
@@ -46,24 +46,19 @@
 at once. ## Highlights [Examine pull requests created by Sweep!](https://
 docs.sweep.dev/about/examples) ## Pricing Every user receives unlimited GPT-3.5
 tickets and 5 GPT-4 tickets per month. For professionals who want to try
 unlimited GPT-4 tickets and priority support, you can get a one week free trial
 of [Sweep Pro](https://buy.stripe.com/00g5npeT71H2gzCfZ8). For more GPT-
 4 tickets visit _o_u_r_ _p_a_y_m_e_n_t_ _p_o_r_t_a_l! You can get enterprise support by
 [contacting us](https://form.typeform.com/to/wliuvyWE). --- > [!WARNING] > ###
-Limitations of Sweep > * **Gigantic repos**: >5000 files. We have default
-extensions and directories to exclude but sometimes this doesn't catch them
-all. You may need to block some directories (see [`blocked_dirs`](https://
-docs.sweep.dev/usage/config#blocked_dirs)) * If Sweep is stuck at 0% for over
-30 min and your repo has a few thousand files, let us know. > * **Large-scale
-refactors**: >3 files or >150 lines of code changes * e.g. Refactor the entire
-codebase from TensorFlow to PyTorch * Sweep works best when pointed to a file,
-and we're continously improving Sweep's automation! > * **Editing images** and
-other non-text assets * e.g. Use the logo to create favicons for our landing
-page --- ## Contributing Contributions are welcome and greatly appreciated! To
-get set up, see [Development](https://github.com/sweepai/sweep#development).
-For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md]
-(CONTRIBUTING.md) file.
+Limitations of Sweep > * **Large-scale refactors**: > 10 files or > 400 lines
+of code changes * e.g. Refactor the entire codebase from TensorFlow to PyTorch
+* If this is a use case you're looking forward to, let us know! > * **Reading
+or editing images** and other non-text assets * e.g. Use the logo to create
+favicons for our landing page --- ## Contributing Contributions are welcome and
+greatly appreciated! To get set up, see [Development](https://github.com/
+sweepai/sweep#development). For detailed guidelines on how to contribute,
+please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
                            ********** CCoonnttrriibbuuttoorrss **********
                        Thank you for your contribution!
                _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_s_w_e_e_p_a_i_/_s_w_e_e_p_]
                             and, of course, Sweep!
```

### Comparing `sweepai-2.0.0.dev1/pyproject.toml` & `sweepai-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 Community = "https://discord.gg/sweep"
 Documentation = "https://docs.sweep.dev"
 Homepage = "https://sweep.dev"
 "Bug Tracker" = "https://github.com/sweepai/sweep/issues"
 
 [project]
 name = "sweepai"
-version = "2.0.0.dev1"
+version = "2.0.1"
 description = "Sweep fixes GitHub issues"
 authors = [
     {name = "Kevin Lu", email = "kevin@sweep.dev"},
     {name = "William Zeng", email = "william@sweep.dev"},
     {name = "Martin Ye", email = "martin@sweep.dev"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3.10"
 ]
 dependencies = [
   "anthropic==0.21.3",
   "beautifulsoup4==4.12.3",
+  "cohere==5.2.5",
   "typer==0.10.0",
   "pygithub==2.2.0",
   "loguru==0.7.2",
   "rich==13.7.1",
   "fastapi==0.110.0",
   "prometheus-fastapi-instrumentator==7.0.0",
   "pyyaml==6.0.1",
@@ -68,15 +69,16 @@
   "jinja2==3.1.3",
   "tiktoken==0.6.0",
   "uvicorn==0.29.0",
   "pylint==3.1.0",
   "parea-ai==0.2.114",
   "voyageai==0.2.1",
   "boto3==1.34.70",
-  "scipy==1.12.0"
+  "scipy==1.12.0",
+  "jira==3.8.0",
 ]
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 string-normalization = false
```

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/agent_utils.py` & `sweepai-2.0.1/sweepai/agents/agent_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/assistant_function_modify.py` & `sweepai-2.0.1/sweepai/agents/modify.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,212 +1,101 @@
-from copy import deepcopy
 import copy
 import os
-import json
-import subprocess
-import traceback
-from collections import defaultdict
 
-from loguru import logger
+from rapidfuzz import fuzz, process
 
-from sweepai.agents.assistant_wrapper import openai_assistant_call, tool_call_parameters
-from sweepai.agents.agent_utils import ensure_additional_messages_length
-from sweepai.config.client import SweepConfig
-from sweepai.core.entities import AssistantRaisedException, FileChangeRequest, Message
-from sweepai.logn.cache import file_cache
-from sweepai.utils.chat_logger import ChatLogger, discord_log_error
+from loguru import logger
+from tqdm import tqdm
+from sweepai.core.chat import ChatGPT, parse_function_calls_for_openai
+from sweepai.core.entities import FileChangeRequest, Message
+from sweepai.core.reflection_utils import ModifyEvaluatorAgent
+from sweepai.utils.chat_logger import ChatLogger
+from sweepai.utils.convert_openai_anthropic import AnthropicFunctionCall
 from sweepai.utils.diff import generate_diff
-from sweepai.utils.file_utils import read_file_with_fallback_encodings
-from sweepai.utils.github_utils import ClonedRepo, update_file
-from sweepai.utils.progress import AssistantConversation, TicketProgress
-from sweepai.utils.utils import chunk_code, get_check_results
-from sweepai.utils.modify_utils import post_process_rg_output, manual_code_check
-
-# Pre-amble using ideas from https://github.com/paul-gauthier/aider/blob/main/aider/coders/udiff_prompts.py
-# Doesn't regress on the benchmark but improves average code generated and avoids empty comments.
-
-# Add COT to each tool
-
-instructions = """You are an expert software developer tasked with editing code to fulfill the user's request. Your goal is to make the necessary changes to the codebase while following best practices and respecting existing conventions. 
-
-To complete the task, follow these steps:
-
-1. Carefully analyze the user's request to identify the key requirements and changes needed. Break down the problem into smaller sub-tasks.
-
-2. Search the codebase for relevant files, functions, classes, and variables related to the task at hand. Use the search results to determine where changes need to be made. 
-
-3. For each relevant file, identify the minimal code changes required to implement the desired functionality. Consider edge cases, error handling, and necessary imports.
-
-4. If new functionality is required that doesn't fit into existing files, create a new file with an appropriate name and location.
-
-5. Make the code changes in a targeted way:
-   - Preserve existing whitespace, comments and code style
-   - Make surgical edits to only the required lines of code
-   - If a change is complex, break it into smaller incremental changes
-   - Ensure each change is complete and functional before moving on
-
-6. When providing code snippets, be extremely precise with indentation:
-   - Count the exact number of spaces used for indentation
-   - If tabs are used, specify that explicitly 
-   - Ensure the indentation of the code snippet matches the original file exactly
-7. After making all the changes, review the modified code to verify it fully satisfies the original request.
-8. Once you are confident the task is complete, submit the final solution.
-
-In this environment, you have access to the following tools to assist in fulfilling the user request:
-
-You MUST call them like this:
-<function_calls>
-<invoke>
-<tool_name>$TOOL_NAME</tool_name>
-<parameters>
-<$PARAMETER_NAME>$PARAMETER_VALUE</$PARAMETER_NAME>
-...
-</parameters>
-</invoke>
-</function_calls>
-
-Here are the tools available:
-<tools>
-<tool_description>
-<tool_name>analyze_problem_and_propose_plan</tool_name>
-<description>
-Carefully analyze the user's request to identify the key requirements, changes needed, and any constraints or considerations. Break down the problem into sub-tasks.
-</description>
-<parameters>
-<parameter>
-<name>problem_analysis</name>
-<type>str</type>
-<description>
-Provide a thorough analysis of the user's request, identifying key details, requirements, intended behavior changes, and any other relevant information. Organize and prioritize the sub-tasks needed to fully address the request.
-</description>
-</parameter>
-<parameter>
-<name>proposed_plan</name>
-<type>str</type>
-<description>
-Describe the plan to solve the problem, including the keywords to search, modifications to make, and all required imports to complete the task.
-</description>
-</parameter>
-</parameters>
-</tool_description>
-
-<tool_description>
-<tool_name>search_codebase</tool_name>
-<description>
-Search the codebase for files, functions, classes, or variables relevant to a task. Searches can be scoped to a single file or across the entire codebase.
-</description>
-<parameters>
-<parameter>
-<name>justification</name>
-<type>str</type>
-<description>
-Explain why searching for this query is relevant to the task and how the results will inform the code changes.
-</description>
-</parameter>
-<parameter>
-<name>file_name</name>
-<type>str</type>
-<description>
-(Optional) The name of a specific file to search within. If not provided, the entire codebase will be searched.
-</description>
-</parameter>
-<parameter>
-<name>keyword</name>
-<type>str</type>
-<description>
-The search query, such as a function name, class name, or variable. Provide only one query term per search.
-</description>
-</parameter>
-</parameters>
-</tool_description>
-
-<tool_description>
-<tool_name>analyze_and_identify_changes</tool_name>
-<description>
-Determine the minimal code changes required in a file to implement a piece of the functionality. Consider edge cases, error handling, and necessary imports.
-</description>
-<parameters>
-<parameter>
-<name>file_name</name>
-<type>str</type>
-<description>
-The name of the file where changes need to be made.
-</description>
-</parameter>
-<name>changes</name>
-<type>str</type>
-<description>
-Describe the changes to make in the file. Specify the location of each change and provide the code modifications. Include any required imports or updates to existing code.
-</description>
-</parameter>
-</parameters>
-</tool_description>
-
-<tool_description>
-<tool_name>view_file</tool_name>
-<description>
-View the contents of a file from the codebase. Useful for viewing code in context before making changes.
-</description>
-<parameters>
-<parameter>
-<name>justification</name>
-<type>str</type>
-<description>
-Explain why viewing this file is necessary to complete the task or better understand the existing code.
-</description>
-</parameter>
-<parameter>
-<name>file_name</name>
-<type>str</type>
-<description>
-The name of the file to retrieve, including the extension. File names are case-sensitive.
-</description>
-</parameter>
-</parameters>
-</tool_description>
+from sweepai.utils.github_utils import ClonedRepo
+from sweepai.utils.modify_utils import manual_code_check
+from sweepai.utils.utils import get_check_results
+
+
+modify_tools_openai = """
+# make_change - Make a SINGLE, TARGETED code change in a file. Preserve whitespace, comments, and style. Changes should be minimal, self-contained, and address only one specific modification. If a change affects multiple separate code sections, use multiple calls to this tool, one for each section.
+To call this tool you must respond in the following xml format:
+
+<make_change>
+<justification>
+Explain how this SINGLE change contributes to fulfilling the user's request.
+</justification>
+<file_name>
+Name of the file where the change will be made. Ensure correct spelling as this is case-sensitive.
+</file_name>
+<original_code>
+The existing lines of code that need modification or replacement. This should be a SINGLE, CONTINUOUS block of code, not multiple separate sections. Include unchanged surrounding lines for context.
+</original_code>
+<new_code>
+The new lines of code to replace the original code, implementing the SINGLE desired change. If the change is complex, break it into smaller targeted changes and use separate make_change calls for each.
+</new_code>
+</make_change>
+
+# create_file - Create a new code file in the specified location with the given file name and extension. This is useful when the task requires adding entirely new functionality or classes to the codebase.
+To call this tool you must respond in the following xml format:
+<create_file>
+<file_path>
+The path where the new file should be created, relative to the root of the codebase. Do not include the file name itself.
+</file_path>
+<file_name>
+he name to give the new file, including the extension. Ensure the name is clear, descriptive, and follows existing naming conventions.
+</file_name>
+<contents>
+The initial contents of the new file.
+</contents>
+<justification>
+Explain why creating this new file is necessary to complete the task and how it integrates with the existing codebase structure.
+</justification>
+</create_file>
+
+# submit_result - Indicate that the task is complete and all requirements have been met. Provide the final code changes or solution.
+To call this tool you must respond in the following xml format:
+<submit_result>
+<justification>
+Summarize the code changes made and explain how they fulfill the user's original request. Provide the complete, modified code if applicable.
+</justification>
+</submit_result>"""
 
-<tool_description>
+modify_tools = """<tool_description>
 <tool_name>make_change</tool_name>
 <description>
-Make a single code change in a file. Preserve whitespace, comments and style. Changes should be minimal and targeted.
+Make a SINGLE, TARGETED code change in a file. Preserve whitespace, comments, and style. Changes should be minimal, self-contained, and address only one specific modification. If a change affects multiple separate code sections, use this tool for one change at a time, one for each section.
 </description>
 <parameters>
 <parameter>
 <name>justification</name>
 <type>str</type>
 <description>
-Explain how this change contributes to fulfilling the user's request.
+Explain how this SINGLE change contributes to fulfilling the user's request.
 </description>
 </parameter>
 <parameter>
 <name>file_name</name>
 <type>str</type>
 <description>
-Name of the file to make changes in. Ensure correct spelling as this is case-sensitive.
-</description>
-</parameter>
-<parameter>
-<name>section_id</name>
-<type>str</type>
-<description>
-The section ID where the original code belongs to, helping to locate the specific area within the file.
+Name of the file where the change will be made. Ensure correct spelling as this is case-sensitive.
 </description>
 </parameter>
 <parameter>
 <name>original_code</name>
 <type>str</type>
 <description>
-The existing lines of code that need to be modified or replaced. Include unchanged surrounding lines for context.
+The existing lines of code that need modification or replacement. This should be a short SINGLE, CONTINUOUS block of code, not multiple separate sections. Include unchanged surrounding lines for context.
 </description>
 </parameter>
 <parameter>
 <name>new_code</name>
 <type>str</type>
 <description>
-The new lines of code to replace the original code, implementing the desired change.
+The new lines of code to replace the original code, implementing the SINGLE desired change. If the change is complex, break it into smaller targeted changes and use separate make_change calls for each.
 </description>
 </parameter>
 </parameters>
 </tool_description>
 
 <tool_description>
 <tool_name>create_file</tool_name>
@@ -225,747 +114,720 @@
 <name>file_name</name>
 <type>str</type>
 <description>
 The name to give the new file, including the extension. Ensure the name is clear, descriptive, and follows existing naming conventions.
 </description>
 </parameter>
 <parameter>
-<parameter>
 <name>contents</name>
 <type>str</type>
 <description>
-The contents of this new file.
+The initial contents of the new file.
 </description>
 </parameter>
 <parameter>
 <name>justification</name>
 <type>str</type>
 <description>
-Explain why creating this new file is necessary to complete the task and how it fits into the existing codebase structure.
+Explain why creating this new file is necessary to complete the task and how it integrates with the existing codebase structure.
 </description>
 </parameter>
 </parameters>
 </tool_description>
 
 <tool_description>
 <tool_name>submit_result</tool_name>
 <description>
-Indicate that the task is complete and all requirements have been satisfied. Provide the final code changes or solution.
+Indicate that the task is complete and all requirements have been met. Provide the final code changes or solution.
 </description>
 <parameters>
 <parameter>
 <name>justification</name>
 <type>str</type>
 <description>
-Summarize the code changes made and how they fulfill the user's original request. Provide the complete, modified code if applicable.
+Summarize the code changes made and explain how they fulfill the user's original request. Provide the complete, modified code if applicable.
 </description>
 </parameter>
 </parameters>
-</tool_description>
+</tool_description>"""
+
+instructions = """You are an expert software developer tasked with editing code to fulfill the user's request. Your goal is to make the necessary changes to the codebase while following best practices and respecting existing conventions. 
+
+To complete the task, follow these steps:
+
+1. If new functionality is required that doesn't fit into existing files, create a new file with an appropriate name and location.
+
+2. Make the code changes in a targeted way:
+    - Preserve existing whitespace, comments and code style
+    - Make surgical edits to only the required lines of code
+    - If a change is complex, break it into smaller incremental changes
+    - Ensure each change is complete and functional before moving on
+        When providing code snippets, be extremely precise with indentation:
+        - Count the exact number of spaces used for indentation
+        - If tabs are used, specify that explicitly 
+        - Ensure the indentation of the code snippet matches the original file exactly
+3. After making all the changes, review the modified code to verify it fully satisfies the original request.
+4. Once you are confident the task is complete, submit the final solution.
+
+In this environment, you have access to the following tools to assist in fulfilling the user request:
+
+You MUST call them like this:
+<function_call>
+<invoke>
+<tool_name>$TOOL_NAME</tool_name>
+<parameters>
+<$PARAMETER_NAME>$PARAMETER_VALUE</$PARAMETER_NAME>
+...
+</parameters>
+</invoke>
+</function_call>
+
+Here are the tools available:
+
 """
 
-unformatted_tool_call_response = "<function_results>\n<result>\n<tool_name>{tool_name}<tool_name>\n<stdout>\n{tool_call_response_contents}\n</stdout>\n</result>\n</function_results>"
+NO_TOOL_CALL_PROMPT = """FAILURE
+No function calls were made or your last function call was incorrectly formatted. The correct syntax for function calling is this:
 
+<function_call>
+<invoke>
+<tool_name>tool_name</tool_name>
+<parameters>
+<param_name>param_value</param_name>
+</parameters>
+</invoke>
+</function_call>
 
-def int_to_excel_col(n):
-    result = ""
-    if n == 0:
-        result = "A"
-    while n > 0:
-        n, remainder = divmod(n - 1, 26)
-        result = chr(65 + remainder) + result
-    return result
-
-
-def excel_col_to_int(s):
-    result = 0
-    for char in s:
-        result = result * 26 + (ord(char) - 64)
-    return result - 1
-
-TOOLS_MAX_CHARS = 20000
-
-def build_keyword_search_match_results(
-    match_indices: list[int],
-    chunks: list[str],
-    keyword: str,
-    success_message,
-    readonly: bool = False,
-) -> str:
-    for match_index in match_indices:
-        # TODO: handle multiple matches in one line
-        match = chunks[match_index]
-        match_lines = match.split("\n")
-        lines_containing_keyword = [
-            i for i, line in enumerate(match_lines) if keyword in line
-        ]
-        cols_of_keyword = [
-            match_lines[line_containing_keyword].index(keyword)
-            for line_containing_keyword in lines_containing_keyword
-        ]
-        match_display = ""
-        for i, line in enumerate(match_lines):
-            if i in lines_containing_keyword:
-                match_display += (
-                    f"{line}\n"
-                    + " " * (cols_of_keyword[lines_containing_keyword.index(i)])
-                    + "^" * len(keyword)
-                    + "\n"
-                )
-            else:
-                match_display += f"{line}\n"
-        match_display = match_display.strip("\n")
-        num_matches_message = f" ({len(lines_containing_keyword)} matches)" if lines_containing_keyword else " (No keyword matches, just shown for context)"
-        if not readonly:
-            success_message += f"<section id='{int_to_excel_col(match_index + 1)}'>{num_matches_message}\n{match_display}\n</section>\n"
-        else:
-            success_message += f"<readonly_section id='{int_to_excel_col(match_index + 1)}>{num_matches_message}\n{match_display}\n</readonly_section>\n"
-    return success_message
+Here is an example:
+
+<function_call>
+<invoke>
+<tool_name>analyze_problem_and_propose_plan</tool_name>
+<parameters>
+<problem_analysis>The problem analysis goes here</problem_analysis>
+<proposed_plan>The proposed plan goes here</proposed_plan>
+</parameters>
+</invoke>
+</function_call>
 
+If you are really done, call the submit_result function.
+"""
+
+NO_TOOL_CALL_PROMPT_OPENAI = """FAILURE
+No function calls were made or your last function call was incorrectly formatted. The correct syntax for function calling is this:
+
+<function_call>
+<tool_name>
+<parameter1>
+parameter1 value here
+</parameter1>
+<parameter2>
+parameter2 value here
+</parameter2>
+</tool_name>
+</function_call>
+
+Here is an example:
+
+<function_call>
+<make_change>
+<justification>
+The justification for making this change goes here
+</justification>
+<file_name>
+example-file.file
+</file_name>
+<original_code>
+old code line here
+</original_code>
+<new_code>
+new code line here
+</new_code>
+</make_change>
+</function_call>
+
+If you are really done, call the submit_result function.
+"""
+
+tool_call_parameters = {
+    "make_change": ["justification", "file_name", "original_code", "new_code"],
+    "create_file": ["justification", "file_name", "file_path", "contents"],
+    "submit_result": ["justification"],
+}
 
 def english_join(items: list[str]) -> str:
     if len(items) == 0:
         return ""
     if len(items) == 1:
         return items[0]
     if len(items) == 2:
         return f"{items[0]} and {items[1]}"
     return ", ".join(items[:-1]) + f", and {items[-1]}"
 
-def generate_status_message(file_path: str, fcrs: list[FileChangeRequest]) -> str:
-    if not fcrs or len(fcrs) == 1:
-        return f"You will resolve the issue by editing {file_path}."
-    index = -1
-    for i, fcr in enumerate(fcrs):
-        if fcr.filename == file_path:
-            index = i
+def find_best_match(needle: str, haystack: str, threshold: int = 80):
+    best_match = 0
+    best_score = 0
+    threshold = 80
+    file_contents_lines = haystack.split("\n")
+    num_lines = len(file_contents_lines)
+    num_match_lines = len(needle.split("\n"))
+    for start_line in tqdm(range(num_lines), total=num_lines):
+        potential_choices = []
+        for end_line in range(start_line + max(1, num_match_lines - 5), start_line + num_match_lines + 5):
+            if end_line > num_lines:
+                break
+            potential_choice = "\n".join(file_contents_lines[start_line:end_line])
+            potential_choices.append(potential_choice)
+
+        results = process.extractOne(needle, potential_choices, scorer=fuzz.QRatio, score_cutoff=threshold)
+            
+        if results is not None:
+            choice, score, _index = results
+
+            if score > best_score:
+                best_score = score
+                best_match = choice
+    
+    if best_score > threshold:
+        return best_match, best_score
+    return "", 0
+
+MODEL = "claude-3-opus-20240229"
+
+def validate_and_parse_function_call_openai(
+    function_calls_string: str, chat_gpt: ChatGPT
+) -> list[AnthropicFunctionCall]:
+    function_calls = parse_function_calls_for_openai(
+        function_calls_string.strip("\n") + "\n</function_call>"
+    )
+    if len(function_calls) > 0:
+        function_calls[0] = AnthropicFunctionCall(
+            function_name=function_calls[0]['tool'],
+            function_parameters=function_calls[0]['arguments'],
+        )
+        if "<function_call>" in function_calls_string:
+            chat_gpt.messages[-1].content = (
+                chat_gpt.messages[-1].content.rstrip("\n") + "\n</function_call>"
+            )
+    return function_calls[0] if len(function_calls) > 0 else None
+
+
+def validate_and_parse_function_call(
+    function_calls_string: str, chat_gpt: ChatGPT
+) -> list[AnthropicFunctionCall]:
+    function_calls = AnthropicFunctionCall.mock_function_calls_from_string(
+        function_calls_string.strip("\n") + "\n</function_call>"
+    )  # add end tag
+    if len(function_calls) > 0:
+        chat_gpt.messages[-1].content = (
+            chat_gpt.messages[-1].content.rstrip("\n") + "\n</function_call>"
+        )  # add end tag to assistant message
+        return function_calls[0] if len(function_calls) > 0 else None
+
+    # try adding </invoke> tag as well
+    function_calls = AnthropicFunctionCall.mock_function_calls_from_string(
+        function_calls_string.strip("\n") + "\n</invoke>\n</function_call>"
+    )
+    if len(function_calls) > 0:
+        # update state of chat_gpt
+        chat_gpt.messages[-1].content = (
+            chat_gpt.messages[-1].content.rstrip("\n") + "\n</invoke>\n</function_call>"
+        )
+        return function_calls[0] if len(function_calls) > 0 else None
+    # try adding </parameters> tag as well
+    function_calls = AnthropicFunctionCall.mock_function_calls_from_string(
+        function_calls_string.strip("\n")
+        + "\n</parameters>\n</invoke>\n</function_call>"
+    )
+    if len(function_calls) > 0:
+        # update state of chat_gpt
+        chat_gpt.messages[-1].content = (
+            chat_gpt.messages[-1].content.rstrip("\n")
+            + "\n</parameters>\n</invoke>\n</function_call>"
+        )
+    return function_calls[0] if len(function_calls) > 0 else None
+
+def create_user_message(
+        fcrs: list[FileChangeRequest],
+        request: str,
+        cloned_repo: ClonedRepo,
+        relevant_filepaths: list[str] = None,
+        modify_files_dict: dict[str, dict[str, str]] = None
+    ) -> str:
+    current_fcr_index = 0
+    for current_fcr_index, fcr in enumerate(fcrs):
+        if not fcr.is_completed:
             break
-    else:
-        logger.warning(f"Could not find file {file_path} in list of FCRs.")
-        return f"You will resolve the issue by editing {file_path}."
-    message = ""
-    if index > 1:
-        message += f"You have already made changes to {english_join([fcr.filename for fcr in fcrs[:index]])}. "
-    message += f"You will resolve the issue by editing {file_path}. "
-    if index < len(fcrs) - 1:
-        message += f"You will edit the files {english_join([fcr.filename for fcr in fcrs[index + 1:]])} later."
-    return message.strip()
+    combined_request_unformatted = "{relevant_files}# Plan of Code Changes\n\nIn order to solve the user's request you will need to modify or create {files_to_modify_list}.{completed_prompt} Here are the instructions for the edits you need to make:\n\n<files_to_change>\n{files_to_modify}\n</files_to_change>"
+    completed_prompt = "" if current_fcr_index == 0 else f" You have already completed {current_fcr_index} of the {len(fcrs)} required changes."
+    if modify_files_dict:
+        combined_request_unformatted += "\nThe above files reflect the latest updates you have already made. READ THROUGH THEM CAREFULLY TO FIGURE OUT WHAT YOUR NEXT STEPS ARE. Call the make_change, create_file or submit_result tools."
+    files_to_modify_string = ""
 
-# returns formatted response
-def create_tool_call_response(tool_name: str, tool_call_response_contents: str) -> str:
-    return unformatted_tool_call_response.replace("{tool_name}", tool_name).replace("{tool_call_response_contents}", tool_call_response_contents)
+    files_to_modify_messages = {fcr.filename: "" for fcr in fcrs}
+    for i, fcr in enumerate(fcrs):
+        # first add the instructions to the user message
+        if i < current_fcr_index: # already done
+            files_to_modify_messages[fcr.filename] += f"\n\nYou have already {fcr.change_type} {fcr.filename}, where the specific instructions were to:\n\n{fcr.instructions}"
+        elif i == current_fcr_index:
+            files_to_modify_messages[fcr.filename] += f"\n\nYour current task is to {fcr.change_type} {fcr.filename}. The specific instructions to do so are listed below:\n\n{fcr.instructions}"
+        else:
+            files_to_modify_messages[fcr.filename] += f"\n\nYou will later need to {fcr.change_type} {fcr.filename}. The specific instructions to do so are listed below:\n\n{fcr.instructions}"
+        # now add the contents of the file to the user message
+        # only add the contents if this is the last fcr for the filename
+        last_occurence = i
+        # loop from current index to end of fcrs to see if this fcr is the last time the filename shows up
+        for j in range(i + 1, len(fcrs)):
+            if fcrs[j].filename == fcr.filename:
+                last_occurence = j
+        if last_occurence == i:
+            if fcr.change_type == "modify":
+                if not modify_files_dict:
+                    files_to_modify_messages[fcr.filename] += f"\n\n<file_to_modify filename=\"{fcr.filename}\">\n{cloned_repo.get_file_contents(file_path=fcr.filename)}\n</file_to_modify>"
+                else: # show the latest contents of the file
+                    latest_file_contents = get_latest_contents(fcr.filename, cloned_repo, modify_files_dict)
+                    files_to_modify_messages[fcr.filename] += f"\n\n<file_to_modify filename=\"{fcr.filename}\">\n{latest_file_contents}\n</file_to_modify>"
+            elif fcr.change_type == "create":
+                files_to_modify_messages[fcr.filename] += f"\n<file_to_create filename=\"{fcr.filename}\">\n{fcr.instructions}\n</file_to_create>"
+    # now we combine the messages into a single string
+    already_added_files = set([])
+    for fcr in fcrs:
+        if fcr.filename in already_added_files:
+            continue
+        files_to_modify_string += files_to_modify_messages[fcr.filename]
+        already_added_files.add(fcr.filename)
+
+    deduped_file_names = list(set([fcr.filename for fcr in fcrs]))
+    combined_request_message = combined_request_unformatted \
+        .replace("{files_to_modify}", files_to_modify_string.lstrip('\n')) \
+        .replace("{files_to_modify_list}", english_join(deduped_file_names)) \
+        .replace("{completed_prompt}", completed_prompt)
+    if relevant_filepaths:
+        relevant_file_paths_string = ""
+        for relevant_file_path in relevant_filepaths:
+            if relevant_file_path not in cloned_repo.get_file_list():
+                logger.warning(f"Relevant file path {relevant_file_path} not found in cloned repo.")
+                continue
+            if relevant_file_path in [fcr.filename for fcr in fcrs]:
+                logger.warning(f"Relevant file path {relevant_file_path} is already in the list of files to modify.")
+                continue
+            relevant_file_paths_string += f"\n\n<relevant_module filename=\"{relevant_file_path}\">\n{cloned_repo.get_file_contents(file_path=relevant_file_path)}\n</relevant_module>"
+        relevant_file_paths_string = f"<relevant_files>\n{relevant_file_paths_string}\n</relevant_files>"
+        combined_request_message.replace("{relevant_files}", f'\nHere are some relevant modules, such as useful helper functions for resolving this issue. You likely will not need to edit these modules but may need to import them or understand their usage interface: {relevant_file_paths_string}\n')
+    else:
+        combined_request_message.replace("{relevant_files}", "")
+    user_message = f"<user_request>\n{request}\n</user_request>\n{combined_request_message}"
+    return user_message
+
+# find out if any changes were made by matching the contents of the files
+def changes_made(modify_files_dict: dict[str, dict[str, str]], previous_modify_files_dict) -> bool:
+    # check if there are any changes made
+    for file_name, file_data in modify_files_dict.items():
+        if file_name not in previous_modify_files_dict:
+            if file_data['contents'] != file_data["original_contents"]:
+                return True
+            else:
+                continue
+        if file_data['contents'] != previous_modify_files_dict[file_name]['contents']:
+            return True
+    return False
+
+past_tense_mapping = {
+    "modify": "modified",
+    "create": "created",
+}
+
+# Magic
+def ordinal(n: int):
+    return "%d%s" % (n,"tsnrhtdd"[(n//10%10!=1)*(n%10<4)*n%10::4]) # noqa
+
+def render_plan(fcrs: list[FileChangeRequest]) -> str:
+    current_fcr_index = 0
+    for current_fcr_index, fcr in enumerate(fcrs):
+        if not fcr.is_completed:
+            break
+    plan = f"You have {len(fcrs)} changes to make and you are currently working on the {ordinal(current_fcr_index + 1)} task."
+    for i, fcr in enumerate(fcrs):
+        if i < current_fcr_index:
+            plan += f"\n\nTask {i}: You have previously {past_tense_mapping[fcr.change_type]} {fcr.filename}, where you were asked to:\n\n{fcr.instructions}"
+        elif i == current_fcr_index:
+            plan += f"\n\nTask {i}: Your CURRENT TASK is to {fcr.change_type} {fcr.filename}. The specific instructions to do so are listed below:\n\n{fcr.instructions}"
+        else:
+            plan += f"\n\nTask {i}: You will later need to {fcr.change_type} {fcr.filename}. The specific instructions to do so are listed below:\n\n{fcr.instructions}"
+    return plan.strip('\n')
 
-def default_dict_value():
-    return {"chunks": [], "contents": "", "original_contents": ""}
+def render_current_task(fcrs: list[FileChangeRequest]) -> str:
+    current_fcr_index = 0
+    for current_fcr_index, fcr in enumerate(fcrs):
+        if not fcr.is_completed:
+            break
+    fcr = fcrs[current_fcr_index]
+    return f"The CURRENT TASK is to {fcr.change_type} {fcr.filename}. The specific instructions to do so are listed below:\n\n<current_task>\n{fcr.instructions}\n</current_task>"
 
-# returns dictionary of all changes made
-@file_cache(ignore_params=["file_path", "chat_logger", "cloned_repo", "assistant_id", "ticket_progress", "assistant_conversation", "cwd"])
-def function_modify(
+def modify(
+    fcrs: list[FileChangeRequest],
     request: str,
-    file_path: str,
-    contents_of_file: str,
     cloned_repo: ClonedRepo,
-    additional_messages: list[Message] = [],
+    relevant_filepaths: list[str],
     chat_logger: ChatLogger | None = None,
-    assistant_id: str = None,
-    ticket_progress: TicketProgress | None = None,
-    assistant_conversation: AssistantConversation | None = None,
-    seed: int = None,
-    relevant_filepaths: list[str] = [],
-    cwd: str | None = None,
-    fcrs: list[FileChangeRequest]=[],
-    previous_modify_files_dict: dict[str, dict[str, str | list[str]]] = None,
-) -> dict[str, dict[str, str | list[str]]] | None:
+    use_openai: bool = False,
+) -> dict[str, dict[str, str]]:
+    # join fcr in case of duplicates
+    user_message = create_user_message(
+        fcrs=fcrs,
+        request=request,
+        cloned_repo=cloned_repo,
+        relevant_filepaths=relevant_filepaths,
+    )
+    chat_gpt = ChatGPT()
+    full_instructions = instructions + (modify_tools_openai if use_openai else modify_tools)
+    chat_gpt.messages = [Message(role="system", content=full_instructions)]
     try:
-        logger.info("Starting function_modify_unstable")
-        def save_ticket_progress(assistant_id: str, thread_id: str, run_id: str):
-            if assistant_conversation:
-                assistant_conversation.update_from_ids(
-                    assistant_id=assistant_id, run_id=run_id, thread_id=thread_id
-                )
-            ticket_progress.save()
-        # dictionary mapping a file path to various data used in modify, this needs to be stateful, so it is possible that previous_modify_files_dict
-        modify_files_dict = previous_modify_files_dict or defaultdict(default_dict_value)
-        cwd = cwd or cloned_repo.repo_dir
-        current_contents = contents_of_file
-        initial_check_results = get_check_results(file_path, current_contents)
-        # save chunks and contents of file if its not already present
-        if file_path not in modify_files_dict:
-            original_snippets = chunk_code(current_contents, file_path, 1400, 500)
-            file_contents_lines = current_contents.split("\n")
-            chunks = [
-                "\n".join(file_contents_lines[max(snippet.start - 1, 0) : snippet.end])
-                for snippet in original_snippets
-            ]
-            modify_files_dict[file_path] = {"chunks": copy.deepcopy(chunks), "contents": current_contents, "original_contents": current_contents}
-        sweep_config: SweepConfig = SweepConfig()
-        chunked_file_contents = "\n".join(
-            [
-                f'<section id="{int_to_excel_col(i + 1)}">\n{chunk}\n</section id="{int_to_excel_col(i + 1)}>'
-                for i, chunk in enumerate(modify_files_dict[file_path]["chunks"])
-            ]
+        function_calls_string = chat_gpt.chat_anthropic(
+            content=f"Here is the intial user request, plan, and state of the code files:\n{user_message}",
+            stop_sequences=["</function_call>"],
+            model=MODEL,
+            message_key="user_request",
+            use_openai=use_openai,
         )
-        current_file_to_modify_contents = f"<current_file_to_modify filename=\"{file_path}\">\n{chunked_file_contents}\n</current_file_to_modify>"
-        fcrs_message = generate_status_message(file_path, fcrs)
-        relevant_file_paths_string = ", ". join(relevant_filepaths) 
-        new_additional_messages = [
-            Message(
-                role="user",
-                content=f"# Request\n{request}\n\n{fcrs_message}",
-            ),
-            Message(
-                role="user",
-                content=current_file_to_modify_contents,
-            ),
-        ]
-        if relevant_file_paths_string:
-            new_additional_messages.append(Message(
-                role="user",
-                content=f'You should view the following relevant files: {relevant_file_paths_string}'
-            ))
-        additional_messages = new_additional_messages + additional_messages
-        # add any already made changes to the additional_messages
-        for file_path, file_data in modify_files_dict.items():
-            diff = generate_diff(file_data["original_contents"], file_data["contents"])
-            if diff:
-                additional_messages.append(
-                    Message(
-                        role="user",
-                        content=f"The following changes in {file_path} have already been applied in an attempt to address this problem:\n```\n"
-                        + diff
-                        + "\n```",
-                    )
+    except Exception as e:
+        logger.error(f"Error in chat_anthropic: {e}")
+        chat_logger.add_chat(
+            {
+                "model": chat_gpt.model,
+                "messages": [{"role": message.role, "content": message.content} for message in chat_gpt.messages],
+                "output": f"ERROR:\n{e}\nEND OF ERROR",
+            })
+        return {}
+    modify_files_dict = {}
+    llm_state = {
+        "initial_check_results": {},
+        "done_counter": 0,
+        "request": request,
+        "plan": render_plan(fcrs), 
+        "current_task": render_current_task(fcrs),
+        "user_message_index": 1,
+        "user_message_index_chat_logger": 1,
+        "fcrs": fcrs,
+        "previous_attempt": "",
+    }
+    # this message list is for the chat logger to have a detailed insight into why failures occur
+    detailed_chat_logger_messages = [{"role": message.role, "content": message.content} for message in chat_gpt.messages]
+    # used to determine if changes were made
+    previous_modify_files_dict = copy.deepcopy(modify_files_dict)
+    for i in range(len(fcrs) * 15):
+        if use_openai:
+            function_call = validate_and_parse_function_call_openai(function_calls_string, chat_gpt)
+        else:
+            function_call = validate_and_parse_function_call(function_calls_string, chat_gpt)
+        if function_call:
+            # note that detailed_chat_logger_messages is meant to be modified in place by handle_function_call
+            function_output, modify_files_dict, llm_state = handle_function_call(cloned_repo, function_call, modify_files_dict, llm_state, chat_logger_messages=detailed_chat_logger_messages, use_openai=use_openai)
+            if function_output == "DONE":
+                # add the diff of all changes to chat_logger
+                if chat_logger:
+                    final_message = "DONE\nHere is a summary of all the files changed:\n\n"
+                    for file_name, file_data in modify_files_dict.items():
+                        file_diff = generate_diff(file_data['original_contents'], file_data['contents'])
+                        if file_diff:
+                            final_message += f"\nChanges made to {file_name}:\n{file_diff}"
+                    chat_logger.add_chat({
+                        "model": chat_gpt.model,
+                        "messages": detailed_chat_logger_messages,
+                        "output": f"{final_message}",
+                    })
+                break
+            detailed_chat_logger_messages.append({"role": "user", "content": function_output})
+
+            if modify_files_dict: # update the state of the LLM
+                user_message = create_user_message(
+                    fcrs=fcrs,
+                    request=request,
+                    cloned_repo=cloned_repo,
+                    relevant_filepaths=relevant_filepaths,
+                    modify_files_dict=modify_files_dict
                 )
-        assistant_generator = openai_assistant_call(
-            request="",  # already present in additional_messages
-            instructions=instructions,
-            additional_messages=ensure_additional_messages_length(additional_messages),
-            chat_logger=chat_logger,
-            assistant_id=assistant_id,
-            save_ticket_progress=(
-                save_ticket_progress if ticket_progress is not None else None
-            ),
-            assistant_name="Code Modification Function Assistant",
-            tools=[],
-        )
-
+                user_message = f"Here is the UPDATED user request, plan, and state of the code changes. REVIEW THIS CAREFULLY!\n{user_message}"
+                
+                # update context if a change was made
+                if changes_made(modify_files_dict, previous_modify_files_dict):
+                    # remove the previous user message and add it to the end, do not remove if it is the inital user message
+                    if llm_state["user_message_index"] != 1:
+                        chat_gpt.messages.pop(llm_state["user_message_index"])
+                    if llm_state["user_message_index_chat_logger"] != 1:
+                        detailed_chat_logger_messages.pop(llm_state["user_message_index_chat_logger"])
+                    chat_gpt.messages.append(Message(role="user", content=user_message))
+                    detailed_chat_logger_messages.append({"role": "user", "content": user_message})
+                    # update the index
+                    llm_state["user_message_index"] = len(chat_gpt.messages) - 1
+                    llm_state["user_message_index_chat_logger"] = len(detailed_chat_logger_messages) - 1
+                previous_modify_files_dict = copy.deepcopy(modify_files_dict)
+        else:
+            function_output = "FAILURE: No function calls were made or your last function call was incorrectly formatted. The correct syntax for function calling is this:\n" \
+                + "<function_call>\n<invoke>\n<tool_name>tool_name</tool_name>\n<parameters>\n<param_name>param_value</param_name>\n</parameters>\n</invoke>\n</function_call>"
+        if chat_logger:
+            if i == len(fcrs) * 10 - 1:
+                chat_logger.add_chat(
+                    {
+                        "model": chat_gpt.model,
+                        "messages": detailed_chat_logger_messages,
+                        "output": f"WARNING We have reached the end the max amount of iterations: {i + 1}, but we have not finished with our changes yet!",
+                    })
+            else:
+                chat_logger.add_chat(
+                    {
+                        "model": chat_gpt.model,
+                        "messages": detailed_chat_logger_messages,
+                        "output": detailed_chat_logger_messages[-1]["content"],
+                    })
         try:
-            done_counter = 0
-            tool_name, tool_call = assistant_generator.send(None)
-            for i in range(100):  # TODO: tune this parameter
-                print(tool_name, json.dumps(tool_call, indent=2))
-                if tool_name == "done":
-                    changes_made = False
-                    # iterate through modify_files_dict and generate diffs
-                    diffs_made = defaultdict(str)
-                    for file_name, file_data in modify_files_dict.items():
-                        new_contents = file_data["contents"]
-                        original_contents = file_data["original_contents"]
-                        diff = generate_diff(original_contents, new_contents)
-                        if diff:
-                            changes_made = True
-                            diffs_made[file_name] = diff
+            function_calls_string = chat_gpt.chat_anthropic(
+                content=function_output,
+                model=MODEL,
+                stop_sequences=["</function_call>"],
+                use_openai=use_openai,
+            )
+            detailed_chat_logger_messages.append({"role": "assistant", "content": function_calls_string})
+        except Exception as e:
+            logger.error(f"Error in chat_anthropic: {e}")
+            chat_logger.add_chat(
+                {
+                    "model": chat_gpt.model,
+                    "messages": detailed_chat_logger_messages,
+                    "output": f"ERROR: AN ERROR OCCURED ON ITERATION {i + 1}:\n{e}\nEND OF ERROR",
+                })
+            break
+    # before we return clean up modify files dict by removing any files with no changes
+    files_to_remove = []
+    for file_name, file_data in modify_files_dict.items():
+        if not file_data or file_data['original_contents'] == file_data['contents']:
+            files_to_remove.append(file_name)
+    for file_name in files_to_remove:
+        modify_files_dict.pop(file_name)
+        logger.info(f"Removed file {file_name} from modify_files_dict as it had no changes.")
+    return modify_files_dict
+
+
+def generate_diffs(modify_files_dict: dict[str, dict[str, str]]) -> dict[str, str]:
+    changes_made = False
+    for file_name, file_data in modify_files_dict.items():
+        new_contents = file_data["contents"]
+        original_contents = file_data["original_contents"]
+        diff = generate_diff(original_contents, new_contents)
+        if diff:
+            changes_made = True
+    return changes_made
 
-                    if changes_made:
-                        break
-                    else:
-                        done_counter += 1
-                        if done_counter >= 3:
-                            break
-                        error_message = create_tool_call_response("submit_result", "ERROR\n\nNo changes were made. Please continue working on your task.")
-                        tool_name, tool_call = assistant_generator.send(
-                            error_message
-                        )                  
-                elif tool_name == "no_tool_call":
-                    error_message = ""
-                    tool_name, tool_call = assistant_generator.send(
-                        "ERROR\n No tool calls were made. If you are done, please use the submit_result tool to indicate that you have completed the task. If you believe you are stuck, use the search_codebase tool to further explore the codebase or get additional context if necessary."
-                    )
-                elif tool_name == "analyze_problem_and_propose_plan":
-                    error_message = ""
-                    success_message = create_tool_call_response(tool_name, "SUCCESS\n\nSounds like a great plan! Let's get started.")
-                    tool_name, tool_call = assistant_generator.send(
-                        success_message
-                    )
-                elif tool_name == "analyze_and_identify_changes":
-                    error_message = ""
-                    # make sure the change is for an existing or newly created file
-                    if "file_name" not in tool_call:
-                        error_message = "Missing file_name in tool call. Call the tool again but this time provide the file_name."
-                    if not error_message:
-                        file_name = tool_call["file_name"].strip()
-                        if not os.path.exists(os.path.join(cwd, file_name)) and file_name not in modify_files_dict:
-                            error_message = f"The file {file_name} does not exist. Make sure that you have spelled the file name correctly!"
-                    if not error_message:
-                        success_message = create_tool_call_response(tool_name, "SUCCESS\n\nNice work! Now use the make_change tool to make the listed changes one at a time. If there are multiple changes required, call the make_change tool multiple times.")
-                        tool_name, tool_call = assistant_generator.send(
-                            success_message
-                        )
-                    else:
-                        error_message = create_tool_call_response(tool_name, f"ERROR\n\n{error_message}")
-                        tool_name, tool_call = assistant_generator.send(
-                            error_message
-                        )
-                elif tool_name == "view_file":
-                    error_message = ""
+def create_tool_call_response(tool_name: str, tool_call_response_contents: str) -> str:
+    return f"<function_results>\n<result>\n<tool_name>{tool_name}<tool_name>\n<stdout>\n{tool_call_response_contents}\n</stdout>\n</result>\n</function_results>"
+
+def get_latest_contents(file_name: str, cloned_repo: ClonedRepo, modify_files_dict: dict) -> str:
+    if file_name in modify_files_dict and "contents" in modify_files_dict[file_name]:
+        return modify_files_dict[file_name]["contents"]
+    elif file_name in cloned_repo.get_file_list():
+        return cloned_repo.get_file_contents(file_name)
+    else:
+        return ""
+
+def handle_function_call(
+    cloned_repo: ClonedRepo,
+    function_call: AnthropicFunctionCall,
+    modify_files_dict: dict[str, dict[str, str]],
+    llm_state: dict,
+    chat_logger_messages: list[dict[str, str]] | None = None,
+    use_openai: bool = False,
+) :
+    # iterate through modify_files_dict and generate diffs
+    llm_response = ""
+    tool_name = function_call.function_name
+    tool_call = function_call.function_parameters
+    if tool_name == "submit_result":
+        changes_made = False
+        changes_made = generate_diffs(modify_files_dict)
+        if changes_made:
+            llm_response = "DONE"
+        else:
+            llm_state["done_counter"] += 1
+            if llm_state["done_counter"] > 3:
+                llm_response = "DONE"
+            else:
+                llm_response = "ERROR\n\nNo changes were made. Please continue working on your task."
+    elif tool_name == "no_tool_call":
+        if use_openai:
+            llm_response = NO_TOOL_CALL_PROMPT_OPENAI
+        else:
+            llm_response = NO_TOOL_CALL_PROMPT
+    elif tool_name == "make_change":
+        error_message = ""
+        for key in ["file_name", "original_code", "new_code"]:
+            if key not in tool_call:
+                error_message += f"Missing {key} in tool call. Call the tool again but this time provide the {key}.\n"
+                if key == "new_code" or key == "original_code":
+                    error_message += "\n\nIt is likely the reason why you have missed these keys is because the original_code block you provided is WAY TOO LARGE and as such you have missed the closing xml tags. REDUCE the original_code block to be under 10 lines of code!"
+        warning_message = ""
+        if not error_message:
+            for _ in range(1): # this is super jank code but it works for now - only for easier error message handling
+                # ensure the file we are editting exists and is in modify_files_dict
+                if "file_name" in tool_call:
                     file_name = tool_call["file_name"].strip()
-                    full_file_name = os.path.join(cwd, file_name)
-                    # not in code base and not created
-                    if not os.path.exists(full_file_name) and file_name not in modify_files_dict:
-                        similar_file_paths = "\n".join(
-                            [
-                                f"- {path}"
-                                for path in cloned_repo.get_similar_file_paths(
-                                    file_name
-                                )
-                            ]
-                        )
-                        error_message = f"The file {file_name} does not exists. {'Did you mean one of the following files?' if similar_file_paths else ''}\n{similar_file_paths}"
-                    if not error_message:
-                        # if this is the first time viewing this file
-                        if file_name not in modify_files_dict:
-                            try:
-                                file_contents = read_file_with_fallback_encodings(full_file_name)
-                            except Exception as e:
-                                error_message = f"Error occured while attempting to read the file {file_name}: {e}"
-                            if not error_message:
-                                # chunk the file
-                                file_original_snippets = chunk_code(file_contents, file_name, 1400, 500)
-                                view_file_contents_lines = file_contents.split("\n")
-                                file_chunks = [
-                                    "\n".join(view_file_contents_lines[max(snippet.start - 1, 0) : snippet.end])
-                                    for snippet in file_original_snippets
-                                ]
-                                # update chunks for this file inside modify_files_dict unless it already exists
-                                modify_files_dict[file_name] = {"chunks": copy.deepcopy(file_chunks), "contents": file_contents, "original_contents": file_contents}
-                                chunked_file_contents = ""
-                                for i, chunk in enumerate(file_chunks):
-                                    idx = int_to_excel_col(i + 1)
-                                    chunked_file_contents += f'\n<section id="{idx}">\n{chunk}\n</section id="{idx}">'
-                        else:
-                            # filename already exists in modify_files_dict, implies edits were made to it
-                            chunked_file_contents = "\n".join(
-                                [
-                                    f'<section id="{int_to_excel_col(i + 1)}">\n{chunk}\n</section id="{int_to_excel_col(i + 1)}>'
-                                    for i, chunk in enumerate(modify_files_dict[file_name]["chunks"])
-                                ]
-                            )
-                        logger.debug(f'SUCCESS\n\nHere is the file:\n\n<file filename="{file_name}">\n{chunked_file_contents}\n</file filename="{file_name}">')
-                        success_message = create_tool_call_response(tool_name, f'SUCCESS\n\nHere is the file:\n\n<file filename="{file_name}">\n{chunked_file_contents}\n</file filename="{file_name}">')
-                        tool_name, tool_call = assistant_generator.send(
-                            success_message
-                        )
-                    if error_message:
-                        logger.debug(f"ERROR in ViewFile\n\n{error_message}")
-                        error_message = create_tool_call_response(tool_name, f"ERROR\n\n{error_message}")
-                        tool_name, tool_call = assistant_generator.send(
-                            error_message
-                        )
-                elif tool_name == "make_change":
-                    error_message = ""
-                    for key in ["file_name", "section_id", "original_code", "new_code"]:
-                        if key not in tool_call:
-                            error_message += f"Missing {key} in tool call.Call the tool again but this time provide the {key}.\n"
-                    for _ in range(1): # this is super jank code but it works for now - only for easier error message handling
-                        # ensure the file we are editting exists and is in modify_files_dict
-                        if "file_name" in tool_call:
-                            file_name = tool_call["file_name"].strip()
-                            # if not in codebase or has not been created
-                            if not os.path.exists(os.path.join(cwd, file_name)) and file_name not in modify_files_dict:
-                                error_message += f"The file {file_name} does not exist. Make sure that you have spelled the file name correctly!\n"
-                            if file_name not in modify_files_dict:
-                                error_message += f"You have not viewed {file_name} yet! Are you CERTAIN this is the file you want to modify? If so, view the file first with the view_file tool and then call the make_change tool again.\n"
-                        if error_message:
-                            break
-                        success_message = ""
-                        section_letter = tool_call["section_id"].strip()
-                        section_id = excel_col_to_int(section_letter)
-                        original_code = tool_call["original_code"].strip("\n")
-                        new_code = tool_call["new_code"].strip("\n")
-                        if new_code == original_code:
-                            error_message += "The new_code and original_code are the same. Are you CERTAIN this change needs to be made? If you are certain this change needs to be made, MAKE SURE that the new_code and original_code are NOT the same."
-                            break
-                        # get the chunks and contents for the file
-                        file_chunks = deepcopy(modify_files_dict[file_name]['chunks'])  
-                        file_contents = modify_files_dict[file_name]['contents']
-                        warning_message = ""
-                        if section_id >= len(file_chunks):
-                            error_message = f"Could not find section {section_letter} in file {file_name}, which has {len(file_chunks)} sections."
-                            break
-                        elif section_id < 0:
-                            error_message = f"The section id {section_letter} can not be parsed."
-                            break
-
-                        # fetch the chunk of code we will be modifying
-                        try:
-                            current_chunk = file_chunks[section_id]
-                        except Exception:
-                            error_message = f"Could not fetch the chunk of code for section {section_letter} in file {file_name}. Make sure you are modifying the correct file: {file_name}"
-                            break
-                        
-                        # handle special case where there are \r\n characters in the current chunk as this will cause search and replace to ALWAYS fail
-                        carriage_return = False
-                        if "\r\n" in current_chunk:
-                            # replace in current chunk
-                            previous_chunk = current_chunk
-                            current_chunk = current_chunk.replace("\r\n", "\n")
-                            carriage_return = True
-                        # check to see that the original_code is in the new_code by trying all possible indentations
-                        correct_indent, rstrip_original_code = manual_code_check(current_chunk, original_code)
-                        # if the original_code couldn't be found in the chunk we need to let the llm know
-                        if original_code not in current_chunk and correct_indent == -1:
-                            chunks_with_original_code = [
-                                index
-                                for index, chunk in enumerate(file_chunks)
-                                if original_code in chunk.replace("\r\n", "\n") or manual_code_check(chunk.replace("\r\n", "\n"), original_code)[0] != -1
-                            ]
-                            chunks_with_original_code = chunks_with_original_code[:5]
-
-                            error_message = f"The original_code provided does not appear to be present in section {section_letter}. The original_code contains:\n```\n{original_code}\n```\nBut section {section_letter} in {file_name} has code:\n```\n{current_chunk}\n```"
-                            if chunks_with_original_code:
-                                error_message += "\n\nDid you mean one of the following sections?"
-                                error_message += "\n".join(
-                                    [
-                                        f'\n<section id="{int_to_excel_col(index + 1)}">\n{file_chunks[index]}\n</section>\n```'
-                                        for index in chunks_with_original_code
-                                    ]
-                                )
-                            else:
-                                # first check the lines in original_code, if it is too long, ask for smaller changes
-                                original_code_lines_length = len(original_code.split("\n"))
-                                if original_code_lines_length > 7:
-                                    error_message += f"\n\nThe original_code seems to be quite long with {original_code_lines_length} lines of code. Break this large change up into a series of SMALLER changes to avoid errors like these! Try to make sure the original_code is under 7 lines."
-                                else:
-                                    # generate the diff between the original code and the current chunk to help the llm identify what it messed up
-                                    chunk_original_code_diff = generate_diff(original_code, current_chunk)
-                                    error_message += f"\n\nHere is the diff between the original_code you provided and what is actually in section {section_letter}:\n\n{chunk_original_code_diff}\n\nIdentify what should be the correct original_code should be, and make another replacement with the corrected original_code."
-                            break
-                        # ensure original_code and new_code has the correct indents
-                        new_code_lines = new_code.split("\n")
-                        new_code = "\n".join(f'{correct_indent*" "}{line}' for line in new_code_lines)
-                        if rstrip_original_code:
-                            original_code_lines = [line.rstrip() for line in original_code.split("\n")]
-                        else:
-                            original_code_lines = original_code.split("\n")
-                        original_code = "\n".join(f'{correct_indent*" "}{line}' for line in original_code_lines)
-                        # before we apply changes make sure original_code is unique inside current_chunk
-                        current_chunk_occurences = current_chunk.count(original_code)
-                        if current_chunk_occurences > 1:
-                            error_message = f"The original_code is not unique in the section {section_letter}. It appears {current_chunk_occurences} times! Make sure the original_code is unique in section {section_letter}!"
-                            break
-
-                        # apply changes
-                        new_chunk = current_chunk.replace(original_code, new_code, 1)
-                        if new_chunk == current_chunk:
-                            logger.warning("No changes were made to the code.")
-                        
-                        file_chunks[section_id] = new_chunk
-                        # if we had carriage returns, we need to update file_contents to remove them also from current_chunk
-                        if carriage_return:
-                            file_contents = file_contents.replace(previous_chunk, current_chunk, 1)
-                        new_contents = file_contents.replace(
-                            current_chunk, new_chunk, 1
-                        )
-
-                        # Check if changes were made
-                        if new_contents == file_contents:
-                            logger.warning("No changes were made to the code.")
-                            error_message = "No changes were made, make sure original_code and new_code are not the same."
-                            break
-                        
-                        # Check if the changes are valid
-                        if not error_message:
-                            check_results = get_check_results(file_name, new_contents) # the filename may be wrong here
-                            # check_results_message = check_results.is_worse_than_message(initial_check_results) - currently unused
-                            failing_parse = check_results.parse_error_message if not initial_check_results.parse_error_message else ""
-                            current_diff = generate_diff(
-                                file_contents, new_contents
-                            )
-                            if failing_parse:
-                                error_message = f"Error: Invalid code changes have been applied. You requested the following changes:\n\n```diff\n{current_diff}\n```\n\nBut it produces invalid code.\nFirst, identify where the broken code occurs, why it is broken and what the correct change should be. Then, retry the make_change tool with different changes that yield valid code."
-                                break
-                    if error_message:
-                        logger.error(f"ERROR occured in make_change tool: {error_message}")
-                        error_message = create_tool_call_response(tool_name, f"ERROR\n\n{error_message}")
-                        tool_name, tool_call = assistant_generator.send(
-                            error_message
-                        )
-
-                    if not error_message:
-                        success_message = (
-                            f"SUCCESS\n\nThe following changes have been applied to {file_name}:\n\n"
-                            + generate_diff(file_contents, new_contents)
-                        ) + f"{warning_message}\n\nYou can continue to make changes to the code sections and call the make_change tool again, or go back to searching for keywords using the search_codebase tool, which is great for finding all definitions or usages of a function or class."
-                        # set contents
-                        modify_files_dict[file_name]['contents'] = new_contents
-                        modify_files_dict[file_name]['chunks'] = file_chunks
-                        logger.info(success_message)
-
-                        success_message = create_tool_call_response(tool_name, f"SUCCESS\n\n{success_message}")
-                        
-                        tool_name, tool_call = assistant_generator.send(
-                            success_message
-                        )
-                elif tool_name == "create_file":
-                    error_message = ""
-                    success_message = ""
-                    for key in tool_call_parameters[tool_name]:
-                        if key not in tool_call:
-                            logger.debug(f"No {key} was provided in the {tool_name} tool call. Call the tool again but this time provide the {key}.")
-                            error_message += f"No {key} was provided in the {tool_name} tool call. Call the tool again but this time provide the {key}.\n"
-                    if not error_message:
-                        new_file_path = tool_call["file_path"].strip()
-                        new_file_name = tool_call["file_name"].strip()
-                        new_file_contents = tool_call["contents"].strip()
-                        new_file_dir = os.path.join(cwd, new_file_path)
-                        new_full_file_path = os.path.join(new_file_path, new_file_name)
-                        new_full_file_path_with_cwd = os.path.join(cwd, new_file_path, new_file_name)
-                        # ensure file doesn't already exist
-                        if os.path.exists(new_full_file_path_with_cwd):
-                            error_message = f"The file {new_full_file_path} already exists. Modify this existing file instead of attempting to create a new one!"
-                        # ensure directory is valid
-                        if not os.path.isdir(new_file_dir):
-                            error_message = f"The directory {new_file_path} is not valid. Make sure you have the correct directory path!"
-                        # ensure that the directory of the new full path exists, in case the file name is weird
-                        if not os.path.exists(os.path.dirname(new_full_file_path_with_cwd)):
-                            error_message = f"The directory {os.path.dirname(new_full_file_path)} does not exist. Make sure you the new file you want to create exists within an existing directory!"
-                        # if no issues, create the file by placing it in modify_files_dict
-                        if not error_message:
-                            new_file_snippets = chunk_code(new_file_contents, new_full_file_path, 1400, 500)
-                            new_file_contents_lines = new_file_contents.split("\n")
-                            new_file_chunks = [
-                                "\n".join(new_file_contents_lines[max(snippet.start - 1, 0) : snippet.end])
-                                for snippet in new_file_snippets
-                            ]
-                            modify_files_dict[new_full_file_path] = {"chunks": new_file_chunks, "contents": new_file_contents, "original_contents": new_file_contents}
-                            success_message = f"The new file {new_full_file_path} has been created successfully with the following contents:\n\n{new_file_contents}"
-                    if error_message:
-                        logger.debug(f"ERROR occured in create_file tool: {error_message}")
-                        error_message = create_tool_call_response(tool_name, f"ERROR\n\n{error_message}")
-                        tool_name, tool_call = assistant_generator.send(
-                            error_message
-                        )
+                    # if not in codebase or has not been created
+                    if not os.path.exists(os.path.join(cloned_repo.repo_dir, file_name)) and file_name not in modify_files_dict:
+                        error_message += f"The file {file_name} does not exist. Make sure that you have spelled the file name correctly!\n"
+                        break
+                llm_state['initial_check_results'][file_name] = get_check_results(file_name, get_latest_contents(file_name, cloned_repo, modify_files_dict))
+                success_message = ""
+                original_code = tool_call["original_code"].strip("\n")
+                new_code = tool_call["new_code"].strip("\n")
+                if new_code == original_code:
+                    error_message += "The new_code and original_code are the same. Are you CERTAIN this change needs to be made? If you are certain this change needs to be made, MAKE SURE that the new_code and original_code are NOT the same."
+                    break
+                if not original_code:
+                    error_message = "The original_code is empty. Make sure that the original_code is not empty and that it is a valid section of code that you are trying to replace."
+                # get the latest contents of the file
+                file_contents = get_latest_contents(file_name, cloned_repo, modify_files_dict)
+                warning_message = ""
+                
+                # handle special case where there are \r\n characters in the current chunk as this will cause search and replace to ALWAYS fail
+                if "\r\n" in file_contents:
+                    # replace in current chunk
+                    file_contents = file_contents.replace("\r\n", "\n")
+                # check to see that the original_code is in the new_code by trying all possible indentations
+                correct_indent, rstrip_original_code = manual_code_check(file_contents, original_code)
+                # if the original_code couldn't be found in the chunk we need to let the llm know
+                if original_code not in file_contents and correct_indent == -1:
+                    # TODO: add weighted ratio to the choices, penalize whitespace less
+                    best_match, best_score = find_best_match(original_code, file_contents)
+
+                    if best_score > 80:
+                        error_message = f"The original_code provided does not appear to be present in file {file_name}. The original_code contains:\n```\n{tool_call['original_code']}\n```\nDid you mean the following?\n```\n{best_match}\n```\nHere is the diff:\n```\n{generate_diff(tool_call['original_code'], best_match)}\n```"
                     else:
-                        logger.debug(f"SUCCESS\n\n{success_message}")
-                        success_message = create_tool_call_response(tool_name, f"SUCCESS\n\n{success_message}")
-                        tool_name, tool_call = assistant_generator.send(
-                            success_message
-                        )
-                elif tool_name == "search_codebase":
-                    error_message = ""
-                    success_message = ""
-                    for key in ["keyword"]:
-                        if key not in tool_call:
-                            logger.debug(f"No {key} was provided in the search_codebase tool call. Call the tool again but this time provide the {key}.")
-                            error_message += f"No {key} was provided in the search_codebase tool call. Call the tool again but this time provide the {key}.\n"
-
-                    file_name = ""
-                    if "file_name" in tool_call:
-                        file_name = tool_call["file_name"].strip()
-                        # see if we are searching the whole codebase or not
-                        if file_name: # search specific file
-                            full_file_path = os.path.join(cwd, file_name)
-                            # not in codebase and also not a newly created file
-                            if not os.path.exists(full_file_path) and file_name not in modify_files_dict:
-                                logger.debug(f"The file {file_name} does not exist. Make sure that you have spelled the file name correctly!")
-                                error_message = f"The file {file_name} does not exist. Make sure that you have spelled the file name correctly!"
-                            
-                    # if no issues continue with search
-                    if not error_message:
-                        keyword = tool_call["keyword"].strip()
-                        # search specific file
-                        if file_name:
-                            logger.info(f"Searching for keyword {keyword} in file {file_name}")
-                            match_indices = []
-                            match_context_indices = []
-                            # if the current code file is not in the modify_files_dict, add it
-                            if file_name not in modify_files_dict:
-                                file_contents = read_file_with_fallback_encodings(full_file_path)
-                                file_contents_lines = file_contents.split("\n")
-                                original_file_snippets = chunk_code(file_contents, file_name, 1400, 500)
-                                file_chunks = [
-                                    "\n".join(file_contents_lines[max(snippet.start - 1, 0) : snippet.end])
-                                    for snippet in original_file_snippets
-                                ]
-                                modify_files_dict[file_name] = {"chunks": copy.deepcopy(file_chunks), "contents": file_contents, "original_contents": file_contents}
-                            # search current code file
-                            file_chunks = modify_files_dict[file_name]["chunks"]
-                            for i, chunk in enumerate(file_chunks):
-                                if keyword in chunk:
-                                    match_indices.append(i)
-                                    match_context_indices.append(max(0, i - 1))
-                                    match_context_indices.append(i)
-                                    match_context_indices.append(min(len(file_chunks) - 1, i + 1))
-
-                            match_indices = sorted(list(set(match_indices)))
-                            match_context_indices = sorted(list(set(match_context_indices)))
-                            if not match_indices:
-                                logger.debug(f"The keyword {keyword} does not appear to be present in the file: {file_name}. Consider missing or misplaced whitespace, comments or delimiters in the keyword.")
-                                error_message = f"The keyword {keyword} does not appear to be present in the file: {file_name}. Consider missing or misplaced whitespace, comments or delimiters in the keyword."
-                            else:
-                                # for matches inside current code file
-                                sections_message = english_join(
-                                    [
-                                        int_to_excel_col(match_index + 1)
-                                        for match_index in match_indices
-                                    ]
-                                )
-                                starter_message = f"The keyword {keyword} was found in section(s) {sections_message} of {file_name}. They appear in the following places:\n\n"
-                                success_message += (
-                                    build_keyword_search_match_results(
-                                        match_indices,
-                                        file_chunks,
-                                        keyword,
-                                        starter_message,
-                                        readonly=True
-                                    )
-                                )
-                        else: # search whole codebase
-                            logger.info(f"Searching for keyword {keyword} in the entire codebase.")
-                            rg_command = ["rg", "-n", "-i" , f'"{keyword}"', cwd]
-                            try:
-                                # update the cloned repo before running ripgrep as it is possible some of the files have been editted
-                                for file_name, file_data in modify_files_dict.items():
-                                    updated = update_file(cloned_repo.repo_dir, file_name, file_data["contents"])
-                                    if not updated:
-                                        raise Exception(f"Failed to update file {file_name} in the cloned repo.")
-                            except Exception as e:
-                                logger.error(f"FAILURE: An Error occured while trying to update the cloned repo on file {file_name}: {e}")
-                                error_message = f"FAILURE: An Error occured while trying to update the cloned repo on file {file_name}: {e}\n"
-                                # attempt to undo the updates
-                                for file_name, file_data in modify_files_dict.items():
-                                    update_file(cloned_repo.repo_dir, file_name, file_data["original_contents"])
-                                
-                            try:
-                                result = subprocess.run(" ".join(rg_command), text=True, shell=True, capture_output=True)
-                                output = result.stdout
-                                if output:
-                                    # post process rip grep output to be more condensed
-                                    rg_output_pretty = post_process_rg_output(cwd, sweep_config, output)
-                                else:
-                                    error_message += f"FAILURE: No results found for keyword: {keyword} in the entire codebase. Please try a new keyword. If you are searching for a function definition try again with different whitespaces.\n"
-                            except Exception as e:
-                                logger.error(f"FAILURE: An Error occured while trying to reset the cloned repo on file {file_name}: {e}\n")
-                                error_message += f"FAILURE: An Error occured while trying to rest the cloned repo on file {file_name}: {e}\n"
-
-                            try:
-                                # reset cloned_repo to original state
-                                for file_name, file_data in modify_files_dict.items():
-                                    updated = update_file(cloned_repo.repo_dir, file_name, file_data["original_contents"])
-                                    if not updated:
-                                        raise Exception(f"Failed to update file {file_name} in the cloned repo.")
-                            except Exception as e:
-                                logger.error(f"FAILURE: An Error occured while trying to update the cloned repo on file {file_name}: {e}")
-                                error_message = f"FAILURE: An Error occured while trying to update the cloned repo on file {file_name}: {e}"
-
-                            if not error_message:
-                                success_message = f"Here are the search_codebase results:\n{rg_output_pretty}\n\n You can use these results to revise your plan by calling the analyze_problem_and_propose_plan tool again. You can also call the analyze_and_identify_changes tool again."
-                                logger.debug(f"SUCCESS\n\nHere are the search_codebase results:\n{rg_output_pretty}\n\n")
-
-                    if error_message:
-                        logger.debug(f"ERROR in search_codebase\n\n{error_message}")
-                        error_message = create_tool_call_response(tool_name, f"ERROR\n\n{error_message}")
-                        tool_name, tool_call = assistant_generator.send(
-                            error_message
-                        )
+                        error_message = f"The original_code provided does not appear to be present in file {file_name}. The original_code contains:\n```\n{tool_call['original_code']}\n```\nBut this section of code was not found anywhere inside the current file. DOUBLE CHECK that the change you are trying to make is not already implemented in the code!"
+                    
+                    # first check the lines in original_code, if it is too long, ask for smaller changes
+                    original_code_lines_length = len(original_code.split("\n"))
+                    if original_code_lines_length > 10:
+                        error_message += f"\n\nThe original_code seems to be quite long with {original_code_lines_length} lines of code. Break this large change up into a series of SMALLER changes to avoid errors like these! Try to make sure the original_code is under 10 lines. DOUBLE CHECK to make sure that this make_change tool call is only attempting a singular change, if it is not, make sure to split this make_change tool call into multiple smaller make_change tool calls!"
                     else:
-                        logger.debug(success_message)
-                        suffix = "\n\nMake additional search_codebase calls to find other keywords or start making changes by calling the make_change tool."
-                        success_message = create_tool_call_response(tool_name, f"SUCCESS\n\n{success_message}{suffix}")
-                        tool_name, tool_call = assistant_generator.send(
-                            success_message
-                        )
+                        # generate the diff between the original code and the current chunk to help the llm identify what it messed up
+                        # chunk_original_code_diff = generate_diff(original_code, current_chunk) - not necessary
+                        error_message += "\n\nDOUBLE CHECK that the original_code you have provided is correct, if it is not, correct it then make another replacement with the corrected original_code. The original_code MUST be in section A in order for you to make a change. DOUBLE CHECK to make sure that this make_change tool call is only attempting a singular change, if it is not, make sure to split this make_change tool call into multiple smaller make_change tool calls!"
+                    break
+                # ensure original_code and new_code has the correct indents
+                new_code_lines = new_code.split("\n")
+                new_code = "\n".join(f'{correct_indent*" "}{line}' for line in new_code_lines)
+                if rstrip_original_code:
+                    original_code_lines = [line.rstrip() for line in original_code.split("\n")]
                 else:
-                    error_message = create_tool_call_response("UNKNOWN TOOL NAME", f"ERROR\nUnexpected tool name: {tool_name}")
-                    tool_name, tool_call = assistant_generator.send(
-                        error_message
+                    original_code_lines = original_code.split("\n")
+                original_code = "\n".join(f'{correct_indent*" "}{line}' for line in original_code_lines)
+                # before we apply changes make sure original_code is unique inside current_chunk
+                current_chunk_occurences = file_contents.count(original_code)
+                if current_chunk_occurences > 1:
+                    error_message = f"The original_code is not unique in the file {file_name}. It appears {current_chunk_occurences} times! original_code MUST be unique, add some more lines for context!"
+                    break
+
+                # apply changes
+                new_file_contents = file_contents.replace(original_code, new_code, 1)
+                # Check if changes were made
+                if new_file_contents == file_contents:
+                    logger.warning("No changes were made to the code.")
+                    error_message = "No changes were made, it seems the changes you requested were not applied or made no difference to the code file."
+                    break
+                
+                # Check if the changes are valid
+                if not error_message:
+                    check_results = get_check_results(file_name, new_file_contents)
+                    check_results_message = check_results.is_worse_than_message(llm_state['initial_check_results'][file_name])
+                    failing_parse = check_results.parse_error_message if not llm_state['initial_check_results'][file_name].parse_error_message else ""
+                    current_diff = generate_diff(
+                        file_contents, new_file_contents
                     )
+                    if failing_parse:
+                        error_message = f"Error: Invalid code changes have been applied. You requested the following changes:\n\n```diff\n{current_diff}\n```\n\nBut it produces invalid code with the following error logs:\n```\n{failing_parse}\n```\n\nFirst, identify where the broken code occurs, why it is broken and what the correct change should be. Then, retry the make_change tool with different changes that yield valid code."
+                        break
+                    elif check_results_message:
+                        warning_message = check_results_message
+        if error_message:
+            llm_response = f"ERROR\n\n{error_message}"
+        if not error_message:
+            success_message = (
+                f"SUCCESS\n\nThe following changes have been applied to {file_name}:\n\n"
+                + generate_diff(file_contents, new_file_contents)
+            ) + f"{warning_message}\n\nYou can continue to make changes to the file {file_name} and call the make_change tool again, or handle the rest of the plan. REMEMBER to add all necessary imports at the top of the file, if the import is not already there!"
+            # set contents
+            if file_name not in modify_files_dict:
+                modify_files_dict[file_name] = {
+                    "contents": file_contents,
+                    "original_contents": file_contents,
+                }
+            next_step, feedback = ModifyEvaluatorAgent().evaluate_patch(
+                problem_statement=llm_state["request"],
+                patch = generate_diff(file_contents, new_file_contents, n=10),
+                changed_files=modify_files_dict,
+                new_file_contents=new_file_contents,
+                current_plan=llm_state["plan"],
+                current_task=llm_state["current_task"],
+                previous_attempt=llm_state["previous_attempt"],
+                file_name=file_name,
+                warning_message=warning_message,
+                chat_logger_messages=chat_logger_messages,
+            )
+
+            if next_step == "COMPLETE":
+                # Sets first fcr that is not completed to completed
+                for fcr in llm_state["fcrs"]:
+                    if not fcr.is_completed:
+                        fcr.is_completed = True
+                        break
+                llm_state["plan"] = render_plan(llm_state["fcrs"])
+                llm_state["current_task"] = render_current_task(llm_state["fcrs"])
+                llm_response = f"{success_message}"
+                modify_files_dict[file_name]["original_contents"] = file_contents if "original_contents" not in modify_files_dict[file_name] else modify_files_dict[file_name]["original_contents"]
+                modify_files_dict[file_name]['contents'] = new_file_contents
+                llm_state["previous_attempt"] = ""
+            elif next_step == "CONTINUE":
+                # guard modify files
+                llm_response = f"SUCCESS\n\nThe changes have been applied. However, we need to fix a few more things before moving to the next task of the plan. Here is the feedback from the user:\n\n```\n{generate_diff(file_contents, new_file_contents)}\n```\n{feedback}"
+                modify_files_dict[file_name]["original_contents"] = file_contents if "original_contents" not in modify_files_dict[file_name] else modify_files_dict[file_name]["original_contents"]
+                modify_files_dict[file_name]['contents'] = new_file_contents
+                previous_attempt = f"<previous_attempt>\nThe contractor previously made this change:\n\n```diff\n{generate_diff(file_contents, new_file_contents)}\n```\n\nAnd you accepted with the following feedback:\n{feedback}\n</previous_attempt>"
+                llm_state["previous_attempt"] = previous_attempt
             else:
-                logger.error("Too many iterations.")
-        except StopIteration:
-            pass
-        # return dictionary of file paths to their new contents
-        changes_made = False
-        diffs_made = defaultdict(str)
-        unmodified_files = []
-        for file_name, file_data in modify_files_dict.items():
-            diff = generate_diff(file_data["original_contents"], file_data["contents"])
-            if diff:
-                changes_made = True
-                diffs_made[file_name] = diff
-            else:
-                # remove this file from the dictionary
-                unmodified_files.append(file_name)
-        # remove any unmodified files
-        for file_name in unmodified_files:
-            modify_files_dict.pop(file_name)
-            logger.info(f"Removing {file_name} from modify_files_dict as no changes were made to this file.")
-
-        if changes_made:
-            for file_name, diff in diffs_made.items():
-                logger.info(f"Changes made to {file_name}:\n\n{diff}")
+                previous_attempt = f"<previous_attempt>\nThe contractor previously attempted at making this change:\n\n```diff\n{generate_diff(file_contents, new_file_contents)}\n```\n\nAnd you rejected it with the following feedback:\n{feedback}\n</previous_attempt>"
+                llm_state["previous_attempt"] = previous_attempt
+                llm_response = f"Changes Rejected with ERROR:\n\n{feedback}"
+    elif tool_name == "create_file":
+        error_message = ""
+        success_message = ""
+        for key in tool_call_parameters[tool_name]:
+            if key not in tool_call:
+                error_message += f"No {key} was provided in the {tool_name} tool call. Call the tool again but this time provide the {key}.\n"
+        if not error_message:
+            new_file_path = tool_call["file_path"].strip()
+            new_file_name = tool_call["file_name"].strip()
+            new_file_contents = tool_call["contents"].strip()
+            new_file_dir = os.path.join(cloned_repo.repo_dir, new_file_path)
+            new_full_file_path = os.path.join(new_file_path, new_file_name)
+            new_full_file_path_with_cwd = os.path.join(cloned_repo.repo_dir, new_file_path, new_file_name)
+            # ensure file doesn't already exist
+            if os.path.exists(new_full_file_path_with_cwd):
+                error_message = f"The file {new_full_file_path} already exists. Modify this existing file instead of attempting to create a new one!"
+            # ensure directory is valid
+            if not os.path.isdir(new_file_dir):
+                error_message = f"The directory {new_file_path} is not valid. Make sure you have the correct directory path!"
+            # ensure that the directory of the new full path exists, in case the file name is weird
+            if not os.path.exists(os.path.dirname(new_full_file_path_with_cwd)):
+                error_message = f"The directory {os.path.dirname(new_full_file_path)} does not exist. Make sure the new file you want to create exists within an existing directory!"
+            # if no issues, create the file by placing it in modify_files_dict
+            if not error_message:
+                modify_files_dict[new_full_file_path] = {"contents": new_file_contents, "original_contents": ""}
+                success_message = f"The new file {new_full_file_path} has been created successfully with the following contents:\n\n{new_file_contents}"
+        if error_message:
+            llm_response = f"ERROR\n\n{error_message}"
         else:
-            logger.warning("No changes were made.")
-        if changes_made:
-            logger.info("Finished modifying files!")
-            return modify_files_dict
-    except AssistantRaisedException as e:
-        logger.exception(e)
-        discord_log_error(
-            str(e)
-            + "\n\n"
-            + traceback.format_exc()
-            + "\n\n"
-            + str(chat_logger.data if chat_logger else "")
-            + "\n\n"
-            + str(ticket_progress.tracking_id if ticket_progress else "")
-        )
-    except Exception as e:
-        logger.exception(e)
-        # TODO: Discord
-        discord_log_error(
-            str(e)
-            + "\n\n"
-            + traceback.format_exc()
-            + "\n\n"
-            + str(chat_logger.data if chat_logger else "")
-            + "\n\n"
-            + str(ticket_progress.tracking_id if ticket_progress else "")
-        )
-        return None
-    return None
+            llm_response = f"SUCCESS\n\n{success_message}"
+    else:
+        llm_response = f"ERROR\nUnexpected tool name: {tool_name}"
+    return llm_response, modify_files_dict, llm_state
 
 if __name__ == "__main__":
-    from sweepai.config.server import INSTALLATION_ID
-    # request = "Convert any all logger.errors to logger.exceptions in on_ticket.py"
-    request = """Split any logger.errors to:
-logger = Logger()
-logger.errors()
-in on_ticket.py""" # this causes a pylint error so it's great for testing
-    cloned_repo = ClonedRepo(
-        repo_full_name="sweepai/sweep",
-        installation_id=INSTALLATION_ID
-    )
-    additional_messages = [
-        Message(
-            role="user",
-            content="# Repo & Issue Metadata\nRepo: sweep: Sweep: AI-powered Junior Developer for small features and bug fixes.\nIssue Title: Convert any all logger.errors to logger.exceptions in on_ticket.py",
-            name=None,
-            function_call=None,
-            key="issue_metadata",
-        )
-    ]
-    file_contents = open("sweepai/handlers/on_ticket.py", "r").read()
-    response = function_modify(
-        request=request,
-        file_path="sweepai/handlers/on_ticket.py",
-        contents_of_file=file_contents,
-        cloned_repo=cloned_repo,
-        chat_logger=ChatLogger(
-            {
-                "username": "kevinlu1248",
-                "title": request
-            }
-        ),
-        additional_messages=additional_messages,
-        ticket_progress=TicketProgress(tracking_id="test_remove_assistant_1"),
-    )
+    pass
```

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/assistant_functions.py` & `sweepai-2.0.1/sweepai/agents/assistant_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/assistant_wrapper.py` & `sweepai-2.0.1/sweepai/core/chat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,496 +1,503 @@
-import json
+from math import inf
+import os
 import re
+import time
 import traceback
-from time import sleep
-from typing import Any, Callable, Optional
+from typing import Any, Literal
 
-import openai
+from anthropic import Anthropic, BadRequestError, AnthropicBedrock
+from openai import OpenAI
+import backoff
 from loguru import logger
-from openai.pagination import SyncCursorPage
-from openai.types.chat.chat_completion_message_tool_call import (
-    ChatCompletionMessageToolCall,
-    Function,
-)
 from pydantic import BaseModel
 
-from sweepai.config.server import DEFAULT_GPT4_32K_MODEL, IS_SELF_HOSTED
-from sweepai.core.entities import AssistantRaisedException, Message
+from sweepai.agents.agent_utils import ensure_additional_messages_length
+from sweepai.config.client import get_description
+from sweepai.config.server import (
+    ANTHROPIC_AVAILABLE,
+    AWS_ACCESS_KEY,
+    AWS_REGION,
+    AWS_SECRET_KEY,
+    DEFAULT_GPT4_32K_MODEL,
+    PAREA_API_KEY
+)
+from sweepai.core.entities import Message
+from sweepai.core.prompts import repo_description_prefix_prompt, system_message_prompt
+from sweepai.logn.cache import file_cache
+from sweepai.utils.anthropic_client import sanitize_anthropic_messages
 from sweepai.utils.chat_logger import ChatLogger
 from sweepai.utils.event_logger import posthog
-from sweepai.utils.openai_proxy import get_client
-from sweepai.utils.anthropic_client import AnthropicClient
+from sweepai.utils.github_utils import ClonedRepo
+from sweepai.utils.openai_proxy import OpenAIProxy
+from sweepai.utils.prompt_constructor import HumanMessagePrompt
+from sweepai.utils.utils import Tiktoken
+from parea import Parea
+
+parea_client = None
+try:
+    if PAREA_API_KEY:
+        parea_client = Parea(api_key=PAREA_API_KEY)
+except Exception as e:
+    logger.info(f"Failed to initialize Parea client: {e}")
+
+openai_proxy = OpenAIProxy()
+
+OpenAIModel = (
+    Literal["gpt-3.5-turbo"]
+    | Literal["gpt-3.5-turbo-1106"]
+    | Literal["gpt-3.5-turbo-16k"]
+    | Literal["gpt-3.5-turbo-16k-0613"]
+    | Literal["gpt-4-1106-preview"]
+    | Literal["gpt-4-0125-preview"]
+)
+
+AnthropicModel = (
+    Literal["claude-3-haiku-20240307"]
+    | Literal["claude-3-sonnet-20240229"]
+    | Literal["claude-3-opus-20240229"]
+)
 
-def openai_retry_with_timeout(call, *args, num_retries=3, timeout=5, **kwargs):
-    """
-    Pass any OpenAI client call and retry it num_retries times, incorporating timeout into the call.
-
-    Usage:
-    run = openai_retry_with_timeout(client.beta.threads.runs.submit_tool_outputs, thread_id=thread.id, run_id=run.id, tool_outputs=tool_outputs, num_retries=3, timeout=10)
-
-    Parameters:
-    call (callable): The OpenAI client call to be retried.
-    *args: Positional arguments for the callable.
-    num_retries (int): The number of times to retry the call.
-    timeout (int): The timeout value to be applied to the call.
-    **kwargs: Keyword arguments for the callable.
-
-    Returns:
-    The result of the OpenAI client call.
-    """
-    error_message = None
-    e = None
-    for attempt in range(num_retries):
-        try:
-            return call(*args, **kwargs, timeout=timeout)
-        except Exception as e_:
-            logger.exception(f"Retry {attempt + 1} failed with error: {e_}")
-            error_message = str(e_)
-            e = e_
-    if e:
-        raise Exception(
-            f"Maximum retries reached. The call failed for call {error_message}"
-        ) from e
-    else:
-        raise Exception(
-            f"Maximum retries reached. The call failed for call {error_message}"
+ChatModel = OpenAIModel | AnthropicModel
+model_to_max_tokens = {
+    "gpt-3.5-turbo": 4096,
+    "gpt-3.5-turbo-1106": 16385,
+    "gpt-3.5-turbo-16k": 16385,
+    "gpt-4-1106-preview": 128000,
+    "gpt-4-0125-preview": 128000,
+    "gpt-4-turbo-2024-04-09": 128000,
+    "claude-v1": 9000,
+    "claude-v1.3-100k": 100000,
+    "claude-instant-v1.3-100k": 100000,
+    "anthropic.claude-3-haiku-20240229-v1:0": 200000,
+    "anthropic.claude-3-sonnet-20240229-v1:0": 200000,
+    "claude-3-opus-20240229": 200000,
+    "claude-3-sonnet-20240229": 200000,
+    "claude-3-haiku-20240307": 200000,
+    "gpt-3.5-turbo-16k-0613": 16000,
+}
+default_temperature = 0.1
+
+class MessageList(BaseModel):
+    messages: list[Message] = [
+        Message(
+            role="system",
+            content=system_message_prompt,
         )
+    ]
 
+    @property
+    def messages_dicts(self):
+        # Remove the key from the message object before sending to OpenAI
+        cleaned_messages = [message.to_openai() for message in self.messages]
+        return cleaned_messages
+
+    def delete_messages_from_chat(
+        self, key_to_delete: str, delete_user=True, delete_assistant=True
+    ):
+        self.messages = [
+            message
+            for message in self.messages
+            if not (
+                key_to_delete in (message.key or "")
+                and (
+                    delete_user
+                    and message.role == "user"
+                    or delete_assistant
+                    and message.role == "assistant"
+                )
+            )  # Only delete if message matches key to delete and role should be deleted
+        ]
 
-def fix_tool_calls(tool_calls: Optional[list[ChatCompletionMessageToolCall]]):
-    if tool_calls is None:
-        return
-
-    fixed_tool_calls = []
-
-    for tool_call in tool_calls:
-        current_function = tool_call.function.name
-        try:
-            function_args = json.loads(tool_call.function.arguments)
-        except json.JSONDecodeError:
-            logger.error(
-                f"Error: could not decode function arguments: {tool_call.function.args}"
+def determine_model_from_chat_logger(chat_logger: ChatLogger, model: str):
+    if chat_logger is not None:
+        if (
+            chat_logger.active is False
+            and not chat_logger.is_paying_user()
+            and not chat_logger.is_consumer_tier()
+        ):
+            raise ValueError(
+                "You have no more tickets! Please upgrade to a paid plan."
             )
-            fixed_tool_calls.append(tool_call)
-            continue
-        if current_function in ("parallel", "multi_tool_use.parallel"):
-            for _fake_i, _fake_tool_use in enumerate(function_args["tool_uses"]):
-                _function_args = _fake_tool_use["parameters"]
-                _current_function = _fake_tool_use["recipient_name"]
-                if _current_function.startswith("functions."):
-                    _current_function = _current_function[len("functions.") :]
-
-                fixed_tc = ChatCompletionMessageToolCall(
-                    id=f"{tool_call.id}_{_fake_i}",
-                    type="function",
-                    function=Function(
-                        name=_current_function, arguments=json.dumps(_function_args)
-                    ),
-                )
-                fixed_tool_calls.append(fixed_tc)
         else:
-            fixed_tool_calls.append(tool_call)
-
-    return fixed_tool_calls
-
-
-save_ticket_progress_type = Callable[[str, str, str], None]
-
-
-class AssistantResponse(BaseModel):
-    messages: SyncCursorPage[Any]
-    assistant_id: str
-    run_id: str
-    thread_id: str
-
-
-allowed_exts = [
-    "c",
-    "cpp",
-    "csv",
-    "docx",
-    "html",
-    "java",
-    "json",
-    "md",
-    "pdf",
-    "php",
-    "pptx",
-    "py",
-    "rb",
-    "tex",
-    "txt",
-    "css",
-    "jpeg",
-    "jpg",
-    "js",
-    "gif",
-    "png",
-    "tar",
-    "ts",
-    "xlsx",
-    "xml",
-    "zip",
-    "elm",
-]
+            tickets_allocated = inf if chat_logger.is_paying_user() else 5
+            tickets_count = chat_logger.get_ticket_count()
+            purchased_tickets = chat_logger.get_ticket_count(purchased=True)
+            if tickets_count < tickets_allocated:
+                logger.info(
+                    f"{tickets_count} tickets found in MongoDB, using {model}"
+                )
+                return model
+            elif purchased_tickets > 0:
+                
+                logger.info(
+                    f"{purchased_tickets} purchased tickets found in MongoDB, using {model}"
+                )
+                return model
+            else:
+                raise ValueError(
+                    f"Tickets allocated: {tickets_allocated}, tickets found: {tickets_count}. You have no more tickets!"
+                )
+    return model
 
 tool_call_parameters = {
-    "analyze_problem_and_propose_plan": ["problem_analysis", "proposed_plan"],
-    "search_codebase": ["justification", "file_name", "keyword"],
-    "analyze_and_identify_changes": ["file_name", "changes"],
-    "view_file": ["justification", "file_name"],
-    "make_change": ["justification", "file_name", "section_id", "original_code", "new_code"],
+    "make_change": ["justification", "file_name", "original_code", "new_code"],
     "create_file": ["justification", "file_name", "file_path", "contents"],
     "submit_result": ["justification"],
 }
 
-def get_json_messages(
-    thread_id: str,
-    run_id: str,
-    assistant_id: str,
-):
-    model, client = get_client()
-    assistant = openai_retry_with_timeout(
-        client.beta.assistants.retrieve,
-        assistant_id=assistant_id,
-    )
-    messages = openai_retry_with_timeout(
-        client.beta.threads.messages.list,
-        thread_id=thread_id,
-    )
-    run_steps = openai_retry_with_timeout(
-        client.beta.threads.runs.steps.list, run_id=run_id, thread_id=thread_id
-    )
-    system_message_json = {
-        "role": "system",
-        "content": assistant.instructions,
-    }
-    messages_json = [system_message_json]
-    for message in messages:
-        if message.role == "user":
-            messages_json.append(
-                {
-                    "role": "user",
-                    "content": message.content[0].text.value,
-                }
-            )
-    for message_obj in list(run_steps.data)[:0:-1]:
-        if message_obj.type == "message_creation":
-            message_id = message_obj.step_details.message_creation.message_id
-            thread_messages = openai_retry_with_timeout(
-                client.beta.threads.messages.retrieve,
-                message_id=message_id,
-                thread_id=thread_id,
-            )
-            message_content = thread_messages.content[0].text.value
-            messages_json.append(
-                {
-                    "role": "assistant",
-                    "content": message_content,
-                }
-            )
-            # TODO: handle annotations
-        elif message_obj.type == "tool_calls":
-            for tool_call in message_obj.step_details.tool_calls:
-                if tool_call.type == "code_interpreter":
-                    code_interpreter = tool_call.code_interpreter
-                    input_ = code_interpreter.input
-                    if not input_:
-                        continue
-                    input_content = f"Code interpreter input:\n```\n{input_}\n```"
-                    messages_json.append(
-                        {
-                            "role": "assistant",
-                            "content": input_content,
-                        }
-                    )
-                    outputs = code_interpreter.outputs
-                    output = outputs[0].logs if outputs else "__No output__"
-                    output_content = f"Code interpreter output:\n```\n{output}\n```"
-                    messages_json.append(
-                        {
-                            "role": "user",
-                            "content": output_content,
-                        }
-                    )
-                else:
-                    function = tool_call.function
-                    input_content = f"Function call of {function.name}:\n```\n{function.arguments}\n```"
-                    messages_json.append(
-                        {
-                            "role": "assistant",
-                            "content": input_content,
-                        }
-                    )
-                    if function.output:
-                        output_content = (
-                            f"Function output:\n```\n{function.output}\n```"
-                        )
-                        messages_json.append(
-                            {
-                                "role": "user",
-                                "content": output_content,
-                            }
-                        )
-    return messages_json
-
 # returns a dictionary of the tool call parameters, assumes correct
-def parse_tool_call_parameters(tool_call_contents: str, parameters: list[str]) -> dict[str, Any]:
+def parse_function_call_parameters(tool_call_contents: str, parameters: list[str]) -> dict[str, Any]:
     tool_args = {}
     for param in parameters:
         param_regex = rf'<{param}>\s*(?P<{param}>.*?)\s*<\/{param}>'
         match = re.search(param_regex, tool_call_contents, re.DOTALL)
         if match:
             param_contents = match.group(param)
             tool_args[param] = param_contents
     return tool_args
 
 # parse llm response for tool calls in xml format
-def parse_tool_calls(response_contents: str) -> list[dict[str, Any]]:
+def parse_function_calls_for_openai(response_contents: str) -> list[dict[str, str]]:
     tool_calls = []
     # first get all tool calls
-    tool_call_regex = r'<invoke>\s*(?P<function_call>.*?)\s*<\/invoke>'
-    tool_call_matches = re.finditer(tool_call_regex, response_contents, re.DOTALL)
-
-    # now we extract each tool name and its parameters
-    for tool_call_match in tool_call_matches:
-        tool_name_regex = r'<tool_name>\s*(?P<tool_name>.*?)\s*<\/tool_name>'
-        tool_call_contents = tool_call_match.group("function_call")
-        tool_name = re.search(tool_name_regex, tool_call_contents).group("tool_name").strip()
-        # now we extract the arguments based on the tool name
-        if tool_name in tool_call_parameters:
+    for tool_name in tool_call_parameters.keys():
+        tool_call_regex = rf'<{tool_name}>\s*(?P<function_call>.*?)\s*<\/{tool_name}>'
+        tool_call_matches = re.finditer(tool_call_regex, response_contents, re.DOTALL)
+        # now we extract its parameters
+        for tool_call_match in tool_call_matches:
+            tool_call_contents = tool_call_match.group("function_call")
             # get parameters based off of tool name
             parameters = tool_call_parameters[tool_name]
             tool_call = { "tool": tool_name, 
-                         "arguments": parse_tool_call_parameters(tool_call_contents, parameters) 
+                        "arguments": parse_function_call_parameters(tool_call_contents, parameters) 
                         }
             tool_calls.append(tool_call)
-        else:
-            logger.debug(f"WARNING! Tool name {tool_name} not recognized")
     return tool_calls
 
-def run_until_complete(
-    tools: list[dict[str, str]],
-    model: str = DEFAULT_GPT4_32K_MODEL,
-    chat_logger: ChatLogger | None = None,
-    sleep_time: int = 3,
-    max_iterations: int = 100,
-    save_ticket_progress: save_ticket_progress_type | None = None,
-    messages: list[Message] = [],
-):
-    normal_messages_remaining = 3
-    # used for chat logger
-    for i in range(max_iterations):
-        # log our progress
-        if i % 5 == 0:
-            logger.info(
-                f"run_until_complete iteration {i}, current message length: {len(messages)}"
-            )
-        # if we are somehow about to hit the max iterations, log a warning
-        if i == max_iterations - 1:
-            logger.warning(
-                f"run_until_complete about to hit max iterations! iteration {i} out {max_iterations}"
-            )
-        # get the response from openai
-        try:
-            client = AnthropicClient()                
-            response = client.get_response_message(messages, max_tokens=3072, temperature=0.2, stop_sequences=["</invoke>"])
-        # sometimes deployment for opennai is not found, retry after a minute
-        except openai.NotFoundError as e:
-            logger.error(
-                f"Openai deployment not found on iteration {i} with error: {e}\n Retrying in 60 seconds..."
+class ChatGPT(MessageList):
+    prev_message_states: list[list[Message]] = []
+    model: ChatModel = DEFAULT_GPT4_32K_MODEL
+    chat_logger: ChatLogger | None = None
+    human_message: HumanMessagePrompt | None = None
+    file_change_paths: list[str] = []
+    cloned_repo: ClonedRepo | None = None
+    temperature: float = default_temperature
+
+    class Config:
+        arbitrary_types_allowed = True
+
+    @classmethod
+    def from_system_message_content(
+        cls,
+        human_message: HumanMessagePrompt,
+        is_reply: bool = False,
+        chat_logger=None,
+        cloned_repo: ClonedRepo | None = None,
+        **kwargs,
+    ):
+        content = system_message_prompt
+        repo = kwargs.get("repo")
+        if repo:
+            repo_info = get_description(repo)
+            repo_description = repo_info["description"]
+            repo_info["rules"]
+            if repo_description:
+                content += f"{repo_description_prefix_prompt}\n{repo_description}"
+        messages = [Message(role="system", content=content, key="system")]
+
+        added_messages = human_message.construct_prompt()  # [ { role, content }, ... ]
+        for msg in added_messages:
+            messages.append(Message(**msg))
+        messages = ensure_additional_messages_length(messages)
+
+        return cls(
+            messages=messages,
+            human_message=human_message,
+            chat_logger=chat_logger,
+            cloned_repo=cloned_repo,
+            **kwargs,
+        )
+
+    @classmethod
+    def from_system_message_string(
+        cls, prompt_string: str, chat_logger: ChatLogger | None = None, **kwargs
+    ) -> Any:
+        return cls(
+            messages=[Message(role="system", content=prompt_string, key="system")],
+            chat_logger=chat_logger,
+            **kwargs,
+        )
+
+    def delete_messages_from_chat(
+        self, key_to_delete: str, delete_user=True, delete_assistant=True
+    ):
+        self.messages = [
+            message
+            for message in self.messages
+            if not (
+                key_to_delete in (message.key or "")
+                and (
+                    delete_user
+                    and message.role == "user"
+                    or delete_assistant
+                    and message.role == "assistant"
+                )
+            )  # Only delete if message matches key to delete and role should be deleted
+        ]
+
+    def chat(
+        self,
+        content: str,
+        model: ChatModel | None = None,
+        message_key: str | None = None,
+        temperature: float | None = None,
+        max_tokens: int | None = None,
+        stop_sequences: list[str] = [],
+    ):
+        self.messages.append(Message(role="user", content=content, key=message_key))
+        model = model or self.model
+        temperature = temperature or self.temperature or default_temperature
+        self.messages.append(
+            Message(
+                role="assistant",
+                content=self.call_openai(
+                    model=model,
+                    temperature=temperature,
+                    requested_max_tokens=max_tokens,
+                    stop_sequences=stop_sequences,
+                ),
+                key=message_key,
             )
-            sleep(60)
-            continue
-        except Exception as e:
-            logger.error(f"chat completions failed on interation {i} with error: {e}")
-            sleep(sleep_time)
-            continue
-        # extend conversation
-        response_role, response_contents = client.parse_role_content_from_response(response)
-        if not response_contents:
-            done_response = yield "done", {
-                "status": "completed",
-                "message": "Run completed",
-            }
-        # if a function call was made
-        if "<invoke>" in response_contents:
-            response_contents += "</invoke>\n</function_calls>"
-        tool_calls = parse_tool_calls(response_contents)
-        # extend conversation with llm, must rstrip to remove trailing whitespace or else anthropic complains
-        messages.append({"role": response_role, "content": response_contents.rstrip() or  "No tool call made!"})
-        # if a tool call was made
-        done_response = None
-        if len(tool_calls) > 1:
-            logger.debug(f"WARNING MULTIPLE TOOL CALLS MADE: {len(tool_calls)}")
-        if tool_calls:
-            for tool_call in tool_calls:
-                tool_name = tool_call['tool']
-                try:
-                    tool_args = tool_call["arguments"]
-                except json.JSONDecodeError as e:
-                    logger.debug(
-                        f'Error: could not decode function arguments: {tool_call["arguments"]}'
+        )
+        self.prev_message_states.append(self.messages)
+        return self.messages[-1].content
+
+    @file_cache(ignore_params=["chat_logger", "cloned_repo"])
+    def call_openai(
+        self,
+        model: ChatModel | None = None,
+        temperature=temperature,
+        requested_max_tokens: int | None = None,
+        stop_sequences: list[str] = [],
+    ):
+        model = determine_model_from_chat_logger(chat_logger=self.chat_logger, model=model)
+        if model not in model_to_max_tokens:
+            raise ValueError(f"Model {model} not supported")
+        count_tokens = Tiktoken().count
+        messages_length = sum(
+            [count_tokens(message.content or "") for message in self.messages]
+        )
+        max_tokens = (
+            model_to_max_tokens[model] - int(messages_length) - 400
+        )  # this is for the function tokens
+        messages_raw = "\n".join([(message.content or "") for message in self.messages])
+        logger.info(f"Input to call openai:\n{messages_raw}")
+        if len(self.file_change_paths) > 0:
+            self.file_change_paths.remove(self.file_change_paths[0])
+        if max_tokens < 0:
+            if len(self.file_change_paths) > 0:
+                pass
+            else:
+                raise ValueError(f"Message is too long, max tokens is {max_tokens}")
+        messages_dicts = [self.messages_dicts[0]]
+        for message_dict in self.messages_dicts[:1]:
+            if message_dict["role"] == messages_dicts[-1]["role"]:
+                messages_dicts[-1]["content"] += "\n" + message_dict["content"]
+            messages_dicts.append(message_dict)
+        max_tokens = min(max_tokens, 4096)
+        max_tokens = (
+            min(requested_max_tokens, max_tokens)
+            if requested_max_tokens
+            else max_tokens
+        )
+        logger.info(f"Using the model {model} with {messages_length} input tokens and {max_tokens} tokens remaining")
+        global retry_counter
+        retry_counter = 0
+
+        @backoff.on_exception(
+            backoff.expo,
+            Exception,
+            max_tries=16,
+            jitter=backoff.random_jitter,
+        )
+        def fetch():
+            global retry_counter
+            retry_counter += 1
+            token_sub = retry_counter * 200
+            try:
+                output = None
+                output = openai_proxy.call_openai(
+                    model=model,
+                    messages=self.messages_dicts,
+                    max_tokens=max_tokens - token_sub,
+                    temperature=temperature,
+                    stop_sequences=stop_sequences,
+                ).choices[0].message.content
+                if self.chat_logger is not None:
+                    self.chat_logger.add_chat(
+                        {
+                            "model": model,
+                            "messages": self.messages_dicts,
+                            "max_tokens": max_tokens - token_sub,
+                            "temperature": temperature,
+                            "output": output,
+                        }
                     )
-                    tool_output = f"ERROR\nCould not decode function arguments:\n{e}"
-                else:
-                    if tool_name == "submit_result":
-                        logger.info(
-                            "Submit function was called"
+                if self.chat_logger:
+                    try:
+                        token_count = count_tokens(output)
+                        posthog.capture(
+                            self.chat_logger.data.get("username"),
+                            "call_openai",
+                            {
+                                "model": model,
+                                "max_tokens": max_tokens - token_sub,
+                                "input_tokens": messages_length,
+                                "output_tokens": token_count,
+                                "repo_full_name": self.chat_logger.data.get(
+                                    "repo_full_name"
+                                ),
+                                "username": self.chat_logger.data.get("username"),
+                                "pr_number": self.chat_logger.data.get("pr_number"),
+                                "issue_url": self.chat_logger.data.get("issue_url"),
+                            },
                         )
-                        if "justification" in tool_args:
-                            done_response = yield "done", {
-                                "status": "completed",
-                                "message": tool_args["justification"],
-                            }
+                    except SystemExit:
+                        raise SystemExit
+                    except Exception as e2:
+                        logger.warning(e2)
+                return output
+            except SystemExit:
+                raise SystemExit
+            except Exception as e:
+                logger.warning(f"{e}\n{traceback.format_exc()}")
+                raise e
+
+        result = fetch()
+        logger.info(f"Output to call openai:\n{result}")
+        return result
+    
+    def chat_anthropic(
+        self,
+        content: str,
+        assistant_message_content: str = "",
+        model: ChatModel = "claude-3-haiku-20240307",
+        message_key: str | None = None,
+        temperature: float | None = None,
+        stop_sequences: list[str] = [],
+        max_tokens: int = 4096,
+        use_openai: bool = False,
+    ):
+        # use openai
+        if use_openai:
+            OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY")
+            assert OPENAI_API_KEY
+            self.model = 'gpt-4-turbo'
+        else:
+            ANTHROPIC_API_KEY = os.environ.get("ANTHROPIC_API_KEY")
+            assert ANTHROPIC_API_KEY
+            self.model = model
+        self.messages.append(Message(role="user", content=content, key=message_key))
+        if assistant_message_content:
+            self.messages.append(Message(role="assistant", content=assistant_message_content))
+        temperature = temperature or self.temperature or default_temperature
+        messages_string = '\n\n'.join([message.content for message in self.messages])
+        logger.debug(f"Calling anthropic with model {model}\nMessages:{messages_string}\nInput:\n{content}")
+        system_message = "\n\n".join([message.content for message in self.messages if message.role == "system"])
+        content = ""
+        e = None
+        NUM_ANTHROPIC_RETRIES = 4
+        for i in range(NUM_ANTHROPIC_RETRIES):
+            try:
+                @file_cache(redis=True) # must be in the inner scope because this entire function manages state
+                def call_anthropic(
+                    message_dicts: list[dict[str, str]], 
+                    system_message: str = system_message, 
+                    model: str = model,
+                    use_openai: bool = use_openai,
+                ) -> str: # add system message and model to cache
+                    if use_openai:
+                        client = OpenAI()
+                    else:
+                        if ANTHROPIC_AVAILABLE and "opus" not in model:
+                            if "anthropic" not in model:
+                                model = f"anthropic.{model}-v1:0"
+                                self.model = f"anthropic.{self.model}-v1:0"
+                            client = AnthropicBedrock(
+                                aws_access_key=AWS_ACCESS_KEY,
+                                aws_secret_key=AWS_SECRET_KEY,
+                                aws_region=AWS_REGION,
+                            )
                         else:
-                            done_response = yield "done", {
-                                "status": "completed",
-                                "message": "No justification provided",
-                            }
-                        logger.info(
-                            f"run_until_complete done_response: {done_response} completed after {i} iterations"
-                        )
-                        if not done_response:
-                            break
+                            client = Anthropic(api_key=ANTHROPIC_API_KEY)
+                    if parea_client:
+                        if use_openai:
+                            parea_client.wrap_openai_client(client)
+                        else:
+                            parea_client.wrap_anthropic_client(client)
+                    if use_openai:
+                        response = client.chat.completions.create(
+                            model=model,
+                            messages=self.messages_dicts,
+                            max_tokens=max_tokens,
+                            temperature=temperature,
+                            stop=stop_sequences,
+                        ).choices[0].message.content
                     else:
-                        logger.debug(
-                            f"tool_call: {tool_name} with args: {tool_args}"
-                        )
-                        tool_output: str = yield tool_name, tool_args
-                        if not tool_output:
-                            break
-                        messages.append(
-                            {
-                                "role": "user",
-                                "content": f"{tool_output.rstrip()}",
-                            }
-                        )  # extend conversation with function response
-                
-        else:  # no tool call being made implies either an error or a success
-            logger.error(
-                f"No tool calls were made, yielding with tool_call no_tool_call: {response_contents}"
-            )
-            done_response = yield "no_tool_call", {
-                "status": "no tool call",
-                "message": "No tool call made",
-            }
-            normal_messages_remaining -= 1
-            if normal_messages_remaining < 0:
-                return
-
-            if not done_response:
+                        response = client.messages.create(
+                            model=model,
+                            temperature=temperature,
+                            max_tokens=max_tokens,
+                            messages=message_dicts,
+                            system=system_message,
+                            stop_sequences=stop_sequences,
+                        ).content[0].text
+                    return response
+                if use_openai:
+                    message_dicts = [
+                        {
+                            "role": message.role,
+                            "content": message.content,
+                        } for message in self.messages
+                    ]
+                    message_dicts = sanitize_anthropic_messages(message_dicts)
+                else: 
+                    message_dicts = [
+                        {
+                            "role": message.role,
+                            "content": message.content,
+                        } for message in self.messages if message.role != "system"
+                    ]
+                    message_dicts = sanitize_anthropic_messages(message_dicts)
+                content = call_anthropic(message_dicts, self.messages[0].content, self.model, use_openai=use_openai)
                 break
-
-        # on each iteration of the for loop, we will log to chat_logger
-        if chat_logger is not None and len(messages):
-            descriptive_messages = [message for message in messages]
-            # for tool calls, the content is empty, replace that with the function contents
-            for message in descriptive_messages:
-                if message.get("content", "") == "" and "tool_calls" in message:
-                    # if there were multiple tool calls, add them both
-                    for tool_call in message["tool_calls"]:
-                        message[
-                            "content"
-                        ] += f"\n\ntool_call: {tool_call.get('function', '')}"
-            chat_logger.add_chat(
-                {
-                    "model": model,
-                    "messages": descriptive_messages,
-                    "output": descriptive_messages[-1]["content"],
-                    "max_tokens": 1000,
-                    "temperature": 0,
-                }
-            )
-        # update ticket_progress
-        # if save_ticket_progress is not None:
-        #     save_ticket_progress(
-        #         messages=messages
-        #     )
-    return messages
-
-
-def openai_assistant_call_helper(
-    request: str,
-    instructions: str | None = None,
-    additional_messages: list[Message] = [],
-    file_paths: list[str] = [],  # use either file_paths or file_ids
-    uploaded_file_ids: list[str] = [],
-    tools: list[dict[str, str]] = [{"type": "code_interpreter"}],
-    model: str = DEFAULT_GPT4_32K_MODEL,
-    sleep_time: int = 3,
-    chat_logger: ChatLogger | None = None,
-    assistant_id: str | None = None,
-    assistant_name: str | None = None,
-    save_ticket_progress: save_ticket_progress_type | None = None,
-):
-    logger.debug(instructions)
-    messages = [{"role": "system", "content": instructions}]
-    for message in additional_messages:
-        messages.append({"role": message.role, "content": message.content})
-    return run_until_complete(
-        tools=tools,
-        messages=messages,
-        model=model,
-        chat_logger=chat_logger,
-        sleep_time=sleep_time,
-        save_ticket_progress=save_ticket_progress,
-    )
-
-
-# Split in two so it can be cached
-def openai_assistant_call(
-    request: str,
-    instructions: str | None = None,
-    additional_messages: list[Message] = [],
-    file_paths: list[str] = [],
-    uploaded_file_ids: list[str] = [],
-    tools: list[dict[str, str]] = [{"type": "code_interpreter"}],
-    model: str = DEFAULT_GPT4_32K_MODEL,
-    sleep_time: int = 3,
-    chat_logger: ChatLogger | None = None,
-    assistant_id: str | None = None,
-    assistant_name: str | None = None,
-    save_ticket_progress: save_ticket_progress_type | None = None,
-):
-    model, client = get_client()
-    if chat_logger and chat_logger.use_faster_model():
-        raise Exception("GPT-3.5 is not supported on assistant calls.")
-    model = DEFAULT_GPT4_32K_MODEL
-    posthog.capture(
-        chat_logger.data.get("username") if chat_logger is not None else "anonymous",
-        "call_assistant_api",
-        {
-            "query": request,
-            "model": model,
-            "username": (
-                chat_logger.data.get("username", "anonymous")
-                if chat_logger is not None
-                else "anonymous"
-            ),
-            "is_self_hosted": IS_SELF_HOSTED,
-            "trace": "".join(traceback.format_list(traceback.extract_stack())),
-        },
-    )
-    retries = range(3)
-    for _ in retries:
-        try:
-            response = openai_assistant_call_helper(
-                request=request,
-                instructions=instructions,
-                additional_messages=additional_messages,
-                file_paths=file_paths,
-                uploaded_file_ids=uploaded_file_ids,
-                tools=tools,
-                model=model,
-                sleep_time=sleep_time,
-                chat_logger=chat_logger,
-                assistant_id=assistant_id,
-                assistant_name=assistant_name,
-                save_ticket_progress=save_ticket_progress,
+            except BadRequestError as e_:
+                e = e_ # sometimes prompt is too long
+                raise e_
+            except Exception as e_:
+                logger.exception(e_)
+                e = e_
+                time.sleep(4 * 2 ** i) # faster debugging
+        else:
+            raise Exception("Anthropic call failed") from e
+        self.messages.append(
+            Message(
+                role="assistant",
+                content=content,
+                key=message_key,
             )
-            return response
-        except AssistantRaisedException as e:
-            logger.warning(e.message)
-        except Exception as e:
-            logger.error(e)
-            raise e
+        )
+        logger.debug(f'{"Openai" if use_openai else "Anthropic"} response: {self.messages[-1].content}')
+        self.prev_message_states.append(self.messages)
+        return self.messages[-1].content
+
+    @property
+    def messages_dicts(self):
+        # Remove the key from the message object before sending to OpenAI
+        cleaned_messages = [message.to_openai() for message in self.messages]
+        return cleaned_messages
+
+    def undo(self):
+        if len(self.prev_message_states) > 0:
+            self.messages = self.prev_message_states.pop()
+        return self.messages
```

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/assistant_wrapper_test.py` & `sweepai-2.0.1/sweepai/agents/assistant_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/complete_code.py` & `sweepai-2.0.1/sweepai/agents/complete_code.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/complete_code_test.py` & `sweepai-2.0.1/sweepai/agents/complete_code_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/distill_issue.py` & `sweepai-2.0.1/sweepai/agents/distill_issue.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/modify_bot.py` & `sweepai-2.0.1/sweepai/agents/modify_bot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 import re
 from dataclasses import dataclass
 
-from sweepai.agents.assistant_function_modify import (
-    excel_col_to_int,
-    function_modify,
-    int_to_excel_col,
-)
 from sweepai.agents.complete_code import ExtractLeftoverComments
+from sweepai.agents.modify import modify
 from sweepai.agents.prune_modify_snippets import PruneModifySnippets
 from sweepai.core.chat import ChatGPT
 from sweepai.core.entities import FileChangeRequest, Message, Snippet, UnneededEditError
-from sweepai.core.prompts import dont_use_chunking_message, use_chunking_message
 from sweepai.core.update_prompts import (
     update_snippets_prompt,
     update_snippets_prompt_test,
     update_snippets_system_prompt,
     update_snippets_system_prompt_python,
 )
 from sweepai.utils.autoimport import add_auto_imports
 from sweepai.utils.diff import generate_diff, sliding_window_replacement
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import ClonedRepo
 from sweepai.utils.progress import AssistantConversation, TicketProgress
-from sweepai.utils.utils import chunk_code
 
 fetch_snippets_system_prompt = """You are a masterful engineer. Your job is to extract the original sections from the code that should be modified.
 
 Extract the smallest spans that let you handle the request by adding sections of sections_to_modify containing the code you want to modify. Use this for implementing or changing functionality.
 
 <analysis_and_identification file="file_path">
 Identify all changes that need to be made to the file.
@@ -247,50 +241,40 @@
             )
         diff += self.additional_diffs
         diff = diff.strip("\n")
         return f"\n# Changes Made\nHere are changes we already made to this file:\n<diff>\n{diff}\n</diff>\n"
 
     def try_update_file(
         self,
-        file_path: str,
-        file_contents: str,
-        file_change_request: FileChangeRequest,
+        instructions: str,
         cloned_repo: ClonedRepo,
         assistant_conversation: AssistantConversation | None = None,
         seed: str | None = None,
         relevant_filepaths: list[str] = [],
         fcrs: list[FileChangeRequest]=[],
         previous_modify_files_dict: dict[str, dict[str, str | list[str]]] = None,
+        use_openai: bool = False,
     ):
-        new_files = function_modify(
-            request=file_change_request.instructions,
-            file_path=file_path,
-            contents_of_file=file_contents,
+        new_files = modify(
+            request=instructions,
             cloned_repo=cloned_repo,
-            additional_messages=self.additional_messages,
-            chat_logger=self.chat_logger,
-            ticket_progress=self.ticket_progress,
-            assistant_conversation=assistant_conversation,
-            seed=seed,
             relevant_filepaths=relevant_filepaths,
             fcrs=fcrs,
-            cwd=cloned_repo.repo_dir,
-            previous_modify_files_dict=previous_modify_files_dict,
+            chat_logger=self.chat_logger,
+            use_openai=use_openai,
         )
         if new_files:
             posthog.capture(
                 (
                     self.chat_logger.data["username"]
                     if self.chat_logger is not None
                     else "anonymous"
                 ),
                 "function_modify_succeeded",
                 {
-                    "file_path": file_path,
-                    "instructions": file_change_request.instructions,
                     "repo_full_name": cloned_repo.repo_full_name,
                 },
             )
             # new_file is now a dictionary
             for file_path, new_file_data in new_files.items():
                 new_file_data["contents"] = add_auto_imports(file_path, cloned_repo.repo_dir, new_file_data["contents"], run_isort=False)
             return new_files
@@ -298,99 +282,19 @@
             (
                 self.chat_logger.data["username"]
                 if self.chat_logger is not None
                 else "anonymous"
             ),
             "function_modify_succeeded",
             {
-                "file_path": file_path,
-                "instructions": file_change_request.instructions,
                 "repo_full_name": cloned_repo.repo_full_name,
             },
         )
         raise UnneededEditError("No snippets edited")
 
-    def get_snippets_to_modify(
-        self,
-        file_path: str,
-        file_contents: str,
-        file_change_request: FileChangeRequest,
-        chunking: bool = False,
-    ):
-        diffs_message = self.get_diffs_message(file_contents)
-        fetch_prompt = (
-            fetch_snippets_prompt_with_diff if diffs_message else fetch_snippets_prompt
-        )
-        original_snippets = chunk_code(file_contents, file_path, 700, 200)
-        file_contents_lines = file_contents.split("\n")
-        chunks = [
-            "\n".join(file_contents_lines[snippet.start : snippet.end])
-            for snippet in original_snippets
-        ]
-        code_sections = []
-        for i, chunk in enumerate(chunks):
-            idx = int_to_excel_col(i + 1)
-            code_sections.append(f'<section id="{idx}">\n{chunk}\n</section>')
-
-        fetch_snippets_response = self.fetch_snippets_bot.chat(
-            fetch_prompt.format(
-                code="\n".join(code_sections),
-                changes_made=self.get_diffs_message(file_contents),
-                file_path=file_path,
-                request=file_change_request.instructions,
-                chunking_message=(
-                    use_chunking_message if chunking else dont_use_chunking_message
-                ),
-            )
-        )
-        analysis_and_identification_pattern = r"<analysis_and_identification.*?>\n(?P<code>.*)\n</analysis_and_identification>"
-        analysis_and_identification_match = re.search(
-            analysis_and_identification_pattern, fetch_snippets_response, re.DOTALL
-        )
-        analysis_and_identifications_str = (
-            analysis_and_identification_match.group("code").strip()
-            if analysis_and_identification_match
-            else ""
-        )
-
-        extraction_terms = []
-        extraction_term_pattern = (
-            r"<extraction_terms.*?>\n(?P<extraction_term>.*?)\n</extraction_terms>"
-        )
-        for extraction_term in re.findall(
-            extraction_term_pattern, fetch_snippets_response, re.DOTALL
-        ):
-            for term in extraction_term.split("\n"):
-                term = term.strip()
-                if term:
-                    extraction_terms.append(term)
-        snippet_queries = []
-        snippets_query_pattern = r"<section_to_modify.*?(reason=\"(?P<reason>.*?)\")?>\n(?P<section>.*?)\n</section_to_modify>"
-        for match_ in re.finditer(
-            snippets_query_pattern, fetch_snippets_response, re.DOTALL
-        ):
-            section = match_.group("section").strip()
-            # processing logic to sanitize input, sometimes adds "SECTION_ID: A"
-            if " " in section:
-                section_pieces = section.split(" ")
-                # get the smallest piece if there is a space
-                section = min(section_pieces, key=len)
-            snippet_index = excel_col_to_int(section)
-            if snippet_index < 0 or snippet_index >= len(original_snippets):
-                continue
-            snippet = original_snippets[snippet_index]
-            reason = match_.group("reason").strip()
-            snippet_queries.append(
-                SnippetToModify(reason=reason or "", snippet=snippet)
-            )
-
-        if len(snippet_queries) == 0:
-            raise UnneededEditError("No snippets found in file")
-        return snippet_queries, extraction_terms, analysis_and_identifications_str
-
     def update_file(
         self,
         file_path: str,
         file_contents: str,
         file_change_request: FileChangeRequest,
         snippet_queries: list[SnippetToModify],
         extraction_terms: list[str],
```

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/pr_description_bot.py` & `sweepai-2.0.1/sweepai/agents/pr_description_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/agents/prune_modify_snippets.py` & `sweepai-2.0.1/sweepai/agents/prune_modify_snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/api.py` & `sweepai-2.0.1/sweepai/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 import threading
 import time
 from typing import Any, Optional
 
 import requests
 from fastapi import (
     Body,
-    Depends,
     FastAPI,
     Header,
     HTTPException,
     Path,
     Request,
     Security,
     status,
 )
 from fastapi.responses import HTMLResponse
 from fastapi.security import HTTPAuthorizationCredentials, HTTPBearer
 from fastapi.templating import Jinja2Templates
 from github.Commit import Commit
-from prometheus_fastapi_instrumentator import Instrumentator
 
 from sweepai.config.client import (
     DEFAULT_RULES,
     RESTART_SWEEP_BUTTON,
     REVERT_CHANGED_FILES_TITLE,
     RULES_LABEL,
     RULES_TITLE,
@@ -58,14 +56,15 @@
 from sweepai.handlers.on_button_click import handle_button_click
 from sweepai.handlers.on_check_suite import (  # type: ignore
     clean_gh_logs,
     download_logs,
     on_check_suite,
 )
 from sweepai.handlers.on_comment import on_comment
+from sweepai.handlers.on_jira_ticket import handle_jira_ticket
 from sweepai.handlers.on_merge import on_merge
 from sweepai.handlers.on_merge_conflict import on_merge_conflict
 from sweepai.handlers.on_ticket import on_ticket
 from sweepai.handlers.pr_utils import make_pr
 from sweepai.handlers.stack_pr import stack_pr
 from sweepai.utils.buttons import (
     Button,
@@ -120,25 +119,14 @@
     if credentials.credentials != "example_token":  # grafana requires authentication
         raise HTTPException(
             status_code=status.HTTP_401_UNAUTHORIZED, detail="Invalid token."
         )
     return True
 
 
-if not IS_SELF_HOSTED:
-    Instrumentator().instrument(app).expose(
-        app,
-        should_gzip=False,
-        endpoint="/metrics",
-        include_in_schema=True,
-        tags=["metrics"],
-        dependencies=[Depends(auth_metrics)],
-    )
-
-
 def run_on_ticket(*args, **kwargs):
     tracking_id = get_hash()
     with logger.contextualize(
         **kwargs,
         name="ticket_" + kwargs["username"],
         tracking_id=tracking_id,
     ):
@@ -210,17 +198,14 @@
         terminate_thread(e)
 
     thread = threading.Thread(target=run_on_ticket, args=args, kwargs=kwargs)
     on_ticket_events[key] = thread
     thread.start()
     global_threads.append(thread)
 
-    # delayed_kill_thread = threading.Thread(target=delayed_kill, args=(thread,))
-    # delayed_kill_thread.start()
-
 
 def call_on_check_suite(*args, **kwargs):
     kwargs["request"].repository.full_name
     kwargs["request"].check_run.pull_requests[0].number
     thread = threading.Thread(target=run_on_check_suite, args=args, kwargs=kwargs)
     thread.start()
     global_threads.append(thread)
@@ -356,14 +341,22 @@
 ):
     """Handle a webhook request from GitHub."""
     with logger.contextualize(tracking_id="main", env=ENV):
         action = request_dict.get("action", None)
         logger.info(f"Received event: {x_github_event}, {action}")
         return handle_request(request_dict, event=x_github_event)
 
+@app.post("/jira")
+def jira_webhook(
+    request_dict: dict = Body(...),
+) -> None:
+    def call_jira_ticket(*args, **kwargs):
+        thread = threading.Thread(target=handle_jira_ticket, args=args, kwargs=kwargs)
+        thread.start()
+    call_jira_ticket(event=request_dict)
 
 # Set up cronjob for this
 @app.get("/update_sweep_prs_v2")
 def update_sweep_prs_v2(repo_full_name: str, installation_id: int):
     # Get a Github client
     _, g = get_github_client(installation_id)
```

### Comparing `sweepai-2.0.0.dev1/sweepai/api_test.py` & `sweepai-2.0.1/sweepai/api_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/cli.py` & `sweepai-2.0.1/sweepai/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,19 +40,22 @@
 
 
 def load_config():
     if os.path.exists(config_path):
         cprint(f"\nLoading configuration from {config_path}", style="yellow")
         with open(config_path, "r") as f:
             config = json.load(f)
-        os.environ["GITHUB_PAT"] = config.get("GITHUB_PAT", "")
-        os.environ["OPENAI_API_KEY"] = config.get("OPENAI_API_KEY", "")
-        os.environ["ANTHROPIC_API_KEY"] = config.get("ANTHROPIC_API_KEY", "")
-        os.environ["VOYAGE_API_KEY"] = config.get("VOYAGE_API_KEY", "")
-        os.environ["POSTHOG_DISTINCT_ID"] = str(config.get("POSTHOG_DISTINCT_ID", ""))
+        os.environ.update(config)
+        os.environ["POSTHOG_DISTINCT_ID"] = str(os.environ.get("POSTHOG_DISTINCT_ID", ""))
+        # Should contain:
+        # GITHUB_PAT
+        # OPENAI_API_KEY
+        # ANTHROPIC_API_KEY
+        # VOYAGE_API_KEY
+        # POSTHOG_DISTINCT_ID
 
 
 def fetch_issue_request(issue_url: str, __version__: str = "0"):
     (
         protocol_name,
         _,
         _base_url,
@@ -268,15 +271,15 @@
         "\nGreat! Next, we'll need just your GitHub PAT. Here's a link with all the permissions pre-filled:\nhttps://github.com/settings/tokens/new?description=Sweep%20Self-hosted&scopes=repo,workflow\n",
         style="yellow",
     )
     github_pat = Prompt.ask("GitHub PAT", password=True)
     assert len(github_pat) > 30, "GitHub PAT must be of length at least 30."
     assert github_pat.startswith("ghp_"), "GitHub PAT must start with 'ghp_'."
     cprint(
-        "\nAwesome! Lastly, let's get your Voyage AI API key from https://dash.voyageai.com/api-keys. This is optional, but improves code search by about [cyan]5%[/cyan]. You can always return to this later by re-running 'sweep init'.",
+        "\nAwesome! Lastly, let's get your Voyage AI API key from https://dash.voyageai.com/api-keys. This is optional, but improves code search by about [cyan]3%[/cyan]. You can always return to this later by re-running 'sweep init'.",
         style="yellow",
     )
     voyage_api_key = Prompt.ask("Voyage AI API key", password=True)
     if voyage_api_key:
         assert len(voyage_api_key) > 30, "Voyage AI API key must be of length at least 30."
         assert voyage_api_key.startswith("pa-"), "Voyage API key must start with 'pa-'."
```

### Comparing `sweepai-2.0.0.dev1/sweepai/cli_test.py` & `sweepai-2.0.1/sweepai/cli_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/config/client.py` & `sweepai-2.0.1/sweepai/config/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 import yaml
 from github.Repository import Repository
 from loguru import logger
 from pydantic import BaseModel
 
 from sweepai.core.entities import EmptyRepository
 from sweepai.utils.file_utils import read_file_with_fallback_encodings
-from sweepai.utils.utils import Tiktoken
 
 
 class SweepConfig(BaseModel):
     include_dirs: list[str] = []
     exclude_dirs: list[str] = [
         ".git",
         "node_modules",
+        "build",
+        ".venv",
         "venv",
         "patch",
         "packages/blobs",
         "dist",
     ]
-    exclude_path_dirs: list[str] = ["node_modules", "venv", ".git", "dist"]
+    exclude_path_dirs: list[str] = ["node_modules", "build", ".venv", "venv", ".git", "dist"]
     exclude_substrings_aggressive: list[str] = [ # aggressively filter out file paths, may drop some relevant files
         "integration",
         ".spec",
         ".test",
         ".json",
         "test"
     ]
@@ -224,15 +225,15 @@
         for part in parts:
             if part in self.exclude_dirs or part in self.exclude_exts:
                 return True
         return False
     
     # returns if file is excluded or not, this version may drop actual relevant files
     def is_file_excluded_aggressive(self, dir: str, file_path: str) -> bool:
-        tiktoken_client = Tiktoken()
+        # tiktoken_client = Tiktoken()
         # must exist
         if not os.path.exists(os.path.join(dir, file_path)) and not os.path.exists(file_path):
             return True
         full_path = os.path.join(dir, file_path)
         if os.stat(full_path).st_size > 240000 or os.stat(full_path).st_size < 5:
             return True
         # exclude binary 
@@ -252,20 +253,20 @@
             logger.warning(f"UnicodeDecodeError in is_file_excluded_aggressive: {full_path}, skipping")
             return True
         line_count = len(lines)
         # if average line length is greater than 200, then it is likely not human readable
         if len(data)/line_count > 200:
             return True
     
-         # check token density, if it is greater than 2, then it is likely not human readable
-        token_count = tiktoken_client.count(data)
-        if token_count == 0:
-            return True
-        if len(data)/token_count < 2:
-            return True
+        # check token density, if it is greater than 2, then it is likely not human readable
+        # token_count = tiktoken_client.count(data)
+        # if token_count == 0:
+        #     return True
+        # if len(data)/token_count < 2:
+        #     return True
         
         # now check the file name
         parts = file_path.split(os.path.sep)
         for part in parts:
             if part in self.exclude_dirs or part in self.exclude_exts:
                 return True
         for part in self.exclude_substrings_aggressive:
@@ -276,24 +277,24 @@
 
 
 @lru_cache(maxsize=None)
 def get_gha_enabled(repo: Repository) -> bool:
     try:
         contents = repo.get_contents("sweep.yaml")
         gha_enabled = yaml.safe_load(contents.decoded_content.decode("utf-8")).get(
-            "gha_enabled", True
+            "gha_enabled", False
         )
         return gha_enabled
     except SystemExit:
         raise SystemExit
-    except Exception as e:
-        logger.exception(
-            f"Error when getting gha enabled: {e}, traceback: {traceback.format_exc()}, falling back to True"
+    except Exception:
+        logger.info(
+            "Error when getting gha enabled, falling back to False"
         )
-        return True
+        return False
 
 
 @lru_cache(maxsize=None)
 def get_description(repo: Repository) -> dict:
     try:
         contents = repo.get_contents("sweep.yaml")
         sweep_yaml = yaml.safe_load(contents.decoded_content.decode("utf-8"))
@@ -373,16 +374,15 @@
         )
         sweep_yaml = yaml.safe_load(sweep_yaml_content)
         rules = sweep_yaml.get("rules", [])
         return rules
     except SystemExit:
         raise SystemExit
     except Exception:
-        return []
-
+        return []    
 
 # optional, can leave env var blank
 GITHUB_APP_CLIENT_ID = os.environ.get("GITHUB_APP_CLIENT_ID", "Iv1.91fd31586a926a9f")
 
 RESTART_SWEEP_BUTTON = "↻ Restart Sweep"
 SWEEP_GOOD_FEEDBACK = "👍 Sweep Did Well"
 SWEEP_BAD_FEEDBACK = "👎 Sweep Needs Improvement"
```

### Comparing `sweepai-2.0.0.dev1/sweepai/config/server.py` & `sweepai-2.0.1/sweepai/config/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     WHITELISTED_USERS = WHITELISTED_USERS.split(",")
     WHITELISTED_USERS.append(GITHUB_BOT_USERNAME)
 
 DEFAULT_GPT4_32K_MODEL = os.environ.get("DEFAULT_GPT4_32K_MODEL", "gpt-4-0125-preview")
 DEFAULT_GPT35_MODEL = os.environ.get("DEFAULT_GPT35_MODEL", "gpt-3.5-turbo-1106")
 
 RESEND_API_KEY = os.environ.get("RESEND_API_KEY", None)
-LOKI_URL = os.environ.get("LOKI_URL", None)
+LOKI_URL = None
 
 DEBUG = os.environ.get("DEBUG", "false").lower() == "true"
 ENV = "prod" if GITHUB_BOT_USERNAME != TEST_BOT_NAME else "dev"
 
 PROGRESS_BASE_URL = os.environ.get(
     "PROGRESS_BASE_URL", "https://progress.sweep.dev"
 ).rstrip("/")
@@ -221,22 +221,30 @@
 AWS_SECRET_KEY=os.environ.get("AWS_SECRET_KEY")
 AWS_REGION=os.environ.get("AWS_REGION")
 ANTHROPIC_AVAILABLE = AWS_ACCESS_KEY and AWS_SECRET_KEY and AWS_REGION
 
 USE_ASSISTANT = os.environ.get("USE_ASSISTANT", "true").lower() == "true"
 ANTHROPIC_API_KEY = os.environ.get("ANTHROPIC_API_KEY", None)
 
+COHERE_API_KEY = os.environ.get("COHERE_API_KEY", None)
+
 VOYAGE_API_KEY = os.environ.get("VOYAGE_API_KEY", None)
 
 VOYAGE_API_AWS_ACCESS_KEY=os.environ.get("VOYAGE_API_AWS_ACCESS_KEY_ID")
 VOYAGE_API_AWS_SECRET_KEY=os.environ.get("VOYAGE_API_AWS_SECRET_KEY")
 VOYAGE_API_AWS_REGION=os.environ.get("VOYAGE_API_AWS_REGION")
 VOYAGE_API_AWS_ENDPOINT_NAME=os.environ.get("VOYAGE_API_AWS_ENDPOINT_NAME", "voyage-code-2")
 
 VOYAGE_API_USE_AWS = VOYAGE_API_AWS_ACCESS_KEY and VOYAGE_API_AWS_SECRET_KEY and VOYAGE_API_AWS_REGION
 
 PAREA_API_KEY = os.environ.get("PAREA_API_KEY", None)
 
-# TODO: we need to ake this dynamic + backoff
+# TODO: we need to make this dynamic + backoff
 BATCH_SIZE = int(
-    os.environ.get("BATCH_SIZE", 24 if VOYAGE_API_KEY else 256) # Voyage only allows 128 items per batch and 120000 tokens per batch
-)
+    os.environ.get("BATCH_SIZE", 64 if VOYAGE_API_KEY else 256) # Voyage only allows 128 items per batch and 120000 tokens per batch
+)
+
+DEPLOYMENT_GHA_ENABLED = os.environ.get("DEPLOYMENT_GHA_ENABLED", "true").lower() == "true"
+
+JIRA_USER_NAME = os.environ.get("JIRA_USER_NAME", None)
+JIRA_API_TOKEN = os.environ.get("JIRA_API_TOKEN", None)
+JIRA_URL = os.environ.get("JIRA_URL", None)
```

### Comparing `sweepai-2.0.0.dev1/sweepai/core/context_pruning.py` & `sweepai-2.0.1/sweepai/core/context_pruning.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,256 +1,180 @@
 from copy import deepcopy
+from math import log
 import os
 import subprocess
 import urllib
 from dataclasses import dataclass, field
 
 import networkx as nx
 import openai
 from loguru import logger
 from openai.types.beta.thread import Thread
 from openai.types.beta.threads.run import Run
 
 from sweepai.config.client import SweepConfig
 from sweepai.core.chat import ChatGPT
 from sweepai.core.entities import Message, Snippet
-from sweepai.core.reflection_utils import EvaluatorAgent
+from sweepai.logn.cache import file_cache
 from sweepai.utils.chat_logger import ChatLogger
-from sweepai.utils.code_tree import CodeTree
-from sweepai.utils.convert_openai_anthropic import MockFunctionCall
+from sweepai.utils.convert_openai_anthropic import AnthropicFunctionCall, mock_function_calls_to_string
 from sweepai.utils.github_utils import ClonedRepo
 from sweepai.utils.modify_utils import post_process_rg_output
+from sweepai.utils.openai_listwise_reranker import listwise_rerank_snippets
 from sweepai.utils.progress import AssistantConversation, TicketProgress
 from sweepai.utils.tree_utils import DirectoryTree
 
 ASSISTANT_MAX_CHARS = 4096 * 4 * 0.95  # ~95% of 4k tokens
 NUM_SNIPPETS_TO_SHOW_AT_START = 15
+MAX_REFLECTIONS = 1
+MAX_ITERATIONS = 25
+NUM_ROLLOUTS = 1 # dev speed
+SCORE_THRESHOLD = 8 # good score
+STOP_AFTER_SCORE_THRESHOLD_IDX = 0 # stop after the first good score and past this index
+MAX_PARALLEL_FUNCTION_CALLS = 1
+NUM_BAD_FUNCTION_CALLS = 5
 
 # TODO:
 # - Add self-evaluation / chain-of-verification
-# - Add list of tricks for finding definitions
 
 anthropic_function_calls = """<tool_description>
-<tool_name>draft_plan</tool_name>  
-<description>
-Draft a detailed report of the issue and a high-level plan to resolve it. The report should explain the root cause, expected behavior, and list each file that needs to be edited and exactly how it should be edited. Write it for a new intern with no prior knowledge of the codebase or issue.
-
-You should always call this function first
-</description>
-<parameters>
-<parameter>  
-<name>plan</name>
-<type>string</type>
-<description>A report providing background information and explaining the issue for a new intern who is new to the codebase, and a extremely-detailed plan outlining the steps to resolve the issue, including what needs to be modified in each file to modify and which files to use.</description>
-</parameter>
-</parameters>
-</tool_description>
-
-<tool_name>view_file</tool_name>
+<tool_name>code_search</tool_name>
 <description>
-Retrieves the contents of the specified file. After viewing a file, use `code_search` on relevant entities to find their definitions. Use `store_file` to add the file to the context if it's relevant to solving the issue.
+Passes the code_entity into ripgrep to search the entire codebase and return a list of files and line numbers where it appears. Useful for finding definitions, usages, and references to types, classes, functions, and other entities that may be relevant. Review the search results using `view_files` to determine relevance and discover new files to explore.
 </description>
 <parameters>
 <parameter>
-<name>file_path</name>
+<name>analysis</name>
 <type>string</type>
-<description>The path of the file to view.</description>
+<description>Explain what new information you expect to discover from this search and why it's needed to get to the root of the issue. Focus on unknowns rather than already stored information.</description>
 </parameter>
 <parameter>
-<name>justification</name>
+<name>code_entity</name>
 <type>string</type>
-<description>Explain why viewing this file is necessary to solve the issue.</description>
+<description>
+The code entity to search for. This must be a distinctive name, not a generic term. For functions, search for the definition syntax, e.g. 'def foo' in Python or 'function bar' or 'const bar' in JavaScript. Trace dependencies of critical functions/classes, follow imports to find definitions, and explore how key entities are used across the codebase.
+</description>
 </parameter>
 </parameters>
 </tool_description>
 
 <tool_description>
-<tool_name>store_file</tool_name>
+<tool_name>view_files</tool_name>
 <description>
-Adds a file to the context that needs to be modified or used to resolve the issue. Provide a code excerpt in the justification showcasing the file's relevance, i.e. how it should be fixed or another part of the codebase that is relevant and uses this module. After using this tool, use `code_search` to find definitions of unknown functions /classes in the file to add to files to use.
+Retrieves the contents of the specified file(s). After viewing new files, use `code_search` on relevant entities to continue discovering potentially relevant files. You may view three files per tool call. Prioritize viewing new files over ones that are already stored.
 </description>
 <parameters>
 <parameter>
-<name>file_path</name>
+<name>analysis</name>
 <type>string</type>
-<description>The path of the file to store.</description>
+<description>Explain what new information viewing these files will provide and why it's necessary to resolve the issue. Avoid restating already known information.</description>
 </parameter>
 <parameter>
-<name>justification</name>
+<name>first_file_path</name>
 <type>string</type>
-<description>Explain why this file is should be modified or used and what needs to be modified or why it needs to be used. Include a supporting code excerpt.</description>
+<description>The path of a new file to view.</description>
 </parameter>
-</parameters>
-</tool_description>
-
-<tool_description>
-<tool_name>code_search</tool_name>
-<description>
-Searches the entire codebase for the given code entity and returns a list of files and line numbers where it appears. Useful for finding definitions of unknown types, classes and functions. Review the search results using `view_file` to determine relevance. Focus on definitions.
-</description>
-<parameters>
 <parameter>
-<name>code_entity</name>
+<name>second_file_path</name>
 <type>string</type>
-<description>The code entity to search for. Should be a distinctive name, not a generic term like 'if' or 'else'. For functions, search for the definition syntax, e.g. 'def foo(' in Python or 'function bar' or 'const bar' in JavaScript.</description>
+<description>The path of another new file to view (optional).</description>
 </parameter>
 <parameter>
-<name>justification</name>
+<name>third_file_path</name>
 <type>string</type>
-<description>Explain what information you expect to get from this search and why it's needed, e.g. "I need to find the definition of the Foo class to see what methods are available on Foo objects."</description>
+<description>The path of a third new file to view (optional).</description>
 </parameter>
 </parameters>
 </tool_description>
 
 <tool_description>
-<tool_name>submit</tool_name>  
+<tool_name>store_file</tool_name>
 <description>
-Provides a detailed report of the issue and a high-level plan to resolve it. The report should explain the root cause, expected behavior, and which files need to be modified or referenced. The plan should outline the changes needed in each file. Write it for an outside contractor with no prior knowledge of the codebase or issue. You may only call this tool once when you are absolutely certain you have all the necessary information.
+Adds a newly discovered file that provides important context or may need modifications to the list of stored files. You may only store one new file per tool call. Avoid storing files that have already been added.
 </description>
 <parameters>
 <parameter>
-<name>plan</name>
+<name>analysis</name>
+<type>string</type>
+<description>Explain what new information this file provides, why it's important for understanding and resolving the issue, and what potentially needs to be modified. Include a brief supporting code excerpt.</description>
+</parameter>
+<parameter>
+<name>file_path</name>
 <type>string</type>
-<description>Copy the final plan drafted using the draft_plan function.</description>
+<description>The path of the newly discovered relevant file to store.</description>
 </parameter>
 </parameters>
 </tool_description>
 
-You must call one tool at a time using the specified XML format. Here are some generic examples to illustrate the format without referring to a specific task:
-
-<examples>
-
-Example 1:
-<function_call>
-<invoke>
-<tool_name>draft_plan</tool_name>
-<parameters>
-<plan>
-Modify the file user_service.py with the following changes:
-* Go to the `get_user_by_id` method in the `UserService` class that fetches a user by user ID.
-* Add a new optional parameter called `include_deleted` with a default value of `False`.
-* Inside the method, add a condition to check the value of `include_deleted`.
-* If `include_deleted` is `False`, modify the database query to filter out users where the `deleted` column is set to `True`.
-* If `include_deleted` is `True`, no changes are needed to the query.
-* Update the method's docstring to reflect the new parameter and its behavior.
-Modify the file app.py with the following changes:
-* Locate the `get_user` route handler in the Flask app.
-* Find the call to `UserService.get_user_by_id()` within the route handler.
-* Add the `include_deleted=True` argument to the `get_user_by_id()` call to include deleted users.
-</plan>
-</parameters>
-</invoke>
-</function_call>
+You MUST call the tools using this exact XML format:
 
-Example 2:
 <function_call>
 <invoke>
-<tool_name>view_file</tool_name>
+<tool_name>$TOOL_NAME</tool_name>
 <parameters>
-<file_path>src/controllers/user_controller.py</file_path>
-<justification>I found the user_controller.py file in the previous search. I now need to view its contents to understand the UserController class implementation and determine if it needs to be modified to resolve the issue.</justification>
+<$PARAMETER_NAME>$PARAMETER_VALUE</$PARAMETER_NAME>
+...
 </parameters>
 </invoke>
 </function_call>
 
-Example 3:
-<function_call>
-<invoke>
-<tool_name>store_file</tool_name>
-<parameters>
-<file_path>src/controllers/user_controller.py</file_path>
-<justification>The user_controller.py file contains the UserController class referenced in the user request. The create_user method inside this class needs to be updated to fix the bug, as evidenced by this excerpt:
-```python
-def create_user(self, name, email):
-    # BUG: User is created without validating email 
-    user = User(name, email)
-    db.session.add(user)
-    db.session.commit()
-```
-</justification>
-</parameters>
-</invoke>
-</function_call>
+Here is an example illustrating a complex code search to discover new relevant information:
 
-Example 4:
+<example>
 <function_call>
 <invoke>
 <tool_name>code_search</tool_name>
 <parameters>
-<code_entity>class User(db.Model):</code_entity>
-<justification>The user_controller.py file references the User class, but I don't see its definition in this file. I need to search for 'class User(db.Model):' to find where the User model is defined, as this will provide necessary context about the User class to properly fix the create_user bug.</justification>
+<analysis>The get_user_by_id method likely queries from a User model or database table. I need to search for references to "User" to find where and how user records are defined, queried and filtered in order to determine what changes are needed to support excluding deleted users from the get_user_by_id results.</analysis>
+<code_entity>User</code_entity>
 </parameters>
 </invoke>
 </function_call>
+</example>
 
-</examples>
-
-I will provide the tool's response after each call, then you may call another tool as you work towards a solution. Focus on the actual issue at hand rather than these illustrative examples."""
-
-sys_prompt = """You are a brilliant engineer assigned to solve the following GitHub issue. Your task is to generate a complete, detailed, plan to fully resolve a GitHub issue and retrieve relevant files for this. We consider a file RELEVANT if it must either be modified or contains a function or class that must used as part of the issue resolution process. It is critical that you identify and include every relevant line of code that should either be modified or used and validate ALL changes.
-
-Your goal is to generate an extremely detailed and accurate plan of code changes for an intern and a list of relevant files who is unfamliar with the codebase. You will do this by first drafting an initial plan, then validating the plan by searching and viewing for files in the codebase to draft a refined plan. You will do this until you have a finished complete plan where every detail is fully validated.
+Remember, your goal is to discover and store ALL files that are relevant to solving the issue. Perform targeted searches to uncover new information, view new files to understand the codebase, and avoid re-analyzing already stored files."""
 
-Your plan should be complete but should not include tests.
+sys_prompt = """You are a brilliant engineer assigned to solve the following GitHub issue. Your task is to search through the codebase and locate ALL files that are RELEVANT to resolving the issue. A file is considered RELEVANT if it provides important context or may need to be modified as part of the solution.
 
-INSTRUCTIONS
+You will begin with a small set of stored relevant files. However, it is critical that you identify every additional relevant file by exhaustively searching the codebase. Your goal is to generate an extremely comprehensive list of files for an intern engineer who is completely unfamiliar with the codebase. Prioritize finding all relevant files over perfect precision - it's better to include a few extra files than to miss a key one.
 
-Use the following iterative process:
-1. First, summarize the "User Request" and "Relevant Snippets" use the draft_plan function to draft a detailed plan that is complete and indicates every detail that should be used.
+To accomplish this, you will iteratively search for and view new files to gather all the necessary information. Follow these steps:
 
-<example_draft_plan>
-Modify the file user_service.py with the following changes:
-* Go to the `get_user_by_id` method in the `UserService` class that fetches a user by user ID.
-* Add a new optional parameter called `include_deleted` with a default value of `False`.
-* Inside the method, add a condition to check the value of `include_deleted`.
-* If `include_deleted` is `False`, modify the database query to filter out users where the `deleted` column is set to `True`.
-* If `include_deleted` is `True`, no changes are needed to the query.
-* Update the method's docstring to reflect the new parameter and its behavior.
+1. Perform targeted code searches to find definitions, usages, and references for ALL unknown variables, classes, attributes, functions and other entities that may be relevant based on the currently stored files and issue description. Be creative and think critically about what to search for to get to the root of the issue. 
 
-Modify the file app.py with the following changes:
-* Locate the `get_user` route handler in the Flask app.
-* Find the call to `UserService.get_user_by_id()` within the route handler.
-* Add the `include_deleted=True` argument to the `get_user_by_id()` call to include deleted users.
-</example_draft_plan>
+2. View new files from the search results that seem relevant. Avoid viewing files that are already stored, and instead focus on discovering new information.
 
-Only after you have completed the initial draft plan using the draft_plan function should you proceed to view and search for relevant files.
+3. Store additional files that provide important context or may need changes based on the search results, viewed files, and issue description. 
 
-2. View all files that seem relevant based on file paths and entities mentioned in the "User Request" and "Relevant Snippets". For example, if the class foo.bar.Bar is referenced, be sure to view foo/bar.py. Skip irrelevant files. Make sure to check all files referenced in the user request. If you can't find a service, you can also check the "Common modules section".
-3. Use code_search to find definitions for ALL unknown variables, classes, attributes, and functions. For instance, if the method foo(param1: typeX, param2: typeY) -> typeZ is used, search for the keywords typeX, typeY, and typeZ to find where they are defined. If you want to use `user.deleted`, check that the `deleted` attribute exists on the entity. View the relevant files containing those definitions. Make sure to view ALL files when using or changing any function input parameters and accessing methods and attributes.
-4. When you identify a relevant file, use store_file to add it to the context.
-5. When you have retrieved new information, update the drafted plan by using the draft_plan function again.
-
-Repeat steps 1-3 until you are confident you have drafted a plan and have validated all the details, such as all the entities used and the variable and attribute names required.
-5. Submit the plan with the submit function.
-
-It is crucial that you follow the steps in the specified order, starting with drafting an initial plan using the draft_plan function before proceeding to view and search for files.
-
-Here are the tools at your disposal. Call them one at a time as needed until you have gathered all relevant information:
+Repeat steps 1-3, searching and exploring the codebase exhaustively until you are confident you have found all relevant files. Prioritize discovering new information over re-analyzing what is already known.
 
+Here are the tools at your disposal:
 """ + anthropic_function_calls
 
 unformatted_user_prompt = """\
-## Relevant Snippets
-Here are potentially relevant snippets in the repo in decreasing relevance that you should use the `view_file` tool to review:
+## Stored Files
+DO NOT CALL THE STORE OR VIEW TOOLS ON THEM AGAIN AS THEY HAVE ALREADY BEEN STORED.
+<stored_files>
 {snippets_in_repo}
+</stored_files>
 
-## Code files mentioned in the user request
-Here are the code files mentioned in the user request, these code files are very important to the solution and should be considered very relevant:
-<code_files_in_query>
-{file_paths_in_query}
-</code_files_in_query>
 {import_tree_prompt}
 ## User Request
 <user_request>
 {query}
 <user_request>"""
 
-
 PLAN_SUBMITTED_MESSAGE = "SUCCESS: Report and plan submitted."
 
+def escape_ripgrep(text):
+    # Special characters to escape
+    special_chars = ["(", "{"]
+    for s in special_chars:
+        text = text.replace(s, "\\" + s)
+    return text
 
 @staticmethod
 def can_add_snippet(snippet: Snippet, current_snippets: list[Snippet]):
     return (
         len(snippet.xml) + sum([len(snippet.xml) for snippet in current_snippets])
         <= ASSISTANT_MAX_CHARS
     )
@@ -288,41 +212,45 @@
         return any(snippet.file_path == path for snippet in self.snippets)
 
     def format_context(
         self,
         unformatted_user_prompt: str,
         query: str,
     ):
-        new_top_snippets: list[Snippet] = []
-        for snippet in self.current_top_snippets:
-            # if can_add_snippet(snippet, new_top_snippets):
-            if True:
-                new_top_snippets.append(snippet)
-        self.current_top_snippets = new_top_snippets
-        top_snippets_str = [snippet.file_path for snippet in self.current_top_snippets]
-        # dedupe the list inplace
-        top_snippets_str = list(dict.fromkeys(top_snippets_str))
-        top_snippets_str = top_snippets_str[:NUM_SNIPPETS_TO_SHOW_AT_START]
-        snippets_in_repo_str = "\n".join(top_snippets_str)
-        logger.info(f"Snippets in repo:\n{snippets_in_repo_str}")
+        files_in_repo_str = ""
+        stored_files = set()
+        for idx, snippet in enumerate(list(dict.fromkeys(self.current_top_snippets))[:NUM_SNIPPETS_TO_SHOW_AT_START]):
+            if snippet.file_path in stored_files:
+                continue
+            stored_files.add(snippet.file_path)
+            snippet_str = \
+f'''
+<stored_file index="{idx + 1}">
+<file_path>{snippet.file_path}</file_path>
+<source>
+{snippet.content}
+</source>
+</stored_file>
+'''
+            files_in_repo_str += snippet_str
         repo_tree = str(self.dir_obj)
         import_tree_prompt = """
 ## Import trees for code files in the user request
 <import_trees>
 {import_trees}
 </import_trees>
 """
         import_tree_prompt = (
             import_tree_prompt.format(import_trees=self.import_trees.strip("\n"))
             if self.import_trees
             else ""
         )
         user_prompt = unformatted_user_prompt.format(
             query=query,
-            snippets_in_repo=snippets_in_repo_str,
+            snippets_in_repo=files_in_repo_str,
             repo_tree=repo_tree,
             import_tree_prompt=import_tree_prompt,
             file_paths_in_query=", ".join(self.relevant_file_paths),
         )
         return user_prompt
 
     def get_highest_scoring_snippet(self, file_path: str) -> Snippet:
@@ -378,15 +306,14 @@
 main.py
 ├── database.py
 │   └── models.py
 └── utils.py
     └── models.py
 """
 
-
 def build_full_hierarchy(
     graph: nx.DiGraph, start_node: str, k: int, prefix="", is_last=True, level=0
 ):
     if level > k:
         return ""
     if level == 0:
         hierarchy = f"{start_node}\n"
@@ -447,43 +374,139 @@
             else:
                 line = line.strip()
                 current_node = line
                 if current_node:
                     G.add_node(current_node)
     return G
 
+@file_cache(ignore_params=["rcm", "G"])
+def graph_retrieval(formatted_query: str, top_k_paths: list[str], rcm: RepoContextManager, G: nx.DiGraph):
+    # TODO: tune these params
+    top_paths_cutoff = 25
+    num_rerank = 30
+    selected_paths = rcm.top_snippet_paths[:10]
+    top_k_paths = top_k_paths[:top_paths_cutoff]
+
+    snippet_scores = rcm.snippet_scores
+    for snippet, score in snippet_scores.items():
+        if snippet.split(":")[0] in top_k_paths:
+            snippet_scores[snippet] += 1
+
+    personalization = {}
+
+    for snippet in selected_paths:
+        personalization[snippet] = 1
+    try:
+        @file_cache()
+        def get_distilled_file_paths(formatted_query, top_k_paths):
+            personalized_pagerank_scores = nx.pagerank(G, personalization=personalization, alpha=0.85)
+            unpersonalized_pagerank_scores = nx.pagerank(G, alpha=0.85)
+
+            # tfidf style
+            normalized_pagerank_scores = {path: score * log(1 / (1e-6 + unpersonalized_pagerank_scores[path])) for path, score in personalized_pagerank_scores.items()}
+
+            top_pagerank_scores = sorted(normalized_pagerank_scores.items(), key=lambda x: x[1], reverse=True)
+            
+            top_pagerank_paths = [path for path, _score in top_pagerank_scores]
+
+            distilled_file_path_list = []
+
+            for file_path, score in top_pagerank_scores:
+                if file_path.endswith(".js") and file_path.replace(".js", ".ts") in top_pagerank_paths:
+                    continue
+                if file_path in top_k_paths:
+                    continue
+                if "generated" in file_path or "mock" in file_path or "test" in file_path:
+                    continue
+                try:
+                    rcm.cloned_repo.get_file_contents(file_path)
+                except FileNotFoundError:
+                    continue
+                distilled_file_path_list.append(file_path)
+            return distilled_file_path_list
+        distilled_file_path_list = get_distilled_file_paths(formatted_query, top_k_paths)
+        # Rerank once
+        reranked_snippets = []
+        for file_path in distilled_file_path_list[:num_rerank]:
+            contents = rcm.cloned_repo.get_file_contents(file_path)
+            reranked_snippets.append(Snippet(
+                content=contents,
+                start=0,
+                end=contents.count("\n") + 1,
+                file_path=file_path,
+            ))
+        reranked_snippets = listwise_rerank_snippets(formatted_query, reranked_snippets, prompt_type="graph")
+        distilled_file_path_list[:num_rerank] = [snippet.file_path for snippet in reranked_snippets]
+
+        return distilled_file_path_list
+    except Exception as e:
+        logger.error(e)
+        return []
+
+# @file_cache(ignore_params=["repo_context_manager", "override_import_graph"]) # can't cache this because rcm is stateful
+def integrate_graph_retrieval(formatted_query: str, repo_context_manager: RepoContextManager, override_import_graph: nx.DiGraph = None):
+    num_graph_retrievals = 25
+    repo_context_manager, import_graph = parse_query_for_files(formatted_query, repo_context_manager)
+    if override_import_graph:
+        import_graph = override_import_graph
+    if import_graph:
+        # Graph retrieval can fail and return [] if the graph is not found or pagerank does not converge
+        # Happens especially when graph has multiple components
+        graph_retrieved_files = graph_retrieval(formatted_query, sorted(repo_context_manager.top_snippet_paths), repo_context_manager, import_graph) # sort input for caching
+        if graph_retrieved_files:
+            sorted_snippets = sorted(
+                repo_context_manager.snippets,
+                key=lambda snippet: repo_context_manager.snippet_scores[snippet.denotation],
+                reverse=True,
+            )
+            snippets = []
+            for file_path in graph_retrieved_files:
+                for snippet in sorted_snippets[50 - num_graph_retrievals:]:
+                    if snippet.file_path == file_path:
+                        snippets.append(snippet)
+                        break
+            graph_retrieved_files = graph_retrieved_files[:num_graph_retrievals]
+            repo_context_manager.read_only_snippets = snippets[:len(graph_retrieved_files)]
+            repo_context_manager.current_top_snippets = repo_context_manager.current_top_snippets[:50 - num_graph_retrievals]
+    return repo_context_manager, import_graph
 
 # add import trees for any relevant_file_paths (code files that appear in query)
 def build_import_trees(
     rcm: RepoContextManager,
     import_graph: nx.DiGraph,
     override_import_graph: nx.DiGraph = None,
 ) -> tuple[RepoContextManager]:
     if import_graph is None and override_import_graph is None:
         return rcm
     if override_import_graph:
         import_graph = override_import_graph
     # if we have found relevant_file_paths in the query, we build their import trees
     code_files_in_query = rcm.relevant_file_paths
+    # graph_retrieved_files = graph_retrieval(rcm.top_snippet_paths, rcm, import_graph)[:15]
+    graph_retrieved_files = [snippet.file_path for snippet in rcm.read_only_snippets]
     if code_files_in_query:
         for file in code_files_in_query:
             # fetch direct parent and children
             representation = (
                 f"\nThe file '{file}' has the following import structure: \n"
                 + build_full_hierarchy(import_graph, file, 2)
             )
+            if graph_retrieved_files:
+                representation += "\n\nThe following modules may contain helpful services or utility functions:\n- " + "\n- ".join(graph_retrieved_files)
             rcm.add_import_trees(representation)
     # if there are no code_files_in_query, we build import trees for the top 5 snippets
     else:
         for snippet in rcm.current_top_snippets[:5]:
             file_path = snippet.file_path
             representation = (
                 f"\nThe file '{file_path}' has the following import structure: \n"
                 + build_full_hierarchy(import_graph, file_path, 2)
             )
+            if graph_retrieved_files:
+                representation += "\n\nThe following modules may contain helpful services or utility functions:\n- " + "\n-".join(graph_retrieved_files)
             rcm.add_import_trees(representation)
     return rcm
 
 
 # add any code files that appear in the query to current_top_snippets
 def add_relevant_files_to_top_snippets(rcm: RepoContextManager) -> RepoContextManager:
     code_files_in_query = rcm.relevant_file_paths
@@ -544,28 +567,26 @@
             file not in code_files_to_add
         ):
             rcm.append_relevant_file_paths(file)
     return rcm, graph
 
 
 # do not ignore repo_context_manager
-# @file_cache(ignore_params=["ticket_progress", "chat_logger"])
+# @file_cache(ignore_params=["seed", "ticket_progress", "chat_logger"])
 def get_relevant_context(
     query: str,
     repo_context_manager: RepoContextManager,
     seed: int = None,
-    ticket_progress: TicketProgress = None,
-    chat_logger: ChatLogger = None,
-):
+    import_graph: nx.DiGraph = None,
+    num_rollouts: int = NUM_ROLLOUTS,
+    ticket_progress = None,
+    chat_logger = None,
+) -> RepoContextManager:
     logger.info("Seed: " + str(seed))
     try:
-        # attempt to get import tree for relevant snippets that show up in the query
-        repo_context_manager, import_graph = parse_query_for_files(
-            query, repo_context_manager
-        )
         # for any code file mentioned in the query, build its import tree - This is currently not used
         repo_context_manager = build_import_trees(
             repo_context_manager,
             import_graph,
         )
         # for any code file mentioned in the query add it to the top relevant snippets
         repo_context_manager = add_relevant_files_to_top_snippets(repo_context_manager)
@@ -574,30 +595,30 @@
             repo_context_manager.relevant_file_paths
         )
 
         user_prompt = repo_context_manager.format_context(
             unformatted_user_prompt=unformatted_user_prompt,
             query=query,
         )
+        return repo_context_manager # Temporarily disabled context
         chat_gpt = ChatGPT()
         chat_gpt.messages = [Message(role="system", content=sys_prompt)]
-        old_top_snippets = [
-            snippet for snippet in repo_context_manager.current_top_snippets
-        ]
+        old_relevant_snippets = deepcopy(repo_context_manager.current_top_snippets)
+        old_read_only_snippets = deepcopy(repo_context_manager.read_only_snippets)
         try:
             repo_context_manager = context_dfs(
                 user_prompt,
                 repo_context_manager,
                 problem_statement=query,
+                num_rollouts=num_rollouts,
             )
         except openai.BadRequestError as e:  # sometimes means that run has expired
             logger.exception(e)
-        if len(repo_context_manager.current_top_snippets) == 0:
-            raise Exception("No snippets found")
-            repo_context_manager.current_top_snippets = old_top_snippets[:20]
+        repo_context_manager.current_top_snippets.extend(old_relevant_snippets)
+        repo_context_manager.read_only_snippets.extend(old_read_only_snippets)
         return repo_context_manager
     except Exception as e:
         logger.exception(e)
         return repo_context_manager
 
 
 def update_assistant_conversation(
@@ -624,125 +645,142 @@
 
 
 CLAUDE_MODEL = "claude-3-haiku-20240307"
 
 
 def validate_and_parse_function_calls(
     function_calls_string: str, chat_gpt: ChatGPT
-) -> list[MockFunctionCall]:
-    function_calls = MockFunctionCall.mock_function_calls_from_string(
+) -> list[AnthropicFunctionCall]:
+    function_calls = AnthropicFunctionCall.mock_function_calls_from_string(
         function_calls_string.strip("\n") + "\n</function_call>"
     )  # add end tag
     if len(function_calls) > 0:
         chat_gpt.messages[-1].content = (
             chat_gpt.messages[-1].content.rstrip("\n") + "\n</function_call>"
         )  # add end tag to assistant message
         return function_calls
 
     # try adding </invoke> tag as well
-    function_calls = MockFunctionCall.mock_function_calls_from_string(
+    function_calls = AnthropicFunctionCall.mock_function_calls_from_string(
         function_calls_string.strip("\n") + "\n</invoke>\n</function_call>"
     )
     if len(function_calls) > 0:
         # update state of chat_gpt
         chat_gpt.messages[-1].content = (
             chat_gpt.messages[-1].content.rstrip("\n") + "\n</invoke>\n</function_call>"
         )
         return function_calls
     # try adding </parameters> tag as well
-    function_calls = MockFunctionCall.mock_function_calls_from_string(
+    function_calls = AnthropicFunctionCall.mock_function_calls_from_string(
         function_calls_string.strip("\n")
         + "\n</parameters>\n</invoke>\n</function_call>"
     )
     if len(function_calls) > 0:
         # update state of chat_gpt
         chat_gpt.messages[-1].content = (
             chat_gpt.messages[-1].content.rstrip("\n")
             + "\n</parameters>\n</invoke>\n</function_call>"
         )
     return function_calls
 
 
 def handle_function_call(
-    repo_context_manager: RepoContextManager, function_call: MockFunctionCall
+    repo_context_manager: RepoContextManager, function_call: AnthropicFunctionCall, llm_state: dict[str, str]
 ):
     function_name = function_call.function_name
     function_input = function_call.function_parameters
     logger.info(f"Tool Call: {function_name} {function_input}")
-    file_path = function_input.get("file_path")
+    file_path = function_input.get("file_path", None)
     valid_path = False
     output_prefix = f"Output for {function_name}:\n"
     output = ""
-    current_read_only_snippets_string = "\n".join(
-        [snippet.denotation for snippet in repo_context_manager.read_only_snippets]
-    )
     current_top_snippets_string = "\n".join(
-        [snippet.denotation for snippet in repo_context_manager.current_top_snippets]
+        list(dict.fromkeys([snippet.file_path for snippet in repo_context_manager.current_top_snippets]))
     )
     if function_name == "code_search":
         code_entity = f'"{function_input["code_entity"]}"'  # handles cases with two words
+        code_entity = escape_ripgrep(code_entity) # escape special characters
         rg_command = [
             "rg",
             "-n",
             "-i",
             code_entity,
             repo_context_manager.cloned_repo.repo_dir,
         ]
         try:
             result = subprocess.run(
                 " ".join(rg_command), text=True, shell=True, capture_output=True
             )
             rg_output = result.stdout
             if rg_output:
                 # post process rip grep output to be more condensed
-                rg_output_pretty = post_process_rg_output(
+                rg_output_pretty, file_output_dict, file_to_num_occurrences = post_process_rg_output(
                     repo_context_manager.cloned_repo.repo_dir, SweepConfig(), rg_output
                 )
-                output = (
-                    f"SUCCESS: Here are the code_search results:\n\n{rg_output_pretty}"
-                )
+                # return results first by occurrences then by alphabetical order
+                non_stored_files = sorted([
+                    file_path
+                    for file_path in file_output_dict
+                    if file_path not in repo_context_manager.top_snippet_paths
+                ], key=lambda x: (-file_to_num_occurrences[x], x))
+                non_stored_files = [file_path + f" ({file_to_num_occurrences[file_path]} occurrences)" for file_path in non_stored_files]
+                non_stored_files_string = "These search results have not been stored:\n<non_stored_search_results>\n" + "\n".join(non_stored_files) + "\n</non_stored_search_results>\n" if non_stored_files else "All of the files above have already been stored. Search for a new term.\n"
+                if len(file_output_dict) <= 10:
+                    output = (
+                        f"SUCCESS: Here are the code_search results:\n<code_search_results>\n{rg_output_pretty}<code_search_results>\n" +
+                        non_stored_files_string + 
+                        "Use the `view_files` tool to read the most relevant non-stored files. Use `store_file` to add any important non-stored files to the context. DO NOT VIEW FILES THAT HAVE BEEN STORED."
+                    )
+                else:
+                    output = (
+                        f"SUCCESS: Here are the code_search results:\n<code_search_results>\n{rg_output_pretty}<code_search_results>\n" +
+                        non_stored_files_string + "Prioritize viewing the non-stored files with the most occurrences. Use the `view_files` tool to read the most relevant non-stored files. Use `store_file` to add any important non-stored files to the context. DO NOT VIEW FILES THAT HAVE BEEN STORED."
+                    )
+                # too many prompt it to search more specific
             else:
-                output = f"FAILURE: No results found for code_entity: {code_entity} in the entire codebase. Please try a new code_entity. If you are searching for a function defintion try again with different whitespaces."
+                output = f"FAILURE: No results found for code_entity: {code_entity} in the entire codebase. Please try a new code_entity. Consider trying different whitespace or a truncated version of this code_entity."
         except Exception as e:
             logger.error(
                 f"FAILURE: An Error occured while trying to find the code_entity {code_entity}: {e}"
             )
-            output = f"FAILURE: An Error occured while trying to find the code_entity {code_entity}: {e}"
-    elif function_name == "view_file":
-        try:
-            file_contents = repo_context_manager.cloned_repo.get_file_contents(
-                file_path
-            )
-            valid_path = True
-            if (
-                file_path in current_read_only_snippets_string
-                and file_path in current_top_snippets_string
-                and valid_path
-            ):
-                output = f"FAILURE: {file_path} is already in the selected snippets."
-            elif valid_path:
-                suffix = f'\nIf you are CERTAIN this file is RELEVANT, call store_file with the same parameters ({{"file_path": "{file_path}"}}).'
-                output = f'Here are the contents of `{file_path}:`\n```\n{file_contents}\n```'
+            output = f"FAILURE: No results found for code_entity: {code_entity} in the entire codebase. Please try a new code_entity. Consider trying different whitespace or a truncated version of this code_entity."
+    elif function_name == "view_files":
+        output = ""
+        all_viewed_files = [function_input.get("first_file_path", ""), function_input.get("second_file_path", ""), function_input.get("file_path", "")]
+        all_viewed_files = [file_path for file_path in all_viewed_files if file_path]
+        for file_path in all_viewed_files:
+            try:
+                file_contents = repo_context_manager.cloned_repo.get_file_contents(
+                    file_path
+                )
+                # check if file has been viewed already
+                # function_call_history = llm_state.get("function_call_history", [])
+                # # unnest 2d list
+                # previous_function_calls = [
+                #     call for sublist in function_call_history for call in sublist
+                # ]
+                # previously_viewed_files = list(dict.fromkeys(previously_viewed_files))
+                # if file_path in previously_viewed_files:
+                #     previously_viewed_files_str = "\n".join(previously_viewed_files)
+                #     output = f"WARNING: `{file_path}` has already been viewed. Please refer to the file in your previous function call. These files have already been viewed:\n{previously_viewed_files_str}"
                 if file_path not in [snippet.file_path for snippet in repo_context_manager.current_top_snippets]:
-                    output += suffix
-            else:
-                output = (
-                    "FAILURE: This file path does not exist. Please try a new path."
+                    output += f'SUCCESS: Here are the contents of `{file_path}`:\n<source>\n{file_contents}\n</source>\nYou can use the `store_file` tool to add this file to the context.'
+                else:
+                    output += f"FAILURE: {file_path} has already been stored. Please view a new file."
+            except FileNotFoundError:
+                file_contents = ""
+                similar_file_paths = "\n".join(
+                    [
+                        f"- {path}"
+                        for path in repo_context_manager.cloned_repo.get_similar_file_paths(
+                            file_path
+                        )
+                    ]
                 )
-        except FileNotFoundError:
-            file_contents = ""
-            similar_file_paths = "\n".join(
-                [
-                    f"- {path}"
-                    for path in repo_context_manager.cloned_repo.get_similar_file_paths(
-                        file_path
-                    )
-                ]
-            )
-            output = f"FAILURE: This file path does not exist. Did you mean:\n{similar_file_paths}"
+                output += f"FAILURE: {file_path} does not exist. Did you mean:\n{similar_file_paths}\n"
     elif function_name == "store_file":
         try:
             file_contents = repo_context_manager.cloned_repo.get_file_contents(
                 file_path
             )
             valid_path = True
         except Exception:
@@ -759,181 +797,212 @@
         else:
             snippet = Snippet(
                 file_path=file_path,
                 start=0,
                 end=len(file_contents.splitlines()),
                 content=file_contents,
             )
-            if snippet.denotation in current_top_snippets_string:
-                output = f"FAILURE: {file_path} is already in the selected snippets."
+            if snippet.file_path in current_top_snippets_string:
+                output = f"FAILURE: {get_stored_files(repo_context_manager)}"
             else:
                 repo_context_manager.add_snippets([snippet])
                 current_top_snippets_string = "\n".join(
-                    [
-                        snippet.denotation
-                        for snippet in repo_context_manager.current_top_snippets
-                    ]
+                    list(dict.fromkeys([snippet.file_path for snippet in repo_context_manager.current_top_snippets]))
                 )
                 output = (
-                    f"SUCCESS: {file_path} was added. Here are the current selected snippets that will either be modified or use in the code change:\n{current_top_snippets_string}"
+                    f"SUCCESS: {file_path} was added to the stored_files. It will be used as a reference or modified to resolve the issue."
                     if valid_path
-                    else "FAILURE: This file path does not exist. Please try a new path."
+                    else f"FAILURE: The file path '{file_path}' does not exist. Please check the path and try again."
                 )
-    elif function_name == "preview_file":
-        try:
-            code = repo_context_manager.cloned_repo.get_file_contents(file_path)
-            valid_path = True
-        except Exception:
-            code = ""
-            similar_file_paths = "\n".join(
-                [
-                    f"- {path}"
-                    for path in repo_context_manager.cloned_repo.get_similar_file_paths(
-                        file_path
-                    )
-                ]
-            )
-            output = f"FAILURE: This file path does not exist. Did you mean:\n{similar_file_paths}"
-        else:
-            file_preview = CodeTree.from_code(code).get_preview()
-            output = f"SUCCESS: Previewing file {file_path}:\n\n{file_preview}"
-    elif function_name == "draft_plan":
-        output = "SUCCESS: Now let's validate all the details such as the signatures of functions and classes and names of attributes by searching the codebase."
     elif function_name == "submit":
         plan = function_input.get("plan")
         repo_context_manager.update_issue_report_and_plan(f"# Highly Suggested Plan:\n\n{plan}\n\n")
-        issue_report = ""
-        issue_plan = function_input.get("plan")
         output = PLAN_SUBMITTED_MESSAGE
-    elif function_name == "submit_report_and_plan":
-        if "report" not in function_input or "plan" not in function_input:
-            output = "FAILURE: Please provide a report and a plan."
-        else:
-            issue_report = function_input["report"]
-            issue_plan = function_input["plan"]
-            repo_context_manager.update_issue_report_and_plan(
-                f"#Report of Issue:\n\n{issue_report}\n\n#High Level Plan:\n\n{issue_plan}\n\n"
-            )
-            output = PLAN_SUBMITTED_MESSAGE
     else:
         output = f"FAILURE: Invalid tool name {function_name}"
-    justification = (
-        function_input["justification"] if "justification" in function_input else ""
+    analysis = (
+        function_input["analysis"] if "analysis" in function_input else ""
     )
     logger.info(
-        f"Tool Call: {function_name} {justification} Valid Tool Call: {valid_path}"
+        f"Tool Call: {function_name}\n{analysis}\n{output}"
     )
-    return output_prefix + output
+    return (output_prefix + output)
 
 
 reflections_prompt_prefix = """
 CRITICAL FEEDBACK - READ CAREFULLY AND ADDRESS ALL POINTS
 <critical_feedback_to_address>
-Here is the feedback from your previous attempt. You MUST read this extremely carefully and follow ALL of the reviewer's advice. If they tell you to store specific files, store and view all of those first. If you do not fully address this feedback you will fail to retrieve all of the relevant files.
+Here is the feedback from your previous attempt. You MUST read this extremely carefully and follow ALL of the reviewer's advice. If they tell you to store specific files, view store them first. If you do not fully address this feedback you will fail to retrieve all of the relevant files.
 {all_reflections}
 </critical_feedback_to_address>"""
 
 reflection_prompt = """<attempt_and_feedback_{idx}>
 <previous_files_stored>
 Files stored from previous attempt:
 {files_read}
 </previous_files_stored>
+<rating>
+Rating from previous attempt: {score} / 10
+</rating>
 <feedback>
 Reviewer feedback on previous attempt:
 {reflections_string}
 </feedback>
 </attempt_and_feedback_{idx}>"""
 
+def format_reflections(reflections_to_gathered_files: dict[str, tuple[list[str], int]]) -> str:
+    formatted_reflections_prompt = ""
+    if not reflections_to_gathered_files:
+        return formatted_reflections_prompt
+    all_reflections_string = "\n"
+    # take only the MAX_REFLECTIONS sorted by score
+    top_reflections = sorted(
+        reflections_to_gathered_files.items(), key=lambda x: x[1][1] * 100 + len(x[1][0]), reverse=True # break ties by number of files stored
+    )[:MAX_REFLECTIONS]
+    for idx, (reflection, (gathered_files, score)) in enumerate(top_reflections):
+        formatted_reflection = reflection_prompt.format(
+            files_read="\n".join(gathered_files),
+            reflections_string=reflection,
+            score=str(score),
+            idx=str(idx + 1),
+        )
+        all_reflections_string += f"\n{formatted_reflection}"
+    formatted_reflections_prompt = reflections_prompt_prefix.format(
+        all_reflections=all_reflections_string
+    )
+    return formatted_reflections_prompt
+
+def render_all_attempts(function_call_histories: list[list[list[AnthropicFunctionCall]]]) -> str:
+    formatted_attempts = ""
+    for idx, function_call_history in enumerate(function_call_histories):
+        formatted_function_calls = render_function_calls_for_attempt(function_call_history)
+        formatted_attempts += f"<attempt_{idx}>\n{formatted_function_calls}\n</attempt_{idx}>"
+    return formatted_attempts
+
+def render_function_calls_for_attempt(function_call_history: list[list[AnthropicFunctionCall]]) -> str:
+    formatted_function_calls = ""
+    idx = 0
+    for function_calls in function_call_history:
+        for function_call in function_calls:
+            function_call.function_parameters.pop("analysis", None) # remove analysis
+            function_call_cleaned_string = function_call.function_name + " | " + "\n".join([str(k) + " | " + str(v) for k, v in function_call.function_parameters.items()])
+            formatted_function_calls += f"- {function_call_cleaned_string}\n"
+        if function_calls:
+            idx += 1
+    return formatted_function_calls
+
+def get_stored_files(repo_context_manager: RepoContextManager) -> str:
+    fetched_files_that_are_stored = list(dict.fromkeys([snippet.file_path for snippet in repo_context_manager.current_top_snippets]))
+    joined_files_string = "\n".join(fetched_files_that_are_stored)
+    stored_files_string = f'The following files have been stored already. DO NOT CALL THE STORE OR VIEW TOOLS ON THEM AGAIN. \n<stored_files>\n{joined_files_string}\n</stored_files>\n' if fetched_files_that_are_stored else ""
+    return stored_files_string
+
+def search_for_context_with_reflection(repo_context_manager: RepoContextManager, reflections_to_read_files: dict[str, tuple[list[str], int]], user_prompt: str, rollout_function_call_histories: list[list[list[AnthropicFunctionCall]]], problem_statement: str) -> tuple[list[Message], list[list[AnthropicFunctionCall]]]:
+    try:
+        _, function_call_history = perform_rollout(repo_context_manager, reflections_to_read_files, user_prompt)
+        rollout_function_call_histories.append(function_call_history)
+    except Exception as e:
+        logger.error(f"Error in perform_rollout: {e}")
+    rollout_stored_files = [snippet.file_path for snippet in repo_context_manager.current_top_snippets]
+    # truncated_message_results = message_results[1:] # skip system prompt
+    # joined_messages = "\n\n".join([message.content for message in truncated_message_results])
+    # overall_score, message_to_contractor = EvaluatorAgent().evaluate_run(
+    #     problem_statement=problem_statement, 
+    #     run_text=joined_messages,
+    #     stored_files=rollout_stored_files,
+    # )
+    return 0, "", repo_context_manager, rollout_stored_files
+
+def perform_rollout(repo_context_manager: RepoContextManager, reflections_to_gathered_files: dict[str, tuple[list[str], int]], user_prompt: str) -> list[Message]:
+    function_call_history = []
+    formatted_reflections_prompt = format_reflections(reflections_to_gathered_files)
+    updated_user_prompt = user_prompt + formatted_reflections_prompt
+    chat_gpt = ChatGPT()
+    chat_gpt.messages = [Message(role="system", content=sys_prompt + formatted_reflections_prompt)]
+    function_calls_string = chat_gpt.chat_anthropic(
+        content=updated_user_prompt,
+        stop_sequences=["</function_call>"],
+        model=CLAUDE_MODEL,
+        message_key="user_request",
+        assistant_message_content="<function_call>",
+    )
+    bad_call_count = 0
+    llm_state = {} # persisted across one rollout
+    llm_state["function_call_history"] = {}
+    for _ in range(MAX_ITERATIONS):
+        function_calls = validate_and_parse_function_calls(
+            function_calls_string, chat_gpt
+        )
+        function_outputs = ""
+        for function_call in function_calls[:MAX_PARALLEL_FUNCTION_CALLS]:
+            function_outputs += handle_function_call(repo_context_manager, function_call, llm_state) + "\n"
+            logger.info(f"Function outputs: {function_outputs}")
+            logger.info("Function call: " + str(function_call))
+            llm_state["function_call_history"] = function_call_history
+            if PLAN_SUBMITTED_MESSAGE in function_outputs:
+                return chat_gpt.messages, function_call_history
+        function_call_history.append(function_calls)
+        if len(function_calls) == 0:
+            function_outputs = "REMINDER: No function calls were made or your last function call was incorrectly formatted. The correct syntax for function calling is this:\n" \
+                + "<function_call>\n<invoke>\n<tool_name>tool_name</tool_name>\n<parameters>\n<param_name>param_value</param_name>\n</parameters>\n</invoke>\n</function_call>" + "\nRemember to gather ALL relevant files. " + get_stored_files(repo_context_manager)
+            bad_call_count += 1
+        if function_outputs.startswith("FAILURE"):
+            bad_call_count += 1
+        if bad_call_count >= NUM_BAD_FUNCTION_CALLS:
+            return chat_gpt.messages, function_call_history
+        if len(function_calls) > MAX_PARALLEL_FUNCTION_CALLS:
+            remaining_function_calls = function_calls[MAX_PARALLEL_FUNCTION_CALLS:]
+            remaining_function_calls_string = mock_function_calls_to_string(remaining_function_calls)
+            function_outputs += "WARNING: You requested more than 1 function call at once. Only the first function call has been processed. The unprocessed function calls were:\n<unprocessed_function_call>\n" + remaining_function_calls_string + "\n</unprocessed_function_call>"
+        try:
+            function_calls_string = chat_gpt.chat_anthropic(
+                content=function_outputs,
+                model=CLAUDE_MODEL,
+                stop_sequences=["</function_call>"],
+                assistant_message_content="<function_call>",
+            )
+        except Exception as e:
+            logger.error(f"Error in chat_anthropic: {e}")
+            # return all but the last message because it likely causes an error
+            return chat_gpt.messages[:-1], function_call_history
+    return chat_gpt.messages, function_call_history
 
 def context_dfs(
     user_prompt: str,
     repo_context_manager: RepoContextManager,
     problem_statement: str,
+    num_rollouts: int,
 ) -> bool | None:
-    max_iterations = 30 # Tuned to 30 because haiku is cheap
-    # NUM_ROLLOUTS = 5
-    NUM_ROLLOUTS = 2
-    repo_context_manager.current_top_snippets = []
     # initial function call
     reflections_to_read_files = {}
     rollouts_to_scores_and_rcms = {}
-    def perform_rollout(repo_context_manager: RepoContextManager, reflections_to_gathered_files: dict[str, list[str]] = {}):
-        chat_gpt = ChatGPT()
-        chat_gpt.messages = [Message(role="system", content=sys_prompt)]
-        if reflections_to_gathered_files:
-            all_reflections_string = ""
-            for idx, (reflection, gathered_files) in enumerate(reflections_to_gathered_files.items()):
-                formatted_reflection = reflection_prompt.format(
-                    files_read="\n".join(gathered_files),
-                    reflections_string=reflection,
-                    idx=str(idx + 1),
-                )
-                all_reflections_string += f"\n{formatted_reflection}"
-            formatted_reflections_prompt = reflections_prompt_prefix.format(
-                all_reflections=all_reflections_string
-            )
-            updated_user_prompt = user_prompt + "\n" + formatted_reflections_prompt
-        else:
-            updated_user_prompt = user_prompt
-        function_calls_string = chat_gpt.chat_anthropic(
-            content=updated_user_prompt,
-            stop_sequences=["</function_call>"],
-            model=CLAUDE_MODEL,
-            message_key="user_request",
-        )
-        bad_call_count = 0
-        for _ in range(max_iterations):
-            function_calls = validate_and_parse_function_calls(
-                function_calls_string, chat_gpt
-            )
-            for function_call in function_calls:
-                function_output = handle_function_call(repo_context_manager, function_call)
-                if PLAN_SUBMITTED_MESSAGE in function_output:
-                    return chat_gpt.messages
-            if len(function_calls) == 0:
-                function_output = "No function calls were made or your last function call was incorrectly formatted. The correct syntax for function calling is this:\n" \
-                    + "<function_call>\n<invoke>\n<tool_name>tool_name</tool_name>\n<parameters>\n<param_name>param_value</param_name>\n</parameters>\n</invoke>\n</function_call>" + "\n\nIf you would like to submit the plan, call the submit function."
-                bad_call_count += 1
-                if bad_call_count >= 3:
-                    return chat_gpt.messages # set to three, which seems alright
-            try:
-                function_calls_string = chat_gpt.chat_anthropic(
-                    content=function_output,
-                    model=CLAUDE_MODEL,
-                    stop_sequences=["</function_call>"],
-                )
-            except Exception as e:
-                logger.error(f"Error in chat_anthropic: {e}")
-                # return all but the last message because it likely causes an error
-                return chat_gpt.messages[:-1]
-        return chat_gpt.messages
-    for rollout_idx in range(NUM_ROLLOUTS):
-        # operate on a deep copy of the repo context manager
-        copied_repo_context_manager = deepcopy(repo_context_manager)
-        message_results = perform_rollout(copied_repo_context_manager, reflections_to_read_files)
-        rollout_stored_files = [snippet.file_path for snippet in copied_repo_context_manager.current_top_snippets]
-        truncated_message_results = message_results[1:] # skip system prompt
-        joined_messages = "\n\n".join([message.content for message in truncated_message_results])
-        overall_score, message_to_contractor = EvaluatorAgent().evaluate_run(
-            problem_statement=problem_statement, 
-            run_text=joined_messages,
-            stored_files=rollout_stored_files,
+    rollout_function_call_histories = []
+    for rollout_idx in range(num_rollouts):
+        overall_score, message_to_contractor, repo_context_manager, rollout_stored_files = search_for_context_with_reflection(
+            repo_context_manager=repo_context_manager,
+            reflections_to_read_files=reflections_to_read_files,
+            user_prompt=user_prompt,
+            rollout_function_call_histories=rollout_function_call_histories,
+            problem_statement=problem_statement
         )
         logger.info(f"Completed run {rollout_idx} with score: {overall_score} and reflection: {message_to_contractor}")
         if overall_score is None or message_to_contractor is None:
             continue # can't get any reflections here
-        reflections_to_read_files[message_to_contractor] = rollout_stored_files
-        rollouts_to_scores_and_rcms[rollout_idx] = (overall_score, copied_repo_context_manager)
-        if overall_score >= 8:
+        # reflections_to_read_files[message_to_contractor] = rollout_stored_files, overall_score
+        rollouts_to_scores_and_rcms[rollout_idx] = (overall_score, repo_context_manager)
+        if overall_score >= SCORE_THRESHOLD and len(rollout_stored_files) > STOP_AFTER_SCORE_THRESHOLD_IDX:
             break
     # if we reach here, we have not found a good enough solution
     # select rcm from the best rollout
+    logger.info(f"{render_all_attempts(rollout_function_call_histories)}")
     all_scores_and_rcms = list(rollouts_to_scores_and_rcms.values())
-    best_score, best_rcm = max(all_scores_and_rcms, key=lambda x: x[0])
-    logger.info(f"Best score: {best_score}")
+    best_score, best_rcm = max(all_scores_and_rcms, key=lambda x: x[0] * 100 + len(x[1].current_top_snippets)) # sort first on the highest score, break ties with length of current_top_snippets
+    for score, rcm in all_scores_and_rcms:
+        logger.info(f"Rollout score: {score}, Rollout files: {[snippet.file_path for snippet in rcm.current_top_snippets]}")
+    logger.info(f"Best score: {best_score}, Best files: {[snippet.file_path for snippet in best_rcm.current_top_snippets]}")
     return best_rcm
 
 if __name__ == "__main__":
     try:
         from sweepai.utils.github_utils import get_installation_id
         from sweepai.utils.ticket_utils import prep_snippets
```

### Comparing `sweepai-2.0.0.dev1/sweepai/core/entities.py` & `sweepai-2.0.1/sweepai/core/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import string
 from dataclasses import dataclass
 from difflib import unified_diff
 from typing import Any, ClassVar, Literal, Type, TypeVar
 from urllib.parse import quote
 
 from loguru import logger
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from sweepai.utils.str_utils import (
     blockquote,
     clean_logs,
     create_collapsible,
     format_sandbox_success,
 )
@@ -143,14 +143,15 @@
         | Literal["rename"]
         | Literal["rewrite"]
         | Literal["check"]
         | Literal["refactor"]
         | Literal["test"]
     )
     _regex = r"""<(?P<change_type>[a-z_]+)\s+file=\"(?P<filename>[a-zA-Z0-9/\\\.\[\]\(\)\_\+\- @\{\}]*?)\"( start_line=\"(?P<start_line>.*?)\")?( end_line=\"(?P<end_line>.*?)\")?( entity=\"(.*?)\")?( source_file=\"(?P<source_file>.*?)\")?( destination_module=\"(?P<destination_module>.*?)\")?( relevant_files=\"(?P<raw_relevant_files>.*?)\")?(.*?)>(?P<instructions>.*?)\s*<\/\1>"""
+    is_completed: bool = False
     entity: str | None = None
     source_file: str | None = None
     old_content: str | None = None
     new_content: str | None = None
     raw_relevant_files: str | None = None
     # allow inf
     start_line: Any | int | str | None = None
@@ -238,16 +239,14 @@
         return f"{self.change_type.capitalize()} `{self.filename}`"
 
     @property
     def summary(self):
         prefix = {"failed": "✗", "succeeded": "✓", "queued": "▶", "running": "⋯"}[
             self.status
         ] + " "
-        if self.change_type == "check":
-            return prefix + f"Run GitHub Actions for `{self.filename}`"
         return prefix + f"{self.change_type.capitalize()}\n{self.filename}"
 
     @property
     def color(self):
         color_map = {
             "failed": "red2",
             "succeeded": "#0ee832",
@@ -349,19 +348,20 @@
     title: str
     body: str
     issue_id: int | None = None
     _regex = r'<issue\s+title="(?P<title>.*?)">(?P<body>.*?)</issue>'
 
 
 class Snippet(BaseModel):
+    # pylint: disable=E1101
     """
     Start and end refer to line numbers
     """
 
-    content: str
+    content: str = Field(repr=False)
     start: int
     end: int
     file_path: str
 
     def __eq__(self, other):
         if isinstance(other, Snippet):
             return (
```

### Comparing `sweepai-2.0.0.dev1/sweepai/core/external_searcher.py` & `sweepai-2.0.1/sweepai/core/external_searcher.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/core/lexical_search.py` & `sweepai-2.0.1/sweepai/core/lexical_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,20 +272,26 @@
         return res
     except SystemExit:
         raise SystemExit
     except Exception as e:
         logger.exception(e)
         return {}
 
+SNIPPET_FORMAT = """File path: {file_path}
 
-@file_cache(ignore_params=["snippets"])
+{contents}"""
+
+# @file_cache(ignore_params=["snippets"])
 def compute_vector_search_scores(queries: list[str], snippets: list[Snippet]):
     # get get dict of snippet to score
     snippet_str_to_contents = {
-        snippet.denotation: snippet.get_snippet(add_ellipsis=False, add_lines=False)
+        snippet.denotation: SNIPPET_FORMAT.format(
+            file_path=snippet.file_path,
+            contents=snippet.get_snippet(add_ellipsis=False, add_lines=False),
+        )
         for snippet in snippets
     }
     snippet_contents_array = list(snippet_str_to_contents.values())
     multi_query_snippet_similarities = multi_get_query_texts_similarity(
         queries, snippet_contents_array
     )
     snippet_denotations = [snippet.denotation for snippet in snippets]
```

### Comparing `sweepai-2.0.0.dev1/sweepai/core/post_merge.py` & `sweepai-2.0.1/sweepai/core/post_merge.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/core/pr_reader.py` & `sweepai-2.0.1/sweepai/core/pr_reader.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/core/repo_parsing_utils.py` & `sweepai-2.0.1/sweepai/core/repo_parsing_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,25 +99,25 @@
     directory: str, sweep_config: SweepConfig
 ) -> tuple[list[Snippet], list[str]]:
     dir_file_count = {}
 
     def is_dir_too_big(file_name):
         dir_name = os.path.dirname(file_name)
         only_file_name = os.path.basename(dir_name)
-        if only_file_name in ("node_modules", "venv", "patch"):
+        if only_file_name in ("node_modules", ".venv", "build", "venv", "patch"):
             return True
         if dir_name not in dir_file_count:
             dir_file_count[dir_name] = len(os.listdir(dir_name))
         return dir_file_count[dir_name] > FILE_THRESHOLD
 
     logger.info(f"Reading files from {directory}")
     vis = set()
     def dfs(file_path: str = directory):
         only_file_name = os.path.basename(file_path)
-        if only_file_name in ("node_modules", "venv", "patch"):
+        if only_file_name in ("node_modules", ".venv", "build", "venv", "patch"):
             return
         if file_path in vis:
             return
         vis.add(file_path)
         if os.path.isdir(file_path):
             for file_name in os.listdir(file_path):
                 for sub_file_path in dfs(os.path.join(file_path, file_name)):
```

### Comparing `sweepai-2.0.0.dev1/sweepai/core/update_prompts.py` & `sweepai-2.0.1/sweepai/core/update_prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/core/vector_db.py` & `sweepai-2.0.1/sweepai/core/vector_db.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,25 +11,24 @@
 from redis import Redis
 from tqdm import tqdm
 import voyageai
 import boto3
 from botocore.exceptions import ClientError
 from voyageai import error as voyageai_error
 
-from sweepai.config.server import BATCH_SIZE, REDIS_URL, VOYAGE_API_AWS_ACCESS_KEY, VOYAGE_API_AWS_ENDPOINT_NAME, VOYAGE_API_AWS_REGION, VOYAGE_API_AWS_SECRET_KEY, VOYAGE_API_KEY, VOYAGE_API_USE_AWS
+from sweepai.config.server import BATCH_SIZE, REDIS_URL, VOYAGE_API_AWS_ENDPOINT_NAME, VOYAGE_API_KEY, VOYAGE_API_USE_AWS
 from sweepai.utils.hash import hash_sha256
 from sweepai.utils.openai_proxy import get_embeddings_client
 from sweepai.utils.utils import Tiktoken
 
 # Now uses Voyage AI if available, with asymmetric embedding
 # CACHE_VERSION = "v2.0.04" + "-voyage" if VOYAGE_API_KEY else ""
 suffix = "-voyage-aws" if VOYAGE_API_USE_AWS else "-voyage" if VOYAGE_API_KEY else ""
-CACHE_VERSION = "v2.0.05" + suffix 
-redis_client: Redis = None
-# redis_client: Redis = Redis.from_url(REDIS_URL)  # TODO: add lazy loading
+CACHE_VERSION = "v2.0.07" + suffix 
+redis_client: Redis = Redis.from_url(REDIS_URL)  # TODO: add lazy loading
 tiktoken_client = Tiktoken()
 
 
 def cosine_similarity(a, B):
     """
     Updated to handle multi-queries.
     """
@@ -70,24 +69,49 @@
         if norm == 0:
             return x
         return x / norm
     else:
         norm = np.linalg.norm(x, 2, axis=1, keepdims=True)
         return np.where(norm == 0, x, x / norm)
 
+def batch_by_token_count_for_voyage(
+    texts: list[str],
+    max_tokens: int = 120_000,
+    max_length: int = 128,
+) -> list[list[str]]:
+    """
+    This function splits the texts into batches based on the token count.
+    Max token count for Voyage is 120k and max batch length count is 128.
+    """
+    client = voyageai.Client()
+    batches = []
+    batch = []
+    token_count = 0
+    for text in texts:
+        text_token_count = client.count_tokens([text])
+        if token_count + text_token_count > max_tokens * 0.95 or len(batch) >= max_length:
+            batches.append(batch)
+            batch = [text]  # Start the new batch with the current text
+            token_count = text_token_count  # Reset token count for the new batch
+        else:
+            batch.append(text)
+            token_count += text_token_count
+    if batch:
+        batches.append(batch)
+    del client
+    return batches
 
 # lru_cache(maxsize=20)
 # @redis_cache()
 def embed_text_array(texts: tuple[str]) -> list[np.ndarray]:
-    VOYAGE_API_KEY = os.environ.get("VOYAGE_API_KEY", None)
     embeddings = []
     texts = [text if text else " " for text in texts]
     batches = [texts[i : i + BATCH_SIZE] for i in range(0, len(texts), BATCH_SIZE)]
-    workers = max(1, multiprocessing.cpu_count() // 4)
-    if workers > 1 and not VOYAGE_API_KEY:
+    workers = min(max(1, multiprocessing.cpu_count() // 4), 1)
+    if workers > 1:
         with multiprocessing.Pool(
             processes=workers
         ) as pool:
             embeddings = list(
                 tqdm(
                     pool.imap(openai_with_expo_backoff, batches),
                     total=len(batches),
@@ -128,32 +152,31 @@
         )
         body = response["Body"]
         obj = json.load(body)
         data = obj["data"]
         return np.array([vector["embedding"] for vector in data])
     elif VOYAGE_API_KEY:
         client = voyageai.Client(api_key=VOYAGE_API_KEY)
-        result = client.embed(batch, model="voyage-code-2", input_type=input_type)
+        result = client.embed(batch, model="voyage-code-2", input_type=input_type, truncation=True)
         cut_dim = np.array([data for data in result.embeddings])
         normalized_dim = normalize_l2(cut_dim)
+        del client
         return normalized_dim
     else:
         client = get_embeddings_client()
         response = client.embeddings.create(
             input=batch, model="text-embedding-3-small", encoding_format="float"
         )
         cut_dim = np.array([data.embedding for data in response.data])[:, :512]
         normalized_dim = normalize_l2(cut_dim)
         # save results to redis
         return normalized_dim
 
 def openai_call_embedding(batch: list[str], input_type: str="document"):
     # Backoff on batch size by splitting the batch in half.
-    # Better way is to download the tokenizer from https://huggingface.co/voyageai/voyage
-    # and check the token count manually, but it requires an extra dependency. 
     try:
         return openai_call_embedding_router(batch, input_type)
     except (voyageai_error.InvalidRequestError, ClientError) as e: # full error is botocore.errorfactory.ModelError: but I can't find it
         if len(batch) > 1 and "Please lower the number of tokens in the batch." in str(e):
             logger.error(f"Token count exceeded for batch: {max([tiktoken_client.count(text) for text in batch])} retrying by splitting batch in half.")
             mid = len(batch) // 2
             left = openai_call_embedding(batch[:mid], input_type)
```

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/create_pr.py` & `sweepai-2.0.1/sweepai/handlers/create_pr.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 def create_pr_changes(
     file_change_requests: list[FileChangeRequest],
     pull_request: PullRequest,
     sweep_bot: SweepBot,
     username: str,
     installation_id: int,
     issue_number: int | None = None,
-    sandbox=None,
     chat_logger: ChatLogger = None,
     base_branch: str = None,
     additional_messages: list[Message] = []
 ) -> Generator[tuple[FileChangeRequest, int, Any], None, dict]:
     # Flow:
     # 1. Get relevant files
     # 2: Get human message
@@ -97,28 +96,27 @@
             pull_request.branch_name, base_branch=base_branch
         )
         completed_count, fcr_count = 0, len(file_change_requests)
 
         blocked_dirs = get_blocked_dirs(sweep_bot.repo)
 
         for (
-            file_change_request,
+            new_file_contents,
             changed_file,
-            sandbox_error,
             commit,
             file_change_requests,
         ) in sweep_bot.change_files_in_github_iterator(
             file_change_requests,
             pull_request.branch_name,
             blocked_dirs,
             additional_messages=additional_messages
         ):
-            completed_count += changed_file
+            completed_count += len(new_file_contents or [])
             logger.info(f"Completed {completed_count}/{fcr_count} files")
-            yield file_change_request, changed_file, sandbox_error, commit, file_change_requests
+            yield new_file_contents, changed_file, commit, file_change_requests
         if completed_count == 0 and fcr_count != 0:
             logger.info("No changes made")
             posthog.capture(
                 username,
                 "failed",
                 properties={
                     "error": "No changes made",
@@ -194,15 +192,15 @@
             pr_head=pull_request.branch_name,
             base=sweep_bot.repo.get_branch(
                 SweepConfig.get_branch(sweep_bot.repo)
             ).commit,
             head=sweep_bot.repo.get_branch(pull_request.branch_name).commit,
         ),
     }
-    yield result  # Doing this because sometiems using StopIteration doesn't work, kinda jank tho tbh
+    yield result # TODO: refactor this as it doesn't need to be an iterator
     return
 
 
 def safe_delete_sweep_branch(
     pr,  # Github PullRequest
     repo: Repository,
 ) -> bool:
```

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/on_button_click.py` & `sweepai-2.0.1/sweepai/handlers/on_button_click.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/on_button_click_test.py` & `sweepai-2.0.1/sweepai/handlers/on_button_click_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/on_check_suite.py` & `sweepai-2.0.1/sweepai/handlers/on_check_suite.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import time
 import zipfile
 
 import requests
 
 from sweepai.config.client import get_gha_enabled
 from sweepai.core.entities import PRChangeRequest
+from sweepai.logn.cache import file_cache
 from sweepai.utils.github_utils import get_github_client, get_token
 from sweepai.web.events import CheckRunCompleted
 
 log_message = """GitHub actions yielded the following error.
 
 {error_logs}
 
@@ -28,14 +29,15 @@
     return [
         file
         for file in zipfile.namelist()
         if file.startswith(dir) and not file.endswith("/")
     ]
 
 
+@file_cache()
 def download_logs(repo_full_name: str, run_id: int, installation_id: int):
     token = get_token(installation_id)
     headers = {
         "Accept": "application/vnd.github+json",
         "Authorization": f"Bearer {token}",
         "X-GitHub-Api-Version": "2022-11-28",
     }
@@ -53,33 +55,41 @@
                 with zip_file.open(file) as f:
                     logs = f.read().decode("utf-8")
                     last_line = logs.splitlines()[-1]
                     if "##[error]" in last_line:
                         logs_str += logs
     return logs_str
 
+gha_prompt = """\
+The below command yielded the following errors:
+<command>
+{command_line}
+</command>
+{error_content}
+Here are the logs:
+<logs>
+{cleaned_logs_str}
+</logs>"""
+
 
 def clean_gh_logs(logs_str: str):
     # Extraction process could be better
-    MAX_LINES = 50
+    MAX_LINES = 500
+    LINES_TO_KEEP = 100
     log_list = logs_str.split("\n")
     truncated_logs = [log[log.find(" ") + 1 :] for log in log_list]
     logs_str = "\n".join(truncated_logs)
     # extract the group and delete everything between group and endgroup
     gha_pattern = r"##\[group\](.*?)##\[endgroup\](.*?)(##\[error\].*)"
     match = re.search(gha_pattern, logs_str, re.DOTALL)
-
-    # Extract the matched groups
     if not match:
-        return "", ""
-    group_start = match.group(1).strip()
-    command_line = group_start.split("\n")[0]
+        return "\n".join(logs_str.split("\n")[:MAX_LINES])
+    command_line = match.group(1).strip()
     log_content = match.group(2).strip()
-    error_line = match.group(3).strip()
-
+    error_line = match.group(3).strip() # can be super long
     patterns = [
         # for docker
         "Already exists",
         "Pulling fs layer",
         "Waiting",
         "Download complete",
         "Verifying Checksum",
@@ -103,34 +113,28 @@
     ]
     cleaned_logs = [
         log.strip()
         for log in log_content.split("\n")
         if not any(log.strip().startswith(pattern) for pattern in patterns)
     ]
     if len(cleaned_logs) > MAX_LINES:
-        return "", ""
+        # return the first LINES_TO_KEEP and the last LINES_TO_KEEP
+        cleaned_logs = cleaned_logs[:LINES_TO_KEEP] + ["..."] + cleaned_logs[-LINES_TO_KEEP:]
     cleaned_logs_str = "\n".join(cleaned_logs)
-    cleaned_response = f"""\
-The command:
-{command_line}
-yielded the following error:
+    error_content = ""
+    if len(error_line) < 2000:
+        error_content = f"""<errors>
 {error_line}
-
-Here are the logs:
-{cleaned_logs_str}"""
-    response_for_user = f"""\
-The command:
-`{command_line}`
-yielded the following error:
-`{error_line}`
-Here are the logs:
-```
-{cleaned_logs_str}
-```"""
-    return cleaned_response, response_for_user
+</errors>"""
+    cleaned_response = gha_prompt.format(
+        command_line=command_line,
+        error_content=error_content,
+        cleaned_logs_str=cleaned_logs_str,
+    )
+    return cleaned_response
 
 
 def on_check_suite(request: CheckRunCompleted):
     pr_number = request.check_run.pull_requests[0].number
     repo_name = request.repository.full_name
     _, g = get_github_client(request.installation.id)
     repo = g.get_repo(repo_name)
```

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/on_comment.py` & `sweepai-2.0.1/sweepai/handlers/on_comment.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     DEFAULT_GPT4_32K_MODEL,
     ENV,
     GITHUB_BOT_USERNAME,
     MONGODB_URI,
 )
 from sweepai.core.context_pruning import get_relevant_context
 from sweepai.core.entities import FileChangeRequest, MockPR, NoFilesException
-from sweepai.core.sweep_bot import SweepBot
+from sweepai.core.sweep_bot import SweepBot, get_files_to_change, validate_file_change_requests
 from sweepai.handlers.on_review import get_pr_diffs
 from sweepai.utils.chat_logger import ChatLogger
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import ClonedRepo, get_github_client
 from sweepai.utils.progress import TicketProgress
 from sweepai.utils.prompt_constructor import HumanMessageCommentPrompt
 from sweepai.utils.str_utils import BOT_SUFFIX, FASTER_MODEL_MESSAGE
@@ -275,27 +275,26 @@
                         formatted_query,
                         repo_context_manager,
                         TicketProgress(tracking_id="none"),
                         chat_logger=chat_logger,
                     )
                     snippets = repo_context_manager.current_top_snippets
                     tree = str(repo_context_manager.dir_obj)
+                    cloned_repo = repo_context_manager.cloned_repo
                 except Exception as e:
                     logger.error(traceback.format_exc())
                     raise e
             get_documentation_dict(repo)
             docs_results = ""
             logger.info("Getting response from ChatGPT...")
             human_message = HumanMessageCommentPrompt(
                 comment=comment,
                 repo_name=repo_name,
                 repo_description=repo_description if repo_description else "",
                 diffs=diffs,
-                issue_url=pr.html_url,
-                username=username,
                 title=pr_title,
                 tree=tree,
                 summary=pr_body,
                 snippets=snippets,
                 # commit_history=commit_history,
                 pr_file_path=pr_file_path,  # may be None
                 pr_chunk=formatted_pr_chunk,  # may be None
@@ -339,23 +338,22 @@
                         filename=pr_file_path,
                         instructions=f"The user left this comment {comment} in this chunk of code:\n<review_code_chunk>\n{formatted_pr_chunk}\n</review_code_chunk>.\nResolve their comment.",
                         change_type="modify",
                         comment_line=pr_line_position + 1,
                     )
                 ]
             else:
-                non_python_count = sum(
-                    not file_path.endswith(".py")
-                    for file_path in human_message.get_file_paths()
-                )
-                python_count = len(human_message.get_file_paths()) - non_python_count
-                is_python_issue = python_count > non_python_count
-                file_change_requests, _ = sweep_bot.get_files_to_change(
-                    is_python_issue, retries=1, pr_diffs=pr_diff_string
+                file_change_requests, plan = get_files_to_change(
+                    relevant_snippets=repo_context_manager.current_top_snippets,
+                    read_only_snippets=repo_context_manager.read_only_snippets,
+                    problem_statement=formatted_query,
+                    repo_name=repo_name,
+                    pr_diffs=pr_diff_string
                 )
+                validate_file_change_requests(file_change_requests, repo_context_manager.cloned_repo)
                 file_change_requests = sweep_bot.validate_file_change_requests(
                     file_change_requests, branch=branch_name
                 )
 
             sweep_response = "I couldn't find any relevant files to change."
             if file_change_requests:
                 table_message = tabulate(
@@ -384,15 +382,15 @@
             blocked_dirs = get_blocked_dirs(sweep_bot.repo)
 
             sweep_bot.comment_pr_diff_str = pr_diff_string
             sweep_bot.comment_pr_files_modified = pr_files_modified
             changes_made = sum(
                 [
                     change_made
-                    for _, change_made, _, _, _ in sweep_bot.change_files_in_github_iterator(
+                    for _, change_made, _, _ in sweep_bot.change_files_in_github_iterator(
                         file_change_requests, branch_name, blocked_dirs
                     )
                 ]
             )
             try:
                 if comment_id:
                     if changes_made:
```

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/on_merge.py` & `sweepai-2.0.1/sweepai/handlers/on_merge.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/on_merge_conflict.py` & `sweepai-2.0.1/sweepai/handlers/on_merge_conflict.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/on_review.py` & `sweepai-2.0.1/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/on_ticket.py` & `sweepai-2.0.1/sweepai/handlers/on_ticket.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 """
 
 import difflib
 import io
 import os
 import re
 import traceback
+from typing import Any
 import zipfile
-from copy import deepcopy
 from time import time
 
 import markdown
 import openai
 import requests
 import yaml
 import yamllint.config as yamllint_config
@@ -33,37 +33,38 @@
     REVERT_CHANGED_FILES_TITLE,
     RULES_LABEL,
     RULES_TITLE,
     SWEEP_BAD_FEEDBACK,
     SWEEP_GOOD_FEEDBACK,
     SweepConfig,
     get_documentation_dict,
+    get_gha_enabled,
     get_rules,
 )
 from sweepai.config.server import (
+    DEPLOYMENT_GHA_ENABLED,
     DISCORD_FEEDBACK_WEBHOOK_URL,
     ENV,
     GITHUB_LABEL_NAME,
     IS_SELF_HOSTED,
     MONGODB_URI,
     PROGRESS_BASE_URL,
 )
+from sweepai.core.context_pruning import get_relevant_context
 from sweepai.core.entities import (
     AssistantRaisedException,
     FileChangeRequest,
     MaxTokensExceeded,
-    Message,
     NoFilesException,
-    ProposedIssue,
     PullRequest,
     SandboxResponse,
 )
 from sweepai.core.entities import create_error_logs as entities_create_error_logs
 from sweepai.core.pr_reader import PRReader
-from sweepai.core.sweep_bot import SweepBot
+from sweepai.core.sweep_bot import SweepBot, get_files_to_change, validate_file_change_requests
 from sweepai.handlers.create_pr import (
     create_config_pr,
     create_pr_changes,
     safe_delete_sweep_branch,
 )
 from sweepai.handlers.on_check_suite import clean_gh_logs
 from sweepai.utils.buttons import Button, ButtonList, create_action_buttons
@@ -71,14 +72,15 @@
 from sweepai.utils.diff import generate_diff
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import (
     CURRENT_USERNAME,
     ClonedRepo,
     convert_pr_draft_field,
     get_github_client,
+    get_token,
 )
 from sweepai.utils.progress import (
     AssistantConversation,
     PaymentContext,
     TicketContext,
     TicketProgress,
     TicketProgressStatus,
@@ -104,14 +106,15 @@
     to_branch_name,
 )
 from sweepai.utils.ticket_utils import (
     center,
     fetch_relevant_files,
     fire_and_forget_wrapper,
     log_error,
+    prep_snippets,
 )
 from sweepai.utils.user_settings import UserSettings
 
 # from sandbox.sandbox_utils import Sandbox
 
 
 sweeping_gif = """<a href="https://github.com/sweepai/sweep"><img class="swing" src="https://raw.githubusercontent.com/sweepai/sweep/main/.assets/sweeping.gif" width="100" style="width:50px; margin-bottom:10px" alt="Sweeping"></a>"""
@@ -151,17 +154,17 @@
 {sweeping_gif}
 <br/>
 Cheers,
 <br/>
 Sweep
 <br/>"""
 
-FAILING_GITHUB_ACTION_PROMPT = """
+FAILING_GITHUB_ACTION_PROMPT = """\
 The following Github Actions failed on a previous attempt at fixing this issue.
-Review the provided logs to ensure that any code modifications you make do not cause these actions to fail again.
+Propose a fix to the failing github actions. You must edit the source code, not the github action itself.
 {github_action_log}
 """
 
 
 # Add :eyes: emoji to ticket
 def add_emoji(issue: Issue, comment_id: int = None, reaction_content="eyes"):
     item_to_react_to = issue.get_comment(comment_id) if comment_id else issue
@@ -208,25 +211,26 @@
         )
         if sandbox_response
         else ""
     )
 
 
 # takes in a list of workflow runs and returns a list of messages containing the logs of the failing runs
-def get_failing_gha_logs(runs) -> list[Message]:
-    messages: list[Message] = []
+def get_failing_gha_logs(runs, installation_id) -> str:
+    token = get_token(installation_id)
+    all_logs = ""
     for run in runs:
         # jobs_url
         jobs_url = run.jobs_url
         jobs_response = requests.get(
             jobs_url,
             headers={
                 "Accept": "application/vnd.github+json",
-                "X-Github-Api-Version": "2022-11-28",
-                "Authorization": "Bearer " + os.environ["GITHUB_PAT"],
+                "Authorization": f"Bearer {token}",
+                "X-GitHub-Api-Version": "2022-11-28",
             },
         )
         if jobs_response.status_code == 200:
             failed_jobs = []
             jobs = jobs_response.json()["jobs"]
             for job in jobs:
                 if job["conclusion"] == "failure":
@@ -240,49 +244,42 @@
                         failed_jobs_name_list.append(
                             f"{job['name']}/{step['number']}_{step['name']}"
                         )
         else:
             logger.error(
                 "Failed to get jobs for failing github actions, possible a credentials issue"
             )
-            return messages
+            return all_logs
         # logs url
         logs_url = run.logs_url
         logs_response = requests.get(
             logs_url,
             headers={
                 "Accept": "application/vnd.github+json",
-                "X-Github-Api-Version": "2022-11-28",
-                "Authorization": "Bearer " + os.environ["GITHUB_PAT"],
+                "Authorization": f"Bearer {token}",
+                "X-GitHub-Api-Version": "2022-11-28",
             },
             allow_redirects=True,
         )
         # Check if the request was successful
         if logs_response.status_code == 200:
             zip_data = io.BytesIO(logs_response.content)
             zip_file = zipfile.ZipFile(zip_data, "r")
             zip_file_names = zip_file.namelist()
             for file in failed_jobs_name_list:
                 if f"{file}.txt" in zip_file_names:
                     logs = zip_file.read(f"{file}.txt").decode("utf-8")
-                    cleaned_logs, user_message = clean_gh_logs(logs)
-                    messages.append(
-                        Message(
-                            role="user",
-                            content=FAILING_GITHUB_ACTION_PROMPT.replace(
-                                "{github_action_log}", cleaned_logs
-                            ),
-                        )
-                    )
+                    logs_prompt = clean_gh_logs(logs)
+                    all_logs += logs_prompt + "\n"
         else:
             logger.error(
                 "Failed to get logs for failing github actions, likely a credentials issue"
             )
-            return messages
-    return messages
+            return all_logs
+    return all_logs
 
 
 def delete_old_prs(repo: Repository, issue_number: int):
     logger.info("Deleting old PRs...")
     prs = repo.get_pulls(
         state="open",
         sort="created",
@@ -292,14 +289,47 @@
     for pr in tqdm(prs.get_page(0)):
         # # Check if this issue is mentioned in the PR, and pr is owned by bot
         # # This is done in create_pr, (pr_description = ...)
         if pr.user.login == CURRENT_USERNAME and f"Fixes #{issue_number}.\n" in pr.body:
             safe_delete_sweep_branch(pr, repo)
             break
 
+def construct_sweep_bot(
+        repo: Repository,
+        repo_name: str,
+        issue_url: str,
+        repo_description: str,
+        title: str,
+        message_summary: str,
+        cloned_repo: ClonedRepo,
+        ticket_progress: TicketProgress,
+        chat_logger: ChatLogger,
+        snippets: Any = None,
+        tree: Any = None,
+        comments: Any = None,
+    ) -> SweepBot:
+    human_message = HumanMessagePrompt(
+        repo_name=repo_name,
+        issue_url=issue_url,
+        repo_description=repo_description.strip(),
+        title=title,
+        summary=message_summary,
+        snippets=snippets,
+        tree=tree,
+    )
+    sweep_bot = SweepBot.from_system_message_content(
+        human_message=human_message,
+        repo=repo,
+        is_reply=bool(comments),
+        chat_logger=chat_logger,
+        cloned_repo=cloned_repo,
+        ticket_progress=ticket_progress,
+    )
+    return sweep_bot
+
 
 def get_comment_header(
     index: int,
     g: Github,
     repo_full_name: str,
     user_settings: UserSettings,
     progress_headers: list[None | str],
@@ -393,925 +423,783 @@
     )
 
 
 def on_ticket(
     title: str,
     summary: str,
     issue_number: int,
-    issue_url: str,
+    issue_url: str, # purely for logging purposes
     username: str,
     repo_full_name: str,
     repo_description: str,
     installation_id: int,
     comment_id: int = None,
     edited: bool = False,
     tracking_id: str | None = None,
 ):
     with logger.contextualize(
         tracking_id=tracking_id,
     ):
-        # we want to pass in the failing github action messages to the next run in order to fix them
-        failing_gha_messages: list[Message] = []
-        # we rerun this logic 3 times at most if the github actions associated with the created pr fails
-        max_pr_attempts = 1
-        for run_attempt in range(max_pr_attempts):
-            if tracking_id is None:
-                tracking_id = get_hash()
-            on_ticket_start_time = time()
-            logger.info(f"Starting on_ticket with title {title} and summary {summary}")
-            (
-                title,
-                slow_mode,
-                do_map,
-                subissues_mode,
-                sandbox_mode,
-                fast_mode,
-                lint_mode,
-            ) = strip_sweep(title)
-
-            summary = summary or ""
-            summary = re.sub(
-                "<details (open)?>(\r)?\n<summary>Checklist</summary>.*",
-                "",
-                summary,
-                flags=re.DOTALL,
-            ).strip()
-            summary = re.sub(
-                "---\s+Checklist:(\r)?\n(\r)?\n- \[[ X]\].*",
-                "",
-                summary,
-                flags=re.DOTALL,
-            ).strip()
-            summary = re.sub(
-                "### Details\n\n_No response_", "", summary, flags=re.DOTALL
-            )
-            summary = re.sub("\n\n", "\n", summary, flags=re.DOTALL)
+        if tracking_id is None:
+            tracking_id = get_hash()
+        on_ticket_start_time = time()
+        logger.info(f"Starting on_ticket with title {title} and summary {summary}")
+        (
+            title,
+            slow_mode,
+            do_map,
+            subissues_mode,
+            sandbox_mode,
+            fast_mode,
+            lint_mode,
+        ) = strip_sweep(title)
+
+        summary = summary or ""
+        summary = re.sub(
+            "<details (open)?>(\r)?\n<summary>Checklist</summary>.*",
+            "",
+            summary,
+            flags=re.DOTALL,
+        ).strip()
+        summary = re.sub(
+            "---\s+Checklist:(\r)?\n(\r)?\n- \[[ X]\].*",
+            "",
+            summary,
+            flags=re.DOTALL,
+        ).strip()
+        summary = re.sub(
+            "### Details\n\n_No response_", "", summary, flags=re.DOTALL
+        )
+        summary = re.sub("\n\n", "\n", summary, flags=re.DOTALL)
 
-            repo_name = repo_full_name
-            user_token, g = get_github_client(installation_id)
-            repo = g.get_repo(repo_full_name)
-            current_issue: Issue = repo.get_issue(number=issue_number)
-            assignee = current_issue.assignee.login if current_issue.assignee else None
-            if assignee is None:
-                assignee = current_issue.user.login
-
-            ticket_progress = TicketProgress(
-                tracking_id=tracking_id,
-                username=username,
-                context=TicketContext(
-                    title=title,
-                    description=summary,
-                    repo_full_name=repo_full_name,
-                    issue_number=issue_number,
-                    is_public=repo.private is False,
-                    start_time=int(time()),
-                ),
-            )
-            branch_match = re.search(
-                r"([B|b]ranch:) *(?P<branch_name>.+?)(\s|$)", summary
+        repo_name = repo_full_name
+        user_token, g = get_github_client(installation_id)
+        repo = g.get_repo(repo_full_name)
+        current_issue: Issue = repo.get_issue(number=issue_number)
+        assignee = current_issue.assignee.login if current_issue.assignee else None
+        if assignee is None:
+            assignee = current_issue.user.login
+
+        ticket_progress = TicketProgress(
+            tracking_id=tracking_id,
+            username=username,
+            context=TicketContext(
+                title=title,
+                description=summary,
+                repo_full_name=repo_full_name,
+                issue_number=issue_number,
+                is_public=repo.private is False,
+                start_time=int(time()),
+            ),
+        )
+        branch_match = re.search(
+            r"([B|b]ranch:) *(?P<branch_name>.+?)(\s|$)", summary
+        )
+        overrided_branch_name = None
+        if branch_match and "branch_name" in branch_match.groupdict():
+            overrided_branch_name = (
+                branch_match.groupdict()["branch_name"].strip().strip("`\"'")
             )
-            overrided_branch_name = None
-            if branch_match and "branch_name" in branch_match.groupdict():
-                overrided_branch_name = (
-                    branch_match.groupdict()["branch_name"].strip().strip("`\"'")
-                )
-                if overrided_branch_name == "_No response_":
-                    continue
-                # TODO: this code might be finicky, might have missed edge cases
-                if overrided_branch_name.startswith("https://github.com/"):
-                    overrided_branch_name = overrided_branch_name.split("?")[0].split(
-                        "tree/"
-                    )[-1]
-                SweepConfig.get_branch(repo, overrided_branch_name)
-
-            chat_logger = (
-                ChatLogger(
-                    {
-                        "repo_name": repo_name,
-                        "title": title,
-                        "summary": summary,
-                        "issue_number": issue_number,
-                        "issue_url": issue_url,
-                        "username": (
-                            username if not username.startswith("sweep") else assignee
-                        ),
-                        "repo_full_name": repo_full_name,
-                        "repo_description": repo_description,
-                        "installation_id": installation_id,
-                        "type": "ticket",
-                        "mode": ENV,
-                        "comment_id": comment_id,
-                        "edited": edited,
-                        "tracking_id": tracking_id,
-                    },
-                    active=True,
-                )
-                if MONGODB_URI
-                else None
+            # TODO: this code might be finicky, might have missed edge cases
+            if overrided_branch_name.startswith("https://github.com/"):
+                overrided_branch_name = overrided_branch_name.split("?")[0].split(
+                    "tree/"
+                )[-1]
+            SweepConfig.get_branch(repo, overrided_branch_name)
+
+        chat_logger = (
+            ChatLogger(
+                {
+                    "repo_name": repo_name,
+                    "title": title,
+                    "summary": summary,
+                    "issue_number": issue_number,
+                    "issue_url": issue_url,
+                    "username": (
+                        username if not username.startswith("sweep") else assignee
+                    ),
+                    "repo_full_name": repo_full_name,
+                    "repo_description": repo_description,
+                    "installation_id": installation_id,
+                    "type": "ticket",
+                    "mode": ENV,
+                    "comment_id": comment_id,
+                    "edited": edited,
+                    "tracking_id": tracking_id,
+                },
+                active=True,
             )
+            if MONGODB_URI
+            else None
+        )
 
-            if chat_logger and not IS_SELF_HOSTED:
-                is_paying_user = chat_logger.is_paying_user()
-                is_consumer_tier = chat_logger.is_consumer_tier()
-                use_faster_model = chat_logger.use_faster_model()
-            else:
-                is_paying_user = True
-                is_consumer_tier = False
-                use_faster_model = False
-
-            if use_faster_model:
-                raise Exception(FASTER_MODEL_MESSAGE)
+        if chat_logger and not IS_SELF_HOSTED:
+            is_paying_user = chat_logger.is_paying_user()
+            is_consumer_tier = chat_logger.is_consumer_tier()
+            use_faster_model = chat_logger.use_faster_model()
+        else:
+            is_paying_user = True
+            is_consumer_tier = False
+            use_faster_model = False
+
+        if use_faster_model:
+            raise Exception(FASTER_MODEL_MESSAGE)
+
+        if fast_mode:
+            use_faster_model = True
+
+        if not comment_id and not edited and chat_logger and not sandbox_mode:
+            fire_and_forget_wrapper(chat_logger.add_successful_ticket)(
+                gpt3=use_faster_model
+            )
 
-            if fast_mode:
-                use_faster_model = True
+        organization, repo_name = repo_full_name.split("/")
+        metadata = {
+            "issue_url": issue_url,
+            "repo_full_name": repo_full_name,
+            "organization": organization,
+            "repo_name": repo_name,
+            "repo_description": repo_description,
+            "username": username,
+            "comment_id": comment_id,
+            "title": title,
+            "installation_id": installation_id,
+            "function": "on_ticket",
+            "edited": edited,
+            "model": "gpt-3.5" if use_faster_model else "gpt-4",
+            "tier": "pro" if is_paying_user else "free",
+            "mode": ENV,
+            "slow_mode": slow_mode,
+            "do_map": do_map,
+            "subissues_mode": subissues_mode,
+            "sandbox_mode": sandbox_mode,
+            "fast_mode": fast_mode,
+            "is_self_hosted": IS_SELF_HOSTED,
+            "tracking_id": tracking_id,
+        }
+        fire_and_forget_wrapper(posthog.capture)(
+            username, "started", properties=metadata
+        )
 
-            if not comment_id and not edited and chat_logger and not sandbox_mode:
-                fire_and_forget_wrapper(chat_logger.add_successful_ticket)(
-                    gpt3=use_faster_model
-                )
-
-            organization, repo_name = repo_full_name.split("/")
-            metadata = {
-                "issue_url": issue_url,
-                "repo_full_name": repo_full_name,
-                "organization": organization,
-                "repo_name": repo_name,
-                "repo_description": repo_description,
-                "username": username,
-                "comment_id": comment_id,
-                "title": title,
-                "installation_id": installation_id,
-                "function": "on_ticket",
-                "edited": edited,
-                "model": "gpt-3.5" if use_faster_model else "gpt-4",
-                "tier": "pro" if is_paying_user else "free",
-                "mode": ENV,
-                "slow_mode": slow_mode,
-                "do_map": do_map,
-                "subissues_mode": subissues_mode,
-                "sandbox_mode": sandbox_mode,
-                "fast_mode": fast_mode,
-                "is_self_hosted": IS_SELF_HOSTED,
-                "tracking_id": tracking_id,
-            }
-            if run_attempt == 0:
-                # we want to capture restart and start events separately in posthog
+        try:
+            if current_issue.state == "closed":
                 fire_and_forget_wrapper(posthog.capture)(
-                    username, "started", properties=metadata
-                )
-            else:
-                fire_and_forget_wrapper(posthog.capture)(
-                    username, "on_ticket_restarted", properties=metadata
+                    username,
+                    "issue_closed",
+                    properties={
+                        **metadata,
+                        "duration": round(time() - on_ticket_start_time),
+                    },
                 )
+                return {"success": False, "reason": "Issue is closed"}
 
-            try:
-                if current_issue.state == "closed":
-                    fire_and_forget_wrapper(posthog.capture)(
-                        username,
-                        "issue_closed",
-                        properties={
-                            **metadata,
-                            "duration": round(time() - on_ticket_start_time),
-                        },
-                    )
-                    return {"success": False, "reason": "Issue is closed"}
-
-                fire_and_forget_wrapper(add_emoji)(current_issue, comment_id)
-                fire_and_forget_wrapper(remove_emoji)(
-                    current_issue, comment_id, content_to_delete="rocket"
-                )
-                fire_and_forget_wrapper(current_issue.edit)(body=summary)
+            fire_and_forget_wrapper(add_emoji)(current_issue, comment_id)
+            fire_and_forget_wrapper(remove_emoji)(
+                current_issue, comment_id, content_to_delete="rocket"
+            )
+            fire_and_forget_wrapper(current_issue.edit)(body=summary)
 
-                replies_text = ""
-                summary = summary if summary else ""
+            replies_text = ""
+            summary = summary if summary else ""
 
-                fire_and_forget_wrapper(delete_old_prs)(repo, issue_number)
+            fire_and_forget_wrapper(delete_old_prs)(repo, issue_number)
 
-                if not sandbox_mode:
-                    progress_headers = [
-                        None,
-                        "Step 1: 🔎 Searching",
-                        "Step 2: ⌨️ Coding",
-                        "Step 3: 🔁 Code Review",
-                    ]
-                else:
-                    progress_headers = [
-                        None,
-                        "📖 Reading File",
-                        "🛠️ Executing Sandbox",
-                    ]
-
-                issue_comment = None
-                payment_message, payment_message_start = get_payment_messages(
-                    chat_logger
-                )
-
-                ticket_progress.context.payment_context = PaymentContext(
-                    use_faster_model=use_faster_model,
-                    pro_user=is_paying_user,
-                    daily_tickets_used=(
-                        chat_logger.get_ticket_count(use_date=True)
-                        if chat_logger
-                        else 0
-                    ),
-                    monthly_tickets_used=(
-                        chat_logger.get_ticket_count() if chat_logger else 0
-                    ),
-                )
-                ticket_progress.save()
+            if not sandbox_mode:
+                progress_headers = [
+                    None,
+                    "Step 1: 🔎 Searching",
+                    "Step 2: ⌨️ Coding",
+                    "Step 3: 🔁 Code Review",
+                ]
+            else:
+                progress_headers = [
+                    None,
+                    "📖 Reading File",
+                    "🛠️ Executing Sandbox",
+                ]
+
+            issue_comment = None
+            payment_message, payment_message_start = get_payment_messages(
+                chat_logger
+            )
 
-                config_pr_url = None
-                user_settings = UserSettings.from_username(username=username)
-                user_settings_message = user_settings.get_message()
+            ticket_progress.context.payment_context = PaymentContext(
+                use_faster_model=use_faster_model,
+                pro_user=is_paying_user,
+                daily_tickets_used=(
+                    chat_logger.get_ticket_count(use_date=True)
+                    if chat_logger
+                    else 0
+                ),
+                monthly_tickets_used=(
+                    chat_logger.get_ticket_count() if chat_logger else 0
+                ),
+            )
+            ticket_progress.save()
 
-                cloned_repo = ClonedRepo(
-                    repo_full_name,
-                    installation_id=installation_id,
-                    token=user_token,
-                    repo=repo,
-                    branch=overrided_branch_name,
-                )
-                # check that repo's directory is non-empty
-                if os.listdir(cloned_repo.cached_dir) == []:
-                    logger.info("Empty repo")
-                    first_comment = (
-                        "Sweep is currently not supported on empty repositories. Please add some"
-                        f" code to your repository and try again.\n{sep}##"
-                        f" {progress_headers[1]}\n{bot_suffix}{discord_suffix}"
-                    )
-                    if issue_comment is None:
-                        issue_comment = current_issue.create_comment(
-                            first_comment + BOT_SUFFIX
-                        )
-                    else:
-                        issue_comment.edit(first_comment + BOT_SUFFIX)
-                    return {"success": False}
-                indexing_message = (
-                    "I'm searching for relevant snippets in your repository. If this is your first"
-                    " time using Sweep, I'm indexing your repository. You can monitor the progress using the progress dashboard"
-                )
+            config_pr_url = None
+            user_settings = UserSettings.from_username(username=username)
+            user_settings_message = user_settings.get_message()
+
+            cloned_repo = ClonedRepo(
+                repo_full_name,
+                installation_id=installation_id,
+                token=user_token,
+                repo=repo,
+                branch=overrided_branch_name,
+            )
+            # check that repo's directory is non-empty
+            if os.listdir(cloned_repo.cached_dir) == []:
+                logger.info("Empty repo")
                 first_comment = (
-                    f"{get_comment_header(0, g, repo_full_name, user_settings, progress_headers, tracking_id, payment_message_start, user_settings_message)}\n{sep}I am currently looking into this ticket! I"
-                    " will update the progress of the ticket in this comment. I am currently"
-                    f" searching through your code, looking for relevant snippets.\n{sep}##"
-                    f" {progress_headers[1]}\n{indexing_message}{bot_suffix}{discord_suffix}"
-                )
-                # Find Sweep's previous comment
-                comments = []
-                for comment in current_issue.get_comments():
-                    comments.append(comment)
-                    if comment.user.login == CURRENT_USERNAME:
-                        issue_comment = comment
-                        break
+                    "Sweep is currently not supported on empty repositories. Please add some"
+                    f" code to your repository and try again.\n{sep}##"
+                    f" {progress_headers[1]}\n{bot_suffix}{discord_suffix}"
+                )
                 if issue_comment is None:
-                    issue_comment = current_issue.create_comment(first_comment)
+                    issue_comment = current_issue.create_comment(
+                        first_comment + BOT_SUFFIX
+                    )
                 else:
-                    fire_and_forget_wrapper(issue_comment.edit)(first_comment)
-                old_edit = issue_comment.edit
-                issue_comment.edit = lambda msg: old_edit(msg + BOT_SUFFIX)
-                past_messages = {}
-                current_index = 0
-                table = None
-                initial_sandbox_response = -1
-                initial_sandbox_response_file = None
+                    issue_comment.edit(first_comment + BOT_SUFFIX)
+                return {"success": False}
+            indexing_message = (
+                "I'm searching for relevant snippets in your repository. If this is your first"
+                " time using Sweep, I'm indexing your repository. You can monitor the progress using the progress dashboard"
+            )
+            first_comment = (
+                f"{get_comment_header(0, g, repo_full_name, user_settings, progress_headers, tracking_id, payment_message_start, user_settings_message)}\n{sep}I am currently looking into this ticket! I"
+                " will update the progress of the ticket in this comment. I am currently"
+                f" searching through your code, looking for relevant snippets.\n{sep}##"
+                f" {progress_headers[1]}\n{indexing_message}{bot_suffix}{discord_suffix}"
+            )
+            # Find Sweep's previous comment
+            comments = []
+            for comment in current_issue.get_comments():
+                comments.append(comment)
+                if comment.user.login == CURRENT_USERNAME:
+                    issue_comment = comment
+                    break
+            if issue_comment is None:
+                issue_comment = current_issue.create_comment(first_comment)
+            else:
+                fire_and_forget_wrapper(issue_comment.edit)(first_comment)
+            old_edit = issue_comment.edit
+            issue_comment.edit = lambda msg: old_edit(msg + BOT_SUFFIX)
+            past_messages = {}
+            current_index = 0
+            table = None
+            initial_sandbox_response = -1
+            initial_sandbox_response_file = None
 
-                def refresh_token():
-                    user_token, g = get_github_client(installation_id)
-                    repo = g.get_repo(repo_full_name)
-                    return user_token, g, repo
+            def refresh_token():
+                user_token, g = get_github_client(installation_id)
+                repo = g.get_repo(repo_full_name)
+                return user_token, g, repo
 
-                def edit_sweep_comment(
-                    message: str,
-                    index: int,
-                    pr_message="",
-                    done=False,
-                    add_bonus_message=True,
-                ):
-                    nonlocal current_index, user_token, g, repo, issue_comment, initial_sandbox_response, initial_sandbox_response_file
-                    # -1 = error, -2 = retry
-                    # Only update the progress bar if the issue generation errors.
-                    errored = index == -1
-                    if index >= 0:
-                        past_messages[index] = message
-                        current_index = index
-
-                    agg_message = None
-                    # Include progress history
-                    # index = -2 is reserved for
-                    for i in range(
-                        current_index + 2
-                    ):  # go to next header (for Working on it... text)
-                        if i == 0 or i >= len(progress_headers):
-                            continue  # skip None header
-                        header = progress_headers[i]
-                        if header is not None:
-                            header = "## " + header + "\n"
-                        else:
-                            header = "No header\n"
-                        msg = header + (past_messages.get(i) or "Working on it...")
-                        if agg_message is None:
-                            agg_message = msg
-                        else:
-                            agg_message = agg_message + f"\n{sep}" + msg
+            def edit_sweep_comment(
+                message: str,
+                index: int,
+                pr_message="",
+                done=False,
+                add_bonus_message=True,
+            ):
+                nonlocal current_index, user_token, g, repo, issue_comment, initial_sandbox_response, initial_sandbox_response_file
+                # -1 = error, -2 = retry
+                # Only update the progress bar if the issue generation errors.
+                errored = index == -1
+                if index >= 0:
+                    past_messages[index] = message
+                    current_index = index
+
+                agg_message = None
+                # Include progress history
+                # index = -2 is reserved for
+                for i in range(
+                    current_index + 2
+                ):  # go to next header (for Working on it... text)
+                    if i == 0 or i >= len(progress_headers):
+                        continue  # skip None header
+                    header = progress_headers[i]
+                    if header is not None:
+                        header = "## " + header + "\n"
+                    else:
+                        header = "No header\n"
+                    msg = header + (past_messages.get(i) or "Working on it...")
+                    if agg_message is None:
+                        agg_message = msg
+                    else:
+                        agg_message = agg_message + f"\n{sep}" + msg
 
-                    suffix = bot_suffix + discord_suffix
-                    if errored:
-                        agg_message = (
-                            "## ❌ Unable to Complete PR"
-                            + "\n"
-                            + message
-                            + (
-                                "\n\nFor bonus GPT-4 tickets, please report this bug on"
-                                f" **[Discord](https://discord.gg/invite/sweep)** (tracking ID: `{tracking_id}`)."
-                                if add_bonus_message
-                                else ""
-                            )
+                suffix = bot_suffix + discord_suffix
+                if errored:
+                    agg_message = (
+                        "## ❌ Unable to Complete PR"
+                        + "\n"
+                        + message
+                        + (
+                            "\n\nFor bonus GPT-4 tickets, please report this bug on"
+                            f" **[Discord](https://discord.gg/invite/sweep)** (tracking ID: `{tracking_id}`)."
+                            if add_bonus_message
+                            else ""
                         )
-                        if table is not None:
-                            agg_message = (
-                                agg_message
-                                + f"\n{sep}Please look at the generated plan. If something looks"
-                                f" wrong, please add more details to your issue.\n\n{table}"
-                            )
-                        suffix = bot_suffix  # don't include discord suffix for error messages
-
-                    # Update the issue comment
-                    msg = f"{get_comment_header(current_index, g, repo_full_name, user_settings, progress_headers, tracking_id, payment_message_start, user_settings_message, errored=errored, pr_message=pr_message, done=done, initial_sandbox_response=initial_sandbox_response, initial_sandbox_response_file=initial_sandbox_response_file, config_pr_url=config_pr_url)}\n{sep}{agg_message}{suffix}"
-                    try:
-                        issue_comment.edit(msg)
-                    except BadCredentialsException:
-                        logger.error(
-                            f"Bad credentials, refreshing token (tracking ID: `{tracking_id}`)"
+                    )
+                    if table is not None:
+                        agg_message = (
+                            agg_message
+                            + f"\n{sep}Please look at the generated plan. If something looks"
+                            f" wrong, please add more details to your issue.\n\n{table}"
                         )
-                        user_token, g = get_github_client(installation_id)
-                        repo = g.get_repo(repo_full_name)
+                    suffix = bot_suffix  # don't include discord suffix for error messages
 
-                        issue_comment = None
-                        for comment in comments:
-                            if comment.user.login == CURRENT_USERNAME:
-                                issue_comment = comment
-                        current_issue = repo.get_issue(number=issue_number)
-                        if issue_comment is None:
-                            issue_comment = current_issue.create_comment(msg)
-                        else:
-                            issue_comment = [
-                                comment
-                                for comment in current_issue.get_comments()
-                                if comment.user.login == CURRENT_USERNAME
-                            ][0]
-                            issue_comment.edit(msg)
-
-                if use_faster_model:
-                    edit_sweep_comment(
-                        FASTER_MODEL_MESSAGE, -1, add_bonus_message=False
-                    )
-                    posthog.capture(
-                        username,
-                        "ran_out_of_tickets",
-                        properties={
-                            **metadata,
-                            "duration": round(time() - on_ticket_start_time),
-                        },
-                    )
-                    return {
-                        "success": False,
-                        "error_message": "We deprecated supporting GPT 3.5.",
-                    }
-
-                if sandbox_mode:
-                    handle_sandbox_mode(
-                        title, repo_full_name, repo, ticket_progress, edit_sweep_comment
+                # Update the issue comment
+                msg = f"{get_comment_header(current_index, g, repo_full_name, user_settings, progress_headers, tracking_id, payment_message_start, user_settings_message, errored=errored, pr_message=pr_message, done=done, initial_sandbox_response=initial_sandbox_response, initial_sandbox_response_file=initial_sandbox_response_file, config_pr_url=config_pr_url)}\n{sep}{agg_message}{suffix}"
+                try:
+                    issue_comment.edit(msg)
+                except BadCredentialsException:
+                    logger.error(
+                        f"Bad credentials, refreshing token (tracking ID: `{tracking_id}`)"
                     )
-                    return {"success": True}
+                    user_token, g = get_github_client(installation_id)
+                    repo = g.get_repo(repo_full_name)
 
-                if len(title + summary) < 20:
-                    logger.info("Issue too short")
-                    edit_sweep_comment(
-                        (
-                            f"Please add more details to your issue. I need at least 20 characters"
-                            f" to generate a plan. Please join our Discord server for support (tracking_id={tracking_id})"
-                        ),
-                        -1,
-                    )
-                    posthog.capture(
-                        username,
-                        "issue_too_short",
-                        properties={
-                            **metadata,
-                            "duration": round(time() - on_ticket_start_time),
-                        },
-                    )
-                    return {"success": True}
-
-                prs_extracted = PRReader.extract_prs(repo, summary)
-                message_summary = summary
-                if prs_extracted:
-                    message_summary += "\n\n" + prs_extracted
-                    edit_sweep_comment(
-                        create_collapsible(
-                            "I found that you mentioned the following Pull Requests that might be important:",
-                            blockquote(
-                                prs_extracted,
-                            ),
-                        ),
-                        1,
-                    )
+                    issue_comment = None
+                    for comment in comments:
+                        if comment.user.login == CURRENT_USERNAME:
+                            issue_comment = comment
+                    current_issue = repo.get_issue(number=issue_number)
+                    if issue_comment is None:
+                        issue_comment = current_issue.create_comment(msg)
+                    else:
+                        issue_comment = [
+                            comment
+                            for comment in current_issue.get_comments()
+                            if comment.user.login == CURRENT_USERNAME
+                        ][0]
+                        issue_comment.edit(msg)
 
-                try:
-                    # search/context manager
-                    logger.info("Searching for relevant snippets...")
-                    snippets, tree, _ = fetch_relevant_files(
-                        cloned_repo,
-                        title,
-                        message_summary,
-                        replies_text,
-                        username,
-                        metadata,
-                        on_ticket_start_time,
-                        tracking_id,
-                        is_paying_user,
-                        is_consumer_tier,
-                        issue_url,
-                        chat_logger,
-                        ticket_progress,
-                    )
-                except Exception as e:
-                    edit_sweep_comment(
-                        (
-                            "It looks like an issue has occurred around fetching the files."
-                            " Perhaps the repo failed to initialized. If this error persists"
-                            f" contact team@sweep.dev.\n\n> @{username}, editing this issue description to include more details will automatically make me relaunch. Please join our Discord server for support (tracking_id={tracking_id})"
-                        ),
-                        -1,
-                    )
-                    raise Exception("Failed to fetch files") from e
-                _user_token, g = get_github_client(installation_id)
-                user_token, g, repo = refresh_token()
-                cloned_repo.token = user_token
-                repo = g.get_repo(repo_full_name)
-                ticket_progress.search_progress.indexing_progress = (
-                    ticket_progress.search_progress.indexing_total
+            if use_faster_model:
+                edit_sweep_comment(
+                    FASTER_MODEL_MESSAGE, -1, add_bonus_message=False
                 )
-                ticket_progress.status = TicketProgressStatus.PLANNING
-                ticket_progress.save()
+                posthog.capture(
+                    username,
+                    "ran_out_of_tickets",
+                    properties={
+                        **metadata,
+                        "duration": round(time() - on_ticket_start_time),
+                    },
+                )
+                return {
+                    "success": False,
+                    "error_message": "We deprecated supporting GPT 3.5.",
+                }
+
+            if sandbox_mode:
+                handle_sandbox_mode(
+                    title, repo_full_name, repo, ticket_progress, edit_sweep_comment
+                )
+                return {"success": True}
 
-                # Fetch git commit history
-                if not repo_description:
-                    repo_description = "No description provided."
-
-                message_summary += replies_text
-                # removed external search as it provides no real value and only adds noise
-                # external_results = ExternalSearcher.extract_summaries(message_summary)
-                # if external_results:
-                #     message_summary += "\n\n" + external_results
-
-                get_documentation_dict(repo)
-                docs_results = ""
-                human_message = HumanMessagePrompt(
-                    repo_name=repo_name,
-                    issue_url=issue_url,
-                    username=username,
-                    repo_description=repo_description.strip(),
-                    title=title,
-                    summary=message_summary,
-                    snippets=snippets,
-                    tree=tree,
+            if len(title + summary) < 20:
+                logger.info("Issue too short")
+                edit_sweep_comment(
+                    (
+                        f"Please add more details to your issue. I need at least 20 characters"
+                        f" to generate a plan. Please join our Discord server for support (tracking_id={tracking_id})"
+                    ),
+                    -1,
+                )
+                posthog.capture(
+                    username,
+                    "issue_too_short",
+                    properties={
+                        **metadata,
+                        "duration": round(time() - on_ticket_start_time),
+                    },
                 )
+                return {"success": True}
 
-                sweep_bot = SweepBot.from_system_message_content(
-                    human_message=human_message,
-                    repo=repo,
-                    is_reply=bool(comments),
-                    chat_logger=chat_logger,
-                    cloned_repo=cloned_repo,
-                    ticket_progress=ticket_progress,
+            prs_extracted = PRReader.extract_prs(repo, summary)
+            message_summary = summary
+            if prs_extracted:
+                message_summary += "\n\n" + prs_extracted
+                edit_sweep_comment(
+                    create_collapsible(
+                        "I found that you mentioned the following Pull Requests that might be important:",
+                        blockquote(
+                            prs_extracted,
+                        ),
+                    ),
+                    1,
                 )
 
-                # Check repository for sweep.yml file.
-                sweep_yml_exists = False
-                sweep_yml_failed = False
-                for content_file in repo.get_contents(""):
-                    if content_file.name == "sweep.yaml":
-                        sweep_yml_exists = True
-
-                        # Check if YAML is valid
-                        yaml_content = content_file.decoded_content.decode("utf-8")
-                        sweep_yaml_dict = {}
-                        try:
-                            sweep_yaml_dict = yaml.safe_load(yaml_content)
-                        except Exception:
-                            logger.error(f"Failed to load YAML file: {yaml_content}")
-                        if len(sweep_yaml_dict) > 0:
-                            break
-                        linter_config = yamllint_config.YamlLintConfig(custom_config)
-                        problems = list(linter.run(yaml_content, linter_config))
-                        if problems:
-                            errors = [
-                                f"Line {problem.line}: {problem.desc} (rule: {problem.rule})"
-                                for problem in problems
-                            ]
-                            error_message = "\n".join(errors)
-                            markdown_error_message = f"**There is something wrong with your [sweep.yaml](https://github.com/{repo_full_name}/blob/main/sweep.yaml):**\n```\n{error_message}\n```"
-                            sweep_yml_failed = True
-                            logger.error(markdown_error_message)
-                            edit_sweep_comment(markdown_error_message, -1)
-                        else:
-                            logger.info("The YAML file is valid. No errors found.")
-                        break
+            try:
+                # search/context manager
+                logger.info("Searching for relevant snippets...")
+                snippets, tree, _, repo_context_manager = fetch_relevant_files(
+                    cloned_repo,
+                    title,
+                    message_summary,
+                    replies_text,
+                    username,
+                    metadata,
+                    on_ticket_start_time,
+                    tracking_id,
+                    is_paying_user,
+                    is_consumer_tier,
+                    issue_url,
+                    chat_logger,
+                    ticket_progress,
+                )
+                cloned_repo = repo_context_manager.cloned_repo
+            except Exception as e:
+                edit_sweep_comment(
+                    (
+                        "It looks like an issue has occurred around fetching the files."
+                        " Perhaps the repo failed to initialized. If this error persists"
+                        f" contact team@sweep.dev.\n\n> @{username}, editing this issue description to include more details will automatically make me relaunch. Please join our Discord server for support (tracking_id={tracking_id})"
+                    ),
+                    -1,
+                )
+                raise Exception("Failed to fetch files") from e
+            _user_token, g = get_github_client(installation_id)
+            user_token, g, repo = refresh_token()
+            cloned_repo.token = user_token
+            repo = g.get_repo(repo_full_name)
+            ticket_progress.search_progress.indexing_progress = (
+                ticket_progress.search_progress.indexing_total
+            )
+            ticket_progress.status = TicketProgressStatus.PLANNING
+            ticket_progress.save()
 
-                # If sweep.yaml does not exist, then create a new PR that simply creates the sweep.yaml file.
-                if not sweep_yml_exists:
+            # Fetch git commit history
+            if not repo_description:
+                repo_description = "No description provided."
+
+            message_summary += replies_text
+            # removed external search as it provides no real value and only adds noise
+            # external_results = ExternalSearcher.extract_summaries(message_summary)
+            # if external_results:
+            #     message_summary += "\n\n" + external_results
+
+            get_documentation_dict(repo)
+            docs_results = ""
+            sweep_bot = construct_sweep_bot(
+                repo=repo,
+                repo_name=repo_name,
+                issue_url=issue_url,
+                repo_description=repo_description,
+                title=title,
+                message_summary=message_summary,
+                cloned_repo=cloned_repo,
+                ticket_progress=ticket_progress,
+                chat_logger=chat_logger,
+                snippets=snippets,
+                tree=tree,
+                comments=comments,
+            )
+            # Check repository for sweep.yml file.
+            sweep_yml_exists = False
+            sweep_yml_failed = False
+            for content_file in repo.get_contents(""):
+                if content_file.name == "sweep.yaml":
+                    sweep_yml_exists = True
+
+                    # Check if YAML is valid
+                    yaml_content = content_file.decoded_content.decode("utf-8")
+                    sweep_yaml_dict = {}
                     try:
-                        logger.info("Creating sweep.yaml file...")
-                        config_pr = create_config_pr(sweep_bot, cloned_repo=cloned_repo)
-                        config_pr_url = config_pr.html_url
-                        edit_sweep_comment(message="", index=-2)
-                    except SystemExit:
-                        raise SystemExit
-                    except Exception as e:
-                        logger.error(
-                            "Failed to create new branch for sweep.yaml file.\n",
-                            e,
-                            traceback.format_exc(),
-                        )
-                else:
-                    logger.info("sweep.yaml file already exists.")
+                        sweep_yaml_dict = yaml.safe_load(yaml_content)
+                    except Exception:
+                        logger.error(f"Failed to load YAML file: {yaml_content}")
+                    if len(sweep_yaml_dict) > 0:
+                        break
+                    linter_config = yamllint_config.YamlLintConfig(custom_config)
+                    problems = list(linter.run(yaml_content, linter_config))
+                    if problems:
+                        errors = [
+                            f"Line {problem.line}: {problem.desc} (rule: {problem.rule})"
+                            for problem in problems
+                        ]
+                        error_message = "\n".join(errors)
+                        markdown_error_message = f"**There is something wrong with your [sweep.yaml](https://github.com/{repo_full_name}/blob/main/sweep.yaml):**\n```\n{error_message}\n```"
+                        sweep_yml_failed = True
+                        logger.error(markdown_error_message)
+                        edit_sweep_comment(markdown_error_message, -1)
+                    else:
+                        logger.info("The YAML file is valid. No errors found.")
+                    break
 
+            # If sweep.yaml does not exist, then create a new PR that simply creates the sweep.yaml file.
+            if not sweep_yml_exists:
                 try:
-                    # ANALYZE SNIPPETS
-                    newline = "\n"
-                    edit_sweep_comment(
-                        "I found the following snippets in your repository. I will now analyze"
-                        " these snippets and come up with a plan."
-                        + "\n\n"
-                        + create_collapsible(
-                            "Some code snippets I think are relevant in decreasing order of relevance (click to expand). If some file is missing from here, you can mention the path in the ticket description.",
-                            "\n".join(
-                                [
-                                    f"https://github.com/{organization}/{repo_name}/blob/{repo.get_commits()[0].sha}/{snippet.file_path}#L{max(snippet.start, 1)}-L{min(snippet.end, snippet.content.count(newline) - 1)}\n"
-                                    for snippet in snippets
-                                ]
-                            ),
-                        )
-                        + (
-                            create_collapsible(
-                                "I also found that you mentioned the following Pull Requests that may be helpful:",
-                                blockquote(prs_extracted),
-                            )
-                            if prs_extracted
-                            else ""
-                        )
-                        # removed external results as it provides no real value and only adds noise
-                        # + (
-                        #     create_collapsible(
-                        #         "I also found the following external resources that might be helpful:",
-                        #         f"\n\n{external_results}\n\n",
-                        #     )
-                        #     if external_results
-                        #     else ""
-                        # )
-                        + (f"\n\n{docs_results}\n\n" if docs_results else ""),
-                        1,
+                    logger.info("Creating sweep.yaml file...")
+                    config_pr = create_config_pr(sweep_bot, cloned_repo=cloned_repo)
+                    config_pr_url = config_pr.html_url
+                    edit_sweep_comment(message="", index=-2)
+                except SystemExit:
+                    raise SystemExit
+                except Exception as e:
+                    logger.error(
+                        "Failed to create new branch for sweep.yaml file.\n",
+                        e,
+                        traceback.format_exc(),
                     )
+            else:
+                logger.info("sweep.yaml file already exists.")
 
-                    if do_map:
-                        subissues: list[ProposedIssue] = sweep_bot.generate_subissues()
-                        edit_sweep_comment(
-                            "I'm creating the following subissues:\n\n"
-                            + "\n\n".join(
-                                [
-                                    f"#{subissue.title}:\n" + blockquote(subissue.body)
-                                    for subissue in subissues
-                                ]
-                            ),
-                            2,
-                        )
-                        for subissue in tqdm(subissues):
-                            subissue.issue_id = repo.create_issue(
-                                title="Sweep: " + subissue.title,
-                                body=subissue.body
-                                + f"\n\nParent issue: #{issue_number}",
-                                assignee=username,
-                            ).number
-                        subissues_checklist = "\n\n".join(
+            try:
+                # ANALYZE SNIPPETS
+                newline = "\n"
+                edit_sweep_comment(
+                    "I found the following snippets in your repository. I will now analyze"
+                    " these snippets and come up with a plan."
+                    + "\n\n"
+                    + create_collapsible(
+                        "Some code snippets I think are relevant in decreasing order of relevance (click to expand). If some file is missing from here, you can mention the path in the ticket description.",
+                        "\n".join(
                             [
-                                f"- [ ] #{subissue.issue_id}\n\n"
-                                + blockquote(f"**{subissue.title}**\n{subissue.body}")
-                                for subissue in subissues
+                                f"https://github.com/{organization}/{repo_name}/blob/{repo.get_commits()[0].sha}/{snippet.file_path}#L{max(snippet.start, 1)}-L{min(snippet.end, snippet.content.count(newline) - 1)}\n"
+                                for snippet in snippets
                             ]
+                        ),
+                    )
+                    + (
+                        create_collapsible(
+                            "I also found that you mentioned the following Pull Requests that may be helpful:",
+                            blockquote(prs_extracted),
                         )
-                        current_issue.edit(
-                            body=summary
-                            + "\n\n---\n\nChecklist:\n\n"
-                            + subissues_checklist
-                        )
+                        if prs_extracted
+                        else ""
+                    )
+                    + (f"\n\n{docs_results}\n\n" if docs_results else ""),
+                    1,
+                )
+
+                logger.info("Fetching files to modify/create...")
+                file_change_requests, plan = get_files_to_change(
+                    relevant_snippets=repo_context_manager.current_top_snippets,
+                    read_only_snippets=repo_context_manager.read_only_snippets,
+                    problem_statement=f"{title}\n\n{summary}",
+                    repo_name=repo_full_name,
+                )
+                validate_file_change_requests(file_change_requests, cloned_repo)
+                ticket_progress.planning_progress.file_change_requests = (
+                    file_change_requests
+                )
+                ticket_progress.coding_progress.file_change_requests = (
+                    file_change_requests
+                )
+                ticket_progress.coding_progress.assistant_conversations = [
+                    AssistantConversation() for fcr in file_change_requests
+                ]
+                ticket_progress.status = TicketProgressStatus.CODING
+                ticket_progress.save()
+
+                if not file_change_requests:
+                    if len(title + summary) < 60:
                         edit_sweep_comment(
-                            "I finished creating the subissues! Track them at:\n\n"
-                            + "\n".join(
-                                f"* #{subissue.issue_id}" for subissue in subissues
+                            (
+                                "Sorry, I could not find any files to modify, can you please"
+                                " provide more details? Please make sure that the title and"
+                                " summary of the issue are at least 60 characters."
                             ),
-                            3,
-                            done=True,
+                            -1,
                         )
-                        edit_sweep_comment("N/A", 4)
-                        edit_sweep_comment("I finished creating all the subissues.", 5)
-                        posthog.capture(
-                            username,
-                            "subissues_created",
-                            properties={
-                                **metadata,
-                                "count": len(subissues),
-                                "duration": round(time() - on_ticket_start_time),
-                            },
+                    else:
+                        edit_sweep_comment(
+                            (
+                                "Sorry, I could not find any files to modify, can you please"
+                                " provide more details?"
+                            ),
+                            -1,
                         )
-                        return {"success": True}
+                    raise Exception("No files to modify.")
 
-                    logger.info("Fetching files to modify/create...")
-                    non_python_count = sum(
-                        not file_path.endswith(".py")
-                        and not file_path.endswith(".ipynb")
-                        and not file_path.endswith(".md")
-                        for file_path in human_message.get_file_paths()
-                    )
-                    python_count = (
-                        len(human_message.get_file_paths()) - non_python_count
-                    )
-                    is_python_issue = (
-                        python_count >= non_python_count and python_count > 0
-                    )
-                    posthog.capture(
-                        username,
-                        "is_python_issue",
-                        properties={"is_python_issue": is_python_issue},
-                    )
-                    file_change_requests, plan = sweep_bot.get_files_to_change(
-                        is_python_issue
-                    )
-                    ticket_progress.planning_progress.file_change_requests = (
-                        file_change_requests
-                    )
-                    ticket_progress.coding_progress.file_change_requests = (
-                        file_change_requests
-                    )
-                    ticket_progress.coding_progress.assistant_conversations = [
-                        AssistantConversation() for fcr in file_change_requests
-                    ]
-                    ticket_progress.status = TicketProgressStatus.CODING
-                    ticket_progress.save()
-
-                    if not file_change_requests:
-                        if len(title + summary) < 60:
-                            edit_sweep_comment(
-                                (
-                                    "Sorry, I could not find any files to modify, can you please"
-                                    " provide more details? Please make sure that the title and"
-                                    " summary of the issue are at least 60 characters."
-                                ),
-                                -1,
-                            )
-                        else:
-                            edit_sweep_comment(
-                                (
-                                    "Sorry, I could not find any files to modify, can you please"
-                                    " provide more details?"
-                                ),
-                                -1,
-                            )
-                        raise Exception("No files to modify.")
-
-                    file_change_requests: list[
-                        FileChangeRequest
-                    ] = sweep_bot.validate_file_change_requests(
-                        file_change_requests,
-                    )
-                    ticket_progress.planning_progress.file_change_requests = (
-                        file_change_requests
-                    )
-                    ticket_progress.coding_progress.assistant_conversations = [
-                        AssistantConversation() for fcr in file_change_requests
-                    ]
-                    ticket_progress.save()
+                file_change_requests: list[
+                    FileChangeRequest
+                ] = sweep_bot.validate_file_change_requests(
+                    file_change_requests,
+                )
+                ticket_progress.planning_progress.file_change_requests = (
+                    file_change_requests
+                )
+                ticket_progress.coding_progress.assistant_conversations = [
+                    AssistantConversation() for fcr in file_change_requests
+                ]
+                ticket_progress.save()
 
-                    table = tabulate(
+                table = tabulate(
+                    [
                         [
-                            [
-                                file_change_request.entity_display,
-                                file_change_request.instructions_display.replace(
-                                    "\n", "<br/>"
-                                ).replace("```", "\\```"),
-                            ]
-                            for file_change_request in file_change_requests
-                            if file_change_request.change_type != "check"
-                        ],
-                        headers=["File Path", "Proposed Changes"],
-                        tablefmt="pipe",
-                    )
+                            file_change_request.entity_display,
+                            file_change_request.instructions_display.replace(
+                                "\n", "<br/>"
+                            ).replace("```", "\\```"),
+                        ]
+                        for file_change_request in file_change_requests
+                        if file_change_request.change_type != "check"
+                    ],
+                    headers=["File Path", "Proposed Changes"],
+                    tablefmt="pipe",
+                )
 
-                    logger.info("Generating PR...")
-                    pull_request = PullRequest(
-                        title="Sweep: " + title,
-                        branch_name="sweep/" + to_branch_name(title),
-                        content="",
-                    )
-                    logger.info("Making PR...")
+                logger.info("Generating PR...")
+                pull_request = PullRequest(
+                    title="Sweep: " + title,
+                    branch_name="sweep/" + to_branch_name(title),
+                    content="",
+                )
+                logger.info("Making PR...")
 
-                    ticket_progress.context.branch_name = pull_request.branch_name
-                    ticket_progress.save()
+                ticket_progress.context.branch_name = pull_request.branch_name
+                ticket_progress.save()
 
-                    files_progress: list[tuple[str, str, str, str]] = [
-                        (
-                            file_change_request.entity_display,
-                            file_change_request.instructions_display,
-                            "⏳ In Progress",
-                            "",
+                files_progress: list[tuple[str, str, str, str]] = [
+                    (
+                        file_change_request.entity_display,
+                        file_change_request.instructions_display,
+                        "⏳ In Progress",
+                        "",
+                    )
+                    for file_change_request in file_change_requests
+                ]
+
+                checkboxes_progress: list[tuple[str, str, str]] = [
+                    (
+                        file_change_request.entity_display,
+                        file_change_request.instructions_display,
+                        " ",
+                    )
+                    for file_change_request in file_change_requests
+                    if not file_change_request.change_type == "check"
+                ]
+                checkboxes_contents = "\n".join(
+                    [
+                        create_checkbox(
+                            f"`{filename}`", blockquote(instructions), check == "X"
                         )
-                        for file_change_request in file_change_requests
+                        for filename, instructions, check in checkboxes_progress
                     ]
+                )
+                create_collapsible("Checklist", checkboxes_contents, opened=True)
 
-                    checkboxes_progress: list[tuple[str, str, str]] = [
-                        (
-                            file_change_request.entity_display,
-                            file_change_request.instructions_display,
-                            " ",
-                        )
-                        for file_change_request in file_change_requests
-                        if not file_change_request.change_type == "check"
+                file_change_requests[0].status = "running"
+
+                condensed_checkboxes_contents = "\n".join(
+                    [
+                        create_checkbox(f"`{filename}`", "", check == "X").strip()
+                        for filename, instructions, check in checkboxes_progress
                     ]
-                    checkboxes_contents = "\n".join(
-                        [
-                            create_checkbox(
-                                f"`{filename}`", blockquote(instructions), check == "X"
-                            )
-                            for filename, instructions, check in checkboxes_progress
-                        ]
-                    )
-                    create_collapsible("Checklist", checkboxes_contents, opened=True)
+                )
+                condensed_checkboxes_collapsible = create_collapsible(
+                    "Checklist", condensed_checkboxes_contents, opened=True
+                )
 
-                    file_change_requests[0].status = "running"
+                current_issue = repo.get_issue(number=issue_number)
+                current_issue.edit(
+                    body=summary + "\n\n" + condensed_checkboxes_collapsible
+                )
 
-                    condensed_checkboxes_contents = "\n".join(
-                        [
-                            create_checkbox(f"`{filename}`", "", check == "X").strip()
-                            for filename, instructions, check in checkboxes_progress
-                        ]
+                delete_branch = False
+
+                generator = create_pr_changes(
+                    file_change_requests,
+                    pull_request,
+                    sweep_bot,
+                    username,
+                    installation_id,
+                    issue_number,
+                    chat_logger=chat_logger,
+                    base_branch=overrided_branch_name,
+                    additional_messages=[],
+                )
+                edit_sweep_comment(checkboxes_contents, 2)
+                if not file_change_requests:
+                    raise NoFilesException()
+                response = {
+                    "error": Exception(
+                        f"Sweep failed to generate any file change requests! This could mean that Sweep failed to find the correct lines of code to modify or that GPT-4 did not respond in our specified format. Sometimes, retrying will fix this error. Otherwise, reach out to our Discord server for support (tracking_id={tracking_id})."
+                    )
+                }
+
+                changed_files = []
+                for item in generator:
+                    if isinstance(item, dict):
+                        response = item
+                        break
+                    (
+                        new_file_contents,
+                        _,
+                        commit,
+                        file_change_requests,
+                    ) = item
+                    # append all files that have been changed
+                    if new_file_contents:
+                        for file_name, _ in new_file_contents.items():
+                            changed_files.append(file_name)
+                    commit_hash: str = (
+                        commit
+                        if isinstance(commit, str)
+                        else (
+                            commit.sha
+                            if commit is not None
+                            else repo.get_branch(
+                                pull_request.branch_name
+                            ).commit.sha
+                        )
                     )
-                    condensed_checkboxes_collapsible = create_collapsible(
-                        "Checklist", condensed_checkboxes_contents, opened=True
+                    commit_url = (
+                        f"https://github.com/{repo_full_name}/commit/{commit_hash}"
                     )
-
-                    current_issue = repo.get_issue(number=issue_number)
-                    current_issue.edit(
-                        body=summary + "\n\n" + condensed_checkboxes_collapsible
+                    commit_url_display = (
+                        f"<a href='{commit_url}'><code>{commit_hash[:7]}</code></a>"
                     )
-
-                    delete_branch = False
-
-                    # this is to prevent failing_gha_messages from being modified by the generator
-                    additional_messages = deepcopy(failing_gha_messages)
-
-                    generator = create_pr_changes(
-                        file_change_requests,
-                        pull_request,
-                        sweep_bot,
-                        username,
-                        installation_id,
-                        issue_number,
-                        chat_logger=chat_logger,
-                        base_branch=overrided_branch_name,
-                        additional_messages=additional_messages,
+                    create_error_logs(
+                        commit_url_display,
+                        None,
+                        status=(
+                            "✓"
+                        ),
                     )
-                    edit_sweep_comment(checkboxes_contents, 2)
-                    if not file_change_requests:
-                        raise NoFilesException()
-                    response = {
-                        "error": Exception(
-                            f"Sweep failed to make code changes! This could mean that GPT-4 failed to find the correct lines of code to modify or that GPT-4 did not respond in our specified format. Sometimes, retrying will fix this error. Otherwise, reach out to our Discord server for support (tracking_id={tracking_id})."
-                        )
-                    }
-
-                    changed_files = []
-                    for item in generator:
-                        if isinstance(item, dict):
-                            response = item
-                            break
+                    checkboxes_progress = [
                         (
-                            file_change_request,
-                            changed_file,
-                            sandbox_response,
-                            commit,
-                            file_change_requests,
-                        ) = item
-                        changed_files.append(file_change_request.filename)
-                        sandbox_response: SandboxResponse | None = sandbox_response
-                        logger.info(sandbox_response)
-                        commit_hash: str = (
-                            commit
-                            if isinstance(commit, str)
-                            else (
-                                commit.sha
-                                if commit is not None
-                                else repo.get_branch(
-                                    pull_request.branch_name
-                                ).commit.sha
-                            )
-                        )
-                        commit_url = (
-                            f"https://github.com/{repo_full_name}/commit/{commit_hash}"
-                        )
-                        commit_url_display = (
-                            f"<a href='{commit_url}'><code>{commit_hash[:7]}</code></a>"
-                        )
-                        create_error_logs(
-                            commit_url_display,
-                            sandbox_response,
-                            status=(
-                                "✓"
-                                if (
-                                    sandbox_response is None or sandbox_response.success
-                                )
-                                else "❌"
-                            ),
-                        )
-                        checkboxes_progress = [
+                            file_change_request.display_summary
+                            + " "
+                            + file_change_request.status_display
+                            + " "
+                            + (file_change_request.commit_hash_url or "")
+                            + f" [Edit]({file_change_request.get_edit_url(repo.full_name, pull_request.branch_name)})",
+                            file_change_request.instructions_ticket_display
+                            + f"\n\n{file_change_request.diff_display}",
                             (
-                                file_change_request.display_summary
-                                + " "
-                                + file_change_request.status_display
-                                + " "
-                                + (file_change_request.commit_hash_url or "")
-                                + f" [Edit]({file_change_request.get_edit_url(repo.full_name, pull_request.branch_name)})",
-                                file_change_request.instructions_ticket_display
-                                + f"\n\n{file_change_request.diff_display}",
-                                (
-                                    "X"
-                                    if file_change_request.status
-                                    in ("succeeded", "failed")
-                                    else " "
-                                ),
-                            )
-                            for file_change_request in file_change_requests
-                        ]
-                        checkboxes_contents = "\n".join(
-                            [
-                                checkbox_template.format(
-                                    check=check,
-                                    filename=filename,
-                                    instructions=blockquote(instructions),
-                                )
-                                for filename, instructions, check in checkboxes_progress
-                            ]
-                        )
-                        collapsible_template.format(
-                            summary="Checklist",
-                            body=checkboxes_contents,
-                            opened="open",
-                        )
-                        condensed_checkboxes_contents = "\n".join(
-                            [
-                                checkbox_template.format(
-                                    check=check,
-                                    filename=filename,
-                                    instructions="",
-                                ).strip()
-                                for filename, instructions, check in checkboxes_progress
-                                if not instructions.lower().startswith("run")
-                            ]
-                        )
-                        condensed_checkboxes_collapsible = collapsible_template.format(
-                            summary="Checklist",
-                            body=condensed_checkboxes_contents,
-                            opened="open",
-                        )
-
-                        try:
-                            current_issue = repo.get_issue(number=issue_number)
-                        except BadCredentialsException:
-                            user_token, g, repo = refresh_token()
-                            cloned_repo.token = user_token
-
-                        current_issue.edit(
-                            body=summary + "\n\n" + condensed_checkboxes_collapsible
+                                "X"
+                                if file_change_request.status
+                                in ("succeeded", "failed")
+                                else " "
+                            ),
                         )
-
-                        logger.info(files_progress)
-                        logger.info(f"Edited {file_change_request.entity_display}")
-                        edit_sweep_comment(checkboxes_contents, 2)
-                    if not response.get("success"):
-                        raise Exception(f"Failed to create PR: {response.get('error')}")
-
+                        for file_change_request in file_change_requests
+                    ]
                     checkboxes_contents = "\n".join(
                         [
                             checkbox_template.format(
                                 check=check,
                                 filename=filename,
                                 instructions=blockquote(instructions),
                             )
                             for filename, instructions, check in checkboxes_progress
                         ]
                     )
+                    collapsible_template.format(
+                        summary="Checklist",
+                        body=checkboxes_contents,
+                        opened="open",
+                    )
                     condensed_checkboxes_contents = "\n".join(
                         [
                             checkbox_template.format(
                                 check=check,
                                 filename=filename,
                                 instructions="",
                             ).strip()
@@ -1320,494 +1208,558 @@
                         ]
                     )
                     condensed_checkboxes_collapsible = collapsible_template.format(
                         summary="Checklist",
                         body=condensed_checkboxes_contents,
                         opened="open",
                     )
-                    for _ in range(3):
-                        try:
-                            current_issue.edit(
-                                body=summary + "\n\n" + condensed_checkboxes_collapsible
-                            )
-                            break
-                        except Exception:
-                            from time import sleep
 
-                            sleep(1)
+                    try:
+                        current_issue = repo.get_issue(number=issue_number)
+                    except BadCredentialsException:
+                        user_token, g, repo = refresh_token()
+                        cloned_repo.token = user_token
+
+                    current_issue.edit(
+                        body=summary + "\n\n" + condensed_checkboxes_collapsible
+                    )
+
+                    logger.info(files_progress)
                     edit_sweep_comment(checkboxes_contents, 2)
+                if not response.get("success"):
+                    raise Exception(f"Failed to create PR: {response.get('error')}")
 
-                    pr_changes = response["pull_request"]
-                    # change the body here
-                    diff_text = get_branch_diff_text(
-                        repo=repo,
-                        branch=pull_request.branch_name,
-                        base_branch=overrided_branch_name,
-                    )
-                    new_description = PRDescriptionBot().describe_diffs(
-                        diff_text,
-                        pull_request.title,
-                    )
-                    # TODO: update the title as well
-                    if new_description:
-                        pr_changes.body = (
-                            f"{new_description}\n\nFixes"
-                            f" #{issue_number}.\n\n---\n\n{UPDATES_MESSAGE}\n\n---\n\n{INSTRUCTIONS_FOR_REVIEW}{BOT_SUFFIX}"
+                checkboxes_contents = "\n".join(
+                    [
+                        checkbox_template.format(
+                            check=check,
+                            filename=filename,
+                            instructions=blockquote(instructions),
+                        )
+                        for filename, instructions, check in checkboxes_progress
+                    ]
+                )
+                condensed_checkboxes_contents = "\n".join(
+                    [
+                        checkbox_template.format(
+                            check=check,
+                            filename=filename,
+                            instructions="",
+                        ).strip()
+                        for filename, instructions, check in checkboxes_progress
+                        if not instructions.lower().startswith("run")
+                    ]
+                )
+                condensed_checkboxes_collapsible = collapsible_template.format(
+                    summary="Checklist",
+                    body=condensed_checkboxes_contents,
+                    opened="open",
+                )
+                for _ in range(3):
+                    try:
+                        current_issue.edit(
+                            body=summary + "\n\n" + condensed_checkboxes_collapsible
                         )
+                        break
+                    except Exception:
+                        from time import sleep
 
+                        sleep(1)
+                edit_sweep_comment(checkboxes_contents, 2)
+
+                pr_changes = response["pull_request"]
+                # change the body here
+                diff_text = get_branch_diff_text(
+                    repo=repo,
+                    branch=pull_request.branch_name,
+                    base_branch=overrided_branch_name,
+                )
+                new_description = PRDescriptionBot().describe_diffs(
+                    diff_text,
+                    pull_request.title,
+                )
+                # TODO: update the title as well
+                if new_description:
+                    pr_changes.body = (
+                        f"{new_description}\n\nFixes"
+                        f" #{issue_number}.\n\n---\n\n{UPDATES_MESSAGE}\n\n---\n\n{INSTRUCTIONS_FOR_REVIEW}{BOT_SUFFIX}"
+                    )
+
+                edit_sweep_comment(
+                    "I have finished coding the issue. I am now reviewing it for completeness.",
+                    3,
+                )
+                change_location = f" [`{pr_changes.pr_head}`](https://github.com/{repo_full_name}/commits/{pr_changes.pr_head}).\n\n"
+                review_message = (
+                    "Here are my self-reviews of my changes at" + change_location
+                )
+
+                try:
+                    fire_and_forget_wrapper(remove_emoji)(content_to_delete="eyes")
+                except SystemExit:
+                    raise SystemExit
+                except Exception:
+                    pass
+
+                changes_required, review_message = False, ""
+                if changes_required:
                     edit_sweep_comment(
-                        "I have finished coding the issue. I am now reviewing it for completeness.",
+                        review_message
+                        + "\n\nI finished incorporating these changes.",
                         3,
                     )
-                    change_location = f" [`{pr_changes.pr_head}`](https://github.com/{repo_full_name}/commits/{pr_changes.pr_head}).\n\n"
-                    review_message = (
-                        "Here are my self-reviews of my changes at" + change_location
+                else:
+                    edit_sweep_comment(
+                        f"I have finished reviewing the code for completeness. I did not find errors for {change_location}",
+                        3,
                     )
 
-                    try:
-                        fire_and_forget_wrapper(remove_emoji)(content_to_delete="eyes")
-                    except SystemExit:
-                        raise SystemExit
-                    except Exception:
-                        pass
-
-                    changes_required, review_message = False, ""
-                    if changes_required:
-                        edit_sweep_comment(
-                            review_message
-                            + "\n\nI finished incorporating these changes.",
-                            3,
-                        )
-                    else:
-                        edit_sweep_comment(
-                            f"I have finished reviewing the code for completeness. I did not find errors for {change_location}",
-                            3,
-                        )
-
-                    pr_actions_message = (
-                        create_action_buttons(
-                            [
-                                SWEEP_GOOD_FEEDBACK,
-                                SWEEP_BAD_FEEDBACK,
-                            ],
-                            header="### PR Feedback (click)\n",
-                        )
-                        + "\n"
-                        if DISCORD_FEEDBACK_WEBHOOK_URL is not None
-                        else ""
+                pr_actions_message = (
+                    create_action_buttons(
+                        [
+                            SWEEP_GOOD_FEEDBACK,
+                            SWEEP_BAD_FEEDBACK,
+                        ],
+                        header="### PR Feedback (click)\n",
                     )
-                    revert_buttons = []
-                    for changed_file in set(changed_files):
-                        revert_buttons.append(
-                            Button(label=f"{RESET_FILE} {changed_file}")
-                        )
-                    revert_buttons_list = ButtonList(
-                        buttons=revert_buttons, title=REVERT_CHANGED_FILES_TITLE
+                    + "\n"
+                    if DISCORD_FEEDBACK_WEBHOOK_URL is not None
+                    else ""
+                )
+                revert_buttons = []
+                for changed_file in set(changed_files):
+                    revert_buttons.append(
+                        Button(label=f"{RESET_FILE} {changed_file}")
                     )
+                revert_buttons_list = ButtonList(
+                    buttons=revert_buttons, title=REVERT_CHANGED_FILES_TITLE
+                )
 
-                    rule_buttons = []
-                    repo_rules = get_rules(repo) or []
-                    if repo_rules != [""] and repo_rules != []:
-                        for rule in repo_rules or []:
-                            if rule:
-                                rule_buttons.append(
-                                    Button(label=f"{RULES_LABEL} {rule}")
-                                )
-                        if len(repo_rules) == 0:
-                            for rule in DEFAULT_RULES:
-                                rule_buttons.append(
-                                    Button(label=f"{RULES_LABEL} {rule}")
-                                )
-
-                    rules_buttons_list = ButtonList(
-                        buttons=rule_buttons, title=RULES_TITLE
-                    )
-
-                    sandbox_passed = None
-                    for file_change_request in file_change_requests:
-                        if file_change_request.change_type == "check":
-                            if (
-                                file_change_request.sandbox_response
-                                and file_change_request.sandbox_response.error_messages
-                            ):
-                                sandbox_passed = False
-                            elif sandbox_passed is None:
-                                sandbox_passed = True
-
-                    # delete failing sweep yaml if applicable
-                    if sweep_yml_failed:
-                        try:
-                            repo.delete_file(
-                                "sweep.yaml",
-                                "Delete failing sweep.yaml",
-                                branch=pr_changes.pr_head,
-                                sha=repo.get_contents("sweep.yaml").sha,
+                rule_buttons = []
+                repo_rules = get_rules(repo) or []
+                if repo_rules != [""] and repo_rules != []:
+                    for rule in repo_rules or []:
+                        if rule:
+                            rule_buttons.append(
+                                Button(label=f"{RULES_LABEL} {rule}")
+                            )
+                    if len(repo_rules) == 0:
+                        for rule in DEFAULT_RULES:
+                            rule_buttons.append(
+                                Button(label=f"{RULES_LABEL} {rule}")
                             )
-                        except Exception:
-                            pass
 
-                    # create draft pr, then convert to regular pr if it all is well
-                    is_draft_pr = True
-                    # if we are on our last attempt we just create a normal pr
-                    if run_attempt >= max_pr_attempts - 1:
-                        is_draft_pr = False
-                    pr: GithubPullRequest = repo.create_pull(
-                        title=pr_changes.title,
-                        body=pr_actions_message + pr_changes.body,
-                        head=pr_changes.pr_head,
-                        base=overrided_branch_name or SweepConfig.get_branch(repo),
-                        # TODO: reenable it later
-                        draft=is_draft_pr and False,
-                    )
+                rules_buttons_list = ButtonList(
+                    buttons=rule_buttons, title=RULES_TITLE
+                )
 
+                sandbox_passed = None
+                for file_change_request in file_change_requests:
+                    if file_change_request.change_type == "check":
+                        if (
+                            file_change_request.sandbox_response
+                            and file_change_request.sandbox_response.error_messages
+                        ):
+                            sandbox_passed = False
+                        elif sandbox_passed is None:
+                            sandbox_passed = True
+
+                # delete failing sweep yaml if applicable
+                if sweep_yml_failed:
                     try:
-                        pr.add_to_assignees(username)
-                    except Exception as e:
-                        logger.error(
-                            f"Failed to add assignee {username}: {e}, probably a bot."
+                        repo.delete_file(
+                            "sweep.yaml",
+                            "Delete failing sweep.yaml",
+                            branch=pr_changes.pr_head,
+                            sha=repo.get_contents("sweep.yaml").sha,
                         )
+                    except Exception:
+                        pass
 
-                    ticket_progress.status = TicketProgressStatus.COMPLETE
-                    ticket_progress.context.done_time = time()
-                    ticket_progress.context.pr_id = pr.number
-                    ticket_progress.save()
-
-                    if revert_buttons:
-                        pr.create_issue_comment(
-                            revert_buttons_list.serialize() + BOT_SUFFIX
-                        )
-                    if rule_buttons:
-                        pr.create_issue_comment(
-                            rules_buttons_list.serialize() + BOT_SUFFIX
-                        )
+                # create draft pr, then convert to regular pr later
+                pr: GithubPullRequest = repo.create_pull(
+                    title=pr_changes.title,
+                    body=pr_actions_message + pr_changes.body,
+                    head=pr_changes.pr_head,
+                    base=overrided_branch_name or SweepConfig.get_branch(repo),
+                    # TODO: reenable it later
+                    draft=True,
+                )
 
-                    # add comments before labelling
-                    pr.add_to_labels(GITHUB_LABEL_NAME)
-                    current_issue.create_reaction("rocket")
-                    heres_pr_message = f'<h1 align="center">🚀 Here\'s the PR! <a href="{pr.html_url}">#{pr.number}</a></h1>'
-                    progress_message = f'<div align="center"><b>See Sweep\'s progress at <a href="{PROGRESS_BASE_URL}/issues/{tracking_id}">the progress dashboard</a>!</b></div>'
-                    edit_sweep_comment(
-                        review_message + "\n\nSuccess! 🚀",
-                        4,
-                        pr_message=(
-                            f"{center(heres_pr_message)}\n{center(progress_message)}\n{center(payment_message_start)}"
-                        ),
-                        done=True,
+                try:
+                    pr.add_to_assignees(username)
+                except Exception as e:
+                    logger.error(
+                        f"Failed to add assignee {username}: {e}, probably a bot."
                     )
 
-                    user_settings = UserSettings.from_username(username=username)
-                    user = g.get_user(username)
-                    full_name = user.name or user.login
-                    name = full_name.split(" ")[0]
-                    files_changed = []
-                    for fcr in file_change_requests:
-                        if fcr.change_type in ("create", "modify"):
-                            diff = list(
-                                difflib.unified_diff(
-                                    (fcr.old_content or "").splitlines() or [],
-                                    (fcr.new_content or "").splitlines() or [],
-                                    lineterm="",
-                                )
-                            )
-                            added = sum(
-                                1
-                                for line in diff
-                                if line.startswith("+") and not line.startswith("+++")
-                            )
-                            removed = sum(
-                                1
-                                for line in diff
-                                if line.startswith("-") and not line.startswith("---")
-                            )
-                            files_changed.append(
-                                f"<code>{fcr.filename}</code> (+{added}/-{removed})"
-                            )
-                    user_settings.send_email(
-                        subject=f"Sweep Pull Request Complete for {repo_name}#{issue_number} {title}",
-                        html=email_template.format(
-                            name=name,
-                            pr_url=pr.html_url,
-                            issue_number=issue_number,
-                            repo_full_name=repo_full_name,
-                            pr_number=pr.number,
-                            progress_url=f"{PROGRESS_BASE_URL}/issues/{tracking_id}",
-                            summary=markdown.markdown(pr_changes.body),
-                            files_changed="\n".join(
-                                [f"<li>{item}</li>" for item in files_changed]
-                            ),
-                            sweeping_gif=sweeping_gif,
-                        ),
-                    )
+                ticket_progress.status = TicketProgressStatus.COMPLETE
+                ticket_progress.context.done_time = time()
+                ticket_progress.context.pr_id = pr.number
+                ticket_progress.save()
 
-                    # TODO: re-enable this later
-                    # poll for github to check when gha are done or not
-                    pr_created_successfully = False
-                    total_poll_attempts = 0
-                    if False:
-                        while True:
-                            logger.info(
-                                f"Polling to see if Github Actions have finished... {total_poll_attempts}"
-                            )
-                            # we wait at most 60 minutes
-                            if total_poll_attempts >= 60:
-                                pr_created_successfully = False
-                                break
-                            else:
-                                # wait one minute between check attempts
-                                total_poll_attempts += 1
-                                from time import sleep
-
-                                sleep(60)
-                            runs = list(repo.get_workflow_runs(branch=pr.head.ref))
-                            # if all runs have succeeded, break
-                            if all([run.conclusion == "success" for run in runs]):
-                                pr_created_successfully = True
-                                break
-                            # if any of them have failed we retry
-                            if any([run.conclusion == "failure" for run in runs]):
-                                pr_created_successfully = False
-                                failed_runs = [
-                                    run for run in runs if run.conclusion == "failure"
-                                ]
-
-                                failed_gha_logs: list[Message] = get_failing_gha_logs(
-                                    failed_runs
-                                )
-                                if failed_gha_logs:
-                                    failing_gha_messages.extend(failed_gha_logs)
-                                logger.info(
-                                    f"Rerunning issue {issue_url} as some workflows failed! Rerun attempt {run_attempt + 1}"
-                                )
-                                # clean up by closing pr and deleting branch associated with pr before restarting on_ticket logic
-                                # unless this is sweep's last attempt
-                                if run_attempt < 2:
-                                    try:
-                                        pr.edit(
-                                            state="closed",
-                                            title=pr.title
-                                            + f" (Closed due to failing Github Action: Attempt {run_attempt + 1})",
-                                        )
-                                        if pr.head.ref.startswith("sweep"):
-                                            repo.get_git_ref(
-                                                f"heads/{pr.head.ref}"
-                                            ).delete()
-                                    except Exception as e:
-                                        logger.error(
-                                            f"Failed to clean up branch {pr.head.ref} and pr before restarting: {e}"
-                                        )
-                                break
-                            # if none of the runs have completed we wait and poll github
-                            logger.info(
-                                "No Github Actions have failed yet and not all have succeeded yet, waiting for 60 seconds before polling again..."
-                            )
-                        # break from main for loop
-                        if pr_created_successfully:
-                            logger.info(
-                                f"All Github Actions have finished successfully! It took {run_attempt + 1} attempts to create the PR. It took {total_poll_attempts + 1} minutes for all Github Actions to finish."
-                            )
-                            # convert draft pr to normal one
-                            convert_pr_draft_field(pr, is_draft=False)
-                            break
+                if revert_buttons:
+                    pr.create_issue_comment(
+                        revert_buttons_list.serialize() + BOT_SUFFIX
+                    )
+                if rule_buttons:
+                    pr.create_issue_comment(
+                        rules_buttons_list.serialize() + BOT_SUFFIX
+                    )
+
+                # add comments before labelling
+                pr.add_to_labels(GITHUB_LABEL_NAME)
+                current_issue.create_reaction("rocket")
+                heres_pr_message = f'<h1 align="center">🚀 Here\'s the PR! <a href="{pr.html_url}">#{pr.number}</a></h1>'
+                progress_message = f'<div align="center"><b>See Sweep\'s progress at <a href="{PROGRESS_BASE_URL}/issues/{tracking_id}">the progress dashboard</a>!</b></div>'
+                edit_sweep_comment(
+                    review_message + "\n\nSuccess! 🚀",
+                    4,
+                    pr_message=(
+                        f"{center(heres_pr_message)}\n{center(progress_message)}\n{center(payment_message_start)}"
+                    ),
+                    done=True,
+                )
 
-                except MaxTokensExceeded as e:
-                    logger.info("Max tokens exceeded")
-                    ticket_progress.status = TicketProgressStatus.ERROR
-                    ticket_progress.error_message = "Max tokens exceeded. Feel free to add more details to the issue descript for Sweep to better address it, or alternatively, reach out to Kevin or William for help at https://discord.gg/sweep."
-                    ticket_progress.save()
-                    log_error(
-                        is_paying_user,
-                        is_consumer_tier,
-                        username,
-                        issue_url,
-                        "Max Tokens Exceeded",
-                        str(e) + "\n" + traceback.format_exc(),
-                        priority=2,
+                user_settings = UserSettings.from_username(username=username)
+                user = g.get_user(username)
+                full_name = user.name or user.login
+                name = full_name.split(" ")[0]
+                files_changed = []
+                for fcr in file_change_requests:
+                    if fcr.change_type in ("create", "modify"):
+                        diff = list(
+                            difflib.unified_diff(
+                                (fcr.old_content or "").splitlines() or [],
+                                (fcr.new_content or "").splitlines() or [],
+                                lineterm="",
+                            )
+                        )
+                        added = sum(
+                            1
+                            for line in diff
+                            if line.startswith("+") and not line.startswith("+++")
+                        )
+                        removed = sum(
+                            1
+                            for line in diff
+                            if line.startswith("-") and not line.startswith("---")
+                        )
+                        files_changed.append(
+                            f"<code>{fcr.filename}</code> (+{added}/-{removed})"
+                        )
+                user_settings.send_email(
+                    subject=f"Sweep Pull Request Complete for {repo_name}#{issue_number} {title}",
+                    html=email_template.format(
+                        name=name,
+                        pr_url=pr.html_url,
+                        issue_number=issue_number,
+                        repo_full_name=repo_full_name,
+                        pr_number=pr.number,
+                        progress_url=f"{PROGRESS_BASE_URL}/issues/{tracking_id}",
+                        summary=markdown.markdown(pr_changes.body),
+                        files_changed="\n".join(
+                            [f"<li>{item}</li>" for item in files_changed]
+                        ),
+                        sweeping_gif=sweeping_gif,
+                    ),
+                )
+
+                # poll for github to check when gha are done
+                total_poll_attempts = 0
+                total_edit_attempts = 0
+                SLEEP_DURATION_SECONDS = 15
+                GITHUB_ACTIONS_ENABLED = get_gha_enabled(repo=repo) and DEPLOYMENT_GHA_ENABLED
+                GHA_MAX_EDIT_ATTEMPTS = 1 # max number of times to edit PR
+                while True and GITHUB_ACTIONS_ENABLED:
+                    logger.info(
+                        f"Polling to see if Github Actions have finished... {total_poll_attempts}"
                     )
-                    if chat_logger and chat_logger.is_paying_user():
-                        edit_sweep_comment(
-                            (
-                                f"Sorry, I could not edit `{e.filename}` as this file is too long."
-                                " We are currently working on improved file streaming to address"
-                                " this issue.\n"
-                            ),
-                            -1,
-                        )
+                    # we wait at most 60 minutes
+                    if total_poll_attempts * SLEEP_DURATION_SECONDS // 60 >= 60:
+                        break
                     else:
-                        edit_sweep_comment(
-                            (
-                                f"Sorry, I could not edit `{e.filename}` as this file is too"
-                                " long.\n\nIf this file is incorrect, please describe the desired"
-                                " file in the prompt. However, if you would like to edit longer"
-                                " files, consider upgrading to [Sweep Pro](https://sweep.dev/) for"
-                                " longer context lengths.\n"
-                            ),
-                            -1,
-                        )
-                    delete_branch = True
-                    raise e
-                except NoFilesException as e:
-                    ticket_progress.status = TicketProgressStatus.ERROR
-                    ticket_progress.error_message = "Sweep could not find files to modify to address this issue. Feel free to add more details to the issue descript for Sweep to better address it, or alternatively, reach out to Kevin or William for help at https://discord.gg/sweep."
-                    ticket_progress.save()
+                        # wait one minute between check attempts
+                        total_poll_attempts += 1
+                        from time import sleep
+
+                        sleep(SLEEP_DURATION_SECONDS)
+                    runs = list(repo.get_workflow_runs(branch=pr.head.ref, head_sha=pr.head.sha))
+                    # if all runs have succeeded, break
+                    if all([run.conclusion == "success" for run in runs]):
+                        break
+                    # if any of them have failed we retry
+                    if any([run.conclusion == "failure" for run in runs]):
+                        failed_runs = [
+                            run for run in runs if run.conclusion == "failure"
+                        ]
 
-                    logger.info("Sweep could not find files to modify")
-                    log_error(
-                        is_paying_user,
-                        is_consumer_tier,
-                        username,
-                        issue_url,
-                        "Sweep could not find files to modify",
-                        str(e) + "\n" + traceback.format_exc(),
-                        priority=2,
-                    )
+                        failed_gha_logs: list[str] = get_failing_gha_logs(
+                            failed_runs,
+                            installation_id,
+                        )
+                        if failed_gha_logs:
+                            # make edits to the PR
+                            # TODO: look into rollbacks so we don't continue adding onto errors
+                            cloned_repo = ClonedRepo( # reinitialize cloned_repo to avoid conflicts
+                                repo_full_name,
+                                installation_id=installation_id,
+                                token=user_token,
+                                repo=repo,
+                                branch=pr.head.ref,
+                            )
+                            diffs = get_branch_diff_text(repo=repo, branch=pr.head.ref, base_branch=pr.base.ref)
+                            problem_statement = f"{title}\n{summary}\n{replies_text}"
+                            all_information_prompt = f"While trying to address the user request:\n<user_request>\n{problem_statement}\n</user_request>\n{failed_gha_logs}\nThese are the changes that were previously made:\n<diffs>\n{diffs}\n</diffs>\n\nFix the failing logs."
+                            
+                            repo_context_manager = prep_snippets(cloned_repo=cloned_repo, query=(title + summary + replies_text).strip("\n"), ticket_progress=ticket_progress) # need to do this, can use the old query for speed
+                            repo_context_manager = get_relevant_context(
+                                all_information_prompt,
+                                repo_context_manager,
+                                ticket_progress,
+                                chat_logger=chat_logger,
+                                import_graph=None,
+                                num_rollouts=1,
+                            )
+                            sweep_bot: SweepBot = construct_sweep_bot(
+                                repo=repo,
+                                repo_name=repo_name,
+                                issue_url=issue_url,
+                                repo_description=repo_description,
+                                title="Fix the following errors to complete the user request.",
+                                message_summary=all_information_prompt,
+                                cloned_repo=cloned_repo,
+                                ticket_progress=ticket_progress,
+                                chat_logger=chat_logger,
+                                snippets=snippets,
+                                tree=tree,
+                                comments=comments,
+                            )
+                            file_change_requests, plan = get_files_to_change(
+                                relevant_snippets=repo_context_manager.current_top_snippets,
+                                read_only_snippets=repo_context_manager.read_only_snippets,
+                                problem_statement=all_information_prompt,
+                                repo_name=repo_full_name,
+                            )
+                            validate_file_change_requests(file_change_requests, cloned_repo)
+                            previous_modify_files_dict: dict[str, dict[str, str | list[str]]] | None = None
+                            sweep_bot.handle_modify_file_main(
+                                branch=pr.head.ref,
+                                assistant_conversation=None,
+                                additional_messages=[],
+                                previous_modify_files_dict=previous_modify_files_dict,
+                                file_change_requests=file_change_requests
+                            )
+                            pr = repo.get_pull(pr.number) # IMPORTANT: resync PR otherwise you'll fetch old GHA runs
+                            total_edit_attempts += 1
+                            if total_edit_attempts >= GHA_MAX_EDIT_ATTEMPTS:
+                                logger.info(f"Tried to edit PR {GHA_MAX_EDIT_ATTEMPTS} times, giving up.")
+                                break
+                    # if none of the runs have completed we wait and poll github
+                    logger.info(
+                        f"No Github Actions have failed yet and not all have succeeded yet, waiting for {SLEEP_DURATION_SECONDS} seconds before polling again..."
+                    )
+                # break from main for loop
+                convert_pr_draft_field(pr, is_draft=False, installation_id=installation_id)
+            except MaxTokensExceeded as e:
+                logger.info("Max tokens exceeded")
+                ticket_progress.status = TicketProgressStatus.ERROR
+                ticket_progress.error_message = "Max tokens exceeded. Feel free to add more details to the issue descript for Sweep to better address it, or alternatively, reach out to Kevin or William for help at https://discord.gg/sweep."
+                ticket_progress.save()
+                log_error(
+                    is_paying_user,
+                    is_consumer_tier,
+                    username,
+                    issue_url,
+                    "Max Tokens Exceeded",
+                    str(e) + "\n" + traceback.format_exc(),
+                    priority=2,
+                )
+                if chat_logger and chat_logger.is_paying_user():
                     edit_sweep_comment(
                         (
-                            "Sorry, Sweep could not find any appropriate files to edit to address"
-                            " this issue. If this is a mistake, please provide more context and Sweep"
-                            f" will retry!\n\n> @{username}, please edit the issue description to"
-                            " include more details about this issue."
+                            f"Sorry, I could not edit `{e.filename}` as this file is too long."
+                            " We are currently working on improved file streaming to address"
+                            " this issue.\n"
                         ),
                         -1,
                     )
-                    delete_branch = True
-                    raise e
-                except openai.BadRequestError as e:
-                    ticket_progress.status = TicketProgressStatus.ERROR
-                    ticket_progress.error_message = "Sorry, it looks like there is an error with communicating with OpenAI. If this error persists, reach out to Kevin or William for help at https://discord.gg/sweep."
-                    ticket_progress.save()
-
-                    logger.error(traceback.format_exc())
-                    logger.error(e)
+                else:
                     edit_sweep_comment(
                         (
-                            "I'm sorry, but it looks our model has ran out of context length. We're"
-                            " trying to make this happen less, but one way to mitigate this is to"
-                            " code smaller files. If this error persists report it at"
-                            " https://discord.gg/sweep."
+                            f"Sorry, I could not edit `{e.filename}` as this file is too"
+                            " long.\n\nIf this file is incorrect, please describe the desired"
+                            " file in the prompt. However, if you would like to edit longer"
+                            " files, consider upgrading to [Sweep Pro](https://sweep.dev/) for"
+                            " longer context lengths.\n"
                         ),
                         -1,
                     )
-                    log_error(
-                        is_paying_user,
-                        is_consumer_tier,
-                        username,
-                        issue_url,
-                        "Context Length",
-                        str(e) + "\n" + traceback.format_exc(),
-                        priority=2,
-                    )
-                    posthog.capture(
-                        username,
-                        "failed",
-                        properties={
-                            "error": str(e),
-                            "trace": traceback.format_exc(),
-                            "reason": "Invalid request error / context length",
-                            **metadata,
-                            "duration": round(time() - on_ticket_start_time),
-                        },
-                    )
-                    delete_branch = True
-                    raise e
-                except AssistantRaisedException as e:
-                    if ticket_progress is not None:
-                        ticket_progress.status = TicketProgressStatus.ERROR
-                        ticket_progress.error_message = f"Sweep raised an error with the following message: {e.message}. Feel free to add more details to the issue descript for Sweep to better address it, or alternatively, reach out to Kevin or William for help at https://discord.gg/sweep."
-                        ticket_progress.save()
-
-                    logger.exception(e)
-                    edit_sweep_comment(
-                        f"Sweep raised an error with the following message:\n{blockquote(e.message)}",
-                        -1,
-                    )
-                    log_error(
-                        is_paying_user,
-                        is_consumer_tier,
-                        username,
-                        issue_url,
-                        "Workflow",
-                        str(e) + "\n" + traceback.format_exc(),
-                        priority=1,
-                    )
-                    raise e
-                except Exception as e:
-                    ticket_progress.status = TicketProgressStatus.ERROR
-                    ticket_progress.error_message = f"Internal server error: {str(e)}. Feel free to add more details to the issue descript for Sweep to better address it, or alternatively, reach out to Kevin or William for help at https://discord.gg/sweep."
-                    ticket_progress.save()
+                delete_branch = True
+                raise e
+            except NoFilesException as e:
+                ticket_progress.status = TicketProgressStatus.ERROR
+                ticket_progress.error_message = "Sweep could not find files to modify to address this issue. Feel free to add more details to the issue descript for Sweep to better address it, or alternatively, reach out to Kevin or William for help at https://discord.gg/sweep."
+                ticket_progress.save()
 
-                    logger.error(traceback.format_exc())
-                    logger.error(e)
-                    # title and summary are defined elsewhere
-                    if len(title + summary) < 60:
-                        edit_sweep_comment(
-                            (
-                                "I'm sorry, but it looks like an error has occurred due to"
-                                + " a planning failure. Feel free to add more details to the issue description"
-                                + " so Sweep can better address it. Alternatively, reach out to Kevin or William for help at"
-                                + " https://discord.gg/sweep."
-                            ),
-                            -1,
-                        )
-                    else:
-                        edit_sweep_comment(
-                            (
-                                "I'm sorry, but it looks like an error has occurred due to"
-                                + " a planning failure. Feel free to add more details to the issue description"
-                                + " so Sweep can better address it. Alternatively, reach out to Kevin or William for help at"
-                                + " https://discord.gg/sweep."
-                            ),
-                            -1,
-                        )
-                    log_error(
-                        is_paying_user,
-                        is_consumer_tier,
-                        username,
-                        issue_url,
-                        "Workflow",
-                        str(e) + "\n" + traceback.format_exc(),
-                        priority=1,
-                    )
-                    raise e
-                else:
-                    try:
-                        fire_and_forget_wrapper(remove_emoji)(content_to_delete="eyes")
-                        fire_and_forget_wrapper(add_emoji)("rocket")
-                    except SystemExit:
-                        raise SystemExit
-                    except Exception as e:
-                        logger.error(e)
+                logger.info("Sweep could not find files to modify")
+                log_error(
+                    is_paying_user,
+                    is_consumer_tier,
+                    username,
+                    issue_url,
+                    "Sweep could not find files to modify",
+                    str(e) + "\n" + traceback.format_exc(),
+                    priority=2,
+                )
+                edit_sweep_comment(
+                    (
+                        "Sorry, Sweep could not find any appropriate files to edit to address"
+                        " this issue. If this is a mistake, please provide more context and Sweep"
+                        f" will retry!\n\n> @{username}, please edit the issue description to"
+                        " include more details about this issue."
+                    ),
+                    -1,
+                )
+                delete_branch = True
+                raise e
+            except openai.BadRequestError as e:
+                ticket_progress.status = TicketProgressStatus.ERROR
+                ticket_progress.error_message = "Sorry, it looks like there is an error with communicating with OpenAI. If this error persists, reach out to Kevin or William for help at https://discord.gg/sweep."
+                ticket_progress.save()
 
-                if delete_branch:
-                    try:
-                        if pull_request.branch_name.startswith("sweep"):
-                            repo.get_git_ref(
-                                f"heads/{pull_request.branch_name}"
-                            ).delete()
-                        else:
-                            raise Exception(
-                                f"Branch name {pull_request.branch_name} does not start with sweep/"
-                            )
-                    except SystemExit:
-                        raise SystemExit
-                    except Exception as e:
-                        logger.error(e)
-                        logger.error(traceback.format_exc())
-                        logger.info("Deleted branch", pull_request.branch_name)
-            except Exception as e:
+                logger.error(traceback.format_exc())
+                logger.error(e)
+                edit_sweep_comment(
+                    (
+                        "I'm sorry, but it looks our model has ran out of context length. We're"
+                        " trying to make this happen less, but one way to mitigate this is to"
+                        " code smaller files. If this error persists report it at"
+                        " https://discord.gg/sweep."
+                    ),
+                    -1,
+                )
+                log_error(
+                    is_paying_user,
+                    is_consumer_tier,
+                    username,
+                    issue_url,
+                    "Context Length",
+                    str(e) + "\n" + traceback.format_exc(),
+                    priority=2,
+                )
                 posthog.capture(
                     username,
                     "failed",
                     properties={
-                        **metadata,
                         "error": str(e),
                         "trace": traceback.format_exc(),
+                        "reason": "Invalid request error / context length",
+                        **metadata,
                         "duration": round(time() - on_ticket_start_time),
                     },
                 )
+                delete_branch = True
+                raise e
+            except AssistantRaisedException as e:
+                if ticket_progress is not None:
+                    ticket_progress.status = TicketProgressStatus.ERROR
+                    ticket_progress.error_message = f"Sweep raised an error with the following message: {e.message}. Feel free to add more details to the issue descript for Sweep to better address it, or alternatively, reach out to Kevin or William for help at https://discord.gg/sweep."
+                    ticket_progress.save()
+
+                logger.exception(e)
+                edit_sweep_comment(
+                    f"Sweep raised an error with the following message:\n{blockquote(e.message)}",
+                    -1,
+                )
+                log_error(
+                    is_paying_user,
+                    is_consumer_tier,
+                    username,
+                    issue_url,
+                    "Workflow",
+                    str(e) + "\n" + traceback.format_exc(),
+                    priority=1,
+                )
+                raise e
+            except Exception as e:
+                ticket_progress.status = TicketProgressStatus.ERROR
+                ticket_progress.error_message = f"Internal server error: {str(e)}. Feel free to add more details to the issue descript for Sweep to better address it, or alternatively, reach out to Kevin or William for help at https://discord.gg/sweep."
+                ticket_progress.save()
+
+                logger.error(traceback.format_exc())
+                logger.error(e)
+                # title and summary are defined elsewhere
+                if len(title + summary) < 60:
+                    edit_sweep_comment(
+                        (
+                            "I'm sorry, but it looks like an error has occurred due to"
+                            + " a planning failure. Feel free to add more details to the issue description"
+                            + " so Sweep can better address it. Alternatively, reach out to Kevin or William for help at"
+                            + " https://discord.gg/sweep."
+                        ),
+                        -1,
+                    )
+                else:
+                    edit_sweep_comment(
+                        (
+                            "I'm sorry, but it looks like an error has occurred due to"
+                            + " a planning failure. Feel free to add more details to the issue description"
+                            + " so Sweep can better address it. Alternatively, reach out to Kevin or William for help at"
+                            + " https://discord.gg/sweep."
+                        ),
+                        -1,
+                    )
+                log_error(
+                    is_paying_user,
+                    is_consumer_tier,
+                    username,
+                    issue_url,
+                    "Workflow",
+                    str(e) + "\n" + traceback.format_exc(),
+                    priority=1,
+                )
                 raise e
+            else:
+                try:
+                    fire_and_forget_wrapper(remove_emoji)(content_to_delete="eyes")
+                    fire_and_forget_wrapper(add_emoji)("rocket")
+                except SystemExit:
+                    raise SystemExit
+                except Exception as e:
+                    logger.error(e)
+
+            if delete_branch:
+                try:
+                    if pull_request.branch_name.startswith("sweep"):
+                        repo.get_git_ref(
+                            f"heads/{pull_request.branch_name}"
+                        ).delete()
+                    else:
+                        raise Exception(
+                            f"Branch name {pull_request.branch_name} does not start with sweep/"
+                        )
+                except SystemExit:
+                    raise SystemExit
+                except Exception as e:
+                    logger.error(e)
+                    logger.error(traceback.format_exc())
+                    logger.info("Deleted branch", pull_request.branch_name)
+        except Exception as e:
+            posthog.capture(
+                username,
+                "failed",
+                properties={
+                    **metadata,
+                    "error": str(e),
+                    "trace": traceback.format_exc(),
+                    "duration": round(time() - on_ticket_start_time),
+                },
+            )
+            raise e
         posthog.capture(
             username,
             "success",
             properties={**metadata, "duration": round(time() - on_ticket_start_time)},
         )
         logger.info("on_ticket success in " + str(round(time() - on_ticket_start_time)))
         return {"success": True}
@@ -1952,8 +1904,8 @@
         + (purchase_message if not is_paying_user else "")
     )
     payment_message_start = (
         f"{user_type}: I'm using {model_name}. You have {gpt_tickets_left_message}{daily_message}. (tracking ID: <code>{tracking_id}</code>)"
         + (purchase_message if not is_paying_user else "")
     )
 
-    return payment_message, payment_message_start
+    return payment_message, payment_message_start
```

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/pr_utils.py` & `sweepai-2.0.1/sweepai/handlers/pr_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,20 @@
     SWEEP_GOOD_FEEDBACK,
     SweepConfig,
     get_documentation_dict,
 )
 from sweepai.config.server import DISCORD_FEEDBACK_WEBHOOK_URL
 from sweepai.core.context_pruning import get_relevant_context
 from sweepai.core.entities import NoFilesException, SandboxResponse
-from sweepai.core.sweep_bot import SweepBot
+from sweepai.core.sweep_bot import SweepBot, get_files_to_change, validate_file_change_requests
 
 # from sandbox.sandbox_utils import Sandbox
 from sweepai.handlers.create_pr import GITHUB_LABEL_NAME, create_pr_changes
 from sweepai.utils.buttons import Button, ButtonList, create_action_buttons
 from sweepai.utils.chat_logger import ChatLogger
-from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import ClonedRepo, get_github_client
 from sweepai.utils.prompt_constructor import HumanMessagePrompt
 from sweepai.utils.ticket_utils import prep_snippets
 
 
 def make_pr(
     title,
@@ -77,26 +76,21 @@
     sweep_bot = SweepBot.from_system_message_content(
         human_message=human_message,
         repo=repo,
         is_reply=False,
         chat_logger=chat_logger,
         cloned_repo=cloned_repo,
     )
-
-    non_python_count = sum(
-        not file_path.endswith(".py") for file_path in human_message.get_file_paths()
-    )
-    python_count = len(human_message.get_file_paths()) - non_python_count
-    is_python_issue = python_count > non_python_count
-    posthog.capture(
-        username,
-        "is_python_issue",
-        properties={"is_python_issue": is_python_issue},
+    file_change_requests, plan = get_files_to_change(
+        relevant_snippets=repo_context_manager.current_top_snippets,
+        read_only_snippets=repo_context_manager.read_only_snippets,
+        problem_statement=formatted_query,
+        repo_name=repo_name,
     )
-    file_change_requests, plan = sweep_bot.get_files_to_change(is_python_issue)
+    validate_file_change_requests(file_change_requests, repo_context_manager.cloned_repo)
     file_change_requests = sweep_bot.validate_file_change_requests(
         file_change_requests, branch_name
     )
     pull_request = sweep_bot.generate_pull_request()
     generator = create_pr_changes(
         file_change_requests,
         pull_request,
```

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/stack_pr.py` & `sweepai-2.0.1/sweepai/handlers/stack_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/handlers/stack_pr_test.py` & `sweepai-2.0.1/sweepai/handlers/stack_pr_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/logn/cache.py` & `sweepai-2.0.1/sweepai/logn/cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from sweepai.config.server import DEBUG, REDIS_URL
 
 TEST_BOT_NAME = "sweep-nightly[bot]"
 MAX_DEPTH = 6
 # if DEBUG:
 #     logger.debug("File cache is disabled.")
-
+redis_client = Redis.from_url(REDIS_URL) if REDIS_URL else None
 
 def recursive_hash(value, depth=0, ignore_params=[]):
     """Hash primitives recursively with maximum depth."""
     if depth > MAX_DEPTH:
         return hashlib.md5("max_depth_reached".encode()).hexdigest()
 
     if isinstance(value, (int, float, str, bool, bytes)):
@@ -45,28 +45,29 @@
         return hashlib.md5("unknown".encode()).hexdigest()
 
 
 def hash_code(code):
     return hashlib.md5(code.encode()).hexdigest()
 
 
-def file_cache(ignore_params=[], verbose=False):
+def file_cache(ignore_params=[], verbose=False, redis=False):
     """Decorator to cache function output based on its inputs, ignoring specified parameters.
     Ignore parameters are used to avoid caching on non-deterministic inputs, such as timestamps.
     We can also ignore parameters that are slow to serialize/constant across runs, such as large objects.
     """
 
     def decorator(func):
         if DEBUG:
             return func
         func_source_code_hash = hash_code(inspect.getsource(func))
 
         def wrapper(*args, **kwargs):
-            cache_dir = "/tmp/file_cache"
+            cache_dir = os.environ.get("MOUNT_DIR", "") + "/tmp/file_cache"
             os.makedirs(cache_dir, exist_ok=True)
+            result = None
 
             # Convert args to a dictionary based on the function's signature
             args_names = func.__code__.co_varnames[: func.__code__.co_argcount]
             args_dict = dict(zip(args_names, args))
 
             # Remove ignored params
             kwargs_clone = kwargs.copy()
@@ -76,43 +77,62 @@
 
             # Create hash based on function name, input arguments, and function source code
             arg_hash = (
                 recursive_hash(args_dict, ignore_params=ignore_params)
                 + recursive_hash(kwargs_clone, ignore_params=ignore_params)
                 + func_source_code_hash
             )
+            cache_key = f"{func.__module__}_{func.__name__}_{arg_hash}"
             cache_file = os.path.join(
-                cache_dir, f"{func.__module__}_{func.__name__}_{arg_hash}.pickle"
+                cache_dir, f"{cache_key}.pickle"
             )
-
-            try:
-                # If cache exists, load and return it
-                if os.path.exists(cache_file):
-                    if verbose:
-                        print("Used cache for function: " + func.__name__)
-                    with open(cache_file, "rb") as f:
-                        return pickle.load(f)
-            except Exception:
-                logger.info("Unpickling failed")
-
+            if redis and redis_client: # only use this for LLM calls
+                try:
+                    cached_result = redis_client.get(cache_key)
+                    if cached_result:
+                        if verbose:
+                            print("Used redis cache for function: " + func.__name__)
+                        result = pickle.loads(cached_result)
+                except Exception:
+                    pass
+            if result is None:
+                try:
+                    # If cache exists, load and return it
+                    if os.path.exists(cache_file):
+                        if verbose:
+                            print("Used cache for function: " + func.__name__)
+                        with open(cache_file, "rb") as f:
+                            result = pickle.load(f)
+                except Exception:
+                    logger.info("Unpickling failed")
             # Otherwise, call the function and save its result to the cache
-            result = func(*args, **kwargs)
-            try:
-                with open(cache_file, "wb") as f:
-                    pickle.dump(result, f)
-            except Exception as e:
-                logger.info(f"Pickling failed: {e}")
+            if result is None:
+                result = func(*args, **kwargs)
+            # hydrate both caches in all cases
+            if redis and redis_client: # cache this to redis as well
+                try:
+                    # Cache the result using the unique cache key
+                    redis_client.set(cache_key, pickle.dumps(result))
+                except Exception as e:
+                    if verbose:
+                        print(f"Redis caching failed for function: {func.__name__}, Error: {e}")
+            if not isinstance(result, Exception):
+                try:
+                    with open(cache_file, "wb") as f:
+                        pickle.dump(result, f)
+                except Exception as e:
+                    logger.info(f"Pickling failed: {e}")
+            else:
+                logger.info(f"Function {func.__name__} returned an exception")
             return result
 
         return wrapper
 
     return decorator
 
-redis_client = Redis.from_url(REDIS_URL) if REDIS_URL else None
-
 
 def redis_cache(ignore_params=[], verbose=False):
     """Decorator to cache function output based on its inputs, using Redis.
     Ignores specified parameters for caching purposes."""
 
     def decorator(func):
         if not redis_client and DEBUG:
@@ -156,15 +176,15 @@
             return result
 
         return wrapper
 
     return decorator
 
 if __name__ == "__main__":
-    @redis_cache()
+    @file_cache(redis=True)
     def test_func(a, b):
         time.sleep(3)
         return a + b
 
     print("Running...")
     print(test_func(1, 1))
     print("Running again")
```

### Comparing `sweepai-2.0.0.dev1/sweepai/logn/logn.py` & `sweepai-2.0.1/sweepai/logn/logn.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/anthropic_client.py` & `sweepai-2.0.1/sweepai/utils/anthropic_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     DEFAULT_GPT4_32K_MODEL,
     OPENAI_API_KEY,
     OPENAI_API_TYPE,
     PAREA_API_KEY,
 )
 from parea import Parea
 
+from sweepai.logn.cache import file_cache
+
 parea_client = None
 try:
     if PAREA_API_KEY:
         parea_client = Parea(api_key=PAREA_API_KEY)
 except Exception as e:
     logger.info(f"Failed to initialize Parea client: {e}")
 
@@ -44,14 +46,15 @@
             self.client = Anthropic()
             if parea_client:
                 parea_client.wrap_anthropic_client(self.client)
             self.model = "claude-3-opus-20240229"
             logger.info(f"Using Anthropic model: {self.model}")
 
     # returns the clients response object
+    @file_cache(ignore_params=["self"])
     def get_response_message(self, messages: list[dict[str, str]], model: str = "", stop_sequences: list[str] = [], **kwargs):
         model = model or self.model
         # for anthropic the messages must be alternating user and assistant and we cannot have system as a role
         if OPENAI_API_TYPE == "anthropic":
             messages = sanitize_anthropic_messages(messages)
             response = self.client.messages.create(messages=messages, model=model, stop_sequences=stop_sequences, **kwargs)
         else:
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/autoimport.py` & `sweepai-2.0.1/sweepai/utils/autoimport.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/buttons.py` & `sweepai-2.0.1/sweepai/utils/buttons.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/buttons_test.py` & `sweepai-2.0.1/sweepai/utils/buttons_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/chat_logger.py` & `sweepai-2.0.1/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/code_tree.py` & `sweepai-2.0.1/sweepai/utils/code_tree.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/code_tree_test.py` & `sweepai-2.0.1/sweepai/utils/code_tree_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/comment_utils.py` & `sweepai-2.0.1/sweepai/utils/comment_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/comment_utils_test.py` & `sweepai-2.0.1/sweepai/utils/comment_utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/convert_openai_anthropic.py` & `sweepai-2.0.1/sweepai/utils/convert_openai_anthropic.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,20 +34,30 @@
 
 def convert_all_functions(functions: list) -> str:
     # convert all openai functions to print anthropic prompt
     for function in functions:
         print(convert_openai_function_to_anthropic_prompt(function))
 
 @dataclass
-class MockFunctionCall:
+class AnthropicFunctionCall:
     function_name: str
     function_parameters: dict[str, str]
 
+    def to_string(self) -> str:
+        function_call_string = "<invoke>\n"
+        function_call_string += f"<tool_name>{self.function_name}</tool_name>\n"
+        function_call_string += "<parameters>\n"
+        for param_name, param_value in self.function_parameters.items():
+            function_call_string += f"<{param_name}>\n{param_value}\n</{param_name}>\n"
+        function_call_string += "</parameters>\n"
+        function_call_string += "</invoke>"
+        return function_call_string
+
     @staticmethod
-    def mock_function_calls_from_string(function_calls_string: str) -> list[MockFunctionCall]:
+    def mock_function_calls_from_string(function_calls_string: str) -> list[AnthropicFunctionCall]:
         function_calls = []
 
         # Regular expression patterns
         function_name_pattern = r'<tool_name>(.*?)</tool_name>'
         parameters_pattern = r'<parameters>(.*?)</parameters>'
         parameter_pattern = r'<(.*?)>(.*?)<\/\1>'
         
@@ -67,18 +77,25 @@
             function_parameters = {}
             for param in parameter_matches:
                 parameter_name = param[0]
                 parameter_value = param[1]
                 function_parameters[parameter_name] = parameter_value.strip()
 
             if function_name and function_parameters != {}:
-                function_calls.append(MockFunctionCall(function_name, function_parameters))
+                function_calls.append(AnthropicFunctionCall(function_name, function_parameters))
 
         return function_calls
 
+def mock_function_calls_to_string(function_calls: list[AnthropicFunctionCall]) -> str:
+    function_calls_string = "<function_call>\n"
+    for function_call in function_calls:
+        function_calls_string += function_call.to_string() + "\n"
+    function_calls_string += "</function_call>"
+    return function_calls_string
+
 if __name__ == "__main__":    
     test_str = """<function_call>
 <invoke>
 <tool_name>submit_report_and_plan</tool_name>
 <parameters>
 <report>
 The main API implementation for the Sweep application is in the `sweepai/api.py` file. This file handles various GitHub events, such as pull requests, issues, and comments, and triggers corresponding actions.
@@ -102,10 +119,12 @@
 5. Thoroughly test the changes to ensure that all relevant cases are covered, including edge cases and error handling. This may involve writing additional unit tests or integration tests to validate the functionality.
 6. Once the changes have been implemented and tested, submit the modified `sweepai/api.py` file for review and deployment.
 </plan>
 </parameters>
 </invoke>
 </function_call>"""
 
-    function_calls = MockFunctionCall.mock_function_calls_from_string(test_str)
+    function_calls = AnthropicFunctionCall.mock_function_calls_from_string(test_str)
     for function_call in function_calls:
-        print(function_call)
+        print(function_call)
+        print(function_call.to_string())
+    print(mock_function_calls_to_string(function_calls))
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/diff.py` & `sweepai-2.0.1/sweepai/utils/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,44 @@
 import difflib
 import re
 
 from loguru import logger
 from sweepai.utils.search_and_replace import Match, find_best_match
 
 
-def generate_diff(old_code, new_code):
+def generate_diff(old_code, new_code, **kwargs):
     if old_code == new_code:
         return ""
     stripped_old_code = old_code.strip()
     stripped_new_code = new_code.strip()
 
+    default_kwargs = {"n": 5}
+    default_kwargs.update(kwargs)
+
     diff = difflib.unified_diff(
         stripped_old_code.splitlines(keepends=True),
         stripped_new_code.splitlines(keepends=True),
+        **kwargs
+    )
+
+    diff_text = "".join(diff)
+
+    return diff_text
+
+
+def generate_ndiff(old_code, new_code, **kwargs):
+    if old_code == new_code:
+        return ""
+    stripped_old_code = old_code.strip()
+    stripped_new_code = new_code.strip()
+
+    diff = difflib.ndiff(
+        stripped_old_code.splitlines(keepends=True),
+        stripped_new_code.splitlines(keepends=True),
+        **kwargs
     )
 
     diff_text = "".join(diff)
 
     return diff_text
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/diff_test.py` & `sweepai-2.0.1/sweepai/utils/diff_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/docker_utils.py` & `sweepai-2.0.1/sweepai/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/event_logger.py` & `sweepai-2.0.1/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/fuzzy_diff.py` & `sweepai-2.0.1/sweepai/utils/fuzzy_diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,14 +112,24 @@
     if old_string == new_string:
         return ""
     old_lines = old_string.splitlines()
     new_lines = new_string.splitlines()
     diff_lines = patience_fuzzy_diff_lines(old_lines, new_lines)
     return "\n".join(diff_lines)
 
+def patience_fuzzy_additions(
+    old_string: str,
+    new_string: str
+):
+    if old_string == new_string:
+        return ""
+    old_lines = old_string.splitlines()
+    new_lines = new_string.splitlines()
+    diff_lines = patience_fuzzy_diff_lines(old_lines, new_lines)
+    return "\n".join(line[2:] for line in diff_lines if line.startswith("+"))
 
 old_lint_results = """> pylint sweepai/handlers/on_ticket.py
 
 ************* Module on_ticket
 sweepai/handlers/on_ticket.py:167:52: W0613: Unused argument 'reaction_content' (unused-argument)
 sweepai/handlers/on_ticket.py:221:24: W3101: Missing timeout argument for method 'requests.get' can cause your program to hang indefinitely (missing-timeout)
 sweepai/handlers/on_ticket.py:251:24: W3101: Missing timeout argument for method 'requests.get' can cause your program to hang indefinitely (missing-timeout)
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/fuzzy_diff_test.py` & `sweepai-2.0.1/sweepai/utils/fuzzy_diff_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/github_utils.py` & `sweepai-2.0.1/sweepai/utils/github_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         "Authorization": "Bearer " + jwt,
         "X-GitHub-Api-Version": "2022-11-28",
     }
     response = requests.get("https://api.github.com/app", headers=headers)
     return response.json()
 
 
-def get_github_client(installation_id: int):
+def get_github_client(installation_id: int) -> tuple[str, Github]:
     if not installation_id:
         return os.environ["GITHUB_PAT"], Github(os.environ["GITHUB_PAT"])
     token: str = get_token(installation_id)
     return token, Github(token)
 
 # fetch installation object
 def get_installation(username: str): 
@@ -151,15 +151,15 @@
 
 # commits multiple files in a single commit, returns the commit object
 def commit_multi_file_changes(repo: Repository, file_changes: dict[str, str], commit_message: str, branch: str):
     blobs_to_commit = []
     # convert to blob
     for path, content in file_changes.items():
         blob = repo.create_git_blob(content, "utf-8")
-        blobs_to_commit.append(InputGitTreeElement(path=path, mode="100644", type="blob", sha=blob.sha))
+        blobs_to_commit.append(InputGitTreeElement(path=os.path.normpath(path), mode="100644", type="blob", sha=blob.sha))
     latest_commit = repo.get_branch(branch).commit
     base_tree = latest_commit.commit.tree
     # create new git tree
     new_tree = repo.create_git_tree(blobs_to_commit, base_tree=base_tree)
     # commit the changes
     parent = repo.get_git_commit(latest_commit.sha)
     commit = repo.create_git_commit(
@@ -618,15 +618,16 @@
     # Replace any non-alphanumeric characters with hyphens
     name = re.sub(r"[^\w-]", "--", name)
     # Ensure the name is between 3 and 63 characters and starts/ends with alphanumeric
     name = re.sub(r"^(-*\w{0,61}\w)-*$", r"\1", name[:63].ljust(3, "x"))
     return name
 
 # set whether or not a pr is a draft, there is no way to do this using pygithub
-def convert_pr_draft_field(pr: PullRequest, is_draft: bool = False):
+def convert_pr_draft_field(pr: PullRequest, is_draft: bool = False, installation_id: int = 0) -> bool:
+    token = get_token(installation_id)
     pr_id = pr.raw_data['node_id']
     # GraphQL mutation for marking a PR as ready for review
     mutation = """
     mutation MarkPRReady {
     markPullRequestReadyForReview(input: {pullRequestId: {pull_request_id}}) {
     pullRequest {
     id
@@ -637,16 +638,16 @@
 
     # GraphQL API URL
     url = 'https://api.github.com/graphql'
 
     # Headers
     headers={
         "Accept": "application/vnd.github+json",
-        "X-Github-Api-Version": "2022-11-28",
-        "Authorization": "Bearer " + os.environ["GITHUB_PAT"],
+        "Authorization": f"Bearer {token}",
+        "X-GitHub-Api-Version": "2022-11-28",
     }
 
     # Prepare the JSON payload
     json_data = {
         'query': mutation,
     }
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/github_utils_test.py` & `sweepai-2.0.1/sweepai/utils/github_utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/html_extractor.py` & `sweepai-2.0.1/sweepai/utils/html_extractor.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/multi_query.py` & `sweepai-2.0.1/sweepai/utils/multi_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 Summarize the key points of the issue concisely, but also list out any unfamiliar terms, acronyms, or entities mentioned that may require additional context to fully understand the problem space and identify all relevant code areas.
 
 2. Solution
 
 Describe thoroughly in extreme detail what the ideal code fix would look like:
 - Dive deep into the low-level implementation details of how you would change each file. Explain the logic, algorithms, data structures, etc. 
 - Explicitly call out any helper functions, utility modules, libraries or APIs you would leverage.
-- Carefully consider ALL parts of the codebase that could be relevant, including:
+- Carefully consider ALL parts of the codebase that could be relevant, including (in decreasing relevance):
+  - Database schemas, models
   - Type definitions, interfaces, enums, constants
-  - Shared utility code for common operations
-  - Database schemas, models, mutators and query logic 
+  - Shared utility code for common operations like date formatting, string manipulation, etc.
+  - Database mutators and query logic 
   - User-facing messages, error messages, localization, i18n
   - Exception handling, error recovery, retries, fallbacks
   - API routes, request/response handling, serialization
   - UI components, client-side logic, event handlers
   - Backend services, data processing, business logic
   - Logging, monitoring, metrics, error tracking, observability, o11y
   - Auth flows, session management, encryption
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/openai_listwise_reranker.py` & `sweepai-2.0.1/sweepai/utils/openai_listwise_reranker.py`

 * *Files 27% similar despite different names*

```diff
@@ -478,22 +478,373 @@
 As a reminder, the user query is:  
 <user_query>
 {user_query}  
 </user_query>
 
 Provide the explanations and ranking below:"""
 
+graph_example_prompt = """<example>
+<user_query>
+The checkout process is broken. After entering payment info, the order doesn't get created and the user sees an error page.
+</user_query>
+<code_snippets>
+<snippet>
+<snippet_path>checkout_utils.js:5-30</snippet>
+<snippet_contents>
+function processCheckout(cartId, paymentInfo) {
+  return Cart.findById(cartId).populate('items.product')
+    .then(cart => {
+      if (!cart) {
+        throw new Error('Cart not found');
+      }
+      const order = new Order({
+        user: req.user._id,
+        items: cart.items,
+        total: cart.totalPrice,
+        paymentInfo,
+      });
+      return order.save();
+    })
+    .then(order => {
+      return Cart.findByIdAndDelete(cartId)
+        .then(() => order);
+    })
+    .then(order => {
+      return { message: 'Order placed successfully', orderId: order._id };
+    })
+    .catch(err => {
+      console.error(err);
+      throw err;
+    });
+}
+module.exports = {
+  processCheckout
+};
+</snippet_contents>
+</snippet>
+<snippet>
+<snippet_path>payment_service.js:3-20</snippet>
+<snippet_contents>
+const stripe = require('stripe')(process.env.STRIPE_SECRET_KEY);
+function createPaymentCharge(amount, token) {
+  return stripe.charges.create({
+    amount,
+    currency: 'usd',
+    source: token,
+    description: 'Example charge'
+  })
+  .then(charge => {
+    return { message: 'Payment successful', charge };
+  })
+  .catch(err => {
+    console.error(err);
+    throw new Error('Payment failed');
+  });
+}
+module.exports = {
+  createPaymentCharge
+};
+</snippet_contents>
+</snippet>
+<snippet>
+<snippet_path>order_model.js:1-15</snippet>
+<snippet_contents>
+const mongoose = require('mongoose');
+const orderSchema = new mongoose.Schema({
+  user: { 
+    type: mongoose.Schema.Types.ObjectId,
+    ref: 'User',
+    required: true
+  },
+  items: [{
+    product: {
+      type: mongoose.Schema.Types.ObjectId,
+      ref: 'Product'
+    },
+    quantity: Number,
+    price: Number
+  }],
+  total: {
+    type: Number,
+    required: true
+  },
+  paymentInfo: {
+    type: Object,
+    required: true
+  },
+  status: {
+    type: String,
+    enum: ['pending', 'processing', 'shipped', 'delivered'],
+    default: 'pending'
+  }
+}, { timestamps: true });
+module.exports = mongoose.model('Order', orderSchema);
+</snippet_contents>
+</snippet>
+<snippet>
+<snippet_path>cart_model.js:1-20</snippet>
+<snippet_contents>
+const mongoose = require('mongoose');
+const cartSchema = new mongoose.Schema({
+  user: {
+    type: mongoose.Schema.Types.ObjectId,
+    ref: 'User',
+    required: true
+  },
+  items: [{
+    product: {
+      type: mongoose.Schema.Types.ObjectId,
+      ref: 'Product'
+    },
+    quantity: Number,
+    price: Number  
+  }]
+}, { timestamps: true });
+cartSchema.virtual('totalPrice').get(function() {
+  return this.items.reduce((total, item) => total + item.price * item.quantity, 0);
+});
+module.exports = mongoose.model('Cart', cartSchema);
+</snippet_contents>
+</snippet>
+<snippet>
+<snippet_path>db_connect.js:1-15</snippet>
+<snippet_contents>
+const mongoose = require('mongoose');
+function connectToDatabase(uri) {
+  return mongoose.connect(uri, {
+    useNewUrlParser: true,
+    useUnifiedTopology: true
+  })
+  .then(() => {
+    console.log('Connected to MongoDB');
+  })
+  .catch(err => {
+    console.error('MongoDB connection error:', err);
+    process.exit(1);
+  });
+}
+module.exports = connectToDatabase;
+</snippet_contents>
+</snippet>
+<snippet>
+<snippet_path>auth_middleware.js:5-20</snippet>
+<snippet_contents>
+function requireLogin(req, res, next) {
+  if (req.session && req.session.user) {
+    next();
+  } else {
+    res.status(401).json({ message: 'Authentication required' });
+  }
+}
+function requireAdmin(req, res, next) {
+  if (req.session && req.session.user && req.session.user.isAdmin) {
+    next();
+  } else {
+    res.status(403).json({ message: 'Admin access required' });
+  }
+}
+module.exports = {
+  requireLogin,
+  requireAdmin
+};
+</snippet_contents>
+</snippet>
+<snippet>
+<snippet_path>cart_utils.js:5-20</snippet>
+<snippet_contents>
+function addItemToCart(userId, productId, quantity) {
+  return Cart.findOne({ user: userId })
+    .then(cart => {
+      if (cart) {
+        const itemIndex = cart.items.findIndex(item => item.product == productId);
+        if (itemIndex > -1) {
+          cart.items[itemIndex].quantity += quantity;
+        } else {
+          cart.items.push({ product: productId, quantity });
+        }
+        return cart.save();
+      } else {
+        return Cart.create({
+          user: userId,
+          items: [{ product: productId, quantity }]
+        });
+      }
+    });
+}
+module.exports = {
+  addItemToCart
+};
+</snippet_contents>
+</snippet>
+<snippet>
+<snippet_path>order_utils.js:5-25</snippet>
+<snippet_contents>
+function getOrdersByUser(userId) {
+  return Order.find({ user: userId }).sort('-createdAt');
+}
+function getOrderById(orderId, userId) {
+  return Order.findOne({ _id: orderId, user: userId });
+}
+function updateOrderStatus(orderId, status) {
+  return Order.findByIdAndUpdate(orderId, { status }, { new: true });
+}
+module.exports = {
+  getOrdersByUser,
+  getOrderById,
+  updateOrderStatus
+};
+</snippet_contents>
+</snippet>
+<snippet>
+<snippet_path>user_model.js:1-10</snippet>
+<snippet_contents>
+const mongoose = require('mongoose');
+const userSchema = new mongoose.Schema({
+  email: {
+    type: String,
+    required: true,
+    unique: true
+  },
+  password: {
+    type: String,
+    required: true
+  },
+  name: String,
+  address: String,
+  phone: String,
+  isAdmin: {
+    type: Boolean,
+    default: false  
+  }
+}, { timestamps: true });
+module.exports = mongoose.model('User', userSchema);
+</snippet_contents>
+</snippet>
+<snippet>
+<snippet_path>product_model.js:1-12</snippet>
+<snippet_contents>
+const mongoose = require('mongoose');
+const productSchema = new mongoose.Schema({
+  name: {
+    type: String,
+    required: true
+  },
+  description: String,
+  price: {
+    type: Number,
+    required: true,
+    min: 0
+  },
+  category: {
+    type: String,
+    enum: ['electronics', 'clothing', 'home'],
+    required: true  
+  },
+  stock: {
+    type: Number,
+    default: 0,
+    min: 0
+  }
+});
+module.exports = mongoose.model('Product', productSchema);
+</snippet_contents>
+</snippet>
+</code_snippets>
+<explanations>
+checkout_utils.js:5-30
+This module contains the processCheckout function which handles the main checkout logic. It takes a cart ID and payment info, finds the associated cart, creates a new order from the cart data, saves the order, deletes the cart, and returns the order ID. This is the core checkout code and the most likely place for a bug causing the described issue.
+payment_service.js:3-20
+This module handles processing payments via the Stripe API. The createPaymentCharge function takes an amount and token, makes a request to Stripe to create a charge, and returns a success or error message. If payments are failing, this code would need to be checked and possibly debugged.  
+order_model.js:1-15
+This file defines the Mongoose schema and model for orders. It includes the order's user, items, total, payment info, and status. The model definition itself is unlikely to cause bugs, but it's important to understand the order data structure when debugging checkout and payment issues.
+cart_model.js:1-20
+This file defines the Mongoose schema and model for shopping carts. A cart contains the user, product items, quantities, and prices. It also defines a virtual property to calculate the cart's total price. The cart model is a key part of the checkout process, so it's useful to review when investigating checkout bugs.
+db_connect.js:1-15
+This module exports a function to connect to the MongoDB database using Mongoose. It's an essential part of the app's infrastructure, but unlikely to be related to a checkout bug unless there are issues connecting to the database.
+auth_middleware.js:5-20
+This module contains Express middleware functions to require authentication and admin access for certain routes. It checks for the existence of a user object in the session. While authentication and authorization are important for the app overall, this middleware is not directly involved in the checkout process.
+cart_utils.js:5-20
+This module exports a function to add an item to a user's cart. It finds the cart by user ID, updates the quantity if the item already exists or adds a new item. The addItemToCart function is used before starting the checkout, so while it's somewhat related, it's not a likely cause of the described checkout issue.
+order_utils.js:5-25
+This module provides utility functions for fetching a user's orders, getting an order by ID, and updating an order's status. These are used for displaying order history and managing orders, which happen after checkout is already completed. So while they interact with orders, they are not likely to be the source of an error during the checkout process.
+user_model.js:1-10
+This defines the Mongoose schema and model for user accounts. It includes fields for email, password, name, address, phone number, and admin status. The user model is used for authentication and referenced by carts and orders. But the checkout process doesn't directly interact with or modify user documents.
+product_model.js:1-12
+This defines the Mongoose schema and model for products, including name, description, price, category, and stock quantity. The product model is referenced by cart and order items, but the product data is not directly used or modified during the checkout flow. It's unlikely to be related to the checkout error.
+</explanations>
+<ranking>
+checkout_utils.js:5-30
+payment_service.js:3-20
+order_model.js:1-15
+cart_model.js:1-20
+db_connect.js:1-15
+order_utils.js:5-25
+cart_utils.js:5-20
+auth_middleware.js:5-20
+user_model.js:1-10
+product_model.js:1-12
+</ranking>
+</example>"""
+
+graph_reranking_prompt = f"""You are a powerful code search engine. You must order the list of code snippets from the most relevant to the least relevant to the user's query. You must order ALL TEN snippets.
+First, for each code snippet, provide a brief explanation of what the code does and how it relates to the user's query.
+Then, rank the snippets based on probability of it being used in the final solution. The most relevant files are the ones most likely to be needed to resolve the user's issue. The next most relevant snippets are dependencies - code that is crucial to read and understand while using the other files to correctly resolve the user's issue.
+Note: For each code snippet, provide an explanationof what the code does and how it fits into the overall system, even if it's not directly relevant to the user's query. The ranking should be based on probability of being used in the solution, but all snippets should be explained.
+The response format is:
+<explanations>
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+file_path:start_line-end_line
+Explanation of what the code does, regardless of its relevance to the user's query. Provide context on how it fits into the overall system.
+</explanations>
+<ranking>
+most_likely_to_be_used_in_solution
+second_most_likely_to_be_used
+third_most_likely_to_be_used
+fourth_most_likely_to_be_used
+fifth_most_likely_to_be_used
+sixth_most_likely_to_be_used
+seventh_most_likely_to_be_used
+eighth_most_likely_to_be_used
+ninth_most_likely_to_be_used
+least_likely_to_be_used
+</ranking>
+Here is an example:
+{example_prompt}
+This example is for reference. Please provide explanations and rankings for the code snippets based on the user's query."""
+
+prompt_mapping = {
+  "default": reranking_prompt,
+  "graph": graph_reranking_prompt,
+}
 
 class RerankSnippetsBot(ChatGPT):
     def rerank_list_for_query(
         self,
         user_query,
         code_snippets,
+        prompt_type="default",
     ):
-        self.messages = [Message(role="system", content=reranking_prompt)]
+        self.messages = [Message(role="system", content=prompt_mapping[prompt_type])]
         # if the regex match fails return the original list
         # gpt doesn't add all snippets, we move all of the dropped snippets to the end in the original order
         # if we add duplicate snippets, we remove the duplicates
         ranking_pattern = r"<ranking>\n(.*?)\n</ranking>"
         formatted_code_snippets = self.format_code_snippets(code_snippets)
         try:
             ranking_response = self.chat_anthropic(
@@ -526,47 +877,48 @@
             snippet_ranking.extend(remaining_snippets)
         # sort the snippets using the snippet_ranking
         ranked_snippets = sorted(code_snippets, key=lambda snippet: snippet_ranking.index(snippet.denotation))
         return ranked_snippets
     
     def format_code_snippets(self, code_snippets: list[Snippet]):
         result_str = ""
-        for snippet in code_snippets:
+        for idx, snippet in enumerate(code_snippets):
             snippet_str = \
-f"""
-<snippet>
-<snippet_path>{snippet.denotation}</snippet>
-<snippet_contents>
+f'''
+<snippet index="{idx + 1}">
+<snippet_path>{snippet.denotation}</snippet_path>
+<source>
 {snippet.get_snippet(False, False)}
-</snippet_contents>
+</source>
 </snippet>
-"""
+'''
             result_str += snippet_str + "\n"
         result_removed_trailing_newlines = result_str.rstrip("\n")
         return result_removed_trailing_newlines
 
 @file_cache()
 def listwise_rerank_snippets(
     user_query,
     code_snippets,
+    prompt_type="default",
 ):
     # iterate from the bottom of the list to the top, sorting each n items then resorting with next n // 2 items
     number_to_rerank_at_once = 10
     stride = number_to_rerank_at_once // 2
     final_ordering = []
     prev_chunk = []
     for idx in range(len(code_snippets) - stride, 0, -stride):
         # if there is no prev_chunk, rerank the bottom n items
         if not prev_chunk:
-            reranked_chunk = RerankSnippetsBot().rerank_list_for_query(user_query, code_snippets[idx - stride:idx + stride])
+            reranked_chunk = RerankSnippetsBot().rerank_list_for_query(user_query, code_snippets[idx - stride:idx + stride], prompt_type=prompt_type)
         # if there's a prev_chunk, rerank this chunk with the prev_chunk
         else:
             # chunk_to_rerank should be 5 new items and the top 5 items of the prev_chunk
             chunk_to_rerank = code_snippets[idx - stride:idx] + prev_chunk[:stride]
-            reranked_chunk = RerankSnippetsBot().rerank_list_for_query(user_query, chunk_to_rerank)
+            reranked_chunk = RerankSnippetsBot().rerank_list_for_query(user_query, chunk_to_rerank, prompt_type=prompt_type)
         # last iteration, add all items
         if idx - stride <= 0:
             final_ordering = reranked_chunk + final_ordering
         else:
             # add the last n // 2 items to the final_ordering
             final_ordering = reranked_chunk[-stride:] + final_ordering
         prev_chunk = reranked_chunk
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/openai_proxy.py` & `sweepai-2.0.1/sweepai/utils/openai_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     def call_openai(
         self,
         model: str,
         messages: list[Message],
         tools: list[str] = [],
         max_tokens: int = 4096,
         temperature: float = 0.0,
+        stop_sequences: list[str] = [],
         seed: int = 0,
     ):
         try:
             engine = self.determine_openai_engine(model)
             if OPENAI_API_TYPE is None or engine is None:
                 with Timer():
                     response = self.set_openai_default_api_parameters(
@@ -229,35 +230,37 @@
             f"Rate Limit or Timeout Error: {details['tries']} tries. Waiting {details['wait']:.2f} seconds."
         ),
         base=10,
         factor=2,
         max_value=40,
     )
     def set_openai_default_api_parameters(
-        self, model, messages, max_tokens, temperature, tools=[]
+        self, model, messages, max_tokens, temperature, tools=[], stop_sequences=[]
     ):
         client = OpenAI(api_key=OPENAI_API_KEY)
         if len(tools) == 0:
             response = client.chat.completions.create(
                 model=model,
                 messages=messages,
                 max_tokens=max_tokens,
                 temperature=temperature,
                 timeout=OPENAI_TIMEOUT,
                 seed=SEED,
+                stop=stop_sequences,
             )
         else:
             response = client.chat.completions.create(
                 model=model,
                 messages=messages,
                 tools=tools,
                 max_tokens=max_tokens,
                 temperature=temperature,
                 timeout=OPENAI_TIMEOUT,
                 seed=SEED,
+                stop=stop_sequences,
             )
         return response
 
 
 def get_client():
     OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY")
     OPENAI_API_TYPE = os.environ.get("OPENAI_API_TYPE", "openai")
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/openai_proxy_test.py` & `sweepai-2.0.1/sweepai/utils/openai_proxy_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/patch_utils.py` & `sweepai-2.0.1/sweepai/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/progress.py` & `sweepai-2.0.1/sweepai/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/prompt_constructor.py` & `sweepai-2.0.1/sweepai/utils/prompt_constructor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from pydantic import BaseModel
 
 from sweepai.core.prompts import (
     diff_section_prompt,
     final_review_prompt,
     human_message_prompt,
     human_message_prompt_comment,
-    human_message_review_prompt,
 )
 
 
 class HumanMessagePrompt(BaseModel):
     repo_name: str
-    issue_url: str | None
-    username: str
     title: str
     summary: str
     snippets: list
     tree: str
     repo_description: str = ""
     snippet_text: str = ""
     commit_history: list = []
@@ -129,68 +126,35 @@
         issue_description = (
             f"\nIssue Description: {self.summary}" if self.summary else ""
         )
         return f"""# Repo & Issue Metadata
 Repo: {self.repo_name}: {self.repo_description}
 Issue Title: {self.title}
 {issue_description}"""
+    
+    def get_issue_request(self):
+        self.summary = (
+            self.summary if not self.summary.strip().endswith("_No response_") else ""
+        )
+        issue_description = (
+            f"\nIssue Description: {self.summary}" if self.summary else ""
+        )
+        return f"""Issue Title: {self.title}
+{issue_description}"""
 
 
 def render_snippets(snippets):
     res = ""
     for snippet in snippets:
         snippet_text = (
             f"<snippet source={snippet.file_path}>\n{snippet.content}\n</snippet>\n"
         )
         res += snippet_text
     return res
 
-
-class HumanMessagePromptReview(HumanMessagePrompt):
-    pr_title: str
-    pr_message: str = ""
-    diffs: list
-    plan: str
-
-    def format_diffs(self):
-        formatted_diffs = []
-        for file_name, file_patch in self.diffs:
-            if not file_name and not file_patch:
-                continue
-            format_diff = diff_section_prompt.format(
-                diff_file_path=file_name, diffs=file_patch
-            )
-            formatted_diffs.append(format_diff)
-        return "\n".join(formatted_diffs)
-
-    def construct_prompt(self):
-        human_messages = [
-            {
-                "role": msg["role"],
-                "content": msg["content"].format(
-                    repo_name=self.repo_name,
-                    repo_description=self.repo_description,
-                    tree=self.tree,
-                    title=self.title,
-                    description=self.summary,
-                    relevant_snippets=self.render_snippets(),
-                    relevant_directories=self.get_relevant_directories(),
-                    relevant_commit_history=self.get_commit_history(),
-                    diffs=self.format_diffs(),
-                    pr_title=self.pr_title,
-                    pr_message=self.pr_message,
-                    plan=self.plan,
-                ),
-            }
-            for msg in human_message_review_prompt
-        ]
-
-        return human_messages
-
-
 class HumanMessageCommentPrompt(HumanMessagePrompt):
     comment: str
     diffs: list
     relevant_docs: str | None
     pr_file_path: str | None
     pr_chunk: str | None
     original_line: str | None
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/regex_utils.py` & `sweepai-2.0.1/sweepai/utils/regex_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/safe_pqueue.py` & `sweepai-2.0.1/sweepai/utils/safe_pqueue.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/scorer.py` & `sweepai-2.0.1/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/scorer_test.py` & `sweepai-2.0.1/sweepai/utils/scorer_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/search_and_replace.py` & `sweepai-2.0.1/sweepai/utils/search_and_replace.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/search_and_replace_test.py` & `sweepai-2.0.1/sweepai/utils/search_and_replace_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/str_utils.py` & `sweepai-2.0.1/sweepai/utils/str_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -128,7 +128,19 @@
     branch_name = s.strip().lower().replace(" ", "_")
     branch_name = re.sub(r"[^a-z0-9_]", "", branch_name)
     return branch_name[:max_length]
 
 
 def get_hash():
     return hashlib.sha256(str(time.time()).encode()).hexdigest()[:10]
+
+# used for getting all indices of a substring match
+def get_all_indices_of_substring(content: str, substring: str):
+    start = 0
+    indices = []
+    while True:
+        index = content.find(substring, start)
+        if index == -1:  # No more occurrences found
+            break
+        indices.append(index)
+        start = index + 1  # Move past the last found occurrence
+    return indices
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/ticket_utils.py` & `sweepai-2.0.1/sweepai/utils/ticket_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from collections import defaultdict
 import traceback
 from time import time
 
+import cohere
 from loguru import logger
 from tqdm import tqdm
 
 from sweepai.config.client import SweepConfig, get_blocked_dirs
-from sweepai.core.context_pruning import RepoContextManager, get_relevant_context
+from sweepai.config.server import COHERE_API_KEY
+from sweepai.core.context_pruning import RepoContextManager, get_relevant_context, integrate_graph_retrieval
+from sweepai.core.entities import Snippet
 from sweepai.core.lexical_search import (
     compute_vector_search_scores,
     prepare_lexical_search_index,
     search_index,
 )
 from sweepai.logn.cache import file_cache
 from sweepai.utils.chat_logger import discord_log_error
@@ -24,44 +27,78 @@
 Input queries are in natural language so both lexical search 
 and vector search have a heavy bias towards natural language
 files such as tests, docs and localization files. Therefore,
 we add adjustment scores to compensate for this bias.
 """
 
 prefix_adjustment = {
-    "doc": -0.5,
-    "example": -0.75,
+    ".": 0.5,
+    "doc": 0.3,
+    "example": 0.7,
 }
 
 suffix_adjustment = {
-    ".txt": -0.5,
-    ".rst": -0.5,
-    ".md": -0.5,
-    ".html": -0.5,
-    ".po": -1,
-    ".json": -0.5,
-    ".toml": -0.5,
-    ".yaml": -0.5,
-    ".yml": -0.5,
-    ".spec.ts": -1,
-    ".spec.js": -1,
-    ".generated.ts": -1.5,
-    ".generated.graphql": -1.5,
-    ".generated.js": -1.5,
-    "ChangeLog": -1.5,
+    ".cfg": 0.8,
+    ".ini": 0.8,
+    ".txt": 0.8,
+    ".rst": 0.8,
+    ".md": 0.8,
+    ".html": 0.8,
+    ".po": 0.5,
+    ".json": 0.8,
+    ".toml": 0.8,
+    ".yaml": 0.8,
+    ".yml": 0.8,
+    ".1": 0.5, # man pages
+    ".spec.ts": 0.6,
+    ".spec.js": 0.6,
+    ".generated.ts": 0.5,
+    ".generated.graphql": 0.5,
+    ".generated.js": 0.5,
+    "ChangeLog": 0.5,
 }
 
 substring_adjustment = {
-    "tests/": -1,
-    "test_": -1,
-    "_test": -1,
-    "migrations/": -1.5,
+    "tests/": 0.5,
+    "test_": 0.5,
+    "_test": 0.5,
+    "egg-info": 0.5,
+    "LICENSE": 0.5,
 }
 
-NUM_SNIPPETS_TO_RERANK = 50
+def apply_adjustment_score(
+    snippet: str,
+    old_score: float,
+):
+    snippet_score = old_score
+    file_path, *_ = snippet.split(":")
+    file_path = file_path.lower()
+    for prefix, adjustment in prefix_adjustment.items():
+        if file_path.startswith(prefix):
+            snippet_score *= adjustment
+            break
+    for suffix, adjustment in suffix_adjustment.items():
+        if file_path.endswith(suffix):
+            snippet_score *= adjustment
+            break
+    for substring, adjustment in substring_adjustment.items():
+        if substring in file_path:
+            snippet_score *= adjustment
+            break
+    # Penalize numbers as they are usually examples of:
+    # 1. Test files (e.g. test_utils_3*.py)
+    # 2. Generated files (from builds or snapshot tests)
+    # 3. Versioned files (e.g. v1.2.3)
+    # 4. Migration files (e.g. 2022_01_01_*.sql)
+    base_file_name = file_path.split("/")[-1]
+    num_numbers = sum(c.isdigit() for c in base_file_name)
+    snippet_score *= (1 - 1 / len(base_file_name)) ** num_numbers
+    return snippet_score
+
+NUM_SNIPPETS_TO_RERANK = 100
 
 @file_cache()
 def multi_get_top_k_snippets(
     cloned_repo: ClonedRepo,
     queries: list[str],
     ticket_progress: TicketProgress | None = None,
     k: int = 15,
@@ -99,26 +136,17 @@
                 # roughly fine tuned vector score weight based on average score from search_eval.py on 10 test cases Feb. 13, 2024
                 snippet_score = content_to_lexical_score_list[i][snippet.denotation] + (
                     vector_score * 3.5
                 )
                 content_to_lexical_score_list[i][snippet.denotation] = snippet_score
             else:
                 content_to_lexical_score_list[i][snippet.denotation] = snippet_score * vector_score
-            for prefix, adjustment in prefix_adjustment.items():
-                if snippet.file_path.startswith(prefix):
-                    content_to_lexical_score_list[i][snippet.denotation] += adjustment
-                    break
-            for suffix, adjustment in suffix_adjustment.items():
-                if snippet.file_path.endswith(suffix):
-                    content_to_lexical_score_list[i][snippet.denotation] += adjustment
-                    break
-            for substring, adjustment in substring_adjustment.items():
-                if substring in snippet.file_path:
-                    content_to_lexical_score_list[i][snippet.denotation] += adjustment
-                    break
+            content_to_lexical_score_list[i][snippet.denotation] = apply_adjustment_score(
+                snippet.denotation, content_to_lexical_score_list[i][snippet.denotation]
+            )
     
     ranked_snippets_list = [
         sorted(
             snippets,
             key=lambda snippet: content_to_lexical_score[snippet.denotation],
             reverse=True,
         )[:k] for content_to_lexical_score in content_to_lexical_score_list
@@ -133,45 +161,116 @@
     k: int = 15,
 ):
     ranked_snippets_list, snippets, content_to_lexical_score_list = multi_get_top_k_snippets(
         cloned_repo, [query], ticket_progress, k
     )
     return ranked_snippets_list[0], snippets, content_to_lexical_score_list[0]
 
+@file_cache()
+def cohere_rerank_call(
+    query: str,
+    documents: list[str],
+    model='rerank-english-v3.0',
+    **kwargs,
+):
+    # Cohere API call with caching
+    co = cohere.Client(COHERE_API_KEY)
+    return co.rerank(
+        model=model,
+        query=query,
+        documents=documents,
+        **kwargs
+    )
+
+def get_pointwise_reranked_snippet_scores(
+    query: str,
+    snippets: list[Snippet],
+    snippet_scores: dict[str, float],
+):
+    """
+    Ranks 1-5 snippets are frozen. They're just passed into Cohere since it helps with reranking. We multiply the scores by 1_000 to make them more significant.
+    Ranks 6-100 are reranked using Cohere. Then we divide the scores by 1_000 to make them comparable to the original scores.
+    """
+
+    if not COHERE_API_KEY:
+        return snippet_scores
+
+    sorted_snippets = sorted(
+        snippets,
+        key=lambda snippet: snippet_scores[snippet.denotation],
+        reverse=True,
+    )
+
+    NUM_SNIPPETS_TO_KEEP = 5
+    NUM_SNIPPETS_TO_RERANK = 100
+
+    response = cohere_rerank_call(
+        model='rerank-english-v3.0',
+        query=query,
+        documents=[snippet.xml for snippet in sorted_snippets[:NUM_SNIPPETS_TO_RERANK]],
+        max_chunks_per_doc=900 // NUM_SNIPPETS_TO_RERANK,
+    )
+
+    new_snippet_scores = {k: v / 1000 for k, v in snippet_scores.items()}
+
+    for document in response.results:
+        new_snippet_scores[sorted_snippets[document.index].denotation] = apply_adjustment_score(
+            sorted_snippets[document.index].denotation,
+            document.relevance_score,
+        )
+
+    for snippet in sorted_snippets[:NUM_SNIPPETS_TO_KEEP]:
+        new_snippet_scores[snippet.denotation] = snippet_scores[snippet.denotation] * 1_000
+    
+    return new_snippet_scores
 
 def multi_prep_snippets(
     cloned_repo: ClonedRepo,
     queries: list[str],
     ticket_progress: TicketProgress | None = None,
     k: int = 15,
-    skip_reranking: bool = False,
-):
+    skip_reranking: bool = False, # This is only for pointwise reranking
+    skip_pointwise_reranking: bool = False,
+) -> RepoContextManager:
     """
     Assume 0th index is the main query.
     """
     rank_fusion_offset = 0
     if len(queries) > 1:
         logger.info("Using multi query...")
         ranked_snippets_list, snippets, content_to_lexical_score_list = multi_get_top_k_snippets(
             cloned_repo, queries, ticket_progress, k * 3 # k * 3 to have enough snippets to rerank
         )
         # Use RRF to rerank snippets
         content_to_lexical_score = defaultdict(float)
         for i, ordered_snippets in enumerate(ranked_snippets_list):
             for j, snippet in enumerate(ordered_snippets):
-                content_to_lexical_score[snippet.denotation] += content_to_lexical_score_list[i][snippet.denotation] * (1 / (rank_fusion_offset + j + 1))
+                content_to_lexical_score[snippet.denotation] += content_to_lexical_score_list[i][snippet.denotation] * (1 / 2 ** (rank_fusion_offset + j))
+        if not skip_pointwise_reranking:
+            content_to_lexical_score = get_pointwise_reranked_snippet_scores(
+                queries[0], snippets, content_to_lexical_score
+            )
         ranked_snippets = sorted(
             snippets,
             key=lambda snippet: content_to_lexical_score[snippet.denotation],
             reverse=True,
         )[:k]
     else:
         ranked_snippets, snippets, content_to_lexical_score = get_top_k_snippets(
             cloned_repo, queries[0], ticket_progress, k
         )
+        if not skip_pointwise_reranking:
+            content_to_lexical_score = get_pointwise_reranked_snippet_scores(
+                queries[0], snippets, content_to_lexical_score
+            )
+        ranked_snippets = sorted(
+            snippets,
+            key=lambda snippet: content_to_lexical_score[snippet.denotation],
+            reverse=True,
+        )[:k]
     if ticket_progress:
         ticket_progress.search_progress.retrieved_snippets = ranked_snippets
         ticket_progress.save()
     # you can use snippet.denotation and snippet.get_snippet()
     if not skip_reranking:
         ranked_snippets[:NUM_SNIPPETS_TO_RERANK] = listwise_rerank_snippets(queries[0], ranked_snippets[:NUM_SNIPPETS_TO_RERANK])
     snippet_paths = [snippet.file_path for snippet in ranked_snippets]
@@ -199,15 +298,15 @@
 def prep_snippets(
     cloned_repo: ClonedRepo,
     query: str,
     ticket_progress: TicketProgress | None = None,
     k: int = 15,
     skip_reranking: bool = False,
     use_multi_query: bool = True,
-):
+) -> RepoContextManager:
     if use_multi_query:
         queries = [query, *generate_multi_queries(query)]
     else:
         queries = [query]
     return multi_prep_snippets(
         cloned_repo, queries, ticket_progress, k, skip_reranking
     )
@@ -231,22 +330,25 @@
     try:
         search_query = (title + summary + replies_text).strip("\n")
         replies_text = f"\n{replies_text}" if replies_text else ""
         formatted_query = (f"{title.strip()}\n{summary.strip()}" + replies_text).strip(
             "\n"
         )
         repo_context_manager = prep_snippets(cloned_repo, search_query, ticket_progress)
+
+        repo_context_manager, import_graph = integrate_graph_retrieval(search_query, repo_context_manager)
+
         ticket_progress.search_progress.repo_tree = str(repo_context_manager.dir_obj)
         ticket_progress.save()
-
         repo_context_manager = get_relevant_context(
             formatted_query,
             repo_context_manager,
             ticket_progress,
             chat_logger=chat_logger,
+            import_graph=import_graph,
         )
         snippets = repo_context_manager.current_top_snippets
         ticket_progress.search_progress.repo_tree = str(repo_context_manager.dir_obj)
         ticket_progress.search_progress.final_snippets = snippets
         ticket_progress.save()
 
         tree = str(repo_context_manager.dir_obj)
@@ -269,15 +371,15 @@
             properties={
                 **metadata,
                 "error": str(e),
                 "duration": time() - on_ticket_start_time,
             },
         )
         raise e
-    return snippets, tree, dir_obj
+    return snippets, tree, dir_obj, repo_context_manager
 
 
 SLOW_MODE = False
 SLOW_MODE = True
 
 
 def log_error(
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/timer.py` & `sweepai-2.0.1/sweepai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/tree_utils.py` & `sweepai-2.0.1/sweepai/utils/tree_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/user_settings.py` & `sweepai-2.0.1/sweepai/utils/user_settings.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/utils.py` & `sweepai-2.0.1/sweepai/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 import ast
 from io import StringIO
 import os
 import re
 import subprocess
 from tempfile import TemporaryDirectory
+import tempfile
 import traceback
 from dataclasses import dataclass
 from typing import Optional
 import uuid
 
 from pylint.lint import Run
 from pylint.reporters.text import TextReporter
 import tiktoken
 from loguru import logger
 from tree_sitter import Node
 from tree_sitter_languages import get_parser
 
 from sweepai.core.entities import Snippet
-from sweepai.utils.fuzzy_diff import patience_fuzzy_diff
+from sweepai.utils.fuzzy_diff import patience_fuzzy_additions
 
 
 def non_whitespace_len(s: str) -> int:  # new len function
     return len(re.sub("\s", "", s))
 
 
 def get_line_number(index: int, source_code: str) -> int:
@@ -217,39 +218,78 @@
             return self.parse_error_message
         if other.parse_error_message:
             return other.parse_error_message
         if len(self.pylint.splitlines()) > len(other.pylint.splitlines()):
             # return f"The code has the following pylint errors:\n\n{self.pylint}"
             if not other.pylint:
                 return f"The code has the following pylint errors:\n\n{self.pylint}"
-            return f"The following new pylint errors have appeared. Here is the diff:\n\n{patience_fuzzy_diff(other.pylint, self.pylint)}"
+            return f"The following new pylint errors have appeared:\n\n{patience_fuzzy_additions(other.pylint, self.pylint)}"
         if len(self.eslint.splitlines()) > len(other.eslint.splitlines()):
             if not other.eslint:
                 return f"The code has the following eslint errors:\n\n{self.eslint}"
-            return f"The following new eslint errors have appeared. Here is the diff:\n\n{patience_fuzzy_diff(other.eslint, self.eslint)}"
+            return f"The following new eslint errors have appeared:\n\n{patience_fuzzy_additions(other.eslint, self.eslint)}"
         return ""
 
+def strip_ansi_codes(text: str) -> str:
+    # ANSI escape sequences (color codes) are often starting with ESC ([) followed by some numbers and ends with "m".
+    ansi_escape = re.compile(r'(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]')
+    return ansi_escape.sub('', text)
+
+def check_valid_typescript(file_path: str, code: str) -> tuple[bool, str]:
+    is_valid = True
+    message = ""
+    version_check = ["tsc", "--version"]
+    result = subprocess.run(
+        " ".join(version_check),
+        capture_output=True,
+        text=True,
+        shell=True,
+    )
+    # only run if tsc is available
+    if result.returncode == 0:
+        # Create a temporary file to hold the TypeScript code
+        with tempfile.NamedTemporaryFile(suffix=".ts", delete=False) as temp_file:
+            temp_file_path = temp_file.name
+            temp_file.write(code.encode('utf-8'))
+        
+        # Run `tsc` on the temporary file
+        try:
+            commands = ["tsc", "--pretty", "--noEmit", temp_file_path]
+            result = subprocess.run(" ".join(commands), shell=True, text=True, capture_output=True)
 
-def check_valid_typescript(code: str) -> tuple[bool, str]:
-    # with tempfile.TemporaryDirectory() as temp_dir:
-    #     file_hash = uuid.uuid4().hex[:10]
-    #     tmp_file = os.path.join(temp_dir, file_hash + "_" + "temp.ts")
-
-    #     with open(tmp_file, "w") as file:
-    #         file.write(code)
-
-    #     result = subprocess.run(
-    #         ["npx", "prettier", "--parser", "babel-ts", tmp_file],
-    #         capture_output=True,
-    #         timeout=5,
-    #     )
-
-    #     os.remove(tmp_file)
-    #     return result.returncode == 0, (result.stdout + result.stderr).decode("utf-8")
-    return True, ""
+            if result.returncode != 0:
+                message = strip_ansi_codes(result.stdout)
+                index = message.index(temp_file_path)
+                full_temp_file_path = message[:index + len(temp_file_path)]
+                message = message.replace(full_temp_file_path, file_path)
+
+                # import error is TS2307 and should come up after the syntax check
+                import_error = "error TS2307"
+                if import_error in message:
+                    num_of_errors = message.count(import_error)
+                    # see if this matches the total amount of errors:
+                    total_error_message = f"Found {num_of_errors} error"
+                    if total_error_message in message:
+                        # if we only have import errors, we consider it a successful check
+                        return True, ""
+                    else:
+                        # there are more errors than just import errors
+                        # now attempt to parse the message so that we remove import errors
+                        message_lines = message.split("\n")
+                        while num_of_errors > 0:
+                            for line in message_lines:
+                                if import_error in line:
+                                    message_lines = message_lines[5:]
+                                    num_of_errors -= 1
+                        message = "\n".join(message_lines)
+                return False, message
+        finally:
+            # Clean up: remove the temporary file
+            os.remove(temp_file_path)
+    return is_valid, message
 
 def check_syntax(file_path: str, code: str) -> tuple[bool, str]:
     ext = file_path.split(".")[-1]
     if ext in extension_to_language:
         language = extension_to_language[ext]
     else:
         return True, "Unsupported file extension, skipping syntax check."
@@ -259,14 +299,19 @@
     if language == "python":
         # First check for syntax errors
         try:
             ast.parse(code)
         except SyntaxError as e:
             error_message = f"Python syntax error: {e.msg} at line {e.lineno}"
             return False, error_message
+    
+    # we can't do this right now unfortunately as we don't have a way to mimic the production env for the code
+    # if ext in ["ts"]:
+    #     return check_valid_typescript(file_path, code)
+
 
     def find_deepest_error(node: Node) -> Optional[Node]:
         deepest_error = None
         if node.has_error:
             deepest_error = node
         for child in node.children:
             child_error = find_deepest_error(child)
@@ -275,15 +320,15 @@
         return deepest_error
 
     error_location = find_deepest_error(tree.root_node)
     if error_location:
         start = error_location.start_point
         end = error_location.end_point
         if start[0] == end[0]:
-            error_code_lines = code.split("\n")[start[0]]
+            error_code_lines = [code.split("\n")[start[0]]]
         else:
             error_code_lines = code.split("\n")[start[0]:end[0] + 1]
         error_code_lines[0] = error_code_lines[0][start[1]:]
         error_code_lines[-1] = error_code_lines[-1][:end[1]]
         error_span = "\n".join(error_code_lines)
         if start[0] == end[0]:
             error_message = f"Invalid syntax found at line {start[0]}, displayed below:\n{error_span}"
@@ -374,14 +419,15 @@
         except Exception as e:
             logger.exception(e)
     if ext == "ts":
         # see if eslint is installed
         npx_commands = ["npx", "eslint", "--version"]
         result = subprocess.run(
             " ".join(npx_commands),
+            timeout=5,
             capture_output=True,
             text=True,
             shell=True,
         )
         if result.returncode == 0:
             with TemporaryDirectory() as temp_dir:
                 new_file = os.path.join(temp_dir, "temp.ts")
@@ -506,16 +552,14 @@
                 content=code,
                 start=chunk.start,
                 end=chunk.end,
                 file_path=path,
             )
             snippets.append(new_snippet)
         return snippets
-    except SystemExit:
-        raise SystemExit
     except Exception:
         logger.error(traceback.format_exc())
         return []
 
 
 TIKTOKEN_CACHE_DIR = "/tmp/cache/tiktoken"
 
@@ -591,20 +635,23 @@
   return tokens[tokens.length - 1].toLowerCase().trim()
 }
 
 export function removeEmailAlias(email: string): string {
   if (!isPossiblyValidEmail(email)) {
     throw new PulseValidationException(`Email is invalid: ${email}`)
   
+  }
   const atIndex = email.lastIndexOf('@')
   const aliasIndex = email.lastIndexOf('+', atIndex)
 
   if (aliasIndex > 0) {
     return email.substring(0, aliasIndex) + email.substring(atIndex)
   }
 
   return email
-}"""
-    check_results = get_check_results("test.ts", code)
+  }
+"""
+    new_code = """console.log("hello world")"""
+    check_results = check_valid_typescript("test.ts",new_code)
     import pdb
     # pylint: disable=no-member
     pdb.set_trace()
```

### Comparing `sweepai-2.0.0.dev1/sweepai/utils/utils_test.py` & `sweepai-2.0.1/sweepai/utils/utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/watch.py` & `sweepai-2.0.1/sweepai/watch.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/web/events.py` & `sweepai-2.0.1/sweepai/web/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/web/health.py` & `sweepai-2.0.1/sweepai/web/health.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai/web/health_test.py` & `sweepai-2.0.1/sweepai/web/health_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.0.dev1/sweepai.egg-info/SOURCES.txt` & `sweepai-2.0.1/sweepai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 LICENSE
 README.md
 pyproject.toml
-eval/swe_bench.py
-eval/swe_bench_utils.py
 sweepai/__init__.py
 sweepai/api.py
 sweepai/api_test.py
 sweepai/cli.py
 sweepai/cli_test.py
 sweepai/global_threads.py
 sweepai/watch.py
 sweepai.egg-info/PKG-INFO
 sweepai.egg-info/SOURCES.txt
 sweepai.egg-info/dependency_links.txt
 sweepai.egg-info/entry_points.txt
 sweepai.egg-info/requires.txt
 sweepai.egg-info/top_level.txt
 sweepai/agents/agent_utils.py
-sweepai/agents/assistant_function_modify.py
 sweepai/agents/assistant_functions.py
-sweepai/agents/assistant_planning.py
 sweepai/agents/assistant_wrapper.py
 sweepai/agents/assistant_wrapper_test.py
 sweepai/agents/complete_code.py
 sweepai/agents/complete_code_test.py
 sweepai/agents/distill_issue.py
+sweepai/agents/modify.py
 sweepai/agents/modify_bot.py
 sweepai/agents/modify_file.py
 sweepai/agents/pr_description_bot.py
 sweepai/agents/prune_modify_snippets.py
 sweepai/config/__init__.py
 sweepai/config/client.py
 sweepai/config/server.py
@@ -48,14 +45,15 @@
 sweepai/core/vector_db.py
 sweepai/handlers/__init__.py
 sweepai/handlers/create_pr.py
 sweepai/handlers/on_button_click.py
 sweepai/handlers/on_button_click_test.py
 sweepai/handlers/on_check_suite.py
 sweepai/handlers/on_comment.py
+sweepai/handlers/on_jira_ticket.py
 sweepai/handlers/on_merge.py
 sweepai/handlers/on_merge_conflict.py
 sweepai/handlers/on_review.py
 sweepai/handlers/on_ticket.py
 sweepai/handlers/pr_utils.py
 sweepai/handlers/stack_pr.py
 sweepai/handlers/stack_pr_test.py
@@ -104,11 +102,14 @@
 sweepai/utils/str_utils.py
 sweepai/utils/ticket_utils.py
 sweepai/utils/timer.py
 sweepai/utils/tree_utils.py
 sweepai/utils/user_settings.py
 sweepai/utils/utils.py
 sweepai/utils/utils_test.py
+sweepai/web/event_utils.py
 sweepai/web/events.py
 sweepai/web/health.py
 sweepai/web/health_test.py
+tests/test_gha_extraction.py
+tests/test_jira_ticket.py
 tests/test_watch.py
```

### Comparing `sweepai-2.0.0.dev1/sweepai.egg-info/requires.txt` & `sweepai-2.0.1/sweepai.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 anthropic==0.21.3
 beautifulsoup4==4.12.3
+cohere==5.2.5
 typer==0.10.0
 pygithub==2.2.0
 loguru==0.7.2
 rich==13.7.1
 fastapi==0.110.0
 prometheus-fastapi-instrumentator==7.0.0
 pyyaml==6.0.1
@@ -35,7 +36,8 @@
 tiktoken==0.6.0
 uvicorn==0.29.0
 pylint==3.1.0
 parea-ai==0.2.114
 voyageai==0.2.1
 boto3==1.34.70
 scipy==1.12.0
+jira==3.8.0
```

