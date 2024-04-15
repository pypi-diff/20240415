# Comparing `tmp/MindsDB-24.4.2.1.tar.gz` & `tmp/MindsDB-24.4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MindsDB-24.4.2.1.tar", last modified: Thu Apr 11 16:57:53 2024, max compression
+gzip compressed data, was "MindsDB-24.4.3.0.tar", last modified: Mon Apr 15 13:45:12 2024, max compression
```

## Comparing `MindsDB-24.4.2.1.tar` & `MindsDB-24.4.3.0.tar`

### file list

```diff
@@ -1,2085 +1,2090 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.682706 MindsDB-24.4.2.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     5804 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/MindsDB.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)    14576 2024-04-11 16:57:53.000000 MindsDB-24.4.2.1/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)   101186 2024-04-11 16:57:53.000000 MindsDB-24.4.2.1/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 16:57:53.000000 MindsDB-24.4.2.1/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    10785 2024-04-11 16:57:53.000000 MindsDB-24.4.2.1/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-11 16:57:53.000000 MindsDB-24.4.2.1/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    14576 2024-04-11 16:57:53.682706 MindsDB-24.4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     9634 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      189 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/default_handlers.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/
--rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13732 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/common/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/executor/
--rw-r--r--   0 runner    (1000) runner    (1000)       51 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    83474 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/command_executor.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/executor/controllers/
--rw-r--r--   0 runner    (1000) runner    (1000)      267 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/controllers/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4371 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/executor/data_types/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/data_types/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      673 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/data_types/answer.py
--rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/data_types/response_type.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/classes/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1794 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1000) runner    (1000)      175 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datahub.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datanodes/
--rw-r--r--   0 runner    (1000) runner    (1000)      185 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34279 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8233 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7001 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datanodes/project_datanode.py
--rw-r--r--   0 runner    (1000) runner    (1000)      566 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/exceptions.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6775 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/result_set.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11126 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/sql_query.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/
--rw-r--r--   0 runner    (1000) runner    (1000)      728 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15677 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/apply_predictor_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/base.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1286 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/delete_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3809 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/fetch_dataframe.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3333 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/insert_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3164 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/join_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4728 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/map_reduce_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)      653 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/multiple_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1504 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/prepare_steps.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2802 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/project_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1001 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/sql_steps.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4149 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/subselect_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1619 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/union_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4471 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/update_step.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.546710 MindsDB-24.4.2.1/mindsdb/api/executor/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      995 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/utilities/functions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6049 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/executor/utilities/sql.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.550710 MindsDB-24.4.2.1/mindsdb/api/http/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3087 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)      534 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14068 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.550710 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10916 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/agents.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3810 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5483 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10832 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/chatbots.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9382 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.550710 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      124 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/agents.py
--rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1000) runner    (1000)      103 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/chatbots.py
--rw-r--r--   0 runner    (1000) runner    (1000)      102 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)      147 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1000) runner    (1000)      103 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1000) runner    (1000)       86 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1000) runner    (1000)      107 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1000) runner    (1000)      130 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1000) runner    (1000)      130 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/skills.py
--rw-r--r--   0 runner    (1000) runner    (1000)       98 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1000) runner    (1000)      112 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1000) runner    (1000)       93 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10920 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4729 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6319 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6853 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11226 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/models.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1203 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5923 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/skills.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5359 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4054 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3380 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4569 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5675 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/namespaces/views.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2096 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1000) runner    (1000)      589 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.550710 MindsDB-24.4.2.1/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.550710 MindsDB-24.4.2.1/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1000) runner    (1000)      177 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      746 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1764 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1000) runner    (1000)      769 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3217 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1000) runner    (1000)      812 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.550710 MindsDB-24.4.2.1/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1000) runner    (1000)      266 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.554710 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1000) runner    (1000)     2655 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      228 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2364 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1000) runner    (1000)      317 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1767 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1000) runner    (1000)      689 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)      577 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)      487 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1000) runner    (1000)      825 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4221 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1000) runner    (1000)      230 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5835 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1000) runner    (1000)      314 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1000) runner    (1000)      272 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1000) runner    (1000)      244 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9421 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1000) runner    (1000)      446 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1000) runner    (1000)      285 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1536 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1000) runner    (1000)      920 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1000) runner    (1000)      538 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1000) runner    (1000)      223 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1000) runner    (1000)      234 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1000) runner    (1000)      235 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1000) runner    (1000)      890 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1004 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1000) runner    (1000)      180 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14062 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1000) runner    (1000)      420 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.554710 MindsDB-24.4.2.1/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7666 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4256 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2147 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.554710 MindsDB-24.4.2.1/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.554710 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.554710 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3358 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1249 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.554710 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1000) runner    (1000)       75 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      939 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)      586 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4436 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6316 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5094 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1000) runner    (1000)     1550 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4620 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1097 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2982 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5765 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1428 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1520 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)      486 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2927 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3770 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3785 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)      421 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1523 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1426 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1494 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1452 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5422 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9576 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)      619 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5534 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/mysql_executor.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4116 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35316 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33693 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2341 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/nlp/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6499 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12729 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1121 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1093 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40804 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1000) runner    (1000)      626 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8422 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19392 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.558709 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)      259 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      325 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      375 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      633 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6392 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2406 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       25 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1074 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      670 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9103 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/aerospike_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1139 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/tests/test_aerospike_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6830 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1930 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8312 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      182 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1938 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      381 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      517 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7556 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/anomaly_detection_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/requirements.txt
--rwxr-xr-x   0 runner    (1000) runner    (1000)      649 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anthropic_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anthropic_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      588 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anthropic_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3398 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anthropic_handler/anthropic_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      328 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anthropic_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anthropic_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.562709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anyscale_endpoints_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anyscale_endpoints_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      538 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anyscale_endpoints_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8306 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anyscale_endpoints_handler/anyscale_endpoints_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1743 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anyscale_endpoints_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       81 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/anyscale_endpoints_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.574709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/apache_doris_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      358 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/apache_doris_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/apache_doris_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      319 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/apache_doris_handler/apache_doris_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1933 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/apache_doris_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/apache_doris_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.574709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      909 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/aqicn.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3216 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/aqicn_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12837 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/aqicn_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3304 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/icon.png
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.574709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.574709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6352 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      690 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      131 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.574709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1180 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1188 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.578709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      522 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1774 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/autogluon_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)      956 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.578709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      560 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5618 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      693 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autokeras_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autokeras_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.582709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      561 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1683 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      710 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15729 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.582709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      584 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6000 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2303 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       50 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.582709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      914 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.582709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      484 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5334 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7458 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1020 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.586709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      475 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23890 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     4454 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)       27 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.586709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1645 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14968 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       65 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.586709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1353 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.586709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14733 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/chromadb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4199 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1950 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.586709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15883 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/tests/test_chromadb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.590709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      472 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3515 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8453 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.590709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      807 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.590709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      615 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6583 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      387 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.590709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1445 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.590709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      555 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3157 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/clipdrop.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/clipdrop_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1759 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.590709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      669 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7521 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    75313 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.590709 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1592 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      366 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      618 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5153 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27975 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)      195 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1157 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1157 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1857 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1187 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cohere_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cohere_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      542 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cohere_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3248 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1163 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cohere_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/cohere_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      577 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6043 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/coinbase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1658 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/coinbase_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1909 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      522 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2768 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7031 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2500 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2163 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/tests/test_confluence_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8067 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1683 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1237 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7007 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      634 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1484 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      516 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2136 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       68 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.594708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1687 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6919 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2675 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1231 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      685 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1000) runner    (1000)    86110 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)    58645 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)    35986 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)    21694 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)    62078 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)     8455 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      618 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1302 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      544 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      327 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      445 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       65 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8885 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    56094 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1439 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8768 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2278 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1513 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.598708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5600 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/discord_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5899 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/discord_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1330 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2172 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/tests/test_discord.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2277 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/dockerhub.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4222 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16832 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3562 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/documentdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/documentdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      592 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/documentdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2899 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/documentdb_handler/documentdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/documentdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       66 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/documentdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      599 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7312 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5946 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1109 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      362 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7665 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2823 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1084 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5512 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      658 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1479 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dummy_data_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      228 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dummy_data_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      491 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dummy_data_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2740 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dummy_data_handler/dummy_data_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      152 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dummy_data_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      638 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6618 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1929 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1190 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      617 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1869 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      742 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2005 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8374 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3383 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       33 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.602708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1120 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/email_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2734 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/email_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/email_ingestor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5209 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/email_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32416 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1632 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      399 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      615 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7739 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)   328372 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1843 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3267 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18318 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7954 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9086 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2404 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      661 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10364 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/faunadb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      807 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1144 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/tests/test_faunadb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14717 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/file_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      133 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/tests/data/
--rw-r--r--   0 runner    (1000) runner    (1000)      570 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/tests/data/test.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    12750 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/tests/test_file_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9639 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4207 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       41 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.606708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1243 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/flaml_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/flaml_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/flaml_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1617 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3096 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/flaml_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/flaml_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      480 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4374 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7988 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2648 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)      920 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4645 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30742 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1198 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2587 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15320 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1995 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      528 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20489 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      862 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1479 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1332 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      532 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4718 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10179 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1815 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/tests/test_google_analytics_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      379 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6901 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6268 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)      962 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      569 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11062 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8111 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1915 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      110 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.610708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2215 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      424 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      663 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16267 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14279 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2651 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2436 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      358 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      495 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6631 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2496 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1511 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_gemini_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      374 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_gemini_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      581 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_gemini_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2647 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_gemini_handler/google_gemini_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_gemini_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_gemini_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      382 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8089 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7375 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3303 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2178 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hackernews_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hackernews_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hackernews_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3722 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5281 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      611 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11129 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2135 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      592 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5972 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17076 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1638 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7519 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41120 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.614708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2796 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/hubspot_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19979 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/hubspot_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1453 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      381 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      536 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      112 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8782 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9064 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      549 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8085 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/finetune.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13592 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9064 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       77 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/requirements_cpu.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      984 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      761 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7598 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1013 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3532 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5655 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1559 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      514 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2681 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3065 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3019 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3200 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     9626 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       89 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1702 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      389 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2321 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7607 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       79 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1817 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.618708 MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      987 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     4076 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/instatus_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15203 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/instatus_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.622707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3716 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3738 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/intercom_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4953 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/intercom_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      508 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1246 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3225 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5472 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/jira_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/kinetica_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/kinetica_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      681 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/kinetica_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      758 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/kinetica_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1986 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/kinetica_handler/kinetica_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/kinetica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      661 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3475 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    14420 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/lancedb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       37 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3351 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/tests/test_lancedb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_embedding_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_embedding_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      561 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_embedding_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73222 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_embedding_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7473 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_embedding_handler/langchain_embedding_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_embedding_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1989 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/constants.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73222 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    13763 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3750 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/log_callback_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1704 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    11201 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/tools.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/leonardoai_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/leonardoai_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/leonardoai_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    99151 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/leonardoai_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8339 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/leonardoai_handler/leonardo_ai_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/leonardoai_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1387 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6271 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/libsql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1496 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/tests/test_libsql_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.626707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      540 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18709 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11253 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     3186 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/lightdash_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20193 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/lightdash_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.630707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.630707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5263 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1678 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6788 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      143 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.630707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9139 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    23643 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       91 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.630707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10985 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2242 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.630707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      534 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1293 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6694 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/lindorm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.630707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1037 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/tests/test_lindorm_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.630707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      550 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37122 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     4899 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/litellm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2488 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.630707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2269 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/github_loader_helper.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12609 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    11554 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.630707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1000) runner    (1000)      414 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     2395 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      250 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6041 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     1939 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/luma.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2434 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/luma_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5495 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/luma_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      485 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2843 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      315 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      501 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2689 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1285 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1774 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      612 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1573 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6895 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1776 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2141 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7528 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1905 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18250 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     2182 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3299 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      500 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2721 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8696 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4456 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4330 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8498 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2657 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8238 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1117 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    20322 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/milvus_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1154 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mlflow_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3802 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      611 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8134 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       28 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1622 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.634707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1134 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      573 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1050 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     9694 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3890 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/tests/test_mongodb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6960 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monkeylearn_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14734 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monkeylearn_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     3565 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      518 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3934 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7981 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/ms_graph_api_teams_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5389 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21577 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    10192 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11944 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     4830 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4382 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4136 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    10843 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      587 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6374 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/requirements_extra.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      662 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2790 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     7178 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3188 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      575 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2157 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7537 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/notion_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12946 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/notion_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2037 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/tests/test_notion_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      328 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      516 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      786 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)      674 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1651 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/npm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9036 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/npm_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     9850 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1626 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.638707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2615 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1293 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1741 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      658 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1222 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1695 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3389 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6516 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ollama_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ollama_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ollama_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   113588 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ollama_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     6030 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ollama_handler/ollama_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1190 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/constants.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5771 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2625 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    36366 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       34 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      373 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      525 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     4978 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/openbb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11289 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/openbb_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       33 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      613 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1758 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1390 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1379 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4496 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     2669 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7765 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1228 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/tests/test_openstreetmap_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7078 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1064 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      810 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1307 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1747 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/palm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/palm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/palm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1485 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/palm_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    16725 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/palm_handler/palm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/palm_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1833 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3815 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9866 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.642707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pgvector_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pgvector_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pgvector_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13760 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pgvector_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    11463 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pgvector_handler/pgvector_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       76 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pgvector_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43812 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     8788 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1037 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2683 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    14972 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/pinecone_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       15 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10555 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8603 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1132 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pirateweather_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pirateweather_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      695 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pirateweather_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    54926 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pirateweather_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     8203 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pirateweather_handler/pirateweather_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1389 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8103 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5151 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      149 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      621 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      391 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1327 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/popularity_recommender_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/popularity_recommender_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      562 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/popularity_recommender_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3114 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/popularity_recommender_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13757 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    10782 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5815 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/tests/test_postgres_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      564 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10283 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     4759 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/pycaret_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       24 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/test/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/test/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10377 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/test/test_pycaret.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4258 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18842 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1907 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/pypi_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7043 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/pypi_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/qdrant_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/qdrant_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/qdrant_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1629 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/qdrant_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    19040 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/qdrant_handler/qdrant_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/qdrant_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      485 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2029 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      796 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.646707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1172 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.650707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1289 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3395 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13384 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.650707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      517 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5873 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/ingest.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4758 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/rag.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4978 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/rag_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      199 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    15414 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.650707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      595 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1990 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ray_serve_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     2661 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.650707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3986 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3265 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6558 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        4 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.650707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      765 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7618 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.650707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1212 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.650707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      550 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.650707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/assets/
--rw-r--r--   0 runner    (1000) runner    (1000)   355320 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/assets/Arjuna.png
--rw-r--r--   0 runner    (1000) runner    (1000)  1314584 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/assets/groot.png
--rw-r--r--   0 runner    (1000) runner    (1000)  1556534 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/assets/warrior.png
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6893 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/replicate_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      360 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      499 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2492 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5293 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6298 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      539 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1362 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/rockset_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   194064 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1000) runner    (1000)   108141 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/tests/test_rockset_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      591 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1930 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1249 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2168 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5407 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    59422 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9670 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     8412 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1290 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2730 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2601 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10852 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      394 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      604 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2691 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       61 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2686 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/sentence_transformers_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      276 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      533 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4590 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    20746 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4175 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17973 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1896 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/tests/test_sharepoint_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5229 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5628 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5785 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1059 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2452 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     4954 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31708 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.654707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2064 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1446 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      518 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2005 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    17306 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      882 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4088 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     4746 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1309 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solace_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solace_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      480 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solace_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      152 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solace_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solace_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5647 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solace_handler/solace_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      599 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1215 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       15 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     6928 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1215 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/spacy_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/spacy_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      487 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/spacy_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3544 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/spacy_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/spacy_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5829 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/spacy_handler/spacy_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       27 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     7023 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      623 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3379 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6000 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1033 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19052 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     6297 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1434 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1284 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     6901 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/stabilityai.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7274 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/stabilityai_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1945 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1301 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1746 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.658707 MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      374 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/requirements_extra.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     8220 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      529 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5441 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/strapi_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4803 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/strapi_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1904 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/tests/test_strapi_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     3433 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8188 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      704 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2858 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16193 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1174 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      326 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1408 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1449 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     7492 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1891 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      632 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     3586 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/symbl_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18160 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/symbl_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4903 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5370 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1564 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      465 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     8286 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      593 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      470 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1334 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1338 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timegpt_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      390 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timegpt_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      490 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timegpt_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timegpt_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timegpt_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     9845 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timegpt_handler/timegpt_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      497 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6197 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.662706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1552 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1242 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      526 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   114250 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tpot_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     3335 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      457 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9363 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       22 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1630 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6813 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      527 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1769 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     9888 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10822 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14054 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_table.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      559 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2110 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     9351 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16821 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_api_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10747 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twilio_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twilio_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twilio_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1547 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twilio_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twilio_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    13129 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twilio_handler/twilio_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      500 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      471 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    16111 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/api_utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/api_utilities/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/
--rw-r--r--   0 runner    (1000) runner    (1000)       56 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3086 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/ms_graph_api_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)      123 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      258 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/exceptions.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/google/
--rw-r--r--   0 runner    (1000) runner    (1000)      150 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/google/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2412 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_service_account_oauth_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4230 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_user_oauth_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/google/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/
--rw-r--r--   0 runner    (1000) runner    (1000)       62 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4114 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/ms_graph_api_auth_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)      279 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/base_query_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1555 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/delete_query_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)      432 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3110 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4239 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2557 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/update_query_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/validation_utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)       72 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/validation_utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      678 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/validation_utilities/parameter_validation_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      498 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23708 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/requirements.txt
--rwxr-xr-x   0 runner    (1000) runner    (1000)     3942 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/vertex_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3924 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/vertex_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.666706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      604 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1482 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1663 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6038 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2834 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1727 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/weaviate_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/weaviate_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/weaviate_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   115913 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/weaviate_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/weaviate_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    25567 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/weaviate_handler/weaviate_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1385 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1046 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/tests/example_data.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1516 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/tests/test_helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10860 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3161 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/web_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1042 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       84 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5777 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/webz_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6219 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/webz_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/whatsapp_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/whatsapp_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      533 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/whatsapp_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3521 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/whatsapp_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/whatsapp_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    14477 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/whatsapp_handler/whatsapp_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12498 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/evaluate.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1814 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/ingest.py
--rw-r--r--   0 runner    (1000) runner    (1000)      409 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/rag.py
--rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2878 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6883 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/writer_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      646 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2726 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16519 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/xata_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      954 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5294 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16797 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      490 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3292 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1612 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1969 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1113 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2043 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3953 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15080 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.670706 MindsDB-24.4.2.1/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1375 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5252 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers_client/db_grpc_client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7869 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5549 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1098 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10701 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      236 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/api_handler_exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12851 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1000) runner    (1000)      407 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1931 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/handler_helpers.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/libs/llm/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/llm/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2869 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/llm/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22181 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/llm/utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16707 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_exec_base.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/
--rw-r--r--   0 runner    (1000) runner    (1000)      663 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/create_engine_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      444 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/create_validation_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4225 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/describe_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      771 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/handlers_cacher.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6671 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/learn_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1346 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/predict_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/update_engine_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      784 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/update_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      966 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14566 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/process_cache.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1171 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/realtime_chat_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3119 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/storage_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15599 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/libs/vectordatabase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/utilities/datasets/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/datasets/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1665 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/datasets/dataset.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/utilities/datasets/question_answering/
--rw-r--r--   0 runner    (1000) runner    (1000)     6906 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/datasets/question_answering/fda_style_qa.csv
--rw-r--r--   0 runner    (1000) runner    (1000)   104035 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/datasets/question_answering/squad_v2_val_100_sample.csv
--rw-r--r--   0 runner    (1000) runner    (1000)     2769 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2113 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/handler_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2095 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1000) runner    (1000)      384 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/processes.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/loaders/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/loaders/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/loaders/vector_store_loader/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/loaders/vector_store_loader/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4386 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/loaders/vector_store_loader/vector_store_loader.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/pipelines/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/pipelines/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3352 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/pipelines/rag.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2484 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/rag_pipeline_builder.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/retrievers/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/retrievers/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3993 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/retrievers/auto_retriever.py
--rw-r--r--   0 runner    (1000) runner    (1000)      264 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/retrievers/base.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4427 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/retrievers/multi_vector_retriever.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5473 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1623 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3467 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/vector_store.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5928 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)      691 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8312 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)      972 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/interfaces/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/interfaces/agents/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/agents/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11433 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/agents/agents_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.674706 MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11171 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/chatbot_controller.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6514 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/chatbot_executor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3790 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/chatbot_task.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5550 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/memory.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3473 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/model_executor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4292 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/polling.py
--rw-r--r--   0 runner    (1000) runner    (1000)      929 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/types.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4063 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28097 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11064 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/database/log.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11134 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3737 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4629 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14357 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3602 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/knowledge_base/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/knowledge_base/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13849 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/knowledge_base/controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4590 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20365 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/query_context/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/query_context/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9338 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/query_context/context_controller.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7156 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/query_context/last_query.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/skills/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/skills/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4240 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/skills/skill_tool.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5414 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/skills/skills_controller.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7268 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/skills/sql_agent.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17504 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20045 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2925 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8267 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/tabs/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/tabs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8761 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/tabs/tabs_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/tasks/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/tasks/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      401 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/tasks/task.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3863 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/tasks/task_monitor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1666 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/tasks/task_thread.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/interfaces/triggers/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/triggers/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2911 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/triggers/trigger_task.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5376 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/interfaces/triggers/triggers_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/metrics/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/metrics/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1819 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/metrics/metrics.py
--rw-r--r--   0 runner    (1000) runner    (1000)      985 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/metrics/server.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1263 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)      159 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2327 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12845 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3565 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14810 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1263 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)      159 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2170 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5430 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.678706 MindsDB-24.4.2.1/mindsdb/migrations/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2193 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1000) runner    (1000)     2218 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1769 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.682706 MindsDB-24.4.2.1/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1000) runner    (1000)     5871 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1050 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10817 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6163 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2788 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1000) runner    (1000)      849 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1000) runner    (1000)      998 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1000 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1045 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2330 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1957 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1789 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2384 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3486 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1802 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3487 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)      799 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2035 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1008 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1115 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1000) runner    (1000)      836 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1000) runner    (1000)      930 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1567 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1180 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
--rw-r--r--   0 runner    (1000) runner    (1000)      730 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      856 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1138 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1940 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-07-13_a57506731839_triggers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1222 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-07-19_ad04ee0bd385_chatbot_to_task.py
--rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-08-29_b0382f5be48d_predictor_hostname.py
--rw-r--r--   0 runner    (1000) runner    (1000)      732 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-08-31_4c26ad04eeaa_add_skills_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      983 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-06_d44ab65a6a35_add_agents_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      605 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-06_e187961e844a_add_agent_skills_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2519 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-18_011e6f2dd9c2_backfill_agent_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)      701 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-18_f16d4ab03091_add_agent_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1735 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-20_309db3d07cf4_add_knowledge_base.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1023 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-10-03_6cb02dfd7f61_query_context.py
--rw-r--r--   0 runner    (1000) runner    (1000)      824 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-11-01_c67822e96833_jobs_active.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1323 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-12-25_4b3c9d63e89c_predictor_index.py
--rw-r--r--   0 runner    (1000) runner    (1000)      837 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2024-02-02_5a5c49313e52_job_condition.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1419 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/2024-02-12_9461892bd889_llm_log.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.682706 MindsDB-24.4.2.1/mindsdb/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7245 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6450 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1450 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/context_executor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1034 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/exception.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5458 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7184 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.682706 MindsDB-24.4.2.1/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1000) runner    (1000)      796 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2262 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1000) runner    (1000)      965 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2336 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1039 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.682706 MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/
--rw-r--r--   0 runner    (1000) runner    (1000)     2810 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      453 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/base.py
--rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/const.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9413 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/consumer.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2702 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/producer.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3166 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/task.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3177 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.682706 MindsDB-24.4.2.1/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1000) runner    (1000)      251 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3936 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2339 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1000) runner    (1000)      751 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/security.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1377 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1708 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1000) runner    (1000)      122 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 16:57:53.682706 MindsDB-24.4.2.1/requirements/
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/requirements/requirements-grpc.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      842 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-11 16:57:53.682706 MindsDB-24.4.2.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     5998 2024-04-11 16:57:37.000000 MindsDB-24.4.2.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.373869 MindsDB-24.4.3.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5804 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)    14576 2024-04-15 13:45:12.000000 MindsDB-24.4.3.0/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)   101449 2024-04-15 13:45:12.000000 MindsDB-24.4.3.0/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-15 13:45:12.000000 MindsDB-24.4.3.0/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    10808 2024-04-15 13:45:12.000000 MindsDB-24.4.3.0/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-15 13:45:12.000000 MindsDB-24.4.3.0/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    14576 2024-04-15 13:45:12.373869 MindsDB-24.4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     9634 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      189 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/default_handlers.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/
+-rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13732 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/common/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/executor/
+-rw-r--r--   0 runner    (1000) runner    (1000)       51 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    83474 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/command_executor.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/executor/controllers/
+-rw-r--r--   0 runner    (1000) runner    (1000)      267 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/controllers/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4371 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/executor/data_types/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/data_types/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      673 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/data_types/answer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/data_types/response_type.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/classes/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1794 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      175 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datahub.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datanodes/
+-rw-r--r--   0 runner    (1000) runner    (1000)      185 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34334 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8233 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7001 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datanodes/project_datanode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      566 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/exceptions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6775 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/result_set.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11126 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/sql_query.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/
+-rw-r--r--   0 runner    (1000) runner    (1000)      728 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15677 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/apply_predictor_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/base.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1286 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/delete_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3809 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/fetch_dataframe.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3333 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/insert_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3164 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/join_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4728 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/map_reduce_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      653 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/multiple_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1504 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/prepare_steps.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2802 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/project_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1001 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/sql_steps.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4149 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/subselect_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1619 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/union_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4471 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/update_step.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.269869 MindsDB-24.4.3.0/mindsdb/api/executor/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      995 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/utilities/functions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6049 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/executor/utilities/sql.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.273869 MindsDB-24.4.3.0/mindsdb/api/http/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3087 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      534 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14068 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.273869 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10916 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/agents.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3810 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5483 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10832 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/chatbots.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9382 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.273869 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      124 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/agents.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      103 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/chatbots.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      102 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      147 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      103 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       86 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      107 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      130 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      130 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/skills.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       98 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      112 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       93 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10920 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4729 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6319 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6853 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11226 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/models.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1203 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5923 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/skills.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5359 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4054 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3380 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4569 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5675 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/namespaces/views.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2096 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      589 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.273869 MindsDB-24.4.3.0/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.273869 MindsDB-24.4.3.0/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1000) runner    (1000)      177 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      746 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1764 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      769 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3217 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      812 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.273869 MindsDB-24.4.3.0/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1000) runner    (1000)      266 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2655 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      228 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2364 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      317 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1767 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      689 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      577 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      487 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      825 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4221 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      230 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5835 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      314 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      272 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      244 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9421 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      446 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      285 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1536 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      920 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      538 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      223 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      234 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      235 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      890 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1004 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      180 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14062 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      420 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7666 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4256 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2147 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3358 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1249 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1000) runner    (1000)       75 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      939 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      586 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4436 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6316 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5094 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1550 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4620 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1097 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2982 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5765 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1428 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1520 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      486 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2927 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3770 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3785 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      421 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1523 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1426 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1494 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1452 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5422 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9576 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      619 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5534 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/mysql_executor.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4116 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35316 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33693 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2341 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/nlp/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6499 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12729 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1121 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1093 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40804 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      626 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8422 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19392 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)      259 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      325 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/integrations/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.277869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      375 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      633 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6392 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2406 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       25 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1074 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      670 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9103 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/aerospike_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1139 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/tests/test_aerospike_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6830 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1930 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8312 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      182 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1938 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      381 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      517 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7556 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/anomaly_detection_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/requirements.txt
+-rwxr-xr-x   0 runner    (1000) runner    (1000)      649 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anthropic_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anthropic_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      588 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anthropic_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3398 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anthropic_handler/anthropic_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      328 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anthropic_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anthropic_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      538 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8306 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/anyscale_endpoints_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1743 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       81 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/apache_doris_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      358 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/apache_doris_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/apache_doris_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      319 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/apache_doris_handler/apache_doris_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1933 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/apache_doris_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/apache_doris_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      909 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/aqicn.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3216 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12837 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3304 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/icon.png
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6352 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      690 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      131 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1180 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1188 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      522 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1774 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/autogluon_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      956 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.281870 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      560 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5618 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      693 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autokeras_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autokeras_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      561 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1683 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      710 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15729 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      584 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6000 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2303 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       50 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      914 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      484 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5334 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7458 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1020 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      475 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23890 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     4454 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       27 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1645 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14968 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       65 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1353 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14733 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/chromadb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4199 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1950 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15477 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/tests/test_chromadb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      472 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3515 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8453 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      807 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      615 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6583 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      387 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1445 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      555 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3157 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1759 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      669 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7521 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    75313 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1592 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.285869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      366 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      618 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5153 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27975 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)      195 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1157 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1157 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1857 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1187 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cohere_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cohere_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      542 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cohere_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3248 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1163 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cohere_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/cohere_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      577 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6043 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1658 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1909 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      522 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2768 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7031 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2500 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2163 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/tests/test_confluence_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8067 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1683 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1237 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7007 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      634 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1484 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      516 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2136 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       68 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1687 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6919 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2675 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1231 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      685 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1000) runner    (1000)    86110 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)    58645 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)    35986 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)    21694 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)    62078 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8455 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      618 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.289869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1302 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      544 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      327 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      445 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       65 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8885 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    56094 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1439 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8768 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2278 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1513 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5600 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/discord_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5899 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/discord_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1330 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2172 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/tests/test_discord.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2277 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4222 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16832 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3562 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/documentdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/documentdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      592 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/documentdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2899 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/documentdb_handler/documentdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/documentdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       66 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/documentdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      599 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7312 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5946 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1109 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      362 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7665 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2823 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1084 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5512 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      658 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1479 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dummy_data_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      228 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dummy_data_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      491 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dummy_data_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2740 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dummy_data_handler/dummy_data_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      152 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dummy_data_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      638 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6618 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1929 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1190 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.293869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      617 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1869 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      742 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2005 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8374 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3383 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       33 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1120 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/email_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2734 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/email_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/email_ingestor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5209 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/email_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32416 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1632 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      399 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      615 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7739 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   328372 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1843 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3267 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18318 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7954 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9086 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2404 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      661 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10364 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/faunadb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      807 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1144 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/tests/test_faunadb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14717 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/file_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      133 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/tests/data/
+-rw-r--r--   0 runner    (1000) runner    (1000)      570 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/tests/data/test.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    12750 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/tests/test_file_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9639 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4207 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       41 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1243 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/flaml_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/flaml_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/flaml_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1617 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3096 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/flaml_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/flaml_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.297869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      480 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4374 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7988 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2648 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      920 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4645 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30742 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1198 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2587 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15320 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1995 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      528 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20489 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      862 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1479 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1332 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      532 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4718 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10179 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1815 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/tests/test_google_analytics_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      379 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6901 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6268 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      962 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      569 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11062 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8111 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1915 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      110 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2215 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      424 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      663 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16267 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14279 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2651 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2436 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      358 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      495 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6631 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2496 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1511 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_gemini_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      374 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_gemini_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      581 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_gemini_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2647 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_gemini_handler/google_gemini_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_gemini_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_gemini_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      382 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8089 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7375 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3303 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.301869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2178 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hackernews_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hackernews_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hackernews_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3722 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5281 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      611 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11129 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2135 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      592 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5972 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17076 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1638 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7519 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41120 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2796 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19979 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1453 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      381 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      536 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      112 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8782 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9064 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      549 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8085 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/finetune.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13592 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9064 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       77 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/requirements_cpu.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      984 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      761 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7598 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1013 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3532 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5655 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1559 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      514 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2681 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3065 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3019 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3200 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     9626 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       89 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.305869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1702 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      389 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2321 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7607 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       79 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1817 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      987 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     4076 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/instatus_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15203 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/instatus_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3716 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3738 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/intercom_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4953 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/intercom_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      508 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1246 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3225 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5472 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/kinetica_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/kinetica_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      681 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/kinetica_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      758 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/kinetica_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1986 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/kinetica_handler/kinetica_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/kinetica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      661 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3475 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    14420 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/lancedb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       37 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3351 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/tests/test_lancedb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_embedding_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_embedding_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      561 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_embedding_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73222 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_embedding_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7473 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_embedding_handler/langchain_embedding_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_embedding_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1973 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/constants.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73222 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    15417 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3787 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/log_callback_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1704 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      279 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    12588 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/tools.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/leonardoai_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/leonardoai_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/leonardoai_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    99151 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/leonardoai_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8339 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/leonardoai_handler/leonardo_ai_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/leonardoai_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1387 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6271 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/libsql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1496 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/tests/test_libsql_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      540 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18709 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11253 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     3186 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20193 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.309869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5263 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1678 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6788 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      143 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9139 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    23643 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       91 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10985 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2242 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      534 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1293 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6694 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/lindorm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1037 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/tests/test_lindorm_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      550 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37122 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     4899 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/litellm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2488 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2269 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/github_loader_helper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12609 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    11554 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      414 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2395 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      250 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6041 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     1939 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/luma.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2434 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/luma_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5495 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/luma_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      485 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2843 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      315 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      501 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2689 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1285 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1774 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      612 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1573 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6895 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1776 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.313869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2141 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7528 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1905 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18250 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2182 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3299 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      500 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2721 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8696 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4456 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4330 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8498 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2657 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8238 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1117 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    20322 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/milvus_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mindsdb_inference/
+-rw-r--r--   0 runner    (1000) runner    (1000)      368 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mindsdb_inference/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      582 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mindsdb_inference/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3014 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mindsdb_inference/mindsdb_inference_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       65 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mindsdb_inference/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1154 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mlflow_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3802 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      611 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8134 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       28 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1622 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1134 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      573 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1050 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     9694 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3890 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/tests/test_mongodb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6960 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monkeylearn_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14734 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monkeylearn_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     3565 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      518 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3934 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7981 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/ms_graph_api_teams_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5389 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21577 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    10192 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.317869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11944 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     4830 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4382 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4136 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    10843 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      587 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6374 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements_extra.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      662 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2790 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     7178 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3188 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      575 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2157 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7537 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/notion_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12946 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/notion_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2037 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/tests/test_notion_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      328 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      516 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      786 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      674 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1651 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/npm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9036 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/npm_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     9850 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1626 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2615 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1293 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1741 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      658 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1222 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1695 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3389 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6516 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ollama_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ollama_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ollama_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   113588 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ollama_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     6030 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ollama_handler/ollama_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1190 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/constants.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5482 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2625 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    36715 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       34 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.321869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      373 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      525 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     4978 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/openbb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11289 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/openbb_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       33 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      613 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1758 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1390 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1379 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4496 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2669 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7765 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1228 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/test_openstreetmap_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7078 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1064 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      810 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1307 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1747 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/palm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/palm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/palm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1485 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/palm_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    16725 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/palm_handler/palm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/palm_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1833 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3815 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9866 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pgvector_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pgvector_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pgvector_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13760 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pgvector_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    11463 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pgvector_handler/pgvector_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       76 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pgvector_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43812 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     8788 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1037 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2683 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    14972 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/pinecone_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       15 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10555 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8603 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1132 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.325869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pirateweather_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pirateweather_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      695 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pirateweather_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    54926 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pirateweather_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     8203 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pirateweather_handler/pirateweather_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1389 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8103 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5151 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      149 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      621 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      391 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1327 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/popularity_recommender_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/popularity_recommender_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      562 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/popularity_recommender_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3114 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/popularity_recommender_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13757 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    10782 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5815 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/tests/test_postgres_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      564 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10283 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     4759 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/pycaret_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       24 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/test/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/test/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10377 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/test/test_pycaret.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4258 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18842 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1907 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/pypi_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7043 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/pypi_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/qdrant_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/qdrant_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/qdrant_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1629 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/qdrant_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    19040 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/qdrant_handler/qdrant_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/qdrant_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      485 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2029 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      796 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1172 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1289 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3395 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13384 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      517 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5873 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/ingest.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4758 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/rag.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4978 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/rag_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      199 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    15414 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      595 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1990 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2661 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.329869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3986 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3265 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6558 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        4 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.333869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      765 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7618 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.333869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1212 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.333869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      550 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.333869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/assets/
+-rw-r--r--   0 runner    (1000) runner    (1000)   355320 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/assets/Arjuna.png
+-rw-r--r--   0 runner    (1000) runner    (1000)  1314584 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/assets/groot.png
+-rw-r--r--   0 runner    (1000) runner    (1000)  1556534 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/assets/warrior.png
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6893 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/replicate_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.333869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      360 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      499 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2492 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5293 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6298 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.333869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      539 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1362 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/rockset_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.333869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   194064 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1000) runner    (1000)   108141 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test_rockset_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.333869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      591 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1930 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.333869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1249 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2168 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5407 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    59422 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9670 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     8412 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1290 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2730 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2601 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10852 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      394 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      604 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2691 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       61 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2686 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/sentence_transformers_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      276 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      533 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4590 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    20746 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4175 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17973 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1896 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/tests/test_sharepoint_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5229 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5628 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5785 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1059 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2452 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     4954 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31708 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2064 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.337869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1446 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      518 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2005 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    17306 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      882 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4088 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     4746 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1309 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solace_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solace_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      480 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solace_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      152 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solace_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solace_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5647 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solace_handler/solace_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      599 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1215 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       15 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     6928 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1215 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/spacy_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/spacy_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      487 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/spacy_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3544 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/spacy_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/spacy_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5829 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/spacy_handler/spacy_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       27 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     7023 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      623 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3379 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6000 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1033 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19052 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     6297 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1434 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1284 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     6901 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7274 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1945 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1301 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.341869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1746 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      374 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/requirements_extra.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     8220 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      529 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5441 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/strapi_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4803 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/strapi_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1904 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/tests/test_strapi_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     3433 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8188 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      704 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2858 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16193 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1174 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      326 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1408 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1449 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     7492 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1891 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      632 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     3586 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/symbl_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18160 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/symbl_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4903 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5370 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1564 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.345869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      465 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     8286 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      593 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      470 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1334 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1338 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timegpt_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      390 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timegpt_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      490 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timegpt_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timegpt_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timegpt_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     9845 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timegpt_handler/timegpt_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      497 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6197 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1552 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1242 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      526 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   114250 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tpot_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     3335 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      457 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9363 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       22 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1630 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6813 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      527 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1769 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     9888 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10822 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14054 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_table.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      559 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2110 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     9351 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16821 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_api_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10747 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twilio_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twilio_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twilio_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1547 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twilio_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twilio_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    13129 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twilio_handler/twilio_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      500 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      471 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    16111 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/api_utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/api_utilities/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/
+-rw-r--r--   0 runner    (1000) runner    (1000)       56 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3086 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/ms_graph_api_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.349869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)      123 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      258 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/exceptions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/
+-rw-r--r--   0 runner    (1000) runner    (1000)      150 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2412 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_service_account_oauth_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4230 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_user_oauth_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/
+-rw-r--r--   0 runner    (1000) runner    (1000)       62 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4114 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/ms_graph_api_auth_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)      279 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/base_query_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1555 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/delete_query_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      432 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3110 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4239 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2557 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/update_query_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/validation_utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)       72 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/validation_utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      678 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/validation_utilities/parameter_validation_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      498 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23708 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/requirements.txt
+-rwxr-xr-x   0 runner    (1000) runner    (1000)     3942 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/vertex_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3924 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/vertex_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      604 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1482 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1663 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6038 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2834 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1727 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/weaviate_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/weaviate_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/weaviate_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   115913 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/weaviate_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/weaviate_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    25567 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/weaviate_handler/weaviate_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1385 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1046 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/tests/example_data.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1516 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/tests/test_helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10860 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3161 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/web_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1042 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       84 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5777 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/webz_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6219 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/webz_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.353869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/whatsapp_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/whatsapp_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      533 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/whatsapp_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3521 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/whatsapp_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/whatsapp_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    14477 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/whatsapp_handler/whatsapp_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12498 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/evaluate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1814 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/ingest.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      409 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/rag.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2878 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6883 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      646 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2726 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16519 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/xata_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      954 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5294 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16797 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      490 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3292 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1612 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1969 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1113 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2043 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3953 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15080 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1375 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5252 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers_client/db_grpc_client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7869 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5549 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1098 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10701 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      236 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/api_handler_exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12851 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      407 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1931 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/handler_helpers.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.357869 MindsDB-24.4.3.0/mindsdb/integrations/libs/llm/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/llm/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2869 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/llm/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22181 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/llm/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16707 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_exec_base.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/
+-rw-r--r--   0 runner    (1000) runner    (1000)      663 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/create_engine_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      444 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/create_validation_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4225 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/describe_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      771 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/handlers_cacher.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6671 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/learn_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1346 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/predict_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/update_engine_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      784 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/update_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      966 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14566 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/process_cache.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1171 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/realtime_chat_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3119 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/storage_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15599 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/libs/vectordatabase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/integrations/utilities/datasets/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/datasets/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1665 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/datasets/dataset.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/integrations/utilities/datasets/question_answering/
+-rw-r--r--   0 runner    (1000) runner    (1000)     6906 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/datasets/question_answering/fda_style_qa.csv
+-rw-r--r--   0 runner    (1000) runner    (1000)   104035 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/datasets/question_answering/squad_v2_val_100_sample.csv
+-rw-r--r--   0 runner    (1000) runner    (1000)     2769 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2113 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/handler_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2095 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      384 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/processes.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/loaders/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/loaders/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/loaders/vector_store_loader/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/loaders/vector_store_loader/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4356 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/loaders/vector_store_loader/vector_store_loader.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/pipelines/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/pipelines/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3411 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/pipelines/rag.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2797 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/rag_pipeline_builder.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/retrievers/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/retrievers/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3927 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/retrievers/auto_retriever.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      264 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/retrievers/base.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4363 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/retrievers/multi_vector_retriever.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5183 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1623 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3664 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/vector_store.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5928 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      691 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8312 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      972 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/interfaces/agents/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/agents/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11433 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/agents/agents_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11171 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/chatbot_controller.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6514 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/chatbot_executor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3790 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/chatbot_task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5550 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/memory.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3473 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/model_executor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4292 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/polling.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      929 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/types.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4063 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28097 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11064 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/database/log.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11134 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3737 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4629 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14357 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3602 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.361869 MindsDB-24.4.3.0/mindsdb/interfaces/knowledge_base/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/knowledge_base/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17783 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/knowledge_base/controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4590 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20365 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/interfaces/query_context/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/query_context/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9338 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/query_context/context_controller.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7156 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/query_context/last_query.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/interfaces/skills/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/skills/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5289 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/skills/skill_tool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5414 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/skills/skills_controller.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7268 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/skills/sql_agent.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17504 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20364 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2925 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8267 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/interfaces/tabs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/tabs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8761 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/tabs/tabs_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/interfaces/tasks/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/tasks/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      401 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/tasks/task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3863 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/tasks/task_monitor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1666 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/tasks/task_thread.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/interfaces/triggers/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/triggers/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2911 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/triggers/trigger_task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5376 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/interfaces/triggers/triggers_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/metrics/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/metrics/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1819 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/metrics/metrics.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      985 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/metrics/server.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1263 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      159 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2327 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12845 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3565 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14810 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1263 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      159 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2170 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5430 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.365869 MindsDB-24.4.3.0/mindsdb/migrations/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2193 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1000) runner    (1000)     2218 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1769 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.369869 MindsDB-24.4.3.0/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5871 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1050 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10817 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6163 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2788 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      849 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      998 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1000 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1045 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2330 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1957 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1789 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2384 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3486 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1802 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3487 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      799 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2035 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1008 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1115 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      836 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      930 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1567 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1180 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      730 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      856 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1138 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1940 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-07-13_a57506731839_triggers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1222 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-07-19_ad04ee0bd385_chatbot_to_task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-08-29_b0382f5be48d_predictor_hostname.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      732 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-08-31_4c26ad04eeaa_add_skills_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      983 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-06_d44ab65a6a35_add_agents_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      605 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-06_e187961e844a_add_agent_skills_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2519 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-18_011e6f2dd9c2_backfill_agent_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      701 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-18_f16d4ab03091_add_agent_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1735 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-20_309db3d07cf4_add_knowledge_base.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1023 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-10-03_6cb02dfd7f61_query_context.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      824 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-11-01_c67822e96833_jobs_active.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1323 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-12-25_4b3c9d63e89c_predictor_index.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      837 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2024-02-02_5a5c49313e52_job_condition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1419 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/2024-02-12_9461892bd889_llm_log.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.369869 MindsDB-24.4.3.0/mindsdb/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7245 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6743 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1450 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/context_executor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1034 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/exception.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5458 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7184 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.369869 MindsDB-24.4.3.0/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1000) runner    (1000)      796 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2262 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      965 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2336 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1039 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.369869 MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2810 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      453 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/base.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/const.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9413 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/consumer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2702 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/producer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3166 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3177 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.369869 MindsDB-24.4.3.0/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      251 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3936 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2339 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      751 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/security.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1377 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1708 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      122 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-15 13:45:12.373869 MindsDB-24.4.3.0/requirements/
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/requirements/requirements-grpc.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      851 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-15 13:45:12.373869 MindsDB-24.4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5998 2024-04-15 13:44:34.000000 MindsDB-24.4.3.0/setup.py
```

### Comparing `MindsDB-24.4.2.1/LICENSE` & `MindsDB-24.4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/MindsDB.egg-info/PKG-INFO` & `MindsDB-24.4.3.0/MindsDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 24.4.2.1
+Version: 24.4.3.0
 Summary: MindsDB's AI SQL Server enables developers to build AI tools that need access to real-time data to perform their tasks
 Home-page: https://github.com/mindsdb/mindsdb
 Download-URL: https://pypi.org/project/mindsdb/
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: ELv2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MindsDB-24.4.2.1/MindsDB.egg-info/SOURCES.txt` & `MindsDB-24.4.3.0/MindsDB.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -864,14 +864,18 @@
 mindsdb/integrations/handlers/merlion_handler/requirements.txt
 mindsdb/integrations/handlers/milvus_handler/__about__.py
 mindsdb/integrations/handlers/milvus_handler/__init__.py
 mindsdb/integrations/handlers/milvus_handler/icon.svg
 mindsdb/integrations/handlers/milvus_handler/milvus_handler.py
 mindsdb/integrations/handlers/milvus_handler/requirements.txt
 mindsdb/integrations/handlers/milvus_handler/tests/__init__.py
+mindsdb/integrations/handlers/mindsdb_inference/__about__.py
+mindsdb/integrations/handlers/mindsdb_inference/__init__.py
+mindsdb/integrations/handlers/mindsdb_inference/mindsdb_inference_handler.py
+mindsdb/integrations/handlers/mindsdb_inference/requirements.txt
 mindsdb/integrations/handlers/mlflow_handler/__about__.py
 mindsdb/integrations/handlers/mlflow_handler/__init__.py
 mindsdb/integrations/handlers/mlflow_handler/icon.svg
 mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
 mindsdb/integrations/handlers/mlflow_handler/requirements.txt
 mindsdb/integrations/handlers/monetdb_handler/__about__.py
 mindsdb/integrations/handlers/monetdb_handler/__init__.py
```

### Comparing `MindsDB-24.4.2.1/MindsDB.egg-info/requires.txt` & `MindsDB-24.4.3.0/MindsDB.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 psycopg2-binary
 alembic>=1.3.3
 redis<6.0.0,>=5.0.0
 walrus==0.9.3
 flask-compress>=1.0.0
 appdirs>=1.0.0
 mindsdb-sql~=0.12.0
+pydantic>=1.8.2
 mindsdb-evaluator<0.1.0,>=0.0.7
 checksumdir>=1.2.0
 duckdb==0.9.1
 requests>=2.30.0
 pydateinfer==0.3.0
 dataprep_ml==0.0.22
 dill==0.3.6
@@ -38,293 +39,291 @@
 msal
 langchain>=0.1.9
 langchain-core>=0.1.28
 langchain-community
 langchain-openai
 lark
 prometheus-client==0.20.0
-pydantic
 binance-connector
-pyarrow==11.0.0
 virtualenv
+pyarrow==11.0.0
 scylla-driver
-charset-normalizer
 pymupdf
 openpyxl
 python-magic>=0.4.27
+charset-normalizer
 mysql-connector-python
 certifi
 mysql-connector-python
-openai==1.6.1
 tiktoken>=0.3.0
+openai==1.6.1
 scylla-driver
 slack_sdk==3.21.3
 statsforecast==1.6.0
 nixtlats>=0.1.10
 tweepy
 
 [access]
-pyodbc
 sqlalchemy-access
+pyodbc
 
 [aerospike]
 aerospike~=13.0.0
 
 [all_extras]
-pytest-lazy-fixture~=0.6.3
-ollama>=0.1.7
-netifaces>=0.11.0
-grpcio-tools
 flake8==5.0.4
-pytest<8.0.0,>=7.3.0
-lightwood==23.12.4.0
-pytest-subtests
+responses
+coveralls
 pytest-cov
-openai==1.6.1
+pytest-lazy-fixture~=0.6.3
+watchfiles==0.19.0
+deptry==0.12.0
+docker>=5.0.3
 hierarchicalforecast
+grpcio-tools
 locust
-docker>=5.0.3
-pre-commit>=2.16.0
-isort==5.10.1
-watchfiles==0.19.0
+pytest<8.0.0,>=7.3.0
+openai==1.6.1
 wheel
-responses
+isort==5.10.1
+setuptools
+lightwood==23.12.4.0
 black==24.3.0
-twine
-deptry==0.12.0
 anthropic>=0.21.3
-coveralls
-setuptools
+twine
+pytest-subtests
+pre-commit>=2.16.0
+ollama>=0.1.7
+netifaces>=0.11.0
 
 [all_handlers_extras]
-pinecone-client
-trino~=0.313.0
-huggingface-hub
-hugging_py_face
-anthropic==0.18.1
-litellm
-google-analytics-admin
-salesforce-merlion<=1.3.1,>=1.2.0
-ray==2.0.1
-pymssql>=2.1.4
-pymupdf
-xgboost
-symbl
-catboost>=1.2
-plaid-python
-sqlalchemy-firebird<3.0.0,>=2.0.0
-openai==1.6.1
-nltk>=3.8.1
-torch
-influxdb3-python
-google-cloud-bigquery[pandas]
-google-auth-httplib2
-lightwood[extra]==24.3.3.1
-datasets
+pydruid
+IfxPy@ git+https://github.com/OpenInformix/IfxPy#subdirectory=IfxPy
+sib_api_v3_sdk
+torch==2.0.1+cpu
+binance-connector
+aerospike~=13.0.0
+lightfm==1.17
+stripe
+dask
+slack_sdk==3.21.3
+snowflake-sqlalchemy@ git+https://github.com/ea-rus/snowflake-sqlalchemy
+flaml<=1.2.3
+sqlalchemy-hana
+sqlalchemy-redshift
 python-magic>=0.4.27
-lance
+pyarrow~=10.0.1
 writerai~=1.1.0
-hubspot-api-client
-pyod>=1.1
-nltk
-pymilvus==2.3
-pyphoenix
-sqlalchemy-sqlany
-polars
-sqlalchemy-monetdb
-atlassian-python-api
-dotty-dict==1.3.1
-impyla
-aerospike~=13.0.0
+langchain-experimental
+google-generativeai>=0.1.0
+sqlalchemy-solr
 autogluon
-couchbase==4.0.2
-pymysql
-faunadb
-neuralforecast<1.7.0,>=1.6.0
-python-gitlab
-sqlanydb
-ingres_sa_dialect@ git+https://github.com/ActianCorp/ingres_sa_dialect
-tpot<=0.11.7
-tweepy
-pyhive
-evaluate
-sqlalchemy-informix
-statsforecast==1.6.0
-sqlalchemy-access
-pyarrow==11.0.0
-twilio
-litellm==1.23.2
-transformers<5.0.0,>=4.34.0
-mendeley
-youtube-transcript-api
-replicate
-databend-sqlalchemy
-stability-sdk
-lightwood[xai]==24.3.3.1
-qbosdk
-ckanapi
-google-cloud-aiplatform>=1.35.0
-sentence-transformers
-sqlalchemy-vertica-python
+elasticsearch-dbapi
+charset-normalizer
+openai==1.6.1
+scylla-driver
+paypalrestsdk
+atlassian-python-api
+pymonetdb
 ludwig[distributed]>=0.5.2
-clickhouse-sqlalchemy>=0.3.1
-tiktoken>=0.3.0
-ibm-db-sa
-praw
-elasticsearch
-sib_api_v3_sdk
-rocketchat_API
-ibm-db
-lightwood==24.3.3.1
-flaml<=1.2.3
-pysqream_sqlalchemy>=0.8
-pysurrealdb
-mediawikiapi
-pycaret[models]
+faunadb
+google-api-python-client
 newsapi-python
-phoenixdb
-pgvector
-chardet
-pyodbc==4.0.34
-openpyxl
-lightfm==1.17
+xgboost
 llama-hub==0.0.62
-google-cloud-spanner
-sqlalchemy-databricks
-google-api-python-client
-langchain-experimental
-mlflow
-google
-vertica-python
-pygithub
-pyarrow~=10.0.1
-scipy
-anthropic==0.3.5
-slack_sdk==3.21.3
-google-generativeai==0.3.1
+teradatasqlalchemy
+mediawikiapi
+anthropic==0.18.1
+trino~=0.313.0
+lance
+tensorflow
+phoenixdb
+xata
+tpot<=0.11.7
+pymilvus==2.3
 pysqream>=3.2.5
-ShopifyAPI
-jaydebeapi
-taospy
-libsql-experimental
-autokeras
-fdb
-pyignite
-sqlalchemy-redshift
-cohere==4.5.1
-certifi
-weaviate-client~=3.24.2
-torch==2.0.1+cpu
-requests_toolbelt
-snowflake-connector-python>=2.7.12
-binance-connector
-tiktoken~=0.4.0
-dask
-elasticsearch-dbapi
-joblib
+spacy
+tzlocal
+ray[tune]>=2.2.0
+elasticsearch
+sqlanydb
+crate[sqlalchemy]
 wikipedia==1.4.0
-auto-sklearn
-lancedb~=0.3.1
-sqlalchemy-solr
-tensorflow
+pygithub
+redshift_connector
+impyla
+snowflake-connector-python>=2.7.12
+nixtlats>=0.1.10
+requests_toolbelt
 openbb-core==1.0.1
-sqlalchemy_dremio
+lancedb~=0.3.1
 html2text
-sqlalchemy-spanner
-virtualenv
-rouge-score>=0.1.2
-crate[sqlalchemy]
-databricks-sql-connector
-paypalrestsdk
-redshift_connector
-type_infer==0.0.18
-monkeylearn==3.6.0
-spacy
-solace-pubsubplus
-IfxPy@ git+https://github.com/OpenInformix/IfxPy#subdirectory=IfxPy
-snowflake-sqlalchemy@ git+https://github.com/ea-rus/snowflake-sqlalchemy
-langfuse
-hdbcli
-bs4
-pillow
-teradatasqlalchemy
-pydruid
+openbb==4.0.1
+influxdb3-python
+vertica-python
 webzio==1.0.2
-overpy
-tzlocal
-mysql-connector-python
-ray[tune]>=2.2.0
-sqlalchemy-hana
-pymonetdb
+pymssql>=2.1.4
+ray==2.0.1
+stravalib
+certifi
+jaydebeapi
 oracledb==1.0.2
-eventbrite-python
-pyodbc
-nixtlats>=0.1.10
+pysurrealdb
+clickhouse-sqlalchemy>=0.3.1
+sentence-transformers
+litellm==1.35.0
+torch
+google-cloud-aiplatform>=1.35.0
+faiss-cpu
+langfuse
+weaviate-client~=3.24.2
+lightwood==24.3.3.1
+chardet
+praw
+databend-sqlalchemy
+couchbase==4.0.2
 notion-client
-openbb==4.0.1
-xata
-charset-normalizer
-teradatasql
-google-generativeai>=0.1.0
+sqlalchemy_dremio
+hdbcli
+sqlalchemy-monetdb
+sqlalchemy-firebird<3.0.0,>=2.0.0
+pgvector
+tweepy
+transformers<5.0.0,>=4.34.0
+nltk>=3.8.1
+ibm-db-sa
+pillow
+llama-index==0.9.23
+pyodbc==4.0.34
 pycaret
-stravalib
+virtualenv
+pymysql
+tiktoken>=0.3.0
+monkeylearn==3.6.0
+taospy
+auto-sklearn
+statsforecast==1.6.0
+symbl
+polars
+pyignite
+google-generativeai==0.3.1
+ShopifyAPI
+sqlalchemy-bigquery
+pymupdf
+bs4
+pycaret[models]
+mlflow
+pyhive
+evaluate
+rouge-score>=0.1.2
+libsql-experimental
+openpyxl
+ckanapi
+pinecone-client
+teradatasql
+dotty-dict==1.3.1
+qdrant-client
 chromadb~=0.4.8
+pyphoenix
+sqlalchemy-sqlany
+lightwood[xai]==24.3.3.1
+mendeley
+pyodbc
+google-auth-httplib2
+ingres_sa_dialect@ git+https://github.com/ActianCorp/ingres_sa_dialect
+tiktoken~=0.4.0
+datasets
 bs4==0.0.2
-llama-index==0.9.23
+pyarrow==11.0.0
+sqlalchemy-access
+plaid-python
+youtube-transcript-api
+pysqream_sqlalchemy>=0.8
+salesforce-merlion<=1.3.1,>=1.2.0
+google-cloud-spanner
+hubspot-api-client
+nltk
+google-cloud-bigquery[pandas]
+fdb
+scipy
+catboost>=1.2
+stability-sdk
+ibm-db
+mysql-connector-python
+sqlalchemy-spanner
+python-gitlab
+neuralforecast<1.7.0,>=1.6.0
+overpy
 pinotdb
-sqlalchemy-bigquery
-faiss-cpu
-stripe
-scylla-driver
-qdrant-client
+google-analytics-admin
+hugging_py_face
+sqlalchemy-informix
+twilio
+google
+anthropic==0.3.5
+lightwood[extra]==24.3.3.1
+pyod>=1.1
+huggingface-hub
+replicate
+rocketchat_API
+eventbrite-python
+type_infer==0.0.18
+sqlalchemy-databricks
+sqlalchemy-vertica-python
+joblib
+qbosdk
+solace-pubsubplus
+cohere==4.5.1
+autokeras
+databricks-sql-connector
 
 [altibase]
 jaydebeapi
 
 [anomaly_detection]
-pyod>=1.1
-catboost>=1.2
 joblib
+pyod>=1.1
 xgboost
+catboost>=1.2
 
 [anthropic]
 anthropic==0.18.1
 
 [anyscale_endpoints]
-openai==1.6.1
 tiktoken>=0.3.0
+openai==1.6.1
 
 [apache_doris]
 mysql-connector-python
 
 [aurora]
 mysql-connector-python
 
 [autogluon]
 autogluon
 type_infer==0.0.18
 
 [autokeras]
-autokeras
 tensorflow
+autokeras
 
 [autosklearn]
-type_infer==0.0.18
 auto-sklearn
+type_infer==0.0.18
 
 [bigquery]
-google-cloud-bigquery[pandas]
 sqlalchemy-bigquery
+google-cloud-bigquery[pandas]
 
 [binance]
 binance-connector
 
 [byom]
-pyarrow==11.0.0
 virtualenv
+pyarrow==11.0.0
 
 [cassandra]
 scylla-driver
 
 [chromadb]
 chromadb~=0.4.8
 
@@ -361,16 +360,16 @@
 [d0lt]
 pymysql
 
 [databend]
 databend-sqlalchemy
 
 [databricks]
-databricks-sql-connector
 sqlalchemy-databricks
+databricks-sql-connector
 
 [datastax]
 scylla-driver
 
 [db2]
 ibm-db-sa
 ibm-db
@@ -400,16 +399,16 @@
 [druid]
 pydruid
 
 [edgelessdb]
 mysql-connector-python
 
 [elasticsearch]
-elasticsearch-dbapi
 elasticsearch
+elasticsearch-dbapi
 
 [email]
 chardet
 bs4==0.0.2
 
 [empress]
 pyodbc
@@ -417,102 +416,102 @@
 [eventbrite]
 eventbrite-python
 
 [faunadb]
 faunadb
 
 [file]
-charset-normalizer
 pymupdf
 openpyxl
 python-magic>=0.4.27
+charset-normalizer
 
 [firebird]
 fdb
 sqlalchemy-firebird<3.0.0,>=2.0.0
 
 [flaml]
-flaml<=1.2.3
 type_infer==0.0.18
+flaml<=1.2.3
 
 [frappe]
 
 [github]
 pygithub
 
 [gitlab]
 python-gitlab
 
 [gmail]
 google-auth-httplib2
 google-api-python-client
 
 [google_analytics]
-google-analytics-admin
 google-api-python-client
+google-analytics-admin
 
 [google_books]
 google-auth-httplib2
 google-api-python-client
 
 [google_calendar]
 google-auth-httplib2
 google-api-python-client
 
 [google_content_shopping]
 google-auth-httplib2
 google-api-python-client
 
 [google_fit]
-tzlocal
 google
+tzlocal
 google-api-python-client
 
 [google_gemini]
 google-generativeai==0.3.1
 
 [google_search]
 google-auth-httplib2
 google-api-python-client
 
 [grpc]
 grpcio-tools
 
 [hana]
-sqlalchemy-hana
 hdbcli
+sqlalchemy-hana
 
 [hive]
 pyhive
 
 [hsqldb]
 pyodbc==4.0.34
 
 [hubspot]
 hubspot-api-client
 
 [huggingface]
-torch
-transformers<5.0.0,>=4.34.0
-huggingface-hub
-nltk
 datasets
+nltk
 evaluate
-
-[huggingface-cpu]
 transformers<5.0.0,>=4.34.0
-torch==2.0.1+cpu
+torch
 huggingface-hub
-nltk
+
+[huggingface-cpu]
 datasets
+nltk
 evaluate
+torch==2.0.1+cpu
+transformers<5.0.0,>=4.34.0
+huggingface-hub
 
 [huggingface_api]
-huggingface-hub
 hugging_py_face
+huggingface-hub
 
 [ignite]
 pyignite
 
 [impala]
 impyla
 
@@ -520,65 +519,66 @@
 influxdb3-python
 
 [informix]
 IfxPy@ git+https://github.com/OpenInformix/IfxPy#subdirectory=IfxPy
 sqlalchemy-informix
 
 [ingres]
-pyodbc
 ingres_sa_dialect@ git+https://github.com/ActianCorp/ingres_sa_dialect
+pyodbc
 
 [jira]
 atlassian-python-api
 
 [kinetica]
 
 [lancedb]
+lance
 pyarrow~=10.0.1
 lancedb~=0.3.1
-lance
 
 [langchain]
-openai==1.6.1
-langfuse
-litellm==1.23.2
-anthropic==0.3.5
 tiktoken>=0.3.0
-langchain-experimental
+litellm==1.35.0
+tiktoken~=0.4.0
+anthropic==0.3.5
 wikipedia==1.4.0
+openai==1.6.1
+langchain-experimental
+langfuse
 
 [langchain_embedding]
 openai==1.6.1
 tiktoken~=0.4.0
 
 [leonardoai]
 
 [libsql]
 libsql-experimental
 
 [lightfm]
 lightfm==1.17
 
 [lightwood]
-lightwood[extra]==24.3.3.1
-type_infer==0.0.18
 lightwood[xai]==24.3.3.1
+type_infer==0.0.18
+lightwood[extra]==24.3.3.1
 lightwood==24.3.3.1
 
 [lindorm]
 phoenixdb
 pyphoenix
 
 [litellm]
-litellm
+litellm==1.35.0
 
 [llama_index]
+llama-hub==0.0.62
 llama-index==0.9.23
 openai==1.6.1
-llama-hub==0.0.62
 
 [ludwig]
 ludwig[distributed]>=0.5.2
 dask
 ray==2.0.1
 
 [luma]
@@ -597,16 +597,16 @@
 [mediawiki]
 mediawikiapi
 
 [mendeley]
 mendeley
 
 [merlion]
-scipy
 salesforce-merlion<=1.3.1,>=1.2.0
+scipy
 
 [milvus]
 pymilvus==2.3
 
 [mlflow]
 mlflow
 
@@ -645,20 +645,20 @@
 [nuo_jdbc]
 jaydebeapi
 
 [oceanbase]
 mysql-connector-python
 
 [openai]
-openai==1.6.1
 tiktoken>=0.3.0
+openai==1.6.1
 
 [openbb]
-openbb==4.0.1
 openbb-core==1.0.1
+openbb==4.0.1
 
 [opengauss]
 
 [openstreetmap]
 overpy
 
 [oracle]
@@ -703,20 +703,20 @@
 
 [questdb]
 
 [quickbooks]
 qbosdk
 
 [rag]
-writerai~=1.1.0
 chromadb~=0.4.8
+sentence-transformers
 openai==1.6.1
-faiss-cpu
 html2text
-sentence-transformers
+faiss-cpu
+writerai~=1.1.0
 
 [reddit]
 praw
 
 [redshift]
 redshift_connector
 sqlalchemy-redshift
@@ -733,20 +733,20 @@
 [scylla]
 scylla-driver
 
 [sendinblue]
 sib_api_v3_sdk
 
 [sentence_transformers]
-writerai~=1.1.0
 chromadb~=0.4.8
+sentence-transformers
 openai==1.6.1
-faiss-cpu
 html2text
-sentence-transformers
+faiss-cpu
+writerai~=1.1.0
 
 [shopify]
 ShopifyAPI
 
 [singlestore]
 mysql-connector-python
 
@@ -767,20 +767,20 @@
 spacy
 
 [sqlany]
 sqlanydb
 sqlalchemy-sqlany
 
 [sqreamdb]
-pysqream>=3.2.5
 pysqream_sqlalchemy>=0.8
+pysqream>=3.2.5
 
 [stabilityai]
-pillow
 stability-sdk
+pillow
 
 [starrocks]
 mysql-connector-python
 
 [statsforecast]
 statsforecast==1.6.0
 
@@ -833,60 +833,60 @@
 [timescaledb]
 
 [tpot]
 tpot<=0.11.7
 type_infer==0.0.18
 
 [trino]
-trino~=0.313.0
 pyhive
+trino~=0.313.0
 
 [twelve_labs]
 requests_toolbelt
 
 [twilio]
 twilio
 
 [twitter]
 tweepy
 
 [vertex]
 google-cloud-aiplatform>=1.35.0
 
 [vertica]
-sqlalchemy-vertica-python
 vertica-python
+sqlalchemy-vertica-python
 
 [vitess]
 mysql-connector-python
 
 [weaviate]
 weaviate-client~=3.24.2
 
 [web]
 pymupdf
 bs4
 
 [webz]
-webzio==1.0.2
 dotty-dict==1.3.1
+webzio==1.0.2
 
 [whatsapp]
 twilio
 
 [writer]
-nltk>=3.8.1
+chromadb~=0.4.8
 sentence-transformers
+rouge-score>=0.1.2
 scipy
-writerai~=1.1.0
-chromadb~=0.4.8
 openai==1.6.1
-faiss-cpu
 html2text
-rouge-score>=0.1.2
+nltk>=3.8.1
+faiss-cpu
+writerai~=1.1.0
 
 [xata]
 xata
 
 [youtube]
 youtube-transcript-api
 google-api-python-client
```

### Comparing `MindsDB-24.4.2.1/PKG-INFO` & `MindsDB-24.4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 24.4.2.1
+Version: 24.4.3.0
 Summary: MindsDB's AI SQL Server enables developers to build AI tools that need access to real-time data to perform their tasks
 Home-page: https://github.com/mindsdb/mindsdb
 Download-URL: https://pypi.org/project/mindsdb/
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: ELv2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MindsDB-24.4.2.1/README.md` & `MindsDB-24.4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/__main__.py` & `MindsDB-24.4.3.0/mindsdb/__main__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/common/check_auth.py` & `MindsDB-24.4.3.0/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/command_executor.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/command_executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/controllers/session_controller.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/data_types/answer.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/data_types/answer.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/datahub/classes/tables_row.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datanodes/information_schema_datanode.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datanodes/information_schema_datanode.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
             "PROJECT",
             "DATABASE",
             "MODEL_NAME",
             "PARAMS",
             "IS_RUNNING",
             "LAST_ERROR",
         ],
-        "KNOWLEDGE_BASES": ["NAME", "PROJECT", "MODEL", "STORAGE"],
+        "KNOWLEDGE_BASES": ["NAME", "PROJECT", "MODEL", "STORAGE", "PARAMS"],
         "SKILLS": ["NAME", "PROJECT", "TYPE", "PARAMS"],
         "AGENTS": [
             "NAME",
             "PROJECT",
             "MODEL_NAME",
             "SKILLS",
             "PARAMS"
@@ -668,27 +668,28 @@
         # get the project id from the project name
         project_controller = ProjectController()
         project_id = project_controller.get(name=project_name).id
         kb_list = controller.list(project_id=project_id)
 
         columns = self.information_schema['KNOWLEDGE_BASES']
 
-        # columns: NAME, PROJECT, MODEL, STORAGE
+        # columns: NAME, PROJECT, MODEL, STORAGE, PARAMS
         data = []
 
         for kb in kb_list:
             embedding_model = kb.embedding_model
             vector_database = kb.vector_database
             vector_database_name = '' if vector_database is None else vector_database.name
 
             data.append((
                 kb.name,
                 project_name,
                 embedding_model.name if embedding_model is not None else None,
-                vector_database_name + '.' + kb.vector_database_table
+                vector_database_name + '.' + kb.vector_database_table,
+                to_json(kb.params),
             ))
 
         return pd.DataFrame(data, columns=columns)
 
     def _get_skills(self, query: ASTNode = None):
         skills_controller = SkillsController()
         project_name = None
```

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datanodes/integration_datanode.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datanodes/integration_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/datahub/datanodes/project_datanode.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/exceptions.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/result_set.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/result_set.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/sql_query.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/sql_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/__init__.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/apply_predictor_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/apply_predictor_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/delete_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/delete_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/fetch_dataframe.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/fetch_dataframe.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/insert_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/insert_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/join_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/join_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/map_reduce_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/map_reduce_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/multiple_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/multiple_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/prepare_steps.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/prepare_steps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/project_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/project_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/sql_steps.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/sql_steps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/subselect_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/subselect_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/union_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/union_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/sql_query/steps/update_step.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/sql_query/steps/update_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/utilities/functions.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/executor/utilities/sql.py` & `MindsDB-24.4.3.0/mindsdb/api/executor/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/gui.py` & `MindsDB-24.4.3.0/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-24.4.3.0/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/initialize.py` & `MindsDB-24.4.3.0/mindsdb/api/http/initialize.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/agents.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/agents.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/auth.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/chatbots.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/chatbots.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/config.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/databases.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/default.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/file.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/models.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/models.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/projects.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/skills.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/skills.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/sql.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/tab.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/tree.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/util.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/namespaces/views.py` & `MindsDB-24.4.3.0/mindsdb/api/http/namespaces/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/start.py` & `MindsDB-24.4.3.0/mindsdb/api/http/start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/http/utils.py` & `MindsDB-24.4.3.0/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/classes/responder.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/classes/scram.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/classes/session.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/delete.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/find.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/insert.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/server.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-24.4.3.0/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/executor/mysql_executor.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/executor/mysql_executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-24.4.3.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-24.4.3.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/aerospike_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/aerospike_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aerospike_handler/tests/test_aerospike_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aerospike_handler/tests/test_aerospike_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/anomaly_detection_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/anomaly_detection_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/anomaly_detection_handler/utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/anomaly_detection_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/anthropic_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/anthropic_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/anthropic_handler/anthropic_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/anthropic_handler/anthropic_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/anyscale_endpoints_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/anyscale_endpoints_handler/anyscale_endpoints_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/anyscale_endpoints_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/anyscale_endpoints_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/apache_doris_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/apache_doris_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/aqicn.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/aqicn.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/aqicn_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/aqicn_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aqicn_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aqicn_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/autogluon_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/autogluon_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autogluon_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autogluon_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autokeras_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autokeras_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/autosklearn_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/autosklearn_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/chromadb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/chromadb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/settings.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/chromadb_handler/tests/test_chromadb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/chromadb_handler/tests/test_chromadb_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,36 +2,26 @@
 import importlib
 import shutil
 import tempfile
 from unittest.mock import patch
 
 import pandas as pd
 import pytest
-from mindsdb_sql import parse_sql
 
 from tests.unit.executor_test_base import BaseExecutorTest
 
 try:
     importlib.import_module("chromadb")
     CHROMA_DB_INSTALLED = True
 except ImportError:
     CHROMA_DB_INSTALLED = False
 
 
 @pytest.mark.skipif(not CHROMA_DB_INSTALLED, reason="chroma_db is not installed")
 class TestChromaDBHandler(BaseExecutorTest):
-    def run_sql(self, sql):
-        ret = self.command_executor.execute_command(parse_sql(sql, dialect="mindsdb"))
-
-        assert ret.error_code is None
-        if ret.data is not None:
-            columns = [
-                col.alias if col.alias is not None else col.name for col in ret.columns
-            ]
-            return pd.DataFrame(ret.data, columns=columns)
 
     @pytest.fixture(autouse=True, scope="function")
     def setup_method(self):
         super().setup_method()
         # create a chroma database under the tmp directory
         tmp_directory = tempfile.mkdtemp()
         self.run_sql(
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/clipdrop.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/clipdrop_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/clipdrop_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/clipdrop_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cohere_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cohere_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/cohere_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/cohere_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/coinbase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/coinbase_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/coinbase_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/coinbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/confluence_handler/tests/test_confluence_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/confluence_handler/tests/test_confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/discord_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/discord_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/discord_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/discord_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/discord_handler/tests/test_discord.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/discord_handler/tests/test_discord.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/dockerhub.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dockerhub_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dockerhub_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/documentdb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/documentdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/documentdb_handler/documentdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/documentdb_handler/documentdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/documentdb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/documentdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dummy_data_handler/dummy_data_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dummy_data_handler/dummy_data_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/email_client.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/email_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/email_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/email_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/email_ingestor.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/email_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/email_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/email_handler/settings.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/email_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventbrite_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventbrite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/faunadb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/faunadb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/faunadb_handler/tests/test_faunadb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/faunadb_handler/tests/test_faunadb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/tests/data/test.txt` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/tests/data/test.txt`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/file_handler/tests/test_file_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/file_handler/tests/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/flaml_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/flaml_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/flaml_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/flaml_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/frappe_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/frappe_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/github_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/github_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/gmail_handler/utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/gmail_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_analytics_handler/tests/test_google_analytics_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_analytics_handler/tests/test_google_analytics_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_fit_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_fit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_gemini_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_gemini_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_gemini_handler/google_gemini_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_gemini_handler/google_gemini_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/hubspot_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/hubspot_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/hubspot_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/hubspot_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_api_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_api_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/finetune.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/finetune.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/huggingface_handler/settings.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/huggingface_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/instatus_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/instatus_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/instatus_handler/instatus_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/instatus_handler/instatus_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/intercom_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/intercom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/intercom_handler/intercom_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/intercom_handler/intercom_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/jira_handler/jira_table.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/jira_handler/jira_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/kinetica_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/kinetica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/kinetica_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/kinetica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/kinetica_handler/kinetica_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/kinetica_handler/kinetica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/lancedb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/lancedb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lancedb_handler/tests/test_lancedb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lancedb_handler/tests/test_lancedb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_embedding_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_embedding_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_embedding_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_embedding_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_embedding_handler/langchain_embedding_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_embedding_handler/langchain_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/constants.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,12 +83,12 @@
     "duckdb-nsql",
     "notus"
 }
 DEFAULT_ASSISTANT_COLUMN = 'answer'
 DEFAULT_AGENT_TIMEOUT_SECONDS = 300
 # These should require no additional arguments.
 DEFAULT_AGENT_TOOLS = []  
-DEFAULT_AGENT_TYPE = AgentType.CONVERSATIONAL_REACT_DESCRIPTION
+DEFAULT_AGENT_TYPE = AgentType.OPENAI_FUNCTIONS
 DEFAULT_MAX_ITERATIONS = 10
 DEFAULT_MAX_TOKENS = 2048
 DEFAULT_MODEL_NAME = 'gpt-4-0125-preview'
 DEFAULT_USER_COLUMN = 'question'
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,21 +23,22 @@
     DEFAULT_MODEL_NAME,
     OLLAMA_CHAT_MODELS,
     SUPPORTED_PROVIDERS,
     DEFAULT_USER_COLUMN,
     DEFAULT_ASSISTANT_COLUMN
 )
 from mindsdb.integrations.handlers.langchain_handler.log_callback_handler import LogCallbackHandler
-from mindsdb.integrations.handlers.langchain_handler.mindsdb_database_agent import MindsDBSQL
+from mindsdb.integrations.utilities.rag.settings import DEFAULT_RAG_PROMPT_TEMPLATE
 from mindsdb.integrations.handlers.langchain_handler.tools import setup_tools
 from mindsdb.integrations.handlers.openai_handler.constants import CHAT_MODELS as OPEN_AI_CHAT_MODELS
 from mindsdb.integrations.libs.base import BaseMLEngine
 from mindsdb.integrations.libs.llm.utils import get_llm_config
 from mindsdb.integrations.utilities.handler_utils import get_api_key
 from mindsdb.interfaces.storage.model_fs import HandlerStorage, ModelStorage
+from mindsdb.integrations.handlers.langchain_embedding_handler.langchain_embedding_handler import construct_model_from_args
 from mindsdb.utilities import log
 from mindsdb.utilities.context_executor import ContextThreadPoolExecutor
 
 _PARSING_ERROR_PREFIX = 'An output parsing error occured'
 
 logger = log.getLogger(__name__)
 
@@ -72,35 +73,43 @@
         self.generative = True
         self.default_agent_tools = DEFAULT_AGENT_TOOLS
         self.log_callback_handler = log_callback_handler
         self.langfuse_callback_handler = langfuse_callback_handler
         if self.log_callback_handler is None:
             self.log_callback_handler = LogCallbackHandler(logger)
 
-    def _get_provider(self, args: Dict) -> str:
+    def _get_llm_provider(self, args: Dict) -> str:
         if 'provider' in args:
             return args['provider']
         if args['model_name'] in ANTHROPIC_CHAT_MODELS:
             return 'anthropic'
         if args['model_name'] in OPEN_AI_CHAT_MODELS:
             return 'openai'
         if args['model_name'] in OLLAMA_CHAT_MODELS:
             return 'ollama'
         raise ValueError(f"Invalid model name. Please define provider")
 
+    def _get_embedding_model_provider(self, args: Dict) -> str:
+        if 'embedding_model_provider' in args:
+            return args['embedding_model_provider']
+        if 'embedding_model_provider' not in args:
+            logger.warning('No embedding model provider specified. trying to use llm provider.')
+            return args.get('embedding_model_provider', self._get_llm_provider(args))
+        raise ValueError(f"Invalid model name. Please define provider")
+
     def _get_chat_model_params(self, args: Dict, pred_args: Dict) -> Dict:
         model_config = args.copy()
         # Override with prediction args.
         model_config.update(pred_args)
         # Include API keys.
         model_config['api_keys'] = {
             p: get_api_key(p, args, self.engine_storage, strict=False) for p in SUPPORTED_PROVIDERS
         }
-        llm_config = get_llm_config(args.get('provider', self._get_provider(args)), model_config)
-        config_dict = llm_config.model_dump()
+        llm_config = get_llm_config(args.get('provider', self._get_llm_provider(args)), model_config)
+        config_dict = llm_config.dict()
         config_dict = {k: v for k, v in config_dict.items() if v is not None}
         return config_dict
 
     def _get_agent_callbacks(self, args: Dict) -> List:
         all_callbacks = [self.log_callback_handler]
         are_langfuse_args_present = 'langfuse_public_key' in args and 'langfuse_secret_key' in args and 'langfuse_host' in args
         if self.langfuse_callback_handler is None and are_langfuse_args_present:
@@ -127,14 +136,17 @@
             return ChatAnyscale(**model_kwargs)
         if args['provider'] == 'litellm':
             return ChatLiteLLM(**model_kwargs)
         if args['provider'] == 'ollama':
             return ChatOllama(**model_kwargs)
         raise ValueError(f'Unknown provider: {args["provider"]}')
 
+    def _create_embeddings_model(self, args: Dict):
+        return construct_model_from_args(args)
+
     def _handle_parsing_errors(self, error: Exception) -> str:
         response = str(error)
         if not response.startswith(_PARSING_ERROR_PREFIX):
             return f'Agent failed with error:\n{str(error)}...'
         else:
             # As a somewhat dirty workaround, we accept the output formatted incorrectly and use it as a response.
             #
@@ -148,51 +160,69 @@
 
     def create(self, target: str, args: Dict = None, **kwargs):
         self.default_agent_tools = args.get('tools', self.default_agent_tools)
 
         args = args['using']
         args['target'] = target
         args['model_name'] = args.get('model_name', DEFAULT_MODEL_NAME)
-        args['provider'] = args.get('provider', self._get_provider(args))
+        args['provider'] = args.get('provider', self._get_llm_provider(args))
+        args['embedding_model_provider'] = args.get('embedding_model', self._get_embedding_model_provider(args))
+        if args.get('mode') == 'retrieval':
+            # use default prompt template for retrieval i.e. RAG if not provided
+            if "prompt_template" not in args:
+                args["prompt_template"] = DEFAULT_RAG_PROMPT_TEMPLATE
+
         self.model_storage.json_set('args', args)
 
     @staticmethod
     def create_validation(_, args: Dict=None, **kwargs):
         if 'using' not in args:
             raise Exception("LangChain engine requires a USING clause! Refer to its documentation for more details.")
         else:
             args = args['using']
         if 'prompt_template' not in args:
-            raise ValueError('Please provide a `prompt_template` for this engine.')
+            if not args.get('mode') == 'retrieval':
+                raise ValueError('Please provide a `prompt_template` for this engine.')
 
     def predict(self, df: pd.DataFrame, args: Dict=None) -> pd.DataFrame:
         """
         Dispatch is performed depending on the underlying model type. Currently, only the default text completion
         is supported.
         """
         pred_args = args['predict_params'] if args else {}
         args = self.model_storage.json_get('args')
         if 'prompt_template' not in args and 'prompt_template' not in pred_args:
             raise ValueError(f"This model expects a `prompt_template`, please provide one.")
         # Back compatibility for old models
-        args['provider'] = args.get('provider', self._get_provider(args))
+        args['provider'] = args.get('provider', self._get_llm_provider(args))
+        args['embedding_model_provider'] = args.get('embedding_model', self._get_embedding_model_provider(args))
 
         df = df.reset_index(drop=True)
         agent = self.create_agent(df, args, pred_args)
         # Use last message as prompt, remove other questions.
         user_column = args.get('user_column', DEFAULT_USER_COLUMN)
         df.iloc[:-1, df.columns.get_loc(user_column)] = None
         return self.run_agent(df, agent, args, pred_args)
 
     def create_agent(self, df: pd.DataFrame, args: Dict=None, pred_args: Dict=None) -> AgentExecutor:
         pred_args = pred_args if pred_args else {}
 
         # Set up tools.
         model_kwargs = self._get_chat_model_params(args, pred_args)
         llm = self._create_chat_model(args, pred_args)
+
+        # Set up embeddings model if needed.
+        if args.get('mode') == 'retrieval':
+            # get args for embeddings model
+            embeddings_args = args.pop('embedding_model_args', {})
+            # create embeddings model
+            pred_args['embeddings_model'] = self._create_embeddings_model(embeddings_args)
+            pred_args['llm'] = llm
+            pred_args['mindsdb_path'] = self.engine_storage.folder_get
+
         tools = setup_tools(llm,
                             model_kwargs,
                             pred_args,
                             self.default_agent_tools)
 
         # Prefer prediction prompt template over original if provided.
         prompt_template = pred_args.get('prompt_template', args['prompt_template'])
@@ -224,15 +254,15 @@
             # Calls the agent’s LLM Chain one final time to generate a final answer based on the previous steps
             early_stopping_method='generate',
             handle_parsing_errors=self._handle_parsing_errors,
             # Timeout per agent invocation.
             max_execution_time=pred_args.get('timeout_seconds', args.get('timeout_seconds', DEFAULT_AGENT_TIMEOUT_SECONDS)),
             max_iterations=pred_args.get('max_iterations', args.get('max_iterations', DEFAULT_MAX_ITERATIONS)),
             memory=memory,
-            verbose=pred_args.get('verbose', args.get('verbose', False))
+            verbose=pred_args.get('verbose', args.get('verbose', True))
         )
         return agent_executor
 
     def run_agent(self, df: pd.DataFrame, agent: AgentExecutor, args: Dict, pred_args: Dict) -> str:
         # Prefer prediction time prompt template, if available.
         base_template = pred_args.get('prompt_template', args['prompt_template'])
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/log_callback_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/log_callback_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class LogCallbackHandler(BaseCallbackHandler):
     '''Langchain callback handler that logs agent and chain executions.'''
 
     def __init__(self, logger: logging.Logger):
         logger.setLevel('DEBUG')
         self.logger = logger
+        self._num_running_chains = 0
 
     def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> Any:
         '''Run when LLM starts running.'''
         self.logger.debug(f'LLM started with prompts:')
         for prompt in prompts:
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/langchain_handler/tools.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/langchain_handler/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import tiktoken
 
-from typing import Callable
+from typing import Callable, Dict
+
+from langchain.tools.retriever import create_retriever_tool
 from mindsdb_sql import parse_sql, Insert
 
 from langchain.prompts import PromptTemplate
 from langchain.agents import load_tools, Tool
 
 from langchain_experimental.utilities import PythonREPL
-from langchain_community.tools import WikipediaQueryRun
-from langchain_community.utilities import GoogleSerperAPIWrapper, WikipediaAPIWrapper
+from langchain_community.utilities import GoogleSerperAPIWrapper
 
 from langchain.chains.llm import LLMChain
 from langchain.text_splitter import CharacterTextSplitter
 from langchain.chains.combine_documents.stuff import StuffDocumentsChain
 from langchain.chains import ReduceDocumentsChain, MapReduceDocumentsChain
 
-from mindsdb.interfaces.skills.skill_tool import skill_tool
-
+from mindsdb.integrations.utilities.rag.rag_pipeline_builder import RAG
+from mindsdb.integrations.utilities.rag.settings import RAGPipelineModel
+from mindsdb.interfaces.skills.skill_tool import skill_tool, SkillType
 
 # Individual tools
 # Note: all tools are defined in a closure to pass required args (apart from LLM input) through it, as custom tools don't allow custom field assignment.  # noqa
 def get_exec_call_tool(llm, executor, model_kwargs) -> Callable:
     def mdb_exec_call_tool(query: str) -> str:
         try:
             ast_query = parse_sql(query.strip('`'), dialect='mindsdb')
@@ -141,42 +143,92 @@
         else:
             raise ValueError(f"Unsupported tool: {tool}")
     
     all_standard_tools += load_tools(langchain_tools)
     return all_standard_tools
 
 
-def langchain_tool_from_skill(skill):
+def _get_rag_params(pred_args: Dict) -> Dict:
+    model_config = pred_args.copy()
+
+    supported_rag_params = RAGPipelineModel.get_field_names()
+
+    rag_params = {k: v for k, v in model_config.items() if k in supported_rag_params}
+
+    return rag_params
+
+
+def _build_retrieval_tool(tool: dict, pred_args: dict):
+    """
+    Builds a retrieval tool i.e RAG
+    """
+    # build RAG config
+
+    tools_config = tool['config']
+
+    mindsdb_path = pred_args['mindsdb_path']
+
+    # we update the config with the pred_args to allow for custom config
+    tools_config.update(pred_args)
+
+    rag_params = _get_rag_params(tools_config)
+
+    if 'vector_store_config' not in rag_params:
+
+        rag_params['vector_store_config'] = {'persist_directory': mindsdb_path('persisted_chroma')}
+
+    rag_config = RAGPipelineModel(**rag_params)
+
+    # build retriever
+    rag_pipeline = RAG(rag_config)
+
+    # create RAG tool
+    return Tool(
+        func=rag_pipeline,
+        name=tool['name'],
+        description=tool['description']
+    )
+
+def langchain_tool_from_skill(skill, pred_args):
     # Makes Langchain compatible tools from a skill
     tool = skill_tool.get_tool_from_skill(skill)
 
+    if tool['type'] == SkillType.RETRIEVAL.value:
+
+        return _build_retrieval_tool(tool, pred_args)
+
     return Tool(
         name=tool['name'],
         func=tool['func'],
-        description=tool['description']
+        description=tool['description'],
+        return_direct=True
     )
 
+def get_skills(pred_args):
+    return pred_args.get('skills', [])
+
 # Collector
 def setup_tools(llm, model_kwargs, pred_args, default_agent_tools):
+
     toolkit = pred_args['tools'] if pred_args.get('tools') is not None else default_agent_tools
 
     standard_tools = []
     function_tools = []
 
     for tool in toolkit:
         if isinstance(tool, str):
             standard_tools.append(tool)
         else:
             # user defined custom functions
             function_tools.append(tool)
 
     tools = []
-    skills = pred_args.get('skills', [])
+    skills = get_skills(pred_args)
     for skill in skills:
-        tools.append(langchain_tool_from_skill(skill))
+        tools.append(langchain_tool_from_skill(skill, pred_args))
 
     if len(tools) == 0:
         tools = _setup_standard_tools(standard_tools, llm, model_kwargs)
 
     if model_kwargs.get('serper_api_key', False):
         search = GoogleSerperAPIWrapper(serper_api_key=model_kwargs.pop('serper_api_key'))
         tools.append(Tool(
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/leonardoai_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/leonardoai_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/leonardoai_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/leonardoai_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/leonardoai_handler/leonardo_ai_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/leonardoai_handler/leonardo_ai_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/libsql_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/libsql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/libsql_handler/tests/test_libsql_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/libsql_handler/tests/test_libsql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/api.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/lightdash_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightdash_handler/lightdash_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/helpers.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/functions.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lightwood_handler/utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/lindorm_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/lindorm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/lindorm_handler/tests/test_lindorm_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/lindorm_handler/tests/test_lindorm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/litellm_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/litellm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/litellm_handler/settings.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/litellm_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/config.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/github_loader_helper.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/github_loader_helper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/luma.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/luma.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/luma_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/luma_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/luma_handler/luma_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/luma_handler/luma_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/milvus_handler/milvus_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/milvus_handler/milvus_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mlflow_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mlflow_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/tests/test_mongodb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/tests/test_mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/monkeylearn_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/monkeylearn_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/ms_graph_api_teams_client.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/ms_graph_api_teams_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ms_teams_handler/settings.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ms_teams_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/notion_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/notion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/notion_table.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/notion_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/notion_handler/tests/test_notion_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/notion_handler/tests/test_notion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/api.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/npm_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/npm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/npm_handler/npm_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/npm_handler/npm_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ollama_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ollama_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ollama_handler/ollama_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ollama_handler/ollama_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/constants.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/constants.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -137,21 +137,14 @@
         return num_tokens
     else:
         raise NotImplementedError(
             f"""_count_tokens() is not presently implemented for model {model_name}."""
         )
 
 
-def get_available_models(api_key: str, base_url: str) -> List[str]:
+def get_available_models(api_key: str, api_base: str) -> List[str]:
     """
-    Returns a list of all available OpenAI models for the given API key.
-
-    Args:
-        api_key (str): The API key used for authenticating with the OpenAI API. 
-        base_url (str): The base URL of the OpenAI API.
-
-    Returns:
-        List[str]: A list of string identifiers, each representing a model that is available with the provided OpenAI key.
+    Returns a list of available openai models for the given API key.
     """
-    res = OpenAI(api_key=api_key, base_url=base_url).models.list()
+    res = OpenAI(api_key=api_key, base_url=api_base).models.list()
 
     return [models.id for models in res.data]
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,17 @@
             'embedding',
         ]
         self.rate_limit = 60  # requests per minute
         self.max_batch_size = 20
         self.default_max_tokens = 100
         self.chat_completion_models = CHAT_MODELS
         self.supported_ft_models = FINETUNING_MODELS # base models compatible with finetuning
+        # For now this are only used for handlers that inherits OpenAIHandler and don't need to override base methods
+        self.api_key_name = getattr(self, 'api_key_name', self.name)
+        self.api_base = getattr(self, 'api_base', OPENAI_API_BASE)
 
     def create_engine(self, connection_args):
         '''check api key if provided
         '''
         connection_args = {k.lower(): v for k, v in connection_args.items()}
         api_key = connection_args.get('openai_api_key')
         if api_key is not None:
@@ -170,17 +173,17 @@
         client = OpenAIHandler._get_client(api_key=api_key, base_url=api_base, org=org)
         OpenAIHandler._check_client_connection(client)
 
     def create(self, target, args=None, **kwargs):
         args = args['using']
         args['target'] = target
         try:
-            api_key = get_api_key(self.name, args, self.engine_storage)
+            api_key = get_api_key(self.api_key_name, args, self.engine_storage)
             connection_args = self.engine_storage.get_connection_args()
-            api_base = connection_args.get('api_base') or args.get('api_base') or os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE)
+            api_base = connection_args.get('api_base') or self.api_base or args.get('api_base') or os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE)
             available_models = get_available_models(api_key, api_base)
 
             if not args.get('mode'):
                 args['mode'] = self.default_mode
             elif args['mode'] not in self.supported_modes:
                 raise Exception(
                     f"Invalid operation mode. Please use one of {self.supported_modes}"
@@ -201,15 +204,17 @@
         If there is a prompt template, we use it. Otherwise, we use the concatenation of `context_column` (optional) and `question_column` to ask for a completion.
         """  # noqa
         # TODO: support for edits, embeddings and moderation
 
         pred_args = args['predict_params'] if args else {}
         args = self.model_storage.json_get('args')
         connection_args = self.engine_storage.get_connection_args()
+
         args['api_base'] = (pred_args.get('api_base') or
+                            self.api_base or
                             connection_args.get('api_base') or
                             args.get('api_base') or
                             os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE))
         if pred_args.get('api_organization'):
             args['api_organization'] = pred_args['api_organization']
         df = df.reset_index(drop=True)
 
@@ -381,15 +386,15 @@
                     df[[args['question_column']]].isna().all(axis=1).values
                 )[0]
                 prompts = list(df[args['question_column']].apply(lambda x: str(x)))
 
         # remove prompts without signal from completion queue
         prompts = [j for i, j in enumerate(prompts) if i not in empty_prompt_ids]
 
-        api_key = get_api_key(self.name, args, self.engine_storage)
+        api_key = get_api_key(self.api_key_name, args, self.engine_storage)
         api_args = {
             k: v for k, v in api_args.items() if v is not None
         }  # filter out non-specified api args
         completion = self._completion(model_name, prompts, api_key, api_args, args, df)
 
         # add null completion for empty prompts
         for i in sorted(empty_prompt_ids):
@@ -648,15 +653,15 @@
 
         return completion
 
     def describe(self, attribute: Optional[str] = None) -> pd.DataFrame:
         # TODO: Update to use update() artifacts
 
         args = self.model_storage.json_get('args')
-        api_key = get_api_key(self.name, args, self.engine_storage)
+        api_key = get_api_key(self.api_key_name, args, self.engine_storage)
         if attribute == 'args':
             return pd.DataFrame(args.items(), columns=['key', 'value'])
         elif attribute == 'metadata':
             model_name = args.get('model_name', self.default_model)
             try:
                 client= self._get_client(
                     api_key=api_key,
@@ -687,15 +692,15 @@
         Caveats:
           - As base fine-tuning models, OpenAI only supports the original GPT ones: `ada`, `babbage`, `curie`, `davinci`. This means if you fine-tune successively more than once, any fine-tuning other than the most recent one is lost.
           - A bunch of helper methods exist to be overridden in other handlers that follow the OpenAI API, e.g. Anyscale
         """  # noqa
 
         args = args if args else {}
 
-        api_key = get_api_key(self.name, args, self.engine_storage)
+        api_key = get_api_key(self.api_key_name, args, self.engine_storage)
 
         using_args = args.pop('using') if 'using' in args else {}
         
         api_base = using_args.get('api_base', os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE))
         org = using_args.get('api_organization')
         client = self._get_client(api_key=api_key, base_url=api_base, org=org)
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/openbb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/openbb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openbb_handler/openbb_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openbb_handler/openbb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/openstreetmap_handler/tests/test_openstreetmap_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/test_openstreetmap_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/palm_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/palm_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/palm_handler/palm_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/palm_handler/palm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pgvector_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pgvector_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pgvector_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pgvector_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pgvector_handler/pgvector_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pgvector_handler/pgvector_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinecone_handler/pinecone_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinecone_handler/pinecone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pirateweather_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pirateweather_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pirateweather_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pirateweather_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pirateweather_handler/pirateweather_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pirateweather_handler/pirateweather_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/popularity_recommender_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/popularity_recommender_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/postgres_handler/tests/test_postgres_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/postgres_handler/tests/test_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/pycaret_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/pycaret_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pycaret_handler/test/test_pycaret.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pycaret_handler/test/test_pycaret.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/api.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/pypi_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/pypi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/pypi_handler/pypi_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/pypi_handler/pypi_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/qdrant_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/qdrant_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/qdrant_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/qdrant_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/qdrant_handler/qdrant_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/qdrant_handler/qdrant_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/ingest.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/ingest.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/rag.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/rag.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/rag_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/rag_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rag_handler/settings.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rag_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ray_serve_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/assets/Arjuna.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/assets/Arjuna.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/assets/groot.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/assets/groot.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/assets/warrior.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/assets/warrior.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/replicate_handler/replicate_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/replicate_handler/replicate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/rockset_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/rockset_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/rockset_handler/tests/test_rockset_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test_rockset_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/api.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sentence_transformers_handler/sentence_transformers_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sentence_transformers_handler/sentence_transformers_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_api.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/tests/test_sharepoint_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/tests/test_sharepoint_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sharepoint_handler/utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sharepoint_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/solace_handler/solace_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/solace_handler/solace_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/spacy_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/spacy_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/spacy_handler/spacy_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/spacy_handler/spacy_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/stabilityai.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/stabilityai_handler/stabilityai_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/strapi_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/strapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/strapi_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/strapi_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/strapi_handler/tests/test_strapi_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/strapi_handler/tests/test_strapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/symbl_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/symbl_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/symbl_handler/symbl_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/symbl_handler/symbl_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/timegpt_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/timegpt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/timegpt_handler/timegpt_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/timegpt_handler/timegpt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tpot_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tpot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tpot_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tpot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_api.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_table.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/settings.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_api_client.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_api_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/twilio_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/twilio_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/twilio_handler/twilio_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/twilio_handler/twilio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/ms_graph_api_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/ms_graph_api_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_service_account_oauth_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_service_account_oauth_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_user_oauth_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_user_oauth_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/ms_graph_api_auth_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/ms_graph_api_auth_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/base_query_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/base_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/delete_query_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/delete_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/query_utilities/update_query_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/query_utilities/update_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/utilities/validation_utilities/parameter_validation_utilities.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/utilities/validation_utilities/parameter_validation_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/icon.png` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/vertex_client.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/vertex_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertex_handler/vertex_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertex_handler/vertex_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/weaviate_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/weaviate_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/weaviate_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/weaviate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/weaviate_handler/weaviate_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/weaviate_handler/weaviate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/tests/example_data.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/tests/example_data.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/tests/test_helpers.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/web_handler/web_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/web_handler/web_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/webz_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/webz_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/webz_handler/webz_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/webz_handler/webz_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/whatsapp_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/whatsapp_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/whatsapp_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/whatsapp_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/whatsapp_handler/whatsapp_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/whatsapp_handler/whatsapp_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/evaluate.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/evaluate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/settings.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/writer_handler/writer_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/xata_handler/xata_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/xata_handler/xata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/icon.svg` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_tables.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-24.4.3.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/api_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/base.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/llm/config.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/llm/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/llm/utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/llm/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/__init__.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/create_engine_process.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/create_engine_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/describe_process.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/describe_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/handlers_cacher.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/handlers_cacher.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/learn_process.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/learn_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/predict_process.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/predict_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/update_engine_process.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/update_engine_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/ml_handler_process/update_process.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/ml_handler_process/update_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/process_cache.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/process_cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/realtime_chat_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/realtime_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/response.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/libs/vectordatabase_handler.py` & `MindsDB-24.4.3.0/mindsdb/integrations/libs/vectordatabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/datasets/dataset.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/datasets/question_answering/fda_style_qa.csv` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/datasets/question_answering/fda_style_qa.csv`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/datasets/question_answering/squad_v2_val_100_sample.csv` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/datasets/question_answering/squad_v2_val_100_sample.csv`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/handler_utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/handler_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/install.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/loaders/vector_store_loader/vector_store_loader.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/loaders/vector_store_loader/vector_store_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 logger = log.getLogger(__name__)
 
 
 class VectorStoreLoader(BaseModel):
     embeddings_model: Embeddings
     vector_store: VectorStore = None
-    config: dict = None
+    config: VectorStoreConfig = None
 
     class Config:
         arbitrary_types_allowed = True
         extra = "forbid"
         validate_assignment = True
 
     def load(self) -> VectorStore:
@@ -36,22 +36,20 @@
         """
         self.vector_store = VectorStoreFactory.create(self.embeddings_model, self.config)
         return self.vector_store
 
 
 class VectorStoreFactory:
     @staticmethod
-    def create(embeddings_model: Embeddings, config: dict):
+    def create(embeddings_model: Embeddings, config: VectorStoreConfig):
 
-        settings = VectorStoreConfig(**config)
-
-        if settings.vector_store_type == VectorStoreType.CHROMA:
-            return VectorStoreFactory._load_chromadb_store(embeddings_model, settings)
-        elif settings.vector_store_type == VectorStoreType.PGVECTOR:
-            return VectorStoreFactory._load_pgvector_store(embeddings_model, settings)
+        if config.vector_store_type == VectorStoreType.CHROMA:
+            return VectorStoreFactory._load_chromadb_store(embeddings_model, config)
+        elif config.vector_store_type == VectorStoreType.PGVECTOR:
+            return VectorStoreFactory._load_pgvector_store(embeddings_model, config)
         else:
             raise ValueError(f"Invalid vector store type, must be one either {VectorStoreType.__members__.keys()}")
 
     @staticmethod
     def _load_chromadb_store(embeddings_model: Embeddings, settings) -> Chroma:
         return Chroma(
             persist_directory=settings.persist_directory,
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/pipelines/rag.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/pipelines/rag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.runnables import RunnableParallel, RunnablePassthrough, RunnableSerializable
 
 
 from mindsdb.integrations.utilities.rag.retrievers.auto_retriever import AutoRetriever
 from mindsdb.integrations.utilities.rag.retrievers.multi_vector_retriever import MultiVectorRetriever
@@ -58,15 +57,16 @@
         :param config: RAGPipelineModel
 
         :return:
         """
         vector_store_operator = VectorStoreOperator(
             vector_store=config.vector_store,
             documents=config.documents,
-            embeddings_model=config.embeddings_model
+            embeddings_model=config.embeddings_model,
+            vector_store_config=config.vector_store_config
         )
 
         return cls(vector_store_operator.vector_store.as_retriever(), config.rag_prompt_template, config.llm)
 
     @classmethod
     def from_auto_retriever(cls, config: RAGPipelineModel):
         """
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/rag_pipeline_builder.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/rag_pipeline_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from langchain_core.runnables import RunnableSerializable
 from mindsdb.integrations.utilities.rag.pipelines.rag import LangChainRAGPipeline
 from mindsdb.integrations.utilities.rag.settings import (
     RetrieverType,
     RAGPipelineModel
 )
 from mindsdb.integrations.utilities.rag.utils import documents_to_df
+from mindsdb.utilities.log import getLogger
 
+logger = getLogger(__name__)
 
 _retriever_strategies = {
     RetrieverType.VECTOR_STORE: lambda config: _create_pipeline_from_vector_store(config),
     RetrieverType.AUTO: lambda config: _create_pipeline_from_auto_retriever(config),
     RetrieverType.MULTI: lambda config: _create_pipeline_from_multi_retriever(config),
 }
 
@@ -58,13 +60,18 @@
         return retriever_strategy(config).with_returned_sources()
     else:
         raise ValueError(
             f'Invalid retriever type, must be one of: {list(_retriever_strategies.keys())}. Got {config.retriever_type}')
 
 
 class RAG:
-    def __init__(self, config: dict):
-        config = RAGPipelineModel(**config)
+    def __init__(self, config: RAGPipelineModel):
         self.pipeline = get_pipeline_from_retriever(config)
 
-    def __call__(self, question: str):
-        return self.pipeline.invoke(question)
+    def __call__(self, question: str) -> dict:
+        logger.info(f"Processing question using rag pipeline: {question}")
+        result = self.pipeline.invoke(question)
+
+        returned_sources = [docs.page_content for docs in result['context']]
+        logger.info(f"retrieved context used to answer question: {returned_sources}")
+
+        return result
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/retrievers/auto_retriever.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/retrievers/auto_retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import List
 import json
 
 
 from langchain.retrievers.self_query.base import SelfQueryRetriever
 
-from langchain_core.runnables import RunnableSerializable
-
 import pandas as pd
 
 from mindsdb.integrations.utilities.rag.retrievers.base import BaseRetriever
 
 from mindsdb.integrations.utilities.rag.utils import documents_to_df
 from mindsdb.integrations.utilities.rag.vector_store import VectorStoreOperator
 
@@ -99,15 +97,15 @@
 
         :return:
         """
         return VectorStoreOperator(vector_store=self.vectorstore,
                                    documents=self.documents,
                                    embeddings_model=self.embeddings_model).vector_store
 
-    def as_runnable(self) -> RunnableSerializable:
+    def as_runnable(self) -> BaseRetriever:
         """
         return the self-query retriever
         :return:
         """
         vectorstore = self.get_vectorstore()
 
         return SelfQueryRetriever.from_llm(
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/retrievers/multi_vector_retriever.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/retrievers/multi_vector_retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import List
 import uuid
 
 from langchain.retrievers.multi_vector import MultiVectorRetriever as LangChainMultiVectorRetriever
 from langchain_core.documents import Document
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import ChatPromptTemplate
-from langchain_core.runnables import RunnableSerializable
 from langchain_openai import ChatOpenAI
 
 from mindsdb.integrations.utilities.rag.retrievers.base import BaseRetriever
 from mindsdb.integrations.utilities.rag.settings import DEFAULT_LLM_MODEL, \
     MultiVectorRetrieverMode, RAGPipelineModel
 from mindsdb.integrations.utilities.rag.vector_store import VectorStoreOperator
 
@@ -52,15 +51,15 @@
         return split_docs, list(doc_ids)
 
     def _create_retriever_and_vs_operator(self, docs: List[Document]) \
             -> tuple[LangChainMultiVectorRetriever, VectorStoreOperator]:
         vstore_operator = VectorStoreOperator(
             vector_store=self.vectorstore,
             documents=docs,
-            embeddings_model=self.embeddings_model
+            embeddings_model=self.embeddings_model,
         )
         retriever = LangChainMultiVectorRetriever(
             vectorstore=vstore_operator.vector_store,
             byte_store=self.parent_store,
             id_key=self.id_key
         )
         return retriever, vstore_operator
@@ -70,15 +69,15 @@
                 {"doc": lambda x: x.page_content}  # noqa: E126, E122
                 | ChatPromptTemplate.from_template("Summarize the following document:\n\n{doc}")
                 | ChatOpenAI(max_retries=0, model_name=DEFAULT_LLM_MODEL)
                 | StrOutputParser()
         )
         return chain.batch(self.documents, {"max_concurrency": self.max_concurrency})
 
-    def as_runnable(self) -> RunnableSerializable:
+    def as_runnable(self) -> BaseRetriever:
         if self.mode in {MultiVectorRetrieverMode.SPLIT, MultiVectorRetrieverMode.BOTH}:
             split_docs, doc_ids = self._split_documents()
             retriever, vstore_operator = self._create_retriever_and_vs_operator(split_docs)
             summaries = self._get_document_summaries()
             summary_docs = [
                 Document(page_content=s, metadata={self.id_key: doc_ids[i]})
                 for i, s in enumerate(summaries)
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/settings.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseChatModel
 from langchain_core.vectorstores import VectorStore
 from langchain_openai import ChatOpenAI, OpenAIEmbeddings
 from langchain_core.stores import BaseStore
 from langchain.text_splitter import TextSplitter
-from pydantic import BaseModel, root_validator
+from pydantic import BaseModel
 
 # Multi retriever specific
 DEFAULT_ID_KEY = "doc_id"
 DEFAULT_MAX_CONCURRENCY = 5
 
 DEFAULT_CARDINALITY_THRESHOLD = 40
 DEFAULT_CHUNK_SIZE = 1000
@@ -87,15 +87,15 @@
     AUTO = 'auto'
     MULTI = 'multi'
 
 
 class VectorStoreConfig(BaseModel):
     vector_store_type: VectorStoreType = VectorStoreType.CHROMA
     persist_directory: str = None
-    collection_name: str = None
+    collection_name: str = 'default'
     connection_string: str = None
 
     class Config:
         arbitrary_types_allowed = True
         extra = "forbid"
 
 
@@ -104,15 +104,15 @@
 
     # used for loading an existing vector store
     vector_store_config: VectorStoreConfig = VectorStoreConfig()  # Vector store configuration
 
     vector_store: VectorStore = vector_store_map[vector_store_config.vector_store_type]  # Vector store
     db_connection_string: str = None  # Database connection string
     table_name: str = DEFAULT_TEST_TABLE_NAME  # table name
-    llm: BaseChatModel  # Language model
+    llm: BaseChatModel = None  # Language model
     embeddings_model: Embeddings  # Embeddings model
     rag_prompt_template: str = DEFAULT_RAG_PROMPT_TEMPLATE  # RAG prompt template
     retriever_prompt_template: Union[str, dict] = None  # Retriever prompt template
     retriever_type: RetrieverType = RetrieverType.VECTOR_STORE  # Retriever type
 
     # Multi retriever specific
     multi_retriever_mode: MultiVectorRetrieverMode = MultiVectorRetrieverMode.BOTH  # Multi retriever mode
@@ -129,16 +129,10 @@
     content_column_name: str = DEFAULT_CONTENT_COLUMN_NAME  # content column name (the column we will get embeddings)
     dataset_description: str = DEFAULT_DATASET_DESCRIPTION  # Description of the dataset
 
     class Config:
         arbitrary_types_allowed = True
         extra = "forbid"
 
-    @root_validator(pre=True)
-    def check_documents_or_vector_store_config(cls, values):
-        documents = values.get("documents")
-        vector_store_config = values.get("vector_store_config")
-
-        if documents is None and vector_store_config is None:
-            raise ValueError("At least documents or vector_store_config must be provided")
-
-        return values
+    @classmethod
+    def get_field_names(cls):
+        return list(cls.__fields__.keys())
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/rag/vector_store.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/rag/vector_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List
 
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.vectorstores import VectorStore
 
 from mindsdb.integrations.utilities.rag.loaders.vector_store_loader.vector_store_loader import VectorStoreLoader
+from mindsdb.integrations.utilities.rag.settings import VectorStoreConfig
 
 # gpt-3.5-turbo
 _DEFAULT_TPM_LIMIT = 60000
 _DEFAULT_RATE_LIMIT_INTERVAL = timedelta(seconds=10)
 _INITIAL_TOKEN_USAGE = 0
 
 
@@ -19,37 +20,39 @@
     Encapsulates the logic for adding documents to a vector store with rate limiting.
     """
 
     def __init__(self,
                  vector_store: VectorStore,
                  embeddings_model: Embeddings,
                  documents: List[Document] = None,
+                 vector_store_config: VectorStoreConfig = None,
                  token_per_minute_limit: int = _DEFAULT_TPM_LIMIT,
                  rate_limit_interval: timedelta = _DEFAULT_RATE_LIMIT_INTERVAL,
 
                  ):
 
         self.documents = documents
         self.embeddings_model = embeddings_model
         self.token_per_minute_limit = token_per_minute_limit
         self.rate_limit_interval = rate_limit_interval
         self.current_token_usage = _INITIAL_TOKEN_USAGE
         self._vector_store = None
+        self.vector_store_config = vector_store_config
 
         self.verify_vector_store(vector_store, documents)
 
     def verify_vector_store(self, vector_store, documents):
         if documents:
             self._add_documents_to_store(documents, vector_store)
         elif isinstance(vector_store, VectorStore):
             # checking is it instance or subclass instance
             self._vector_store = vector_store
         elif issubclass(vector_store, VectorStore):
-            # checking is it an uninstantiated subclass of VectorStore i.e. Chroma or PGVector
-            raise ValueError("If documents are not provided, an instantiated vector_store must be provided")
+            # if it is subclass instance, then create instance of it using vector_store_config
+            self._vector_store = load_vector_store(self.embeddings_model, self.vector_store_config)
 
     @property
     def vector_store(self):
         return self._vector_store
 
     @staticmethod
     def _calculate_token_usage(document):
@@ -79,15 +82,15 @@
             )
 
     def add_documents(self, documents: List[Document]):
         for document in documents:
             self._add_document(document)
 
 
-def load_vector_store(embeddings_model: Embeddings, config: dict) -> VectorStore:
+def load_vector_store(embeddings_model: Embeddings, config: VectorStoreConfig) -> VectorStore:
     """
     Loads the vector store based on the provided config and embeddings model
     :param embeddings_model:
     :param config:
     :return:
     """
     loader = VectorStoreLoader(embeddings_model=embeddings_model, config=config)
```

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/integrations/utilities/utils.py` & `MindsDB-24.4.3.0/mindsdb/integrations/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/agents/agents_controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/agents/agents_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/chatbot_controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/chatbot_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/chatbot_executor.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/chatbot_executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/chatbot_task.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/chatbot_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/memory.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/memory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/model_executor.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/model_executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/polling.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/polling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/chatbot/types.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/chatbot/types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/database/database.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/database/integrations.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/database/integrations.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/database/log.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/database/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/database/projects.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/database/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/database/views.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/file/file_controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/knowledge_base/controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/knowledge_base/controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -118,78 +118,191 @@
         Adds embedding column to dataframe and calls .upsert method of vector db
         :param df: input dataframe
 
         """
         if df.empty:
             return
 
+        df = self._adapt_column_names(df)
+
         # add embeddings
         df_emb = self._df_to_embeddings(df)
         df = pd.concat([df, df_emb], axis=1)
 
         # send to vector db
         db_handler = self._get_vector_db()
         db_handler.do_upsert(self._kb.vector_database_table, df)
 
+    def _adapt_column_names(self, df: pd.DataFrame) -> pd.DataFrame:
+
+        '''
+            convert input columns for vector db input
+            - id, content and metadata
+        '''
+
+        params = self._kb.params
+
+        columns = list(df.columns)
+
+        # -- prepare id --
+
+        # if id_column is defined:
+        #     use it as id
+        # elif 'id' column exists:
+        #     use it
+        # else:
+        #     use hash(content) -- it happens inside of vector handler
+
+        id_column = params.get('id_column')
+        if id_column is not None and id_column not in columns:
+            # wrong name
+            id_column = None
+
+        if id_column is None and TableField.ID.value in columns:
+            # default value
+            id_column = TableField.ID.value
+
+        if id_column is not None:
+            # remove from lookup list
+            columns.remove(id_column)
+
+        # -- prepare content and metadata --
+
+        # if content_columns is defined:
+        #     if len(content_columns) > 1:
+        #          make text from row (col: value\n col: value)
+        #     if metadata_columns is defined:
+        #          use them as metadata
+        #     else:
+        #          use all unused columns is metadata
+        #     elif metadata_columns is defined:
+        #          metadata_columns go to metadata
+        #          use all unused columns  as content (make text if columns>1)
+        # else:
+        #     no metadata
+        #     all unused columns go to content (make text if columns>1)
+
+        content_columns = params.get('content_columns')
+        metadata_columns = params.get('metadata_columns')
+
+        if content_columns is not None:
+            content_columns = list(set(content_columns).intersection(columns))
+            if len(content_columns) == 0:
+                raise ValueError(f'Content columns {params.get("content_columns")} not found in dataset: {columns}')
+
+            if metadata_columns is not None:
+                metadata_columns = list(set(metadata_columns).intersection(columns))
+            else:
+                # all the rest columns
+                metadata_columns = list(set(columns).difference(content_columns))
+
+        elif metadata_columns is not None:
+            metadata_columns = list(set(metadata_columns).intersection(columns))
+            # use all unused columns is content
+            content_columns = list(set(columns).difference(metadata_columns))
+        else:
+            # all columns go to content
+            content_columns = columns
+
+        if not content_columns:
+            raise ValueError("Can't find content columns")
+
+        def row_to_document(row: pd.Series) -> str:
+            """
+            Convert a row in the input dataframe into a document
+
+            Default implementation is to concatenate all the columns
+            in the form of
+            field1: value1\nfield2: value2\n...
+            """
+            fields = row.index.tolist()
+            values = row.values.tolist()
+            document = "\n".join(
+                [f"{field}: {value}" for field, value in zip(fields, values)]
+            )
+            return document
+
+        # create dataframe
+        if len(content_columns) == 1:
+            c_content = df[content_columns[0]]
+        else:
+            c_content = df[content_columns].apply(row_to_document, axis=1)
+        c_content.name = TableField.CONTENT.value
+        df_out = pd.DataFrame(c_content)
+
+        if id_column is not None:
+            df_out[TableField.ID.value] = df[id_column]
+
+        if metadata_columns and len(metadata_columns) > 0:
+            df_out[TableField.METADATA.value] = df[metadata_columns].apply(lambda row: str(dict(row)), axis=1)
+
+        return df_out
+
     def _replace_query_content(self, node, **kwargs):
         if isinstance(node, BinaryOperation):
             if isinstance(node.args[0], Identifier) and isinstance(node.args[1], Constant):
                 col_name = node.args[0].parts[-1]
                 if col_name.lower() == TableField.CONTENT.value:
                     # replace
                     node.args[0].parts = [TableField.EMBEDDINGS.value]
                     node.args[1].value = [self._content_to_embeddings(node.args[1].value)]
 
     def _get_vector_db(self):
         """
         helper to get vector db handler
         """
         if self._vector_db is None:
-            database_name = db.Integration.query.get(self._kb.vector_database_id).name
+            database = db.Integration.query.get(self._kb.vector_database_id)
+            if database is None:
+                raise ValueError('Vector database not found. Is it deleted?')
+            database_name = database.name
             self._vector_db = self.session.integration_controller.get_data_handler(database_name)
         return self._vector_db
 
     def _df_to_embeddings(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Returns embeddings for input dataframe.
         Uses model embedding model to convert content to embeddings.
         Automatically detects input and output of model using model description
         :param df:
         :return: dataframe with embeddings
         """
 
+        if df.empty:
+            return pd.DataFrame([], columns=[TableField.EMBEDDINGS.value])
+
         model_id = self._kb.embedding_model_id
         # get the input columns
         model_rec = db.session.query(db.Predictor).filter_by(id=model_id).first()
 
         assert model_rec is not None, f"Model not found: {model_id}"
         model_project = db.session.query(db.Project).filter_by(id=model_rec.project_id).first()
 
         project_datanode = self.session.datahub.get(model_project.name)
 
-        # TODO adjust input
+        # keep only content
+        df = df[[TableField.CONTENT.value]]
+
         input_col = model_rec.learn_args.get('using', {}).get('question_column')
+
         if input_col is not None and input_col != TableField.CONTENT.value:
             df = df.rename(columns={TableField.CONTENT.value: input_col})
 
-        if df.empty:
-            df_out = pd.DataFrame([], columns=[TableField.EMBEDDINGS.value])
-        else:
-            data = df.to_dict('records')
-
-            df_out = project_datanode.predict(
-                model_name=model_rec.name,
-                data=data,
-            )
+        data = df.to_dict('records')
 
-            target = model_rec.to_predict[0]
-            if target != TableField.EMBEDDINGS.value:
-                # adapt output for vectordb
-                df_out = df_out.rename(columns={target: TableField.EMBEDDINGS.value})
-            df_out = df_out[[TableField.EMBEDDINGS.value]]
+        df_out = project_datanode.predict(
+            model_name=model_rec.name,
+            data=data,
+        )
+
+        target = model_rec.to_predict[0]
+        if target != TableField.EMBEDDINGS.value:
+            # adapt output for vectordb
+            df_out = df_out.rename(columns={target: TableField.EMBEDDINGS.value})
+        df_out = df_out[[TableField.EMBEDDINGS.value]]
 
         return df_out
 
     def _content_to_embeddings(self, content: str) -> List[float]:
         """
         Converts string to embeddings
         :param content: input string
```

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/model/functions.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/model/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/model/model_controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/model/model_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/query_context/context_controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/query_context/context_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/query_context/last_query.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/query_context/last_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/skills/skill_tool.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/skills/skill_tool.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+import enum
 from typing import List, Optional
 
 from mindsdb_sql.parser.ast import Select, BinaryOperation, Identifier, Constant, Star
 
 from mindsdb.integrations.libs.vectordatabase_handler import TableField
 from mindsdb.interfaces.storage import db
 from .sql_agent import SQLAgent
 
 _DEFAULT_TOP_K_SIMILARITY_SEARCH = 5
 
 
+class SkillType(enum.Enum):
+    TEXT2SQL = 'text2sql'
+    KNOWLEDGE_BASE = 'knowledge_base'
+    RETRIEVAL = 'retrieval'
+
+
 class SkillToolController:
     def __init__(self):
         self.command_executor = None
 
     def get_command_executor(self):
         if self.command_executor is None:
             from mindsdb.api.executor.controllers import SessionController
@@ -62,15 +69,30 @@
         )
         for table in tables:
             description += f'Table name: "{table}", columns {sql_agent.get_table_columns(table)}\n'
 
         return dict(
             name='sql_db_query',
             func=sql_agent.query_safe,
-            description=description
+            description=description,
+            type=skill.type
+        )
+
+    def _make_retrieval_tools(self, skill: db.Skills) -> dict:
+        """
+        creates advanced retrieval tool i.e. RAG
+        """
+        params = skill.params
+        return dict(
+            name=params.get('name', skill.name),
+            config=params.get('retriever_config', {}),
+            description=f'You must use this tool to get more context or information '
+                        f'to answer a question about {params["description"]}. '
+                        f'The input should be the exact question the user is asking.',
+            type=skill.type
         )
 
     def _get_rag_query_function(self, skill: db.Skills):
 
         session_controller = self.get_command_executor().session
 
         def _answer_question(question: str) -> str:
@@ -94,28 +116,36 @@
     def _make_knowledge_base_tools(self, skill: db.Skills) -> dict:
         # To prevent dependency on Langchain unless an actual tool uses it.
         description = skill.params.get('description', '')
 
         return dict(
             name='Knowledge Base Retrieval',
             func=self._get_rag_query_function(skill),
-            description=f'Use this tool to get more context or information to answer a question about {description}. The input should be the exact question the user is asking.'
+            description=f'Use this tool to get more context or information to answer a question about {description}. The input should be the exact question the user is asking.',
+            type=skill.type
         )
 
     def get_tool_from_skill(self, skill: db.Skills) -> dict:
         """
             Creates function for skill and metadata (name, description)
         Args:
             skill (Skills): Skill to make a tool from
 
         Returns:
             dict with keys: name, description, func
         """
 
-        if skill.type == 'text_to_sql':
+        try:
+            skill_type = SkillType(skill.type)
+        except ValueError:
+            raise NotImplementedError(
+                f'skill of type {skill.type} is not supported as a tool, supported types are: {list(SkillType._member_names_)}')
+
+        if skill_type == SkillType.TEXT2SQL:
             return self._make_text_to_sql_tools(skill)
-        elif skill.type == 'knowledge_base':
+        if skill_type == SkillType.KNOWLEDGE_BASE:
             return self._make_knowledge_base_tools(skill)
-        raise NotImplementedError(f'skill of type {skill.type} is not supported as a tool')
+        if skill_type == SkillType.RETRIEVAL:
+            return self._make_retrieval_tools(skill)
 
 
 skill_tool = SkillToolController()
```

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/skills/skills_controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/skills/skills_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/skills/sql_agent.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/skills/sql_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/storage/db.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/storage/db.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/storage/fs.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/storage/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,27 @@
             if entry.is_file():
                 total += entry.stat().st_size
             elif entry.is_dir():
                 total += get_dir_size(entry.path)
     return total
 
 
+class AbsentFSStore(BaseFSStore):
+    """Storage class that does not store anything. It is just a dummy.
+    """
+    def get(self, *args, **kwargs):
+        pass
+
+    def put(self, *args, **kwargs):
+        pass
+
+    def delete(self, *args, **kwargs):
+        pass
+
+
 class LocalFSStore(BaseFSStore):
     """Storage that stores files locally
     """
 
     def __init__(self):
         super().__init__()
 
@@ -389,20 +402,21 @@
     @profiler.profile()
     def delete(self, remote_name):
         self.s3.delete_object(Bucket=self.bucket, Key=remote_name)
 
 
 def FsStore():
     storage_location = Config()['permanent_storage']['location']
+    if storage_location == 'absent':
+        return AbsentFSStore()
     if storage_location == 'local':
         return LocalFSStore()
-    elif storage_location == 's3':
+    if storage_location == 's3':
         return S3FSStore()
-    else:
-        raise Exception(f"Location: '{storage_location}' not supported")
+    raise Exception(f"Location: '{storage_location}' not supported")
 
 
 class FileStorage:
     def __init__(self, resource_group: str, resource_id: int,
                  root_dir: str = 'content', sync: bool = True):
         """
             Args:
```

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/storage/json.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/tabs/tabs_controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/tabs/tabs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/tasks/task_monitor.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/tasks/task_monitor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/tasks/task_thread.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/tasks/task_thread.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/triggers/trigger_task.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/triggers/trigger_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/interfaces/triggers/triggers_controller.py` & `MindsDB-24.4.3.0/mindsdb/interfaces/triggers/triggers_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/metrics/metrics.py` & `MindsDB-24.4.3.0/mindsdb/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/metrics/server.py` & `MindsDB-24.4.3.0/mindsdb/metrics/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-24.4.3.0/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-24.4.3.0/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-24.4.3.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-24.4.3.0/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-24.4.3.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-24.4.3.0/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-24.4.3.0/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-24.4.3.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/alembic.ini` & `MindsDB-24.4.3.0/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/env.py` & `MindsDB-24.4.3.0/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/migrate.py` & `MindsDB-24.4.3.0/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-07-13_a57506731839_triggers.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-07-13_a57506731839_triggers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-07-19_ad04ee0bd385_chatbot_to_task.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-07-19_ad04ee0bd385_chatbot_to_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-08-29_b0382f5be48d_predictor_hostname.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-08-29_b0382f5be48d_predictor_hostname.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-08-31_4c26ad04eeaa_add_skills_table.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-08-31_4c26ad04eeaa_add_skills_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-06_d44ab65a6a35_add_agents_table.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-06_d44ab65a6a35_add_agents_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-06_e187961e844a_add_agent_skills_table.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-06_e187961e844a_add_agent_skills_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-18_011e6f2dd9c2_backfill_agent_id.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-18_011e6f2dd9c2_backfill_agent_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-18_f16d4ab03091_add_agent_id.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-18_f16d4ab03091_add_agent_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-09-20_309db3d07cf4_add_knowledge_base.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-09-20_309db3d07cf4_add_knowledge_base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-10-03_6cb02dfd7f61_query_context.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-10-03_6cb02dfd7f61_query_context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-11-01_c67822e96833_jobs_active.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-11-01_c67822e96833_jobs_active.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2023-12-25_4b3c9d63e89c_predictor_index.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2023-12-25_4b3c9d63e89c_predictor_index.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2024-02-02_5a5c49313e52_job_condition.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2024-02-02_5a5c49313e52_job_condition.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/migrations/versions/2024-02-12_9461892bd889_llm_log.py` & `MindsDB-24.4.3.0/mindsdb/migrations/versions/2024-02-12_9461892bd889_llm_log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/auth.py` & `MindsDB-24.4.3.0/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/cache.py` & `MindsDB-24.4.3.0/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/config.py` & `MindsDB-24.4.3.0/mindsdb/utilities/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,22 @@
         elif os.environ.get('MINDSDB_STORAGE_DIR') is not None:
             root_storage_dir = os.environ['MINDSDB_STORAGE_DIR']
         else:
             root_storage_dir = get_or_create_data_dir()
             os.environ['MINDSDB_STORAGE_DIR'] = root_storage_dir
         # endregion
 
+        # region
+        is_storage_absent = os.environ.get('MINDSDB_STORAGE_BACKUP_DISABLED', '').lower() in ('1', 'true')
+        if is_storage_absent is True:
+            self._override_config['permanent_storage'] = {
+                'location': 'absent'
+            }
+        # endregion
+
         if os.path.isdir(root_storage_dir) is False:
             os.makedirs(root_storage_dir)
 
         if 'storage_db' in self._override_config:
             os.environ['MINDSDB_DB_CON'] = self._override_config['storage_db']
         elif os.environ.get('MINDSDB_DB_CON', '') == '':
             os.environ['MINDSDB_DB_CON'] = 'sqlite:///' + os.path.join(root_storage_dir,
```

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/context.py` & `MindsDB-24.4.3.0/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/context_executor.py` & `MindsDB-24.4.3.0/mindsdb/utilities/context_executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/exception.py` & `MindsDB-24.4.3.0/mindsdb/utilities/exception.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/fs.py` & `MindsDB-24.4.3.0/mindsdb/utilities/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/functions.py` & `MindsDB-24.4.3.0/mindsdb/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/hooks/__init__.py` & `MindsDB-24.4.3.0/mindsdb/utilities/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/hooks/profiling.py` & `MindsDB-24.4.3.0/mindsdb/utilities/hooks/profiling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/json_encoder.py` & `MindsDB-24.4.3.0/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/log.py` & `MindsDB-24.4.3.0/mindsdb/utilities/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/log_controller.py` & `MindsDB-24.4.3.0/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/__init__.py` & `MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/const.py` & `MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/const.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/consumer.py` & `MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/consumer.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/producer.py` & `MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/producer.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/task.py` & `MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/ml_task_queue/utils.py` & `MindsDB-24.4.3.0/mindsdb/utilities/ml_task_queue/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/profiler/profiler.py` & `MindsDB-24.4.3.0/mindsdb/utilities/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/ps.py` & `MindsDB-24.4.3.0/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/security.py` & `MindsDB-24.4.3.0/mindsdb/utilities/security.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/telemetry.py` & `MindsDB-24.4.3.0/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/mindsdb/utilities/wizards.py` & `MindsDB-24.4.3.0/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.4.2.1/requirements/requirements.txt` & `MindsDB-24.4.3.0/requirements/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 psycopg2-binary  # This is required for using sqlalchemy with postgres
 alembic >= 1.3.3
 redis >=5.0.0, < 6.0.0
 walrus==0.9.3
 flask-compress >= 1.0.0
 appdirs >= 1.0.0
 mindsdb-sql ~= 0.12.0
+pydantic >= 1.8.2
 mindsdb-evaluator >= 0.0.7, < 0.1.0
 checksumdir >= 1.2.0
 duckdb == 0.9.1
 requests >= 2.30.0
 pydateinfer==0.3.0
 dataprep_ml==0.0.22
 dill == 0.3.6
@@ -38,8 +39,7 @@
 msal
 langchain>=0.1.9
 langchain-core>=0.1.28
 langchain-community
 langchain-openai
 lark
 prometheus-client==0.20.0
-pydantic
```

### Comparing `MindsDB-24.4.2.1/setup.py` & `MindsDB-24.4.3.0/setup.py`

 * *Files identical despite different names*

