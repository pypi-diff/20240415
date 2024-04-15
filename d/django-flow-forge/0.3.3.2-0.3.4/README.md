# Comparing `tmp/django_flow_forge-0.3.3.2.tar.gz` & `tmp/django_flow_forge-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_flow_forge-0.3.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_flow_forge-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_flow_forge-0.3.3.2.tar` & `django_flow_forge-0.3.4.tar`

### file list

```diff
@@ -1,114 +1,122 @@
--rw-r--r--   0        0        0     6148 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.DS_Store
--rw-r--r--   0        0        0       66 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.gitattributes
--rw-r--r--   0        0        0      862 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.github/workflows/deploy-mkdocs.yml
--rw-r--r--   0        0        0      620 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     2879 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.gitignore
--rw-r--r--   0        0        0     1613 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/.vscode/launch.json
--rw-r--r--   0        0        0     1103 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/Dockerfile
--rw-r--r--   0        0        0     1061 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/LICENSE
--rw-r--r--   0        0        0      151 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/MANIFEST.in
--rw-r--r--   0        0        0      865 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/README.md
--rwxr-xr-x   0        0        0        0 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/__init__.py
--rwxr-xr-x   0        0        0     2599 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/admin.py
--rwxr-xr-x   0        0        0      160 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/apps.py
--rw-r--r--   0        0        0     2253 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/async_utils.py
--rw-r--r--   0        0        0     2950 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/authorization.py
--rw-r--r--   0        0        0    15414 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/flow_engine.py
--rw-r--r--   0        0        0     5435 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0001_initial.py
--rw-r--r--   0        0        0      816 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py
--rw-r--r--   0        0        0      449 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0003_alter_executedtask_exceptions.py
--rw-r--r--   0        0        0      624 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py
--rw-r--r--   0        0        0      428 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0005_alter_flow_options.py
--rw-r--r--   0        0        0      564 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py
--rw-r--r--   0        0        0      436 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/0007_executedflow_params.py
--rwxr-xr-x   0        0        0        0 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/__init__.py
--rw-r--r--   0        0        0      778 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0001_initial.py
--rw-r--r--   0        0        0      392 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0002_processtask_task_output.py
--rw-r--r--   0        0        0     1236 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py
--rw-r--r--   0        0        0      451 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0004_processtask_nested_task.py
--rw-r--r--   0        0        0      400 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0005_rename_nested_task_processtask_bidirectional_task.py
--rw-r--r--   0        0        0      627 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py
--rw-r--r--   0        0        0      448 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0007_rename_bidirectional_dependencies_processtask_depends_bidirectionally_with.py
--rw-r--r--   0        0        0      444 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0008_rename_dependencies_processtask_depends_on.py
--rw-r--r--   0        0        0     1717 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py
--rw-r--r--   0        0        0      414 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0010_processtask_nested.py
--rw-r--r--   0        0        0      573 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py
--rw-r--r--   0        0        0      980 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py
--rw-r--r--   0        0        0      537 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py
--rw-r--r--   0        0        0      732 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py
--rw-r--r--   0        0        0      432 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0015_alter_taskrun_output.py
--rw-r--r--   0        0        0      467 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0016_rename_processrun_executedprocess_and_more.py
--rw-r--r--   0        0        0      613 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py
--rw-r--r--   0        0        0      740 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py
--rw-r--r--   0        0        0      673 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py
--rw-r--r--   0        0        0      451 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0020_executedtask_task_name_snapshot.py
--rw-r--r--   0        0        0      841 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py
--rw-r--r--   0        0        0      554 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py
--rw-r--r--   0        0        0     1295 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0023_mlresult.py
--rw-r--r--   0        0        0      550 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py
--rw-r--r--   0        0        0      542 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py
--rw-r--r--   0        0        0      647 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py
--rw-r--r--   0        0        0      446 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0027_executedtask_task_status.py
--rw-r--r--   0        0        0      639 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py
--rw-r--r--   0        0        0      436 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0029_executedtask_exceptions.py
--rw-r--r--   0        0        0      771 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py
--rwxr-xr-x   0        0        0     5447 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/models.py
--rw-r--r--   0        0        0      627 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/static/django_flow_forge/cytoscape_setup.js
--rw-r--r--   0        0        0    47755 2024-04-08 20:53:34.855604 django_flow_forge-0.3.3.2/django_flow_forge/static/django_flow_forge/htmx.min.js
--rw-r--r--   0        0        0    10490 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/task_utils.py
--rw-r--r--   0        0        0      957 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html
--rw-r--r--   0        0        0      570 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html
--rw-r--r--   0        0        0     3526 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html
--rw-r--r--   0        0        0      754 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html
--rw-r--r--   0        0        0     2701 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html
--rw-r--r--   0        0        0      826 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html
--rw-r--r--   0        0        0     1422 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_result.html
--rw-r--r--   0        0        0     1808 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html
--rw-r--r--   0        0        0     2699 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html
--rw-r--r--   0        0        0     3194 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html
--rw-r--r--   0        0        0     3723 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html
--rw-r--r--   0        0        0     5888 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html
--rwxr-xr-x   0        0        0     2962 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/tests.py
--rw-r--r--   0        0        0      680 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/urls.py
--rwxr-xr-x   0        0        0     9518 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/django_flow_forge/views.py
--rw-r--r--   0        0        0      767 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docker-compose-local.yml
--rw-r--r--   0        0        0      846 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/authorization.md
--rw-r--r--   0        0        0     3996 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/considerations.md
--rw-r--r--   0        0        0      866 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/data_science_experiments.md
--rw-r--r--   0        0        0     1031 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/debugging.md
--rw-r--r--   0        0        0     1295 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/flows_dashboard.md
--rw-r--r--   0        0        0     4269 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/index.md
--rw-r--r--   0        0        0     3613 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/installation.md
--rw-r--r--   0        0        0      270 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/roadmap.md
--rw-r--r--   0        0        0     1037 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/docs/strategies.md
--rw-r--r--   0        0        0        0 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/__init__.py
--rw-r--r--   0        0        0      396 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/asgi.py
--rw-r--r--   0        0        0     4130 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/settings.py
--rw-r--r--   0        0        0      898 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/urls.py
--rw-r--r--   0        0        0      396 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/conf/wsgi.py
--rw-r--r--   0        0        0    32768 2024-04-08 20:53:34.859604 django_flow_forge-0.3.3.2/example_project/db.sqlite3-shm
--rw-r--r--   0        0        0  2904632 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/db.sqlite3-wal
--rw-r--r--   0        0        0      177 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/admin.py
--rw-r--r--   0        0        0      605 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/apps.py
--rw-r--r--   0        0        0      831 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/celery_app.py
--rw-r--r--   0        0        0     4720 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__ml_grid_search.py
--rw-r--r--   0        0        0     1394 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__parallel_celery.py
--rw-r--r--   0        0        0     1409 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__simple.py
--rw-r--r--   0        0        0     2980 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__simple_ml.py
--rw-r--r--   0        0        0     1555 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__simple_with_celery.py
--rw-r--r--   0        0        0     2137 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/flow__with_nested_tasks.py
--rw-r--r--   0        0        0        0 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-04-08 20:53:34.867604 django_flow_forge-0.3.3.2/example_project/example_app/models.py
--rw-r--r--   0        0        0     2134 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html
--rw-r--r--   0        0        0      994 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html
--rw-r--r--   0        0        0     1922 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/templates/example_app/index.html
--rw-r--r--   0        0        0       60 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/tests.py
--rw-r--r--   0        0        0      962 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/urls.py
--rw-r--r--   0        0        0     2531 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/example_app/views.py
--rwxr-xr-x   0        0        0      660 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/manage.py
--rw-r--r--   0        0        0      522 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/example_project/run_tasks_no_server.py
--rw-r--r--   0        0        0      399 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/mkdocs.yml
--rw-r--r--   0        0        0      875 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-08 20:53:34.871604 django_flow_forge-0.3.3.2/requirements.txt
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 django_flow_forge-0.3.3.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.DS_Store
+-rw-r--r--   0        0        0       66 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.gitattributes
+-rw-r--r--   0        0        0      862 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.github/workflows/deploy-mkdocs.yml
+-rw-r--r--   0        0        0      620 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     2879 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1613 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/.vscode/launch.json
+-rw-r--r--   0        0        0     1103 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/Dockerfile
+-rw-r--r--   0        0        0     1061 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/LICENSE
+-rw-r--r--   0        0        0      151 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/MANIFEST.in
+-rw-r--r--   0        0        0      865 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/README.md
+-rwxr-xr-x   0        0        0        0 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/__init__.py
+-rwxr-xr-x   0        0        0     2914 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/admin.py
+-rwxr-xr-x   0        0        0      160 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/apps.py
+-rw-r--r--   0        0        0     2306 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/async_utils.py
+-rw-r--r--   0        0        0     2950 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/authorization.py
+-rw-r--r--   0        0        0     1190 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/batch_utils.py
+-rw-r--r--   0        0        0    15970 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/flow_engine.py
+-rw-r--r--   0        0        0     5435 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0001_initial.py
+-rw-r--r--   0        0        0      816 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py
+-rw-r--r--   0        0        0      449 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0003_alter_executedtask_exceptions.py
+-rw-r--r--   0        0        0      624 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py
+-rw-r--r--   0        0        0      428 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0005_alter_flow_options.py
+-rw-r--r--   0        0        0      564 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py
+-rw-r--r--   0        0        0      436 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0007_executedflow_params.py
+-rw-r--r--   0        0        0      419 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0008_executedflow_meta.py
+-rw-r--r--   0        0        0     1411 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0009_flowbatch_flowbatchtempdata.py
+-rw-r--r--   0        0        0     1066 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0010_batchhandler.py
+-rw-r--r--   0        0        0     2004 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0011_remove_flowbatchtempdata_batch_and_more.py
+-rw-r--r--   0        0        0      416 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0012_rename_total_batches_batchhandler_total_batch_count.py
+-rw-r--r--   0        0        0     1346 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0013_remove_batchtempdata_batch_handler_flowbatch_and_more.py
+-rw-r--r--   0        0        0      345 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/0014_delete_batchtempdata.py
+-rwxr-xr-x   0        0        0        0 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/__init__.py
+-rw-r--r--   0        0        0      778 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0001_initial.py
+-rw-r--r--   0        0        0      392 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0002_processtask_task_output.py
+-rw-r--r--   0        0        0     1236 2024-04-15 10:06:36.500723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py
+-rw-r--r--   0        0        0      451 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0004_processtask_nested_task.py
+-rw-r--r--   0        0        0      400 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0005_rename_nested_task_processtask_bidirectional_task.py
+-rw-r--r--   0        0        0      627 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py
+-rw-r--r--   0        0        0      448 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0007_rename_bidirectional_dependencies_processtask_depends_bidirectionally_with.py
+-rw-r--r--   0        0        0      444 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0008_rename_dependencies_processtask_depends_on.py
+-rw-r--r--   0        0        0     1717 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py
+-rw-r--r--   0        0        0      414 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0010_processtask_nested.py
+-rw-r--r--   0        0        0      573 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py
+-rw-r--r--   0        0        0      980 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py
+-rw-r--r--   0        0        0      537 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py
+-rw-r--r--   0        0        0      732 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py
+-rw-r--r--   0        0        0      432 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0015_alter_taskrun_output.py
+-rw-r--r--   0        0        0      467 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0016_rename_processrun_executedprocess_and_more.py
+-rw-r--r--   0        0        0      613 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py
+-rw-r--r--   0        0        0      740 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py
+-rw-r--r--   0        0        0      673 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py
+-rw-r--r--   0        0        0      451 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0020_executedtask_task_name_snapshot.py
+-rw-r--r--   0        0        0      841 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py
+-rw-r--r--   0        0        0      554 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py
+-rw-r--r--   0        0        0     1295 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0023_mlresult.py
+-rw-r--r--   0        0        0      550 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py
+-rw-r--r--   0        0        0      542 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py
+-rw-r--r--   0        0        0      647 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py
+-rw-r--r--   0        0        0      446 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0027_executedtask_task_status.py
+-rw-r--r--   0        0        0      639 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py
+-rw-r--r--   0        0        0      436 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0029_executedtask_exceptions.py
+-rw-r--r--   0        0        0      771 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py
+-rwxr-xr-x   0        0        0     6549 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/models.py
+-rw-r--r--   0        0        0      627 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/static/django_flow_forge/cytoscape_setup.js
+-rw-r--r--   0        0        0    47755 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/static/django_flow_forge/htmx.min.js
+-rw-r--r--   0        0        0    10754 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/task_utils.py
+-rw-r--r--   0        0        0      957 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html
+-rw-r--r--   0        0        0      570 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html
+-rw-r--r--   0        0        0     3526 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html
+-rw-r--r--   0        0        0      806 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html
+-rw-r--r--   0        0        0     2701 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html
+-rw-r--r--   0        0        0      825 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html
+-rw-r--r--   0        0        0     1422 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_result.html
+-rw-r--r--   0        0        0     1808 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html
+-rw-r--r--   0        0        0     2699 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html
+-rw-r--r--   0        0        0     3194 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html
+-rw-r--r--   0        0        0     3723 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html
+-rw-r--r--   0        0        0     5888 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html
+-rwxr-xr-x   0        0        0     2962 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/tests.py
+-rw-r--r--   0        0        0      680 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/urls.py
+-rwxr-xr-x   0        0        0     9581 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/django_flow_forge/views.py
+-rw-r--r--   0        0        0      767 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docker-compose-local.yml
+-rw-r--r--   0        0        0      846 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/authorization.md
+-rw-r--r--   0        0        0     3996 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/considerations.md
+-rw-r--r--   0        0        0      866 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/data_science_experiments.md
+-rw-r--r--   0        0        0     1031 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/debugging.md
+-rw-r--r--   0        0        0     1295 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/flows_dashboard.md
+-rw-r--r--   0        0        0     4269 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/index.md
+-rw-r--r--   0        0        0     3613 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/installation.md
+-rw-r--r--   0        0        0      270 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/roadmap.md
+-rw-r--r--   0        0        0     1037 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/docs/strategies.md
+-rw-r--r--   0        0        0        0 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/__init__.py
+-rw-r--r--   0        0        0      396 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/asgi.py
+-rw-r--r--   0        0        0     4130 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/settings.py
+-rw-r--r--   0        0        0      898 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/urls.py
+-rw-r--r--   0        0        0      396 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/conf/wsgi.py
+-rw-r--r--   0        0        0    32768 2024-04-15 10:06:36.504723 django_flow_forge-0.3.4/example_project/db.sqlite3-shm
+-rw-r--r--   0        0        0  2904632 2024-04-15 10:06:36.512723 django_flow_forge-0.3.4/example_project/db.sqlite3-wal
+-rw-r--r--   0        0        0      177 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/admin.py
+-rw-r--r--   0        0        0      605 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/apps.py
+-rw-r--r--   0        0        0      831 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/celery_app.py
+-rw-r--r--   0        0        0     4720 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__ml_grid_search.py
+-rw-r--r--   0        0        0     1394 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__parallel_celery.py
+-rw-r--r--   0        0        0     1409 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__simple.py
+-rw-r--r--   0        0        0     2980 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__simple_ml.py
+-rw-r--r--   0        0        0     1555 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__simple_with_celery.py
+-rw-r--r--   0        0        0     2137 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/flow__with_nested_tasks.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/models.py
+-rw-r--r--   0        0        0     2134 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html
+-rw-r--r--   0        0        0      994 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html
+-rw-r--r--   0        0        0     1922 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/templates/example_app/index.html
+-rw-r--r--   0        0        0       60 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/tests.py
+-rw-r--r--   0        0        0      962 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/urls.py
+-rw-r--r--   0        0        0     2531 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/example_app/views.py
+-rwxr-xr-x   0        0        0      660 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/manage.py
+-rw-r--r--   0        0        0      522 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/example_project/run_tasks_no_server.py
+-rw-r--r--   0        0        0      399 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/mkdocs.yml
+-rw-r--r--   0        0        0      873 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-15 10:06:36.516723 django_flow_forge-0.3.4/requirements.txt
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 django_flow_forge-0.3.4/PKG-INFO
```

### Comparing `django_flow_forge-0.3.3.2/.DS_Store` & `django_flow_forge-0.3.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/.github/workflows/deploy-mkdocs.yml` & `django_flow_forge-0.3.4/.github/workflows/deploy-mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/.github/workflows/publish-to-pypi.yml` & `django_flow_forge-0.3.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/.gitignore` & `django_flow_forge-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/.vscode/launch.json` & `django_flow_forge-0.3.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/Dockerfile` & `django_flow_forge-0.3.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/LICENSE` & `django_flow_forge-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/README.md` & `django_flow_forge-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/admin.py` & `django_flow_forge-0.3.4/django_flow_forge/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     get_bidirectional_dependencies_display.short_description = 'Bidirectional Dependencies'
 
 @admin.register(models.ExecutedFlow)
 class ExecutedFlowAdmin(admin.ModelAdmin):
     list_display = ('flow', 'flow_name_snapshot', 'start_time', 'end_time', 'executed_by', 'flow_complete')
     list_filter = ('flow', 'flow_complete')
     search_fields = ['flow__flow_name', 'executed_by']
-    filter_horizontal = ('executed_tasks',)
+    # filter_horizontal = ('executed_tasks',)
     readonly_fields = ('flow_snapshot',)
 
     def get_readonly_fields(self, request, obj=None):
         if obj:  # Editing an existing object
             # flow_snapshot is always read-only
             return self.readonly_fields + ('start_time', 'end_time', 'flow', 'executed_tasks', 'executed_by', 'flow_complete')
         return self.readonly_fields
@@ -47,7 +47,15 @@
     def get_readonly_fields(self, request, obj=None):
         if obj:  # Editing an existing object
             # Making 'output' and 'task_snapshot_id' read-only for existing objects
             return self.readonly_fields + ('task', 'flow_run', 
                                         #    'start_time', 'end_time',
                                              'task_complete')
         return self.readonly_fields
+
+@admin.register(models.BatchHandler)
+class BatchHandlerAdmin(admin.ModelAdmin):
+    list_display = ('id', 'batch_ref_name', 'total_batch_count', 'temp_data',)
+
+@admin.register(models.FlowBatch)
+class FlowBatchAdmin(admin.ModelAdmin):
+    list_display = ('id', 'batch_handler', 'flow_batch_number', 'temp_data',)
```

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/async_utils.py` & `django_flow_forge-0.3.4/django_flow_forge/async_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             **kwargs: Keyword arguments to be passed to the task function.
 
         Returns:
             The output of the task function.
         """
 
         self.task_run.status = 'in_progress'
+        kwargs['current_task_name'] = self.task_name
         accepts_kwargs = self.function_accepts_kwargs(self.function)
 
         if accepts_kwargs:
             filtered_kwargs = kwargs
         
         else:
             filtered_kwargs = self.filter_kwargs_for_function(self.function, kwargs)
```

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/authorization.py` & `django_flow_forge-0.3.4/django_flow_forge/authorization.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/flow_engine.py` & `django_flow_forge-0.3.4/django_flow_forge/flow_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .task_utils import get_cytoscape_nodes_and_edges
 from django.conf import settings
 from django.utils import timezone
 import time
 import inspect
 
 from django.db import transaction
-from .models import Flow, FlowTask
+from .models import Flow, FlowTask, BatchHandler, FlowBatch
 from .task_utils import post_flow_graph_to_add_status, make_task_snapshot, make_flow_snapshot
 
 flow_pipeline_lookup = {}
 
 def register_task(flow, task_name, task_info, nested):
     """
     Registers or updates a single task within a specified flow, handling dependencies.
@@ -117,15 +117,15 @@
         register_tasks_recursively(pipeline, flow)
 
         # Identify and remove tasks that are no longer part of the pipeline
         tasks_to_delete = existing_tasks - updated_tasks
         if tasks_to_delete:
             FlowTask.objects.filter(flow=flow, task_name__in=tasks_to_delete).delete()
 
-        return updated_tasks
+    return updated_tasks
 
 def set_dependencies(task, depends_on, depends_bidirectionally_with, flow):
     """
     Sets dependencies for a given task within a flow. Dependencies can be unidirectional or bidirectional.
     
     This function links a task with its dependencies by creating or retrieving the dependent tasks and associating them
     accordingly. It ensures that each task is properly linked to others upon which it depends or with which it has
@@ -223,15 +223,15 @@
     An executor for the flow with the primary aim of assisting in debugging a flow, cycling through each
     Task function in an ordered and stepwise fashion
     '''
     def debug_mode(self, executor, **kwargs):
         executor.task_output = executor.function(**kwargs)
         return
 
-def run_flow(flow_name, debug_executor=DebugExecutor(), **kwargs):
+def run_flow(flow_name, debug_executor=DebugExecutor(), flow_batch_id=None, **kwargs):
     '''
     Initiates and executes a flow pipeline by name, handling task execution and flow status updates.
 
     Parameters:
     - flow_name (str): The name of the xflow to be executed.
     - **kwargs: Additional keyword arguments that may be required for task execution.
 
@@ -246,75 +246,80 @@
         # Resolve task dependencies and determine the execution order
         all_task_objs, task_order = resolve_dependencies_get_task_order(flow_name)
         
     except Exception as e:
         logging.error(f"Failed to initiate flow run for {flow_name}: {e}")
         raise Exception('You may not have imported the pipeline in to the program, have spelt the flow wrong or are referring to a pipeline that no longer exists.')
 
+    if flow_batch_id:
+        batch = FlowBatch.objects.get(id=flow_batch_id)
+        if flow_name in batch.temp_data.get('executed_flows', []):
+            print(f'''Not running flow "{flow_name}" Batch: f{batch.flow_batch_number} as it is flagged as already run''')
+            return
+
     flow_pipeline = flow_pipeline_lookup.get(flow_name)
     flow_snapshot = make_flow_snapshot(flow_pipeline, task_order)
     flow_snapshot['graph'] = get_cytoscape_nodes_and_edges(all_task_objs, show_nested=True)
     flow_snapshot['flow_name'] = flow_name
     flow_run.flow_snapshot = flow_snapshot
     flow_run.save()
     kwargs['executed_flow_id'] = flow_run.id
+    kwargs['flow_name'] = flow_name
+    kwargs['flow_batch_id'] = flow_batch_id
         
     executors = {}
 
     # assign an executor instance for each task:
     for task_name, task_dict in flow_pipeline.items():
         executor = get_executor(task_dict, task_name, **kwargs)
         executor.flow = flow
         executor.flow_run = flow_run
+        executor.flow_name = flow_name
         executor.setup_flow_task(flow, flow_run,)
         executor.debug_executor = debug_executor
         executors[task_name] = executor
 
     counter = 0
     
     while any(executor.task_run.status != 'complete' for executor in executors.values()):
 
         for task_name in executors:
 
             executor = executors[task_name]
 
-            try:
-                ''' If all dependencies are met, execute the task '''
-                if task_can_start_check(flow_run, task_name, executor, executors, **kwargs):
+            ''' If all dependencies are met, execute the task '''
+            if task_can_start_check(flow_run, task_name, executor, executors, **kwargs):
 
-                    executor.submit_task(**kwargs)
+                executor.submit_task(**kwargs)
 
-                    executor.create_checkpoint()
+                executor.create_checkpoint()
 
-                    if executor.task_is_ready_for_close():
-                        # collect output
-                        executor.collect_and_store_output()
+                if executor.task_is_ready_for_close():
+                    # collect output
+                    executor.collect_and_store_output()
 
-                        executor.task_post_process()
-                
-                elif executor.task_run.status == 'in_progress':
-                    
-                    # Else if task is in progress then check status and collect data #
-                    if counter % 1000 == 0:
-                        executor.create_checkpoint()
-            
-                    if executor.task_is_ready_for_close():
-                        # collect output
-                        executor.collect_and_store_output()
-
-                        executor.task_post_process()
-
-                elif executor.task_run.status == 'failed':
-                    flow_run.status = 'failed'
-                    post_flow_graph_to_add_status(flow_run)
-                    flow_run.save()
-                    break
+                    executor.task_post_process()
             
-            finally:
-                pass
+            elif executor.task_run.status == 'in_progress':
+                
+                # Else if task is in progress then check status and collect data #
+                if counter % 1000 == 0:
+                    executor.create_checkpoint()
+        
+                if executor.task_is_ready_for_close():
+                    # collect output
+                    executor.collect_and_store_output()
+
+                    executor.task_post_process()
+
+            elif executor.task_run.status == 'failed':
+                flow_run.status = 'failed'
+                post_flow_graph_to_add_status(flow_run)
+                flow_run.save()
+                break
 
         # Optional: Implement a more sophisticated mechanism to avoid tight looping
         time.sleep(1)
         counter += 1
 
     if all(executor.task_run.status == 'complete' for executor in executors.values()):
         closing_flow_process(flow_run, flow_complete=True, status='complete')
@@ -325,14 +330,21 @@
         logging.error(f"Flow {flow_name} failed due to task error.")
 
     # Update the flow run status to 'complete' after successful execution of all tasks
     
     post_flow_graph_to_add_status(flow_run)
     flow_run.save()
 
+    if flow_batch_id:
+        batch = FlowBatch.objects.get(id=flow_batch_id)
+        executed = batch.temp_data.get('executed_flows', [])
+        executed.append(flow_name)
+        batch.temp_data['executed_flows'] = executed
+        batch.save(update_fields=['temp_data'])
+
     logging.info(f"All tasks for flow {flow_name} completed successfully.")
 
     return
 
 def closing_flow_process(flow_run, flow_complete:bool, status=None,):
 
     flow_run.flow_complete = flow_complete
```

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/0001_initial.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0001_initial.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0023_mlresult.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0023_mlresult.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py` & `django_flow_forge-0.3.4/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/models.py` & `django_flow_forge-0.3.4/django_flow_forge/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.db import models
+from django.core.serializers.json import DjangoJSONEncoder
 
 class Flow(models.Model):
 
     flow_name = models.CharField(null=False, blank=False, max_length=255, unique=True)  # Assuming each flow name is unique
     flow_display_name = models.CharField(null=True, blank=True, max_length=255,)
     in_current_code_base = models.BooleanField(default=True, null=False, blank=True)
 
@@ -50,22 +51,24 @@
 class ExecutedFlow(models.Model):
 
     flow = models.ForeignKey(Flow, null=True, on_delete=models.SET_NULL, related_name='flow_runs')
     flow_id_snapshot = models.BigIntegerField(null=True, blank=True,)
     flow_name_snapshot = models.CharField(null=True, blank=True, max_length=255)
     start_time = models.DateTimeField(auto_now_add=True)
     end_time = models.DateTimeField(null=True, blank=True)
-    executed_tasks = models.ManyToManyField(FlowTask, related_name='executed_tasks', blank=True)
+    batch_handler = models.ForeignKey('BatchHandler', on_delete=models.CASCADE, related_name='executed_flows', null=True, blank=True)
+    # executed_tasks = models.ManyToManyField(FlowTask, related_name='executed_tasks', blank=True)
     executed_by = models.CharField(null=True, blank=True, max_length=255)
     flow_complete = models.BooleanField(default=False)  # Indicates if the flow run is complete
     status = models.CharField(max_length=20, choices=STATUS_CHOICES, default='pending')
     last_checkpoint_datetime = models.DateTimeField(blank=True, auto_now_add=True)
     flow_snapshot = models.JSONField(default=dict)  # Captures the output of the task for this run
     exceptions = models.JSONField(default=dict, null=True, blank=True)
     params = models.JSONField(default=dict, null=True, blank=True)
+    meta = models.JSONField(default=dict, null=True, blank=True)
 
     def __str__(self):
         if self.flow:
             return f"Run of {self.flow.flow_name} on {self.start_time}. Completed: {self.flow_complete}"
         else:
             return f"Run of an unknown flow on {self.start_time}. Completed: {self.flow_complete}"
 
@@ -85,15 +88,27 @@
 
     def __str__(self):
         if not self.task:
             task_name = self.task_snapshot['task_name']
         else:
             task_name = self.task.task_name
         return f"Run of '{task_name}' for '{self.flow_run}'. Completed: {self.task_complete}"
-    
+
+class BatchHandler(models.Model):
+    '''Model to handle batch processing using the same Flow - sometimes you want to run the flow in batches not batches within a flow.
+       This is also a useful option if you want to chain together Flows in a batch'''
+    batch_ref_name = models.CharField(null=True, blank=True, max_length=255) # Optional reference name
+    total_batch_count = models.IntegerField(default=0, null=False, blank=False,)
+    temp_data = models.JSONField(null=True, default=dict, encoder=DjangoJSONEncoder)
+
+class FlowBatch(models.Model):
+    batch_handler = models.ForeignKey(BatchHandler, on_delete=models.CASCADE, related_name='batch', null=True, blank=True)
+    flow_batch_number = models.IntegerField(default=0, null=False, blank=False,)
+    temp_data = models.JSONField(null=True, default=dict, encoder=DjangoJSONEncoder)
+
 class MLResult(models.Model):
 
     executed_flow = models.ForeignKey(ExecutedFlow, null=True, blank=True, on_delete=models.SET_NULL, related_name='ml_runs')
     experiment = models.CharField(null=True, blank=True, max_length=255)
     dataset = models.CharField(null=True, blank=True, max_length=255)
     algorithm = models.CharField(null=True, blank=True, max_length=255)
     parameters = models.JSONField(default=dict)  # Parameters used for this particular run
```

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/static/django_flow_forge/cytoscape_setup.js` & `django_flow_forge-0.3.4/django_flow_forge/static/django_flow_forge/cytoscape_setup.js`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/static/django_flow_forge/htmx.min.js` & `django_flow_forge-0.3.4/django_flow_forge/static/django_flow_forge/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/task_utils.py` & `django_flow_forge-0.3.4/django_flow_forge/task_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 
     def submit_task(self, **kwargs):
 
         """
         Executes a specific task as part of a flow run, handling logging, execution, and status updates.
 
         """
-        
+        kwargs['current_task_name'] = self.task_name
         self.task_run.status = 'in_progress'
         accepts_kwargs = self.function_accepts_kwargs(self.function)
         
         try:
             if accepts_kwargs:
                 filtered_kwargs = kwargs
+                kwargs['flow_name'] = self.flow_name
+                kwargs['task_name'] = self.task_name
                 
             else:
                 filtered_kwargs = self.filter_kwargs_for_function(self.function, kwargs)
             
             if settings.DEBUG:
                 self.debug_executor.debug_mode(self, **filtered_kwargs)
 
@@ -103,15 +105,15 @@
         self.task_run.end_time = timezone.now()
         self.task_run.status = 'complete'
 
         ''' If task no longer exists, remove it'''
         if not FlowTask.objects.filter(id=self.task_run.task.id).exists():
             self.task_run.task = None
 
-        self.task_run.save()
+        self.task_run.save(update_fields=['status', 'end_time', 'task_complete', 'output'])
         return True
 
     def collect_and_store_output(self):
 
         '''Collection is only necessary for async tasks that override this method'''
 
         self.executed_task_output()
@@ -124,15 +126,15 @@
         self.task_run.end_time = timezone.now()
         self.task_run.exceptions['main_run'] = str(e)
 
         ''' If task no longer exists, remove it'''
         if not FlowTask.objects.filter(id=self.task_run.task.id).exists():
             self.task_run.task = None
             
-        self.task_run.save()
+        self.task_run.save(update_fields=['status', 'end_time', 'exceptions',])
         return False
     
     def function_accepts_kwargs(self, func):
         """
         Check if the function accepts **kwargs.
         """
         sig = inspect.signature(func)
```

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,18 @@
     <hr class="title-hr mb-5">
     
     <div id="data-div1" class="text-light d-none"
         hx-get="{% url 'django-flow-forge:update-concept-node-info' %}"
         hx-trigger="tap from:#data-div1" 
         hx-target="#node-output"
         hx-swap="innerHTML"
-        hx-include="#current_flow_option"
-        hx-vals='js:{clicked_node_id: event.detail["clicked_node_id"]}'>
+        hx-vals='js:{
+            clicked_node_id: event.detail["clicked_node_id"],
+            executed_flow_option: event.detail["executed_flow_option"]
+        }'>
     </div>
 
     <div class="col-lg-7">
     <!-- <div id="cy" style="width: 100%; height: 800px"> -->
         {% include 'django_flow_forge/components/dag_cyto_conceptual_script.html' %}
     </div>
```

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     <hr class="title-hr mb-5">
     
     <div id="data-div1" class="text-light d-none"
         hx-get="{% url 'django-flow-forge:update-node-info' %}"
         hx-trigger="tap from:#data-div1" 
         hx-target="#node-output"
         hx-swap="innerHTML"
-        hx-include="#current_executed_flow_option"
+        hx-include="[name='current_flow_option']"
         hx-vals='js:{clicked_node_id: event.detail["clicked_node_id"]}'>
     </div>
 
     <div class="col-lg-6">
         {% include 'django_flow_forge/components/dag_cyto_clickable_script.html' %}
         
     </div>
```

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_result.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_result.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html` & `django_flow_forge-0.3.4/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/tests.py` & `django_flow_forge-0.3.4/django_flow_forge/tests.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/urls.py` & `django_flow_forge-0.3.4/django_flow_forge/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/django_flow_forge/views.py` & `django_flow_forge-0.3.4/django_flow_forge/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,28 +42,28 @@
         # 'plotly_fig': plot_div,  # The Plotly figure in HTML div format
         'graph_json': graph_json_serialized,
         'all_flowes': all_flows,
         'current_flow_id': flow.id,
     }
 
     if request.htmx:
-
+        context = {'graph_json': graph_json_serialized, 'current_flow_id': flow.id}
         # Render a partial template with the new Cytoscape graph
-        html = render_to_string('django_flow_forge/components/dag_cyto_conceptual_script.html', {'graph_json': graph_json_serialized})
+        html = render_to_string('django_flow_forge/components/dag_cyto_conceptual_script.html', context=context )
         return HttpResponse(html)
 
     return render(request, 'django_flow_forge/dag_conceptual_index.html', context=context)
 
 @user_has_permission(permission='django_flow_forge.django_flow_admin_access')
 def update_conceptual_node_info(request):
 
     if request.htmx:
 
         node_id = request.GET.get('clicked_node_id', None) # this is the id of the task it was when the task was first run
-        flow_id = request.GET.get('current_flow_option', None)
+        flow_id = request.GET.get('executed_flow_option', None)
         context = {}
         if node_id:
 
             flow = models.Flow.objects.get(id=flow_id)
 
             if models.FlowTask.objects.filter(id=node_id, flow=flow).exists():
```

### Comparing `django_flow_forge-0.3.3.2/docker-compose-local.yml` & `django_flow_forge-0.3.4/docker-compose-local.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/docs/authorization.md` & `django_flow_forge-0.3.4/docs/authorization.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/docs/considerations.md` & `django_flow_forge-0.3.4/docs/considerations.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/docs/data_science_experiments.md` & `django_flow_forge-0.3.4/docs/data_science_experiments.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/docs/debugging.md` & `django_flow_forge-0.3.4/docs/debugging.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/docs/flows_dashboard.md` & `django_flow_forge-0.3.4/docs/flows_dashboard.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/docs/index.md` & `django_flow_forge-0.3.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/docs/installation.md` & `django_flow_forge-0.3.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/docs/strategies.md` & `django_flow_forge-0.3.4/docs/strategies.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/conf/settings.py` & `django_flow_forge-0.3.4/example_project/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/conf/urls.py` & `django_flow_forge-0.3.4/example_project/conf/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/db.sqlite3-shm` & `django_flow_forge-0.3.4/example_project/db.sqlite3-shm`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/db.sqlite3-wal` & `django_flow_forge-0.3.4/example_project/db.sqlite3-wal`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/apps.py` & `django_flow_forge-0.3.4/example_project/example_app/apps.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/celery_app.py` & `django_flow_forge-0.3.4/example_project/example_app/celery_app.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/flow__ml_grid_search.py` & `django_flow_forge-0.3.4/example_project/example_app/flow__ml_grid_search.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/flow__parallel_celery.py` & `django_flow_forge-0.3.4/example_project/example_app/flow__parallel_celery.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/flow__simple.py` & `django_flow_forge-0.3.4/example_project/example_app/flow__simple.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/flow__simple_ml.py` & `django_flow_forge-0.3.4/example_project/example_app/flow__simple_ml.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/flow__simple_with_celery.py` & `django_flow_forge-0.3.4/example_project/example_app/flow__simple_with_celery.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/flow__with_nested_tasks.py` & `django_flow_forge-0.3.4/example_project/example_app/flow__with_nested_tasks.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html` & `django_flow_forge-0.3.4/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html` & `django_flow_forge-0.3.4/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/templates/example_app/index.html` & `django_flow_forge-0.3.4/example_project/example_app/templates/example_app/index.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/urls.py` & `django_flow_forge-0.3.4/example_project/example_app/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/example_app/views.py` & `django_flow_forge-0.3.4/example_project/example_app/views.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/manage.py` & `django_flow_forge-0.3.4/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/example_project/run_tasks_no_server.py` & `django_flow_forge-0.3.4/example_project/run_tasks_no_server.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.3.2/pyproject.toml` & `django_flow_forge-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-flow-forge"
-version = "0.3.3.2"
+version = "0.3.4"
 description = "Eliminate unnecessary system complexity in Data Ops and in Machine Learning Ops (MLOps) with this Django module for defining, running and monitoring flows."
 authors = [{name = "Ed Burmicz", email = "eddyojb@gmail.com"}]
 readme = "README.md"
 license = {text = "MIT"} 
 keywords = ["django", "mlops", "data", "machine learning", "data science", "pipelines", "flow", "orchestration", "AI",]
 classifiers = [
     "Framework :: Django",
```

### Comparing `django_flow_forge-0.3.3.2/PKG-INFO` & `django_flow_forge-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flow-forge
-Version: 0.3.3.2
+Version: 0.3.4
 Summary: Eliminate unnecessary system complexity in Data Ops and in Machine Learning Ops (MLOps) with this Django module for defining, running and monitoring flows.
 Keywords: django,mlops,data,machine learning,data science,pipelines,flow,orchestration,AI
 Author-email: Ed Burmicz <eddyojb@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

