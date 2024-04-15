# Comparing `tmp/jupyter_scheduler-2.5.0.tar.gz` & `tmp/jupyter_scheduler-2.5.1.tar.gz`

## Comparing `jupyter_scheduler-2.5.0.tar` & `jupyter_scheduler-2.5.1.tar`

### file list

```diff
@@ -1,183 +1,183 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/.eslintrc.js
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/.prettierrc
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/.readthedocs.yml
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/.stylelintrc
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/.yarnrc.yml
--rw-r--r--   0        0        0    42894 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/MANIFEST.in
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/babel.config.js
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/conftest.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jest.config.js
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/tsconfig.test.json
--rw-r--r--   0        0        0   429247 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/yarn.lock
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/binder/environment.yml
--rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/binder/postBuild
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/dev/seed.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/dev/templates/1.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/dev/templates/2.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/dev/templates/3.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/Makefile
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/conf.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/make.bat
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/requirements.txt
--rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/_static/jupyter_logo.png
--rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/contributors/index.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/developers/index.md
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/operators/index.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/index.md
--rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/actions_definition_details.png
--rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/actions_job_details.png
--rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/actions_list.png
--rw-r--r--   0        0        0   102590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/create_job_form.png
--rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/create_job_from_filebrowser.png
--rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/create_job_from_notebook.png
--rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/custom_schedule.png
--rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/download_button.png
--rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/downloaded_files.png
--rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/headers.png
--rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/item_name.png
--rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/launcher.png
--rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/docs/users/images/run_on_schedule.png
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter-config/nb-config/jupyter_scheduler.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter-config/server-config/jupyter_scheduler.json
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/_version.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/environments.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/exceptions.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/executors.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/extension.py
--rw-r--r--   0        0        0    15497 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/handlers.py
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/job_files_manager.py
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/models.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/orm.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/parameterize.py
--rw-r--r--   0        0        0    31540 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/scheduler.py
--rw-r--r--   0        0        0    11623 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/task_runner.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/utils.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/package.json
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/171.d4610e21027b29e7653a.js
--rw-r--r--   0        0        0   347375 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/177.3502ccdd2c25548ad980.js
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/275.d7f03fdf77443bec5349.js
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/282.7b4e318dca2d64a434c1.js
--rw-r--r--   0        0        0    83134 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/314.1b593fd6b3501a52cc35.js
--rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/378.34aa286b24af0577a1ce.js
--rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
--rw-r--r--   0        0        0   121687 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js.LICENSE.txt
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js.LICENSE.txt
--rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
--rw-r--r--   0        0        0    20648 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js.LICENSE.txt
--rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/747.8e4a60162d1a81804893.js
--rw-r--r--   0        0        0    25936 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/871.5c8b68996069b5cffa43.js
--rw-r--r--   0        0        0    10111 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/remoteEntry.43a78772e27d406d91b4.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/style.js
--rw-r--r--   0        0        0    39580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/pydantic_v1/main.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/mocks.py
--rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_handlers.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_job_files_manager.py
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_scheduler.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/utils.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.html
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/schema/plugin.json
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/advanced-options.tsx
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/context.ts
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/handler.ts
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/hooks.ts
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/index.tsx
--rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/model.ts
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/notebook-jobs-panel.tsx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/size.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/svg.d.ts
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/theme-provider.ts
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/tokens.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/__tests__/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/box.tsx
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/button-bar.tsx
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/button.tsx
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/cluster.tsx
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/collapsible-panel.tsx
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/compute-type-picker.tsx
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/confirm-buttons.tsx
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/confirm-dialog-buttons.tsx
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/create-schedule-options.tsx
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/environment-picker.tsx
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/error-boundary.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/heading.tsx
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/icon-buttons.tsx
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/icons.ts
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/input-file-snapshot.tsx
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/job-definition-row.tsx
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/job-file-link.tsx
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/job-row.tsx
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/labeled-value.tsx
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/output-format-picker.tsx
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/parameters-picker.tsx
--rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/schedule-inputs.tsx
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/stack.tsx
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/advanced-table/advanced-table-header.tsx
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/advanced-table/advanced-table.tsx
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/components/advanced-table/index.tsx
--rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/mainviews/create-job-from-definition.tsx
--rw-r--r--   0        0        0    20654 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/mainviews/create-job.tsx
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/mainviews/edit-job-definition.tsx
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/mainviews/list-jobs.tsx
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/mainviews/detail-view/detail-view.tsx
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/mainviews/detail-view/index.tsx
--rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/mainviews/detail-view/job-definition.tsx
--rw-r--r--   0        0        0    10160 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/mainviews/detail-view/job-detail.tsx
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/util/errors.tsx
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/src/util/job-name-validation.tsx
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/base.css
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/box.css
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/button.css
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/cluster.css
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/collapsible-panel.css
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/edit-job-definitions.css
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/heading.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/index.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/labeled-value.css
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/stack.css
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/variables.css
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/icons/calendar-add-on.svg
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/icons/calendar-month.svg
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/style/icons/event-note.svg
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/.yarnrc
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/package.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   153944 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/helpers/SchedulerHelper.ts
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0    18992 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-filebrowser-linux.png
--rw-r--r--   0        0        0    19577 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-toolbar-linux.png
--rw-r--r--   0        0        0    19747 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/filebrowser-menu-linux.png
--rw-r--r--   0        0        0    26873 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    22246 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/list-view-linux.png
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/notebook-toolbar-linux.png
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/LICENSE
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/README.md
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/.eslintrc.js
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/.prettierrc
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/.stylelintrc
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/.yarnrc.yml
+-rw-r--r--   0        0        0    44117 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/MANIFEST.in
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/babel.config.js
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/conftest.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jest.config.js
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/tsconfig.test.json
+-rw-r--r--   0        0        0   429247 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/yarn.lock
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/binder/environment.yml
+-rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/binder/postBuild
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/dev/seed.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/dev/templates/1.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/dev/templates/2.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/dev/templates/3.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/Makefile
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/conf.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/make.bat
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/_static/jupyter_logo.png
+-rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/contributors/index.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/developers/index.md
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/operators/index.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/index.md
+-rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/actions_definition_details.png
+-rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/actions_job_details.png
+-rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/actions_list.png
+-rw-r--r--   0        0        0   102590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/create_job_form.png
+-rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/create_job_from_filebrowser.png
+-rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/create_job_from_notebook.png
+-rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/custom_schedule.png
+-rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/download_button.png
+-rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/downloaded_files.png
+-rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/headers.png
+-rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/item_name.png
+-rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/launcher.png
+-rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/docs/users/images/run_on_schedule.png
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter-config/nb-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter-config/server-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/_version.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/environments.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/exceptions.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/executors.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/extension.py
+-rw-r--r--   0        0        0    15497 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/handlers.py
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/job_files_manager.py
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/models.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/orm.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/parameterize.py
+-rw-r--r--   0        0        0    31540 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/scheduler.py
+-rw-r--r--   0        0        0    11623 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/task_runner.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/utils.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/package.json
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/171.d4610e21027b29e7653a.js
+-rw-r--r--   0        0        0   347375 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/177.3502ccdd2c25548ad980.js
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/275.d7f03fdf77443bec5349.js
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/282.7b4e318dca2d64a434c1.js
+-rw-r--r--   0        0        0    83215 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/314.37ac184c4c28a29ef5e6.js
+-rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/378.34aa286b24af0577a1ce.js
+-rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
+-rw-r--r--   0        0        0   121687 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js.LICENSE.txt
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js.LICENSE.txt
+-rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
+-rw-r--r--   0        0        0    20648 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js.LICENSE.txt
+-rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/747.8e4a60162d1a81804893.js
+-rw-r--r--   0        0        0    25936 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/871.5c8b68996069b5cffa43.js
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/remoteEntry.c7c7d5449715968d9006.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/style.js
+-rw-r--r--   0        0        0    39580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/pydantic_v1/main.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/mocks.py
+-rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_handlers.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_job_files_manager.py
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_scheduler.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/utils.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.html
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/schema/plugin.json
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/advanced-options.tsx
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/context.ts
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/handler.ts
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/hooks.ts
+-rw-r--r--   0        0        0    10605 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/index.tsx
+-rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/model.ts
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/notebook-jobs-panel.tsx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/size.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/svg.d.ts
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/theme-provider.ts
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/tokens.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/__tests__/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/box.tsx
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/button-bar.tsx
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/button.tsx
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/cluster.tsx
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/collapsible-panel.tsx
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/compute-type-picker.tsx
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/confirm-buttons.tsx
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/confirm-dialog-buttons.tsx
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/create-schedule-options.tsx
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/environment-picker.tsx
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/error-boundary.tsx
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/heading.tsx
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/icon-buttons.tsx
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/icons.ts
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/input-file-snapshot.tsx
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/job-definition-row.tsx
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/job-file-link.tsx
+-rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/job-row.tsx
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/labeled-value.tsx
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/output-format-picker.tsx
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/parameters-picker.tsx
+-rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/schedule-inputs.tsx
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/stack.tsx
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/advanced-table/advanced-table-header.tsx
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/advanced-table/advanced-table.tsx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/components/advanced-table/index.tsx
+-rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/mainviews/create-job-from-definition.tsx
+-rw-r--r--   0        0        0    20654 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/mainviews/create-job.tsx
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/mainviews/edit-job-definition.tsx
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/mainviews/list-jobs.tsx
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/mainviews/detail-view/detail-view.tsx
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/mainviews/detail-view/index.tsx
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/mainviews/detail-view/job-definition.tsx
+-rw-r--r--   0        0        0    10160 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/mainviews/detail-view/job-detail.tsx
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/util/errors.tsx
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/src/util/job-name-validation.tsx
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/base.css
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/box.css
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/button.css
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/cluster.css
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/collapsible-panel.css
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/edit-job-definitions.css
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/heading.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/index.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/labeled-value.css
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/stack.css
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/variables.css
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/icons/calendar-add-on.svg
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/icons/calendar-month.svg
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/style/icons/event-note.svg
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/.yarnrc
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/README.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/package.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   153944 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/helpers/SchedulerHelper.ts
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0    18992 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-filebrowser-linux.png
+-rw-r--r--   0        0        0    19577 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-toolbar-linux.png
+-rw-r--r--   0        0        0    19747 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/filebrowser-menu-linux.png
+-rw-r--r--   0        0        0    26873 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    22246 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/list-view-linux.png
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/notebook-toolbar-linux.png
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/LICENSE
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/README.md
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 jupyter_scheduler-2.5.1/PKG-INFO
```

### Comparing `jupyter_scheduler-2.5.0/.eslintrc.js` & `jupyter_scheduler-2.5.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/.pre-commit-config.yaml` & `jupyter_scheduler-2.5.1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       - id: check-yaml
       - id: debug-statements
       - id: forbid-new-submodules
       - id: check-builtin-literals
       - id: trailing-whitespace
 
   - repo: https://github.com/psf/black
-    rev: 23.12.1
+    rev: 24.2.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.13.2
     hooks:
       - id: isort
@@ -42,15 +42,15 @@
             "flake8-bugbear==20.1.4",
             "flake8-logging-format==0.6.0",
             "flake8-implicit-str-concat==0.2.0",
           ]
         stages: [manual]
 
   - repo: https://github.com/sirosen/check-jsonschema
-    rev: 0.27.3
+    rev: 0.28.0
     hooks:
       - id: check-jsonschema
         name: "Check GitHub Workflows"
         files: ^\.github/workflows/
         types: [yaml]
         args: ["--schemafile", "https://json.schemastore.org/github-workflow"]
         stages: [manual]
```

### Comparing `jupyter_scheduler-2.5.0/.stylelintrc` & `jupyter_scheduler-2.5.1/.stylelintrc`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/CHANGELOG.md` & `jupyter_scheduler-2.5.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 2.5.1
+
+([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v2.5.0...01fc2dca2a01673311abbaf970e0a80ee1368299))
+
+### Bugs fixed
+
+- Fix translator usage, remove @jupyterlab/rendermime-interfaces dependency [#483](https://github.com/jupyter-server/jupyter-scheduler/pull/483) ([@andrii-i](https://github.com/andrii-i))
+- Make server extension verification call during extension startup non-blocking [#480](https://github.com/jupyter-server/jupyter-scheduler/pull/480) ([@andrii-i](https://github.com/andrii-i))
+
+### Maintenance and upkeep improvements
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2024-01-23&to=2024-02-15&type=c))
+
+[@andrii-i](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Aandrii-i+updated%3A2024-01-23..2024-02-15&type=Issues) | [@dlqqq](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Adlqqq+updated%3A2024-01-23..2024-02-15&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Apre-commit-ci+updated%3A2024-01-23..2024-02-15&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 2.5.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v2.4.0...675dba6adaa4cec879c9b4c4e85c07020ee88519))
 
 ### Enhancements made
 
 - Emit telemetry events on success and failure of the Create Job, Create Job Definition, Create Job from Job Definition hooks [#472](https://github.com/jupyter-server/jupyter-scheduler/pull/472) ([@andrii-i](https://github.com/andrii-i))
@@ -16,16 +35,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2023-11-16&to=2024-01-23&type=c))
 
 [@andrii-i](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Aandrii-i+updated%3A2023-11-16..2024-01-23&type=Issues) | [@dependabot](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Adependabot+updated%3A2023-11-16..2024-01-23&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Apre-commit-ci+updated%3A2023-11-16..2024-01-23&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 2.4.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v2.3.0...caa3c1c75d6d03498972aec5bad0b67095a22f62))
 
 ### Enhancements made
 
 - Pydantic v1 and v2 compatibility, add `pydantic_v1` module [#463](https://github.com/jupyter-server/jupyter-scheduler/pull/463) ([@JasonWeill](https://github.com/JasonWeill))
```

### Comparing `jupyter_scheduler-2.5.0/MANIFEST.in` & `jupyter_scheduler-2.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/conftest.py` & `jupyter_scheduler-2.5.1/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jest.config.js` & `jupyter_scheduler-2.5.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/package.json` & `jupyter_scheduler-2.5.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'2.5.1'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.5.0"
+    "version": "2.5.1"
 }
```

### Comparing `jupyter_scheduler-2.5.0/tsconfig.json` & `jupyter_scheduler-2.5.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/yarn.lock` & `jupyter_scheduler-2.5.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/binder/postBuild` & `jupyter_scheduler-2.5.1/binder/postBuild`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/dev/seed.py` & `jupyter_scheduler-2.5.1/dev/seed.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/dev/templates/1.ipynb` & `jupyter_scheduler-2.5.1/dev/templates/1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/dev/templates/2.ipynb` & `jupyter_scheduler-2.5.1/dev/templates/2.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/dev/templates/3.ipynb` & `jupyter_scheduler-2.5.1/dev/templates/3.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/Makefile` & `jupyter_scheduler-2.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/conf.py` & `jupyter_scheduler-2.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/make.bat` & `jupyter_scheduler-2.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/_static/jupyter_logo.png` & `jupyter_scheduler-2.5.1/docs/_static/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/contributors/index.md` & `jupyter_scheduler-2.5.1/docs/contributors/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/developers/index.md` & `jupyter_scheduler-2.5.1/docs/developers/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/operators/index.md` & `jupyter_scheduler-2.5.1/docs/operators/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/index.md` & `jupyter_scheduler-2.5.1/docs/users/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/actions_definition_details.png` & `jupyter_scheduler-2.5.1/docs/users/images/actions_definition_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/actions_job_details.png` & `jupyter_scheduler-2.5.1/docs/users/images/actions_job_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/actions_list.png` & `jupyter_scheduler-2.5.1/docs/users/images/actions_list.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/create_job_form.png` & `jupyter_scheduler-2.5.1/docs/users/images/create_job_form.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/create_job_from_filebrowser.png` & `jupyter_scheduler-2.5.1/docs/users/images/create_job_from_filebrowser.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/create_job_from_notebook.png` & `jupyter_scheduler-2.5.1/docs/users/images/create_job_from_notebook.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/custom_schedule.png` & `jupyter_scheduler-2.5.1/docs/users/images/custom_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/download_button.png` & `jupyter_scheduler-2.5.1/docs/users/images/download_button.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/downloaded_files.png` & `jupyter_scheduler-2.5.1/docs/users/images/downloaded_files.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/headers.png` & `jupyter_scheduler-2.5.1/docs/users/images/headers.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/item_name.png` & `jupyter_scheduler-2.5.1/docs/users/images/item_name.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/launcher.png` & `jupyter_scheduler-2.5.1/docs/users/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/docs/users/images/run_on_schedule.png` & `jupyter_scheduler-2.5.1/docs/users/images/run_on_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/environments.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/environments.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/exceptions.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/executors.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/executors.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/extension.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/handlers.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/job_files_manager.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/job_files_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/models.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/models.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/orm.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/orm.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/parameterize.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/parameterize.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/scheduler.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/task_runner.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/task_runner.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/utils.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/package.json` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c7c7d5449715968d9006.js'}}",*

 * * "'version'": "'2.5.1'"}*

```diff
@@ -71,15 +71,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.43a78772e27d406d91b4.js",
+            "load": "static/remoteEntry.c7c7d5449715968d9006.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_scheduler"
                 },
@@ -141,9 +141,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.5.0"
+    "version": "2.5.1"
 }
```

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'2.5.1'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.5.0"
+    "version": "2.5.1"
 }
```

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/171.d4610e21027b29e7653a.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/171.d4610e21027b29e7653a.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/177.3502ccdd2c25548ad980.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/177.3502ccdd2c25548ad980.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/275.d7f03fdf77443bec5349.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/275.d7f03fdf77443bec5349.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/282.7b4e318dca2d64a434c1.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/282.7b4e318dca2d64a434c1.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/314.1b593fd6b3501a52cc35.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/314.37ac184c4c28a29ef5e6.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5,32 +5,32 @@
             n.r(t), n.d(t, {
                 CommandIDs: () => bt,
                 JobsView: () => E,
                 NotebookJobsPanelId: () => _t,
                 Scheduler: () => pt,
                 default: () => jt
             });
-            var o = n(4111),
-                a = n(5123),
-                l = n(7405),
-                r = n(6155),
-                i = n(5605),
-                s = n(2737),
-                c = n(1562),
+            var o = n(3247),
+                a = n(5162),
+                l = n(3226),
+                r = n(8138),
+                i = n(2544),
+                s = n(5352),
+                c = n(7186),
                 d = n(6029),
                 u = n.n(d),
                 m = n(296);
 
             function h(e) {
                 let t = "jp-jobs-Cluster";
                 return t += ` justify-content-${e.justifyContent||"flex-start"}`, t += ` align-items-${e.alignItems||"center"}`, t += ` gap-${e.gap||1}`, u().createElement("div", {
                     className: t
                 }, e.children)
             }
-            var p = n(2038);
+            var p = n(1386);
             const b = {
                 lineHeight: 0
             };
 
             function v(e) {
                 return u().createElement(m.IconButton, {
                     "aria-label": "delete",
@@ -292,15 +292,15 @@
                     name: "jupyterlab-scheduler:calendar-month",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 18" height="16px" width="16px">\n  <path fill="#0097A7" d="M10 12q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q10.312 12 10 12Zm-3.25 0q-.312 0-.531-.219Q6 11.562 6 11.25q0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q7.062 12 6.75 12Zm6.5 0q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531-.219.219-.531.219ZM10 15q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q10.312 15 10 15Zm-3.25 0q-.312 0-.531-.219Q6 14.562 6 14.25q0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q7.062 15 6.75 15Zm6.5 0q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531-.219.219-.531.219ZM4.5 18q-.625 0-1.062-.448Q3 17.104 3 16.5v-11q0-.604.438-1.052Q3.875 4 4.5 4H6V2h1.5v2h5V2H14v2h1.5q.625 0 1.062.448Q17 4.896 17 5.5v11q0 .604-.438 1.052Q16.125 18 15.5 18Zm0-1.5h11V9h-11v7.5Z"/>\n</svg>\n'
                 }),
                 I = new p.LabIcon({
                     name: "jupyterlab-scheduler:event-note",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 48 48" height="48" width="48">\n  <path fill="#0097A7" d="M14 27v-3h20v3Zm0 9v-3h13.95v3Zm-5 8q-1.2 0-2.1-.9Q6 42.2 6 41V10q0-1.2.9-2.1Q7.8 7 9 7h3.25V4h3.25v3h17V4h3.25v3H39q1.2 0 2.1.9.9.9.9 2.1v31q0 1.2-.9 2.1-.9.9-2.1.9Zm0-3h30V19.5H9V41Z"/>\n</svg>\n'
                 });
-            var O, T = n(6108);
+            var O, T = n(7261);
             class P {
                 constructor(e) {
                     this.serverSettings = e.serverSettings || s.ServerConnection.makeSettings()
                 }
                 serializeToQueryString(e) {
                     return "?" + Object.keys(e).map((t => {
                         if ("sort_by" === t) {
@@ -1700,15 +1700,15 @@
                         })))).catch((t => {
                             const n = pe(t);
                             e.setDisplayError(n)
                         }))
                     }
                 }, u().createElement(Je.Z, null))
             }
-            var Ie = n(3247),
+            var Ie = n(6555),
                 Oe = n(655),
                 Te = n(9144),
                 Pe = n(9557),
                 Le = n(7272);
 
             function $e(e) {
                 const t = e.job.create_time ? new Date(e.job.create_time) : null,
@@ -2955,28 +2955,34 @@
                 return t.pop(), t.join("/") + (t.length > 0 ? "/" : "")
             }
             const jt = [{
                 id: "@jupyterlab/scheduler:plugin",
                 requires: [l.IFileBrowserFactory, i.INotebookTracker, c.ITranslator, o.ILayoutRestorer, pt.IAdvancedOptions, pt.TelemetryHandler],
                 optional: [r.ILauncher],
                 autoStart: !0,
-                activate: async function(e, t, n, o, l, r, i, c) {
+                activate: function(e, t, n, o, l, r, i, c) {
                     const d = o.load("jupyterlab"),
                         u = new P({});
-                    try {
-                        await u.getJobs({
-                            max_items: 0
-                        })
-                    } catch (e) {
-                        if (e instanceof s.ServerConnection.ResponseError && 404 === e.response.status) return void(0, a.showDialog)({
-                            title: d.__("Jupyter Scheduler server extension not found"),
-                            body: he,
-                            buttons: [a.Dialog.okButton()]
-                        }).catch(console.warn)
-                    }
+                    !async function(e) {
+                        const t = e.translator.load("jupyterlab");
+                        try {
+                            await e.api.getJobs({
+                                max_items: 0
+                            })
+                        } catch (e) {
+                            if (e instanceof s.ServerConnection.ResponseError && 404 === e.response.status) return void(0, a.showDialog)({
+                                title: t.__("Jupyter Scheduler server extension not found"),
+                                body: he,
+                                buttons: [a.Dialog.okButton()]
+                            }).catch(console.warn)
+                        }
+                    }({
+                        api: u,
+                        translator: o
+                    });
                     const {
                         commands: m
                     } = e, h = t.tracker, p = new a.WidgetTracker({
                         namespace: "jupyterlab-scheduler"
                     });
                     let b, v;
                     l.restore(p, {
@@ -3139,15 +3145,15 @@
             var a = o(n(4938)),
                 l = n(5893),
                 r = (0, a.default)((0, l.jsx)("path", {
                     d: "M10 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V8c0-1.1-.9-2-2-2h-8l-2-2z"
                 }), "Folder");
             t.Z = r
         },
-        3247: (e, t, n) => {
+        6555: (e, t, n) => {
             "use strict";
             var o = n(5318);
             t.Z = void 0;
             var a = o(n(4938)),
                 l = n(5893),
                 r = (0, a.default)((0, l.jsx)("path", {
                     d: "M6 19h4V5H6v14zm8-14v14h4V5h-4z"
```

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/378.34aa286b24af0577a1ce.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/378.34aa286b24af0577a1ce.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/470.da7e4fe7177a2696e6be.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/506.7bbbaea2be6a025277aa.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/687.e4421b30aab66f8929fd.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/747.8e4a60162d1a81804893.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/747.8e4a60162d1a81804893.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/871.5c8b68996069b5cffa43.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/871.5c8b68996069b5cffa43.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/remoteEntry.43a78772e27d406d91b4.js` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/remoteEntry.c7c7d5449715968d9006.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, l, i, d, u, c, f, s, p, h, b, m, v, y, g, j, w = {
+    var e, r, t, a, n, o, l, i, d, u, c, f, s, p, b, h, m, v, y, g, j, w = {
             947: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(687), t.e(470), t.e(29), t.e(222), t.e(899), t.e(314)]).then((() => () => t(9314))),
                         "./extension": () => Promise.all([t.e(687), t.e(470), t.e(29), t.e(222), t.e(899), t.e(314)]).then((() => () => t(9314))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -51,15 +51,15 @@
         122: "b4ab1a65371e7c0f8bdd",
         171: "d4610e21027b29e7653a",
         177: "3502ccdd2c25548ad980",
         211: "67f62a30584499d40fa9",
         222: "1321ce1c143fee47b94a",
         275: "d7f03fdf77443bec5349",
         282: "7b4e318dca2d64a434c1",
-        314: "1b593fd6b3501a52cc35",
+        314: "37ac184c4c28a29ef5e6",
         378: "34aa286b24af0577a1ce",
         458: "d59c5307102faf5c19a8",
         470: "da7e4fe7177a2696e6be",
         506: "7bbbaea2be6a025277aa",
         613: "17512dda5aad1f2a390f",
         687: "e4421b30aab66f8929fd",
         747: "8e4a60162d1a81804893",
@@ -71,15 +71,15 @@
         122: "b4ab1a65371e7c0f8bdd",
         171: "d4610e21027b29e7653a",
         177: "3502ccdd2c25548ad980",
         211: "67f62a30584499d40fa9",
         222: "1321ce1c143fee47b94a",
         275: "d7f03fdf77443bec5349",
         282: "7b4e318dca2d64a434c1",
-        314: "1b593fd6b3501a52cc35",
+        314: "37ac184c4c28a29ef5e6",
         378: "34aa286b24af0577a1ce",
         458: "d59c5307102faf5c19a8",
         470: "da7e4fe7177a2696e6be",
         506: "7bbbaea2be6a025277aa",
         613: "17512dda5aad1f2a390f",
         687: "e4421b30aab66f8929fd",
         747: "8e4a60162d1a81804893",
@@ -141,15 +141,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@emotion/react", "11.10.4", (() => Promise.all([S.e(275), S.e(506), S.e(29), S.e(171)]).then((() => () => S(5506))))), i("@emotion/styled", "11.10.4", (() => Promise.all([S.e(378), S.e(29), S.e(211), S.e(799), S.e(122)]).then((() => () => S(4378))))), i("@jupyterlab/scheduler", "2.5.0", (() => Promise.all([S.e(687), S.e(470), S.e(29), S.e(222), S.e(899), S.e(314)]).then((() => () => S(9314))))), i("@mui/material", "5.10.6", (() => Promise.all([S.e(687), S.e(177), S.e(470), S.e(29), S.e(222), S.e(899)]).then((() => () => S(4177))))), i("@mui/system", "5.10.6", (() => Promise.all([S.e(275), S.e(687), S.e(871), S.e(29), S.e(211), S.e(222)]).then((() => () => S(1871))))), i("cronstrue", "2.12.0", (() => S.e(458).then((() => () => S(2458))))), i("tzdata", "1.0.33", (() => S.e(613).then((() => () => S(8613)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@emotion/react", "11.10.4", (() => Promise.all([S.e(275), S.e(506), S.e(29), S.e(171)]).then((() => () => S(5506))))), i("@emotion/styled", "11.10.4", (() => Promise.all([S.e(378), S.e(29), S.e(211), S.e(799), S.e(122)]).then((() => () => S(4378))))), i("@jupyterlab/scheduler", "2.5.1", (() => Promise.all([S.e(687), S.e(470), S.e(29), S.e(222), S.e(899), S.e(314)]).then((() => () => S(9314))))), i("@mui/material", "5.10.6", (() => Promise.all([S.e(687), S.e(177), S.e(470), S.e(29), S.e(222), S.e(899)]).then((() => () => S(4177))))), i("@mui/system", "5.10.6", (() => Promise.all([S.e(275), S.e(687), S.e(871), S.e(29), S.e(211), S.e(222)]).then((() => () => S(1871))))), i("cronstrue", "2.12.0", (() => S.e(458).then((() => () => S(2458))))), i("tzdata", "1.0.33", (() => S.e(613).then((() => () => S(8613)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -223,16 +223,16 @@
                     d = !1
                 } else "s" != f && "n" != f && (d = !1, i--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (l = 1; l < e.length; l++) {
-            var h = e[l];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            var b = e[l];
+            s.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? o(b, r) : !p())
         }
         return !!p()
     }, l = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, i = (e, r) => {
@@ -245,47 +245,47 @@
         var n = d(e, t);
         return o(a, n) || s(u(e, t, n, a)), p(e[t][n])
     }, f = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), b = (h = e => function(r, t, a, n) {
+    }, p = e => (e.loaded = 1, e.get()), h = (b = e => function(r, t, a, n) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, a, n)) : e(r, S.S[r], t, a, n)
-    })(((e, r, t, a) => r && S.o(r, t) ? p(i(r, t)) : a())), m = h(((e, r, t, a) => (l(e, t), c(r, 0, t, a)))), v = h(((e, r, t, a, n) => {
+    })(((e, r, t, a) => r && S.o(r, t) ? p(i(r, t)) : a())), m = b(((e, r, t, a) => (l(e, t), c(r, 0, t, a)))), v = b(((e, r, t, a, n) => {
         var o = r && S.o(r, t) && f(r, t, a);
         return o ? p(o) : n()
     })), y = {}, g = {
         6029: () => m("default", "react", [1, 18, 2, 0]),
         2148: () => v("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([S.e(275), S.e(506), S.e(282)]).then((() => () => S(5506))))),
         8800: () => v("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([S.e(378), S.e(211), S.e(799)]).then((() => () => S(4378))))),
         7313: () => v("default", "@mui/system", [1, 5, 10, 6], (() => Promise.all([S.e(275), S.e(871), S.e(211)]).then((() => () => S(1871))))),
         7704: () => m("default", "react-dom", [1, 18, 2, 0]),
         296: () => v("default", "@mui/material", [1, 5, 10, 6], (() => S.e(177).then((() => () => S(4177))))),
         763: () => v("default", "tzdata", [1, 1, 0, 33], (() => S.e(613).then((() => () => S(8613))))),
-        1562: () => m("default", "@jupyterlab/translation", [1, 4, 0, 11]),
-        2038: () => m("default", "@jupyterlab/ui-components", [1, 4, 0, 11]),
+        1386: () => m("default", "@jupyterlab/ui-components", [1, 4, 1, 1]),
         2344: () => v("default", "cronstrue", [1, 2, 12, 0], (() => S.e(458).then((() => () => S(2458))))),
-        2737: () => m("default", "@jupyterlab/services", [1, 7, 0, 11]),
-        4111: () => m("default", "@jupyterlab/application", [1, 4, 0, 11]),
+        2544: () => m("default", "@jupyterlab/notebook", [1, 4, 1, 1]),
+        3226: () => m("default", "@jupyterlab/filebrowser", [1, 4, 1, 1]),
+        3247: () => m("default", "@jupyterlab/application", [1, 4, 1, 1]),
         4901: () => m("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5123: () => m("default", "@jupyterlab/apputils", [1, 4, 1, 11]),
-        5605: () => m("default", "@jupyterlab/notebook", [1, 4, 0, 11]),
-        6108: () => m("default", "@jupyterlab/coreutils", [1, 6, 0, 11]),
-        6155: () => m("default", "@jupyterlab/launcher", [1, 4, 0, 11]),
-        7405: () => m("default", "@jupyterlab/filebrowser", [1, 4, 0, 11]),
+        5162: () => m("default", "@jupyterlab/apputils", [1, 4, 2, 1]),
+        5352: () => m("default", "@jupyterlab/services", [1, 7, 1, 1]),
+        7186: () => m("default", "@jupyterlab/translation", [1, 4, 1, 1]),
+        7261: () => m("default", "@jupyterlab/coreutils", [1, 6, 1, 1]),
         7930: () => m("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        5211: () => b("default", "@emotion/react", (() => Promise.all([S.e(275), S.e(506), S.e(282)]).then((() => () => S(5506))))),
+        8138: () => m("default", "@jupyterlab/launcher", [1, 4, 1, 1]),
+        5211: () => h("default", "@emotion/react", (() => Promise.all([S.e(275), S.e(506), S.e(282)]).then((() => () => S(5506))))),
         799: () => v("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([S.e(275), S.e(506)]).then((() => () => S(5506)))))
     }, j = {
         29: [6029],
         211: [5211],
         222: [2148, 8800],
-        314: [296, 763, 1562, 2038, 2344, 2737, 4111, 4901, 5123, 5605, 6108, 6155, 7405, 7930],
+        314: [296, 763, 1386, 2344, 2544, 3226, 3247, 4901, 5162, 5352, 7186, 7261, 7930, 8138],
         799: [799],
         899: [7313, 7704]
     }, S.f.consumes = (e, r) => {
         S.o(j, e) && j[e].forEach((e => {
             if (S.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, S.m[e] = t => {
```

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/labextension/static/third-party-licenses.json` & `jupyter_scheduler-2.5.1/jupyter_scheduler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/tests/mocks.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_handlers.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_job_files_manager.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_job_files_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_scheduler.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/tests/utils.py` & `jupyter_scheduler-2.5.1/jupyter_scheduler/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb` & `jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb` & `jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz` & `jupyter_scheduler-2.5.1/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/schema/plugin.json` & `jupyter_scheduler-2.5.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/advanced-options.tsx` & `jupyter_scheduler-2.5.1/src/advanced-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/handler.ts` & `jupyter_scheduler-2.5.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/index.tsx` & `jupyter_scheduler-2.5.1/src/index.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,40 @@
 
 type EventLog = {
   body: { name: string; detail?: string };
   timestamp: Date;
 };
 
 /**
+ * Call API to verify that the server extension is actually installed.
+ */
+async function verifyServerExtension(props: {
+  api: SchedulerService;
+  translator: ITranslator;
+}) {
+  const trans = props.translator.load('jupyterlab');
+  try {
+    await props.api.getJobs({ max_items: 0 });
+  } catch (e: unknown) {
+    // in case of 404, show missing server extension dialog and return
+    if (
+      e instanceof ServerConnection.ResponseError &&
+      e.response.status === 404
+    ) {
+      showDialog({
+        title: trans.__('Jupyter Scheduler server extension not found'),
+        body: SERVER_EXTENSION_404_JSX,
+        buttons: [Dialog.okButton()]
+      }).catch(console.warn);
+      return;
+    }
+  }
+}
+
+/**
  * Initialization data for the jupyterlab-scheduler extension.
  */
 const schedulerPlugin: JupyterFrontEndPlugin<void> = {
   id: '@jupyterlab/scheduler:plugin',
   requires: [
     IFileBrowserFactory,
     INotebookTracker,
@@ -134,44 +160,27 @@
   // Remove the final portion of the path, the filename.
   const directories = path.split('/');
   directories.pop();
   // Include a trailing slash only if there is at least one subdirectory.
   return directories.join('/') + (directories.length > 0 ? '/' : '');
 }
 
-async function activatePlugin(
+function activatePlugin(
   app: JupyterFrontEnd,
   browserFactory: IFileBrowserFactory,
   notebookTracker: INotebookTracker,
   translator: ITranslator,
   restorer: ILayoutRestorer,
   advancedOptions: Scheduler.IAdvancedOptions,
   telemetryHandler: Scheduler.TelemetryHandler,
   launcher: ILauncher | null
-): Promise<void> {
+): void {
   const trans = translator.load('jupyterlab');
   const api = new SchedulerService({});
-
-  // Call API to verify that the server extension is actually installed
-  try {
-    await api.getJobs({ max_items: 0 });
-  } catch (e: unknown) {
-    // in case of 404, show missing server extension dialog and return
-    if (
-      e instanceof ServerConnection.ResponseError &&
-      e.response.status === 404
-    ) {
-      showDialog({
-        title: trans.__('Jupyter Scheduler server extension not found'),
-        body: SERVER_EXTENSION_404_JSX,
-        buttons: [Dialog.okButton()]
-      }).catch(console.warn);
-      return;
-    }
-  }
+  verifyServerExtension({ api, translator });
 
   const { commands } = app;
   const fileBrowserTracker = browserFactory.tracker;
   const widgetTracker = new WidgetTracker<MainAreaWidget<NotebookJobsPanel>>({
     namespace: 'jupyterlab-scheduler'
   });
   restorer.restore(widgetTracker, {
```

### Comparing `jupyter_scheduler-2.5.0/src/model.ts` & `jupyter_scheduler-2.5.1/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/notebook-jobs-panel.tsx` & `jupyter_scheduler-2.5.1/src/notebook-jobs-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/theme-provider.ts` & `jupyter_scheduler-2.5.1/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/tokens.ts` & `jupyter_scheduler-2.5.1/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/cluster.tsx` & `jupyter_scheduler-2.5.1/src/components/cluster.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/collapsible-panel.tsx` & `jupyter_scheduler-2.5.1/src/components/collapsible-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/compute-type-picker.tsx` & `jupyter_scheduler-2.5.1/src/components/compute-type-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/confirm-buttons.tsx` & `jupyter_scheduler-2.5.1/src/components/confirm-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/confirm-dialog-buttons.tsx` & `jupyter_scheduler-2.5.1/src/components/confirm-dialog-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/create-schedule-options.tsx` & `jupyter_scheduler-2.5.1/src/components/create-schedule-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/environment-picker.tsx` & `jupyter_scheduler-2.5.1/src/components/environment-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/error-boundary.tsx` & `jupyter_scheduler-2.5.1/src/components/error-boundary.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/heading.tsx` & `jupyter_scheduler-2.5.1/src/components/heading.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/icon-buttons.tsx` & `jupyter_scheduler-2.5.1/src/components/icon-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/icons.ts` & `jupyter_scheduler-2.5.1/src/components/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/input-file-snapshot.tsx` & `jupyter_scheduler-2.5.1/src/components/input-file-snapshot.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/job-definition-row.tsx` & `jupyter_scheduler-2.5.1/src/components/job-definition-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/job-file-link.tsx` & `jupyter_scheduler-2.5.1/src/components/job-file-link.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/job-row.tsx` & `jupyter_scheduler-2.5.1/src/components/job-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/labeled-value.tsx` & `jupyter_scheduler-2.5.1/src/components/labeled-value.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/output-format-picker.tsx` & `jupyter_scheduler-2.5.1/src/components/output-format-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/parameters-picker.tsx` & `jupyter_scheduler-2.5.1/src/components/parameters-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/schedule-inputs.tsx` & `jupyter_scheduler-2.5.1/src/components/schedule-inputs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/advanced-table/advanced-table-header.tsx` & `jupyter_scheduler-2.5.1/src/components/advanced-table/advanced-table-header.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/components/advanced-table/advanced-table.tsx` & `jupyter_scheduler-2.5.1/src/components/advanced-table/advanced-table.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/mainviews/create-job-from-definition.tsx` & `jupyter_scheduler-2.5.1/src/mainviews/create-job-from-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/mainviews/create-job.tsx` & `jupyter_scheduler-2.5.1/src/mainviews/create-job.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/mainviews/edit-job-definition.tsx` & `jupyter_scheduler-2.5.1/src/mainviews/edit-job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/mainviews/list-jobs.tsx` & `jupyter_scheduler-2.5.1/src/mainviews/list-jobs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/mainviews/detail-view/detail-view.tsx` & `jupyter_scheduler-2.5.1/src/mainviews/detail-view/detail-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/mainviews/detail-view/job-definition.tsx` & `jupyter_scheduler-2.5.1/src/mainviews/detail-view/job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/mainviews/detail-view/job-detail.tsx` & `jupyter_scheduler-2.5.1/src/mainviews/detail-view/job-detail.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/util/errors.tsx` & `jupyter_scheduler-2.5.1/src/util/errors.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/src/util/job-name-validation.tsx` & `jupyter_scheduler-2.5.1/src/util/job-name-validation.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/style/base.css` & `jupyter_scheduler-2.5.1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/style/button.css` & `jupyter_scheduler-2.5.1/style/button.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/style/cluster.css` & `jupyter_scheduler-2.5.1/style/cluster.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/style/stack.css` & `jupyter_scheduler-2.5.1/style/stack.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/style/icons/calendar-add-on.svg` & `jupyter_scheduler-2.5.1/style/icons/calendar-add-on.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/style/icons/calendar-month.svg` & `jupyter_scheduler-2.5.1/style/icons/calendar-month.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/README.md` & `jupyter_scheduler-2.5.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/yarn.lock` & `jupyter_scheduler-2.5.1/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/helpers/SchedulerHelper.ts` & `jupyter_scheduler-2.5.1/ui-tests/helpers/SchedulerHelper.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts` & `jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-filebrowser-linux.png` & `jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-filebrowser-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-toolbar-linux.png` & `jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/create-view-from-toolbar-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/filebrowser-menu-linux.png` & `jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/filebrowser-menu-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/launcher-linux.png` & `jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/list-view-linux.png` & `jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/list-view-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/notebook-toolbar-linux.png` & `jupyter_scheduler-2.5.1/ui-tests/tests/jupyter_scheduler.spec.ts-snapshots/notebook-toolbar-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/.gitignore` & `jupyter_scheduler-2.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/LICENSE` & `jupyter_scheduler-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/README.md` & `jupyter_scheduler-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-2.5.0/pyproject.toml` & `jupyter_scheduler-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.3.1", "jupyterlab~=4.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_scheduler"
-version = "2.5.0"
+version = "2.5.1"
 description = "A JupyterLab extension for running notebook jobs"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "Project Jupyter" },
 ]
@@ -89,15 +89,15 @@
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
 build_cmd = "install:extension"
 npm = ["jlpm"]
 source_dir = "src"
 build_dir = "jupyter_scheduler/labextension"
 
 [tool.tbump.version]
-current = "2.5.0"
+current = "2.5.1"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [[tool.tbump.file]]
 src = "pyproject.toml"
 version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\""
 
 [[tool.tbump.file]]
```

### Comparing `jupyter_scheduler-2.5.0/PKG-INFO` & `jupyter_scheduler-2.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_scheduler
-Version: 2.5.0
+Version: 2.5.1
 Summary: A JupyterLab extension for running notebook jobs
 Project-URL: Homepage, https://github.com/jupyter-server/jupyter-scheduler
 Author: Project Jupyter
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Project Jupyter
         All rights reserved.
```

