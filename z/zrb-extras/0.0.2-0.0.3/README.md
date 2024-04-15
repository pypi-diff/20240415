# Comparing `tmp/zrb_extras-0.0.2.tar.gz` & `tmp/zrb_extras-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrb_extras-0.0.2.tar", max compression
+gzip compressed data, was "zrb_extras-0.0.3.tar", max compression
```

## Comparing `zrb_extras-0.0.2.tar` & `zrb_extras-0.0.3.tar`

### file list

```diff
@@ -1,210 +1,210 @@
--rw-r--r--   0        0        0     1790 2024-04-13 23:26:35.443542 zrb_extras-0.0.2/README.md
--rw-r--r--   0        0        0      771 2024-04-14 04:08:31.197276 zrb_extras-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       53 2024-04-14 03:20:57.674901 zrb_extras-0.0.2/src/zrb_extras/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 03:21:31.625909 zrb_extras-0.0.2/src/zrb_extras/__main__.py
--rw-r--r--   0        0        0       53 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/__init__.py
--rw-r--r--   0        0        0     1504 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/_input.py
--rw-r--r--   0        0        0     3094 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/airflow.py
--rw-r--r--   0        0        0      837 2024-04-14 03:32:50.073700 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/__init__.py
--rw-r--r--   0        0        0      405 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_constant.py
--rw-r--r--   0        0        0      847 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_env.py
--rw-r--r--   0        0        0      208 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_group.py
--rw-r--r--   0        0        0     1059 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_input.py
--rw-r--r--   0        0        0      334 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/activate-venv.sh
--rw-r--r--   0        0        0      386 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/__init__.py
--rw-r--r--   0        0        0      372 2024-04-14 03:51:08.228048 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/_env.py
--rw-r--r--   0        0        0      240 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/_group.py
--rw-r--r--   0        0        0      289 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/_service_config.py
--rw-r--r--   0        0        0     1157 2024-04-14 03:50:31.645663 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/init.py
--rw-r--r--   0        0        0      963 2024-04-14 03:50:31.645663 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/remove.py
--rw-r--r--   0        0        0     1685 2024-04-14 03:53:41.017291 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/start.py
--rw-r--r--   0        0        0      948 2024-04-14 03:50:31.645663 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/stop.py
--rw-r--r--   0        0        0     1335 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/deploy.py
--rw-r--r--   0        0        0       24 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/deploy.sh
--rw-r--r--   0        0        0     1161 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/destroy.py
--rw-r--r--   0        0        0       29 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/destroy.sh
--rw-r--r--   0        0        0      263 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/__init__.py
--rw-r--r--   0        0        0      154 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/_env.py
--rw-r--r--   0        0        0      228 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/_group.py
--rw-r--r--   0        0        0      233 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/_input.py
--rw-r--r--   0        0        0      902 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/build.py
--rw-r--r--   0        0        0      903 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/push.py
--rw-r--r--   0        0        0      126 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/init-pulumi-stack.sh
--rw-r--r--   0        0        0       36 2024-04-14 03:36:38.953378 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/.gitignore
--rw-r--r--   0        0        0       64 2024-04-14 03:34:06.897550 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/config/airflow.cfg
--rw-r--r--   0        0        0        0 2024-04-14 03:34:28.328202 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/dags/.gitkeep
--rw-r--r--   0        0        0       12 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/.gitignore
--rw-r--r--   0        0        0      137 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/Pulumi.yaml
--rw-r--r--   0        0        0      437 2024-04-14 04:04:53.528320 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/__main__.py
--rw-r--r--   0        0        0     1196 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/.helmignore
--rw-r--r--   0        0        0      227 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/Chart.lock
--rw-r--r--   0        0        0     2376 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/Chart.yaml
--rw-r--r--   0        0        0      468 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/INSTALL
--rw-r--r--   0        0        0    10850 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/LICENSE
--rw-r--r--   0        0        0      863 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/NOTICE
--rw-r--r--   0        0        0     2873 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/README.md
--rw-r--r--   0        0        0    40813 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/RELEASE_NOTES.rst
--rw-r--r--   0        0        0      333 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/.helmignore
--rw-r--r--   0        0        0      226 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/Chart.lock
--rw-r--r--   0        0        0     1076 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/Chart.yaml
--rw-r--r--   0        0        0   126691 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/README.md
--rw-r--r--   0        0        0      342 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/.helmignore
--rw-r--r--   0        0        0      531 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/Chart.yaml
--rw-r--r--   0        0        0     7119 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/README.md
--rw-r--r--   0        0        0     5480 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     7044 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1703 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     4071 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2431 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0     2147 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2497 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     7500 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      698 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0     1385 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2599 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0      650 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2644 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     4059 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4449 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     4003 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5091 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3334 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2526 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      182 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/values.yaml
--rw-r--r--   0        0        0     7852 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/NOTES.txt
--rw-r--r--   0        0        0    14792 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/_helpers.tpl
--rw-r--r--   0        0        0     5485 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/cronjob.yaml
--rw-r--r--   0        0        0     1617 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/pvc.yaml
--rw-r--r--   0        0        0      189 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/extra-list.yaml
--rw-r--r--   0        0        0     1366 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/networkpolicy-egress.yaml
--rw-r--r--   0        0        0     1047 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/configmap.yaml
--rw-r--r--   0        0        0      818 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/extended-configmap.yaml
--rw-r--r--   0        0        0      755 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/initialization-configmap.yaml
--rw-r--r--   0        0        0      690 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-configmap.yaml
--rw-r--r--   0        0        0     1418 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-svc.yaml
--rw-r--r--   0        0        0     3727 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/networkpolicy.yaml
--rw-r--r--   0        0        0     2314 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/servicemonitor.yaml
--rw-r--r--   0        0        0    36405 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/statefulset.yaml
--rw-r--r--   0        0        0     1827 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc-headless.yaml
--rw-r--r--   0        0        0     2883 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc.yaml
--rw-r--r--   0        0        0     1043 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1069 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/psp.yaml
--rw-r--r--   0        0        0      829 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/extended-configmap.yaml
--rw-r--r--   0        0        0      734 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-configmap.yaml
--rw-r--r--   0        0        0     1473 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-svc.yaml
--rw-r--r--   0        0        0     2390 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/networkpolicy.yaml
--rw-r--r--   0        0        0     2368 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/servicemonitor.yaml
--rw-r--r--   0        0        0    31450 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/statefulset.yaml
--rw-r--r--   0        0        0     1910 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc-headless.yaml
--rw-r--r--   0        0        0     3078 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc.yaml
--rw-r--r--   0        0        0     1077 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/role.yaml
--rw-r--r--   0        0        0      846 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/rolebinding.yaml
--rw-r--r--   0        0        0     5145 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/secrets.yaml
--rw-r--r--   0        0        0      837 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     1963 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/tls-secrets.yaml
--rw-r--r--   0        0        0     4571 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.schema.json
--rw-r--r--   0        0        0    74237 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.yaml
--rw-r--r--   0        0        0     1201 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/README.md
--rw-r--r--   0        0        0     3249 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/Dockerfile
--rw-r--r--   0        0        0     2432 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/build_and_push.sh
--rw-r--r--   0        0        0     2243 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/Dockerfile
--rw-r--r--   0        0        0     2466 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/build_and_push.sh
--rw-r--r--   0        0        0     6199 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/pod-template-file.kubernetes-helm-yaml
--rw-r--r--   0        0        0     2722 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/statsd-mappings.yml
--rw-r--r--   0        0        0     1084 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/37197.significant.rst
--rw-r--r--   0        0        0     1409 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/config.toml
--rw-r--r--   0        0        0       83 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/reproducible_build.yaml
--rw-r--r--   0        0        0     8276 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/NOTES.txt
--rw-r--r--   0        0        0    40339 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/_helpers.yaml
--rw-r--r--   0        0        0     2683 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/check-values.yaml
--rw-r--r--   0        0        0     4982 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-cronjob.yaml
--rw-r--r--   0        0        0     1582 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-serviceaccount.yaml
--rw-r--r--   0        0        0     2531 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/configmap.yaml
--rw-r--r--   0        0        0     1903 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/extra-configmaps.yaml
--rw-r--r--   0        0        0     1753 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/statsd-configmap.yaml
--rw-r--r--   0        0        0     1548 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/webserver-configmap.yaml
--rw-r--r--   0        0        0    13231 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-deployment.yaml
--rw-r--r--   0        0        0     1633 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-serviceaccount.yaml
--rw-r--r--   0        0        0     1888 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dags-persistent-volume-claim.yaml
--rw-r--r--   0        0        0     7836 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-deployment.yaml
--rw-r--r--   0        0        0     3276 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-ingress.yaml
--rw-r--r--   0        0        0     2098 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-networkpolicy.yaml
--rw-r--r--   0        0        0     2161 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-service.yaml
--rw-r--r--   0        0        0     1700 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-serviceaccount.yaml
--rw-r--r--   0        0        0     1692 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job-serviceaccount.yaml
--rw-r--r--   0        0        0     6153 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job.yaml
--rw-r--r--   0        0        0     1697 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job-serviceaccount.yaml
--rw-r--r--   0        0        0     6314 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job.yaml
--rw-r--r--   0        0        0     1312 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/limitrange.yaml
--rw-r--r--   0        0        0     1854 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/logs-persistent-volume-claim.yaml
--rw-r--r--   0        0        0     9469 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-deployment.yaml
--rw-r--r--   0        0        0     2818 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-networkpolicy.yaml
--rw-r--r--   0        0        0     1537 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-poddisruptionbudget.yaml
--rw-r--r--   0        0        0     1836 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-service.yaml
--rw-r--r--   0        0        0     1554 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-serviceaccount.yaml
--rw-r--r--   0        0        0     1400 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/priorityclasses/priority-classes.yaml
--rw-r--r--   0        0        0     1394 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-role.yaml
--rw-r--r--   0        0        0     1558 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-rolebinding.yaml
--rw-r--r--   0        0        0     2113 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-role.yaml
--rw-r--r--   0        0        0     2657 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-rolebinding.yaml
--rw-r--r--   0        0        0     1935 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-role.yaml
--rw-r--r--   0        0        0     2420 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-rolebinding.yaml
--rw-r--r--   0        0        0     3489 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/security-context-constraint-rolebinding.yaml
--rw-r--r--   0        0        0     2058 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-networkpolicy.yaml
--rw-r--r--   0        0        0     1595 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-service.yaml
--rw-r--r--   0        0        0     1619 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-serviceaccount.yaml
--rw-r--r--   0        0        0     5159 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-statefulset.yaml
--rw-r--r--   0        0        0     1322 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/resourcequota.yaml
--rw-r--r--   0        0        0    16802 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-deployment.yaml
--rw-r--r--   0        0        0     1892 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-networkpolicy.yaml
--rw-r--r--   0        0        0     1619 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-poddisruptionbudget.yaml
--rw-r--r--   0        0        0     1715 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-service.yaml
--rw-r--r--   0        0        0     1714 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-serviceaccount.yaml
--rw-r--r--   0        0        0     1765 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/elasticsearch-secret.yaml
--rw-r--r--   0        0        0     2083 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/extra-secrets.yaml
--rw-r--r--   0        0        0     1515 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/fernetkey-secret.yaml
--rw-r--r--   0        0        0     1368 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/flower-secret.yaml
--rw-r--r--   0        0        0     1332 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/kerberos-keytab-secret.yaml
--rw-r--r--   0        0        0     3280 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/metadata-connection-secret.yaml
--rw-r--r--   0        0        0     1600 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-certificates-secret.yaml
--rw-r--r--   0        0        0     1425 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-config-secret.yaml
--rw-r--r--   0        0        0     1712 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-stats-secret.yaml
--rw-r--r--   0        0        0     3084 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/redis-secrets.yaml
--rw-r--r--   0        0        0     1348 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/registry-secret.yaml
--rw-r--r--   0        0        0     2489 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/result-backend-connection-secret.yaml
--rw-r--r--   0        0        0     1494 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/webserver-secret-key-secret.yaml
--rw-r--r--   0        0        0     5423 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-deployment.yaml
--rw-r--r--   0        0        0     1880 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-networkpolicy.yaml
--rw-r--r--   0        0        0     1914 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-service.yaml
--rw-r--r--   0        0        0     1533 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-serviceaccount.yaml
--rw-r--r--   0        0        0    15260 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-deployment.yaml
--rw-r--r--   0        0        0     2266 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-kedaautoscaler.yaml
--rw-r--r--   0        0        0     1981 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-networkpolicy.yaml
--rw-r--r--   0        0        0     1760 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-service.yaml
--rw-r--r--   0        0        0     1690 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-serviceaccount.yaml
--rw-r--r--   0        0        0    14983 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-deployment.yaml
--rw-r--r--   0        0        0     3760 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-ingress.yaml
--rw-r--r--   0        0        0     2007 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-networkpolicy.yaml
--rw-r--r--   0        0        0     1619 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-poddisruptionbudget.yaml
--rw-r--r--   0        0        0     2081 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-service.yaml
--rw-r--r--   0        0        0     1634 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-serviceaccount.yaml
--rw-r--r--   0        0        0    22362 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-deployment.yaml
--rw-r--r--   0        0        0     2015 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-hpa.yaml
--rw-r--r--   0        0        0     2674 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-kedaautoscaler.yaml
--rw-r--r--   0        0        0     1865 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-networkpolicy.yaml
--rw-r--r--   0        0        0     1656 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-service.yaml
--rw-r--r--   0        0        0     1761 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-serviceaccount.yaml
--rw-r--r--   0        0        0   534941 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.schema.json
--rw-r--r--   0        0        0    77957 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.yaml
--rw-r--r--   0        0        0     3242 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values_schema.schema.json
--rw-r--r--   0        0        0       74 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/state/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/template.env
--rw-r--r--   0        0        0       68 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/docker-compose.env
--rw-r--r--   0        0        0     9762 2024-04-14 03:53:41.017291 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/docker-compose.yml
--rw-r--r--   0        0        0       22 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/.dockerignore
--rw-r--r--   0        0        0       23 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/.gitignore
--rw-r--r--   0        0        0      101 2024-04-14 03:28:18.708296 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/Dockerfile
--rw-r--r--   0        0        0       57 2024-04-14 03:33:11.668826 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/requirements.txt
--rw-r--r--   0        0        0       87 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/template.env
--rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 zrb_extras-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1790 2024-04-15 09:18:50.119439 zrb_extras-0.0.3/README.md
+-rw-r--r--   0        0        0      771 2024-04-15 13:35:20.544350 zrb_extras-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       53 2024-04-15 09:18:50.129438 zrb_extras-0.0.3/src/zrb_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:18:50.129438 zrb_extras-0.0.3/src/zrb_extras/__main__.py
+-rw-r--r--   0        0        0       53 2024-04-15 09:18:50.139437 zrb_extras-0.0.3/src/zrb_extras/airflow/__init__.py
+-rw-r--r--   0        0        0     1504 2024-04-15 09:18:50.139437 zrb_extras-0.0.3/src/zrb_extras/airflow/_input.py
+-rw-r--r--   0        0        0     3082 2024-04-15 12:51:37.123872 zrb_extras-0.0.3/src/zrb_extras/airflow/airflow.py
+-rw-r--r--   0        0        0      837 2024-04-15 09:18:50.149435 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-15 09:18:50.199428 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_constant.py
+-rw-r--r--   0        0        0      847 2024-04-15 09:18:50.159434 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_env.py
+-rw-r--r--   0        0        0      208 2024-04-15 09:18:50.159434 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_group.py
+-rw-r--r--   0        0        0     1059 2024-04-15 09:18:50.149435 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_input.py
+-rw-r--r--   0        0        0      334 2024-04-15 09:18:50.179431 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/activate-venv.sh
+-rw-r--r--   0        0        0      386 2024-04-15 09:18:50.169432 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-15 09:18:50.169432 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/_env.py
+-rw-r--r--   0        0        0      240 2024-04-15 09:18:50.169432 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/_group.py
+-rw-r--r--   0        0        0      289 2024-04-15 09:18:50.179431 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/_service_config.py
+-rw-r--r--   0        0        0     1157 2024-04-15 09:18:50.179431 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/init.py
+-rw-r--r--   0        0        0      963 2024-04-15 09:18:50.179431 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/remove.py
+-rw-r--r--   0        0        0     1685 2024-04-15 09:18:50.169432 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/start.py
+-rw-r--r--   0        0        0      948 2024-04-15 09:18:50.169432 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/stop.py
+-rw-r--r--   0        0        0     1335 2024-04-15 09:18:50.159434 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/deploy.py
+-rw-r--r--   0        0        0       24 2024-04-15 09:18:50.179431 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/deploy.sh
+-rw-r--r--   0        0        0     1161 2024-04-15 09:18:50.159434 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/destroy.py
+-rw-r--r--   0        0        0       29 2024-04-15 09:18:50.189430 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/destroy.sh
+-rw-r--r--   0        0        0      263 2024-04-15 09:18:50.189430 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-15 09:18:50.189430 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/_env.py
+-rw-r--r--   0        0        0      228 2024-04-15 09:18:50.189430 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/_group.py
+-rw-r--r--   0        0        0      233 2024-04-15 09:18:50.189430 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/_input.py
+-rw-r--r--   0        0        0      902 2024-04-15 09:18:50.199428 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/build.py
+-rw-r--r--   0        0        0      903 2024-04-15 09:18:50.189430 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/push.py
+-rw-r--r--   0        0        0      126 2024-04-15 09:18:50.149435 zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/init-pulumi-stack.sh
+-rw-r--r--   0        0        0       36 2024-04-15 09:18:50.529384 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/.gitignore
+-rw-r--r--   0        0        0       64 2024-04-15 09:18:50.529384 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/config/airflow.cfg
+-rw-r--r--   0        0        0        0 2024-04-15 09:18:50.199428 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/dags/.gitkeep
+-rw-r--r--   0        0        0       12 2024-04-15 09:18:50.509387 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/.gitignore
+-rw-r--r--   0        0        0      137 2024-04-15 09:18:50.209427 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/Pulumi.yaml
+-rw-r--r--   0        0        0      436 2024-04-15 09:18:50.199428 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/__main__.py
+-rw-r--r--   0        0        0     1196 2024-04-15 09:18:50.219426 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/.helmignore
+-rw-r--r--   0        0        0      227 2024-04-15 09:18:50.219426 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/Chart.lock
+-rw-r--r--   0        0        0     2376 2024-04-15 09:18:50.219426 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/Chart.yaml
+-rw-r--r--   0        0        0      468 2024-04-15 09:18:50.489390 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/INSTALL
+-rw-r--r--   0        0        0    10850 2024-04-15 09:18:50.219426 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/LICENSE
+-rw-r--r--   0        0        0      863 2024-04-15 09:18:50.499388 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/NOTICE
+-rw-r--r--   0        0        0     2873 2024-04-15 09:18:50.339410 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/README.md
+-rw-r--r--   0        0        0    40813 2024-04-15 09:18:50.489390 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/RELEASE_NOTES.rst
+-rw-r--r--   0        0        0      333 2024-04-15 09:18:50.229425 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/.helmignore
+-rw-r--r--   0        0        0      226 2024-04-15 09:18:50.229425 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/Chart.lock
+-rw-r--r--   0        0        0     1076 2024-04-15 09:18:50.229425 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/Chart.yaml
+-rw-r--r--   0        0        0   126691 2024-04-15 09:18:50.279418 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/README.md
+-rw-r--r--   0        0        0      342 2024-04-15 09:18:50.239423 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/.helmignore
+-rw-r--r--   0        0        0      531 2024-04-15 09:18:50.239423 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/Chart.yaml
+-rw-r--r--   0        0        0     7119 2024-04-15 09:18:50.239423 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/README.md
+-rw-r--r--   0        0        0     5480 2024-04-15 09:18:50.249422 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_affinities.tpl
+-rw-r--r--   0        0        0     7044 2024-04-15 09:18:50.249422 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_capabilities.tpl
+-rw-r--r--   0        0        0     1703 2024-04-15 09:18:50.269419 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_errors.tpl
+-rw-r--r--   0        0        0     4071 2024-04-15 09:18:50.249422 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_images.tpl
+-rw-r--r--   0        0        0     2431 2024-04-15 09:18:50.269419 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_ingress.tpl
+-rw-r--r--   0        0        0     2147 2024-04-15 09:18:50.239423 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_labels.tpl
+-rw-r--r--   0        0        0     2497 2024-04-15 09:18:50.249422 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_names.tpl
+-rw-r--r--   0        0        0     7500 2024-04-15 09:18:50.269419 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_secrets.tpl
+-rw-r--r--   0        0        0      698 2024-04-15 09:18:50.269419 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_storage.tpl
+-rw-r--r--   0        0        0     1385 2024-04-15 09:18:50.249422 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_tplvalues.tpl
+-rw-r--r--   0        0        0     2599 2024-04-15 09:18:50.269419 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_utils.tpl
+-rw-r--r--   0        0        0      650 2024-04-15 09:18:50.279418 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_warnings.tpl
+-rw-r--r--   0        0        0     2644 2024-04-15 09:18:50.259420 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_cassandra.tpl
+-rw-r--r--   0        0        0     4059 2024-04-15 09:18:50.259420 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mariadb.tpl
+-rw-r--r--   0        0        0     4449 2024-04-15 09:18:50.269419 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mongodb.tpl
+-rw-r--r--   0        0        0     4003 2024-04-15 09:18:50.249422 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mysql.tpl
+-rw-r--r--   0        0        0     5091 2024-04-15 09:18:50.259420 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_postgresql.tpl
+-rw-r--r--   0        0        0     3334 2024-04-15 09:18:50.259420 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_redis.tpl
+-rw-r--r--   0        0        0     2526 2024-04-15 09:18:50.259420 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_validations.tpl
+-rw-r--r--   0        0        0      182 2024-04-15 09:18:50.239423 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/values.yaml
+-rw-r--r--   0        0        0     7852 2024-04-15 09:18:50.289416 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/NOTES.txt
+-rw-r--r--   0        0        0    14792 2024-04-15 09:18:50.279418 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/_helpers.tpl
+-rw-r--r--   0        0        0     5485 2024-04-15 09:18:50.289416 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/cronjob.yaml
+-rw-r--r--   0        0        0     1617 2024-04-15 09:18:50.289416 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/pvc.yaml
+-rw-r--r--   0        0        0      189 2024-04-15 09:18:50.309414 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/extra-list.yaml
+-rw-r--r--   0        0        0     1366 2024-04-15 09:18:50.299415 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/networkpolicy-egress.yaml
+-rw-r--r--   0        0        0     1047 2024-04-15 09:18:50.329411 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/configmap.yaml
+-rw-r--r--   0        0        0      818 2024-04-15 09:18:50.319413 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/extended-configmap.yaml
+-rw-r--r--   0        0        0      755 2024-04-15 09:18:50.339410 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/initialization-configmap.yaml
+-rw-r--r--   0        0        0      690 2024-04-15 09:18:50.329411 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-configmap.yaml
+-rw-r--r--   0        0        0     1418 2024-04-15 09:18:50.339410 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-svc.yaml
+-rw-r--r--   0        0        0     3727 2024-04-15 09:18:50.319413 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/networkpolicy.yaml
+-rw-r--r--   0        0        0     2314 2024-04-15 09:18:50.329411 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/servicemonitor.yaml
+-rw-r--r--   0        0        0    36405 2024-04-15 09:18:50.329411 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/statefulset.yaml
+-rw-r--r--   0        0        0     1827 2024-04-15 09:18:50.329411 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc-headless.yaml
+-rw-r--r--   0        0        0     2883 2024-04-15 09:18:50.329411 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc.yaml
+-rw-r--r--   0        0        0     1043 2024-04-15 09:18:50.289416 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1069 2024-04-15 09:18:50.299415 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/psp.yaml
+-rw-r--r--   0        0        0      829 2024-04-15 09:18:50.309414 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/extended-configmap.yaml
+-rw-r--r--   0        0        0      734 2024-04-15 09:18:50.319413 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-configmap.yaml
+-rw-r--r--   0        0        0     1473 2024-04-15 09:18:50.319413 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-svc.yaml
+-rw-r--r--   0        0        0     2390 2024-04-15 09:18:50.309414 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/networkpolicy.yaml
+-rw-r--r--   0        0        0     2368 2024-04-15 09:18:50.309414 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/servicemonitor.yaml
+-rw-r--r--   0        0        0    31450 2024-04-15 09:18:50.319413 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/statefulset.yaml
+-rw-r--r--   0        0        0     1910 2024-04-15 09:18:50.309414 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc-headless.yaml
+-rw-r--r--   0        0        0     3078 2024-04-15 09:18:50.309414 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc.yaml
+-rw-r--r--   0        0        0     1077 2024-04-15 09:18:50.339410 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/role.yaml
+-rw-r--r--   0        0        0      846 2024-04-15 09:18:50.299415 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/rolebinding.yaml
+-rw-r--r--   0        0        0     5145 2024-04-15 09:18:50.299415 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/secrets.yaml
+-rw-r--r--   0        0        0      837 2024-04-15 09:18:50.289416 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     1963 2024-04-15 09:18:50.279418 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/tls-secrets.yaml
+-rw-r--r--   0        0        0     4571 2024-04-15 09:18:50.339410 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.schema.json
+-rw-r--r--   0        0        0    74237 2024-04-15 09:18:50.229425 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.yaml
+-rw-r--r--   0        0        0     1201 2024-04-15 09:18:50.509387 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/README.md
+-rw-r--r--   0        0        0     3249 2024-04-15 09:18:50.499388 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/Dockerfile
+-rw-r--r--   0        0        0     2432 2024-04-15 09:18:50.499388 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/build_and_push.sh
+-rw-r--r--   0        0        0     2243 2024-04-15 09:18:50.499388 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/Dockerfile
+-rw-r--r--   0        0        0     2466 2024-04-15 09:18:50.509387 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/build_and_push.sh
+-rw-r--r--   0        0        0     6199 2024-04-15 09:18:50.499388 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/pod-template-file.kubernetes-helm-yaml
+-rw-r--r--   0        0        0     2722 2024-04-15 09:18:50.499388 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/statsd-mappings.yml
+-rw-r--r--   0        0        0     1084 2024-04-15 09:18:50.489390 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/37197.significant.rst
+-rw-r--r--   0        0        0     1409 2024-04-15 09:18:50.489390 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/config.toml
+-rw-r--r--   0        0        0       83 2024-04-15 09:18:50.219426 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/reproducible_build.yaml
+-rw-r--r--   0        0        0     8276 2024-04-15 09:18:50.379404 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/NOTES.txt
+-rw-r--r--   0        0        0    40339 2024-04-15 09:18:50.469392 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/_helpers.yaml
+-rw-r--r--   0        0        0     2683 2024-04-15 09:18:50.489390 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/check-values.yaml
+-rw-r--r--   0        0        0     4982 2024-04-15 09:18:50.379404 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-cronjob.yaml
+-rw-r--r--   0        0        0     1582 2024-04-15 09:18:50.379404 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-serviceaccount.yaml
+-rw-r--r--   0        0        0     2531 2024-04-15 09:18:50.469392 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/configmap.yaml
+-rw-r--r--   0        0        0     1903 2024-04-15 09:18:50.459394 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/extra-configmaps.yaml
+-rw-r--r--   0        0        0     1753 2024-04-15 09:18:50.459394 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/statsd-configmap.yaml
+-rw-r--r--   0        0        0     1548 2024-04-15 09:18:50.459394 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/webserver-configmap.yaml
+-rw-r--r--   0        0        0    13231 2024-04-15 09:18:50.479391 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-deployment.yaml
+-rw-r--r--   0        0        0     1633 2024-04-15 09:18:50.469392 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-serviceaccount.yaml
+-rw-r--r--   0        0        0     1888 2024-04-15 09:18:50.379404 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dags-persistent-volume-claim.yaml
+-rw-r--r--   0        0        0     7836 2024-04-15 09:18:50.379404 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-deployment.yaml
+-rw-r--r--   0        0        0     3276 2024-04-15 09:18:50.369406 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-ingress.yaml
+-rw-r--r--   0        0        0     2098 2024-04-15 09:18:50.369406 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-networkpolicy.yaml
+-rw-r--r--   0        0        0     2161 2024-04-15 09:18:50.369406 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-service.yaml
+-rw-r--r--   0        0        0     1700 2024-04-15 09:18:50.369406 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-serviceaccount.yaml
+-rw-r--r--   0        0        0     1692 2024-04-15 09:18:50.389403 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job-serviceaccount.yaml
+-rw-r--r--   0        0        0     6153 2024-04-15 09:18:50.399402 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job.yaml
+-rw-r--r--   0        0        0     1697 2024-04-15 09:18:50.399402 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job-serviceaccount.yaml
+-rw-r--r--   0        0        0     6314 2024-04-15 09:18:50.399402 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job.yaml
+-rw-r--r--   0        0        0     1312 2024-04-15 09:18:50.469392 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/limitrange.yaml
+-rw-r--r--   0        0        0     1854 2024-04-15 09:18:50.469392 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/logs-persistent-volume-claim.yaml
+-rw-r--r--   0        0        0     9469 2024-04-15 09:18:50.389403 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-deployment.yaml
+-rw-r--r--   0        0        0     2818 2024-04-15 09:18:50.389403 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-networkpolicy.yaml
+-rw-r--r--   0        0        0     1537 2024-04-15 09:18:50.389403 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-poddisruptionbudget.yaml
+-rw-r--r--   0        0        0     1836 2024-04-15 09:18:50.379404 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-service.yaml
+-rw-r--r--   0        0        0     1554 2024-04-15 09:18:50.389403 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-serviceaccount.yaml
+-rw-r--r--   0        0        0     1400 2024-04-15 09:18:50.429398 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/priorityclasses/priority-classes.yaml
+-rw-r--r--   0        0        0     1394 2024-04-15 09:18:50.349408 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-role.yaml
+-rw-r--r--   0        0        0     1558 2024-04-15 09:18:50.349408 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-rolebinding.yaml
+-rw-r--r--   0        0        0     2113 2024-04-15 09:18:50.349408 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-role.yaml
+-rw-r--r--   0        0        0     2657 2024-04-15 09:18:50.349408 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-rolebinding.yaml
+-rw-r--r--   0        0        0     1935 2024-04-15 09:18:50.349408 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-role.yaml
+-rw-r--r--   0        0        0     2420 2024-04-15 09:18:50.349408 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-rolebinding.yaml
+-rw-r--r--   0        0        0     3489 2024-04-15 09:18:50.349408 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/security-context-constraint-rolebinding.yaml
+-rw-r--r--   0        0        0     2058 2024-04-15 09:18:50.409400 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-networkpolicy.yaml
+-rw-r--r--   0        0        0     1595 2024-04-15 09:18:50.399402 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-service.yaml
+-rw-r--r--   0        0        0     1619 2024-04-15 09:18:50.409400 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-serviceaccount.yaml
+-rw-r--r--   0        0        0     5159 2024-04-15 09:18:50.399402 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-statefulset.yaml
+-rw-r--r--   0        0        0     1322 2024-04-15 09:18:50.359407 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/resourcequota.yaml
+-rw-r--r--   0        0        0    16802 2024-04-15 09:18:50.419399 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-deployment.yaml
+-rw-r--r--   0        0        0     1892 2024-04-15 09:18:50.419399 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-networkpolicy.yaml
+-rw-r--r--   0        0        0     1619 2024-04-15 09:18:50.419399 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-poddisruptionbudget.yaml
+-rw-r--r--   0        0        0     1715 2024-04-15 09:18:50.419399 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-service.yaml
+-rw-r--r--   0        0        0     1714 2024-04-15 09:18:50.419399 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-serviceaccount.yaml
+-rw-r--r--   0        0        0     1765 2024-04-15 09:18:50.459394 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/elasticsearch-secret.yaml
+-rw-r--r--   0        0        0     2083 2024-04-15 09:18:50.439396 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/extra-secrets.yaml
+-rw-r--r--   0        0        0     1515 2024-04-15 09:18:50.449395 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/fernetkey-secret.yaml
+-rw-r--r--   0        0        0     1368 2024-04-15 09:18:50.449395 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/flower-secret.yaml
+-rw-r--r--   0        0        0     1332 2024-04-15 09:18:50.449395 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/kerberos-keytab-secret.yaml
+-rw-r--r--   0        0        0     3280 2024-04-15 09:18:50.449395 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/metadata-connection-secret.yaml
+-rw-r--r--   0        0        0     1600 2024-04-15 09:18:50.439396 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-certificates-secret.yaml
+-rw-r--r--   0        0        0     1425 2024-04-15 09:18:50.439396 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-config-secret.yaml
+-rw-r--r--   0        0        0     1712 2024-04-15 09:18:50.449395 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-stats-secret.yaml
+-rw-r--r--   0        0        0     3084 2024-04-15 09:18:50.439396 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/redis-secrets.yaml
+-rw-r--r--   0        0        0     1348 2024-04-15 09:18:50.439396 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/registry-secret.yaml
+-rw-r--r--   0        0        0     2489 2024-04-15 09:18:50.459394 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/result-backend-connection-secret.yaml
+-rw-r--r--   0        0        0     1494 2024-04-15 09:18:50.459394 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/webserver-secret-key-secret.yaml
+-rw-r--r--   0        0        0     5423 2024-04-15 09:18:50.419399 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-deployment.yaml
+-rw-r--r--   0        0        0     1880 2024-04-15 09:18:50.409400 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-networkpolicy.yaml
+-rw-r--r--   0        0        0     1914 2024-04-15 09:18:50.409400 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-service.yaml
+-rw-r--r--   0        0        0     1533 2024-04-15 09:18:50.409400 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-serviceaccount.yaml
+-rw-r--r--   0        0        0    15260 2024-04-15 09:18:50.429398 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-deployment.yaml
+-rw-r--r--   0        0        0     2266 2024-04-15 09:18:50.429398 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-kedaautoscaler.yaml
+-rw-r--r--   0        0        0     1981 2024-04-15 09:18:50.429398 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-networkpolicy.yaml
+-rw-r--r--   0        0        0     1760 2024-04-15 09:18:50.439396 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-service.yaml
+-rw-r--r--   0        0        0     1690 2024-04-15 09:18:50.429398 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-serviceaccount.yaml
+-rw-r--r--   0        0        0    14983 2024-04-15 09:18:50.489390 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-deployment.yaml
+-rw-r--r--   0        0        0     3760 2024-04-15 09:18:50.479391 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-ingress.yaml
+-rw-r--r--   0        0        0     2007 2024-04-15 09:18:50.479391 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-networkpolicy.yaml
+-rw-r--r--   0        0        0     1619 2024-04-15 09:18:50.479391 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-poddisruptionbudget.yaml
+-rw-r--r--   0        0        0     2081 2024-04-15 09:18:50.479391 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-service.yaml
+-rw-r--r--   0        0        0     1634 2024-04-15 09:18:50.479391 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-serviceaccount.yaml
+-rw-r--r--   0        0        0    22362 2024-04-15 09:18:50.359407 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-deployment.yaml
+-rw-r--r--   0        0        0     2015 2024-04-15 09:18:50.359407 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-hpa.yaml
+-rw-r--r--   0        0        0     2674 2024-04-15 09:18:50.359407 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-kedaautoscaler.yaml
+-rw-r--r--   0        0        0     1865 2024-04-15 09:18:50.369406 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-networkpolicy.yaml
+-rw-r--r--   0        0        0     1656 2024-04-15 09:18:50.369406 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-service.yaml
+-rw-r--r--   0        0        0     1761 2024-04-15 09:18:50.359407 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-serviceaccount.yaml
+-rw-r--r--   0        0        0   534941 2024-04-15 09:18:50.509387 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.schema.json
+-rw-r--r--   0        0        0    77957 2024-04-15 09:18:50.209427 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.yaml
+-rw-r--r--   0        0        0     3242 2024-04-15 09:18:50.209427 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values_schema.schema.json
+-rw-r--r--   0        0        0       74 2024-04-15 09:18:50.209427 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-15 09:18:50.209427 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/state/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-15 09:18:50.199428 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/template.env
+-rw-r--r--   0        0        0       68 2024-04-15 09:18:50.529384 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/docker-compose.env
+-rw-r--r--   0        0        0    10006 2024-04-15 13:29:45.791559 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/docker-compose.yml
+-rw-r--r--   0        0        0       22 2024-04-15 09:18:50.519386 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/.dockerignore
+-rw-r--r--   0        0        0       23 2024-04-15 09:18:50.519386 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/.gitignore
+-rw-r--r--   0        0        0      101 2024-04-15 09:18:50.519386 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/Dockerfile
+-rw-r--r--   0        0        0       57 2024-04-15 09:18:50.519386 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/requirements.txt
+-rw-r--r--   0        0        0       87 2024-04-15 09:18:50.519386 zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/template.env
+-rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 zrb_extras-0.0.3/PKG-INFO
```

### Comparing `zrb_extras-0.0.2/README.md` & `zrb_extras-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/pyproject.toml` & `zrb_extras-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zrb-extras"
-version = "0.0.2"
+version = "0.0.3"
 description = "Collection of Zrb additional utilities"
 authors = ["Go Frendi Gunawan <gofrendiasgard@gmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/goFrendiAsgard/zrb-extras"
 repository = "https://github.com/goFrendiAsgard/zrb-extras"
 documentation = "https://github.com/goFrendiAsgard/zrb-extras"
```

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/_input.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/_input.py`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/airflow.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/airflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from zrb.builtin.project._helper import (
     create_register_module,
     validate_existing_project_dir,
     validate_inexisting_automation,
 )
 from zrb.builtin.project._input import project_dir_input
-from zrb.builtin.project.add.app._group import project_add_app_group
+from zrb.builtin.project.add._group import project_add_group
 from zrb.helper.accessories.color import colored
 from zrb.helper.typing import Any
 from zrb.helper.util import to_kebab_case
 from zrb.runner import runner
 from zrb.task.decorator import python_task
 from zrb.task.resource_maker import ResourceMaker
 from zrb.task.task import Task
@@ -79,15 +79,15 @@
     inputs=[app_name_input],
     upstreams=[copy_resource],
 )
 
 
 @python_task(
     name="airflow",
-    group=project_add_app_group,
+    group=project_add_group,
     description="Add airflow",
     inputs=[
         project_dir_input,
         app_name_input,
         app_description_input,
         app_author_name_input,
         app_author_email_input,
```

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/__init__.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/__init__.py`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_env.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_env.py`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_input.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_input.py`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/init.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/init.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from zrb import DockerComposeTask
 
 from .._constant import RESOURCE_DIR
 from .._input import host_input, local_input
 from ..image import build_snake_zrb_app_name_image
 from ..image._env import image_env
 from ..image._input import image_input
-from ._env import compose_env_file, airflow_webserver_port_env
+from ._env import airflow_webserver_port_env, compose_env_file
 from ._group import snake_zrb_app_name_container_group
 from ._service_config import snake_zrb_app_name_service_config
 from .remove import remove_snake_zrb_app_name_container
 
 init_snake_zrb_app_name_container = DockerComposeTask(
     icon="🔥",
     name="init",
```

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/remove.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/remove.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from zrb import DockerComposeTask, runner
 
 from ..._project import remove_project_containers
 from .._constant import RESOURCE_DIR
 from ..image._env import image_env
-from ._env import compose_env_file, airflow_webserver_port_env
+from ._env import airflow_webserver_port_env, compose_env_file
 from ._group import snake_zrb_app_name_container_group
 from ._service_config import snake_zrb_app_name_service_config
 
 remove_snake_zrb_app_name_container = DockerComposeTask(
     icon="💨",
     name="remove",
     description="Remove human readable zrb app name container",
```

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/start.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/start.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from zrb import DockerComposeTask, HTTPChecker, runner
 
-from ..._project import start_project_containers, start_project
+from ..._project import start_project, start_project_containers
 from .._constant import RESOURCE_DIR
 from .._input import host_input, https_input, local_input
 from ..image._env import image_env
 from ..image._input import image_input
-from ._env import compose_env_file, airflow_webserver_port_env
+from ._env import airflow_webserver_port_env, compose_env_file
 from ._group import snake_zrb_app_name_container_group
 from ._service_config import snake_zrb_app_name_service_config
 from .init import init_snake_zrb_app_name_container
 
 start_snake_zrb_app_name_container = DockerComposeTask(
     icon="🐳",
     name="start",
```

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/stop.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/stop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from zrb import DockerComposeTask, runner
 
 from ..._project import stop_project_containers
 from .._constant import RESOURCE_DIR
 from ..image._env import image_env
-from ._env import compose_env_file, airflow_webserver_port_env
+from ._env import airflow_webserver_port_env, compose_env_file
 from ._group import snake_zrb_app_name_container_group
 from ._service_config import snake_zrb_app_name_service_config
 
 stop_snake_zrb_app_name_container = DockerComposeTask(
     icon="⛔",
     name="stop",
     description="Stop human readable zrb app name container",
```

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/deploy.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/deploy.py`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/destroy.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/destroy.py`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/build.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/build.py`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/push.py` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/push.py`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/.helmignore` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/.helmignore`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/Chart.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/LICENSE` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/LICENSE`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/NOTICE` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/NOTICE`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/README.md` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/README.md`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/RELEASE_NOTES.rst` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/RELEASE_NOTES.rst`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/Chart.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/README.md` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/README.md`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/Chart.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/Chart.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/README.md` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/README.md`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_affinities.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_affinities.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_capabilities.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_capabilities.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_errors.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_errors.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_images.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_images.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_ingress.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_ingress.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_labels.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_labels.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_names.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_names.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_secrets.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_secrets.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_storage.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_storage.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_tplvalues.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_tplvalues.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_utils.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_utils.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_warnings.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_warnings.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_cassandra.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_cassandra.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mariadb.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mariadb.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mongodb.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mongodb.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mysql.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mysql.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_postgresql.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_postgresql.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_redis.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_redis.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_validations.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_validations.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/NOTES.txt` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/_helpers.tpl` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/cronjob.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/cronjob.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/pvc.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/pvc.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/networkpolicy-egress.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/networkpolicy-egress.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/configmap.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/extended-configmap.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/extended-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/initialization-configmap.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/initialization-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-configmap.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-svc.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/servicemonitor.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/statefulset.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc-headless.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc-headless.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/prometheusrule.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/psp.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/psp.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/extended-configmap.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/extended-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-configmap.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-svc.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/servicemonitor.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/statefulset.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc-headless.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc-headless.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/role.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/rolebinding.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/secrets.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/tls-secrets.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/tls-secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.schema.json` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.schema.json`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/README.md` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/README.md`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/Dockerfile` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/Dockerfile`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/build_and_push.sh` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/build_and_push.sh`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/Dockerfile` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/Dockerfile`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/build_and_push.sh` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/build_and_push.sh`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/pod-template-file.kubernetes-helm-yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/pod-template-file.kubernetes-helm-yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/statsd-mappings.yml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/statsd-mappings.yml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/37197.significant.rst` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/37197.significant.rst`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/config.toml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/config.toml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/NOTES.txt` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/_helpers.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/_helpers.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/check-values.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/check-values.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-cronjob.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-cronjob.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/configmap.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/extra-configmaps.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/extra-configmaps.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/statsd-configmap.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/statsd-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/webserver-configmap.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/webserver-configmap.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-deployment.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dags-persistent-volume-claim.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dags-persistent-volume-claim.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-deployment.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-ingress.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-service.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/limitrange.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/limitrange.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/logs-persistent-volume-claim.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/logs-persistent-volume-claim.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-deployment.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-poddisruptionbudget.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-poddisruptionbudget.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-service.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/priorityclasses/priority-classes.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/priorityclasses/priority-classes.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-role.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-role.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-rolebinding.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-role.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-role.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-rolebinding.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-role.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-role.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-rolebinding.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/security-context-constraint-rolebinding.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/security-context-constraint-rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-service.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-statefulset.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-statefulset.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/resourcequota.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/resourcequota.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-deployment.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-poddisruptionbudget.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-poddisruptionbudget.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-service.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/elasticsearch-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/elasticsearch-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/extra-secrets.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/extra-secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/fernetkey-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/fernetkey-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/flower-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/flower-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/kerberos-keytab-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/kerberos-keytab-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/metadata-connection-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/metadata-connection-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-certificates-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-certificates-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-config-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-config-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-stats-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-stats-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/redis-secrets.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/redis-secrets.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/registry-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/registry-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/result-backend-connection-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/result-backend-connection-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/webserver-secret-key-secret.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/webserver-secret-key-secret.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-deployment.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-service.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-deployment.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-kedaautoscaler.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-kedaautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-service.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-deployment.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-ingress.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-ingress.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-poddisruptionbudget.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-poddisruptionbudget.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-service.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-deployment.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-deployment.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-hpa.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-hpa.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-kedaautoscaler.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-kedaautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-networkpolicy.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-networkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-service.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-service.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-serviceaccount.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.schema.json` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.schema.json`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.yaml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.yaml`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values_schema.schema.json` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values_schema.schema.json`

 * *Files identical despite different names*

### Comparing `zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/docker-compose.yml` & `zrb_extras-0.0.3/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/docker-compose.yml`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
   kebab-zrb-app-name-postgres:
     image: postgres:13
     container_name: "${CONTAINER_PREFIX:-my}-kebab-zrb-app-name-postgres"
     environment:
       POSTGRES_USER: admin
       POSTGRES_PASSWORD: admin
-      POSTGRES_MULTIPLE_DATABASES: airflow,metabase,rekon
+      POSTGRES_DB: airflow
     volumes:
       - ./postgresql-data:/var/lib/postgresql/data
     ports:
       - "${POSTGRES_PORT:-5432}:5432"
     healthcheck:
       test: ["CMD", "pg_isready", "-U", "airflow"]
       interval: 10s
@@ -87,53 +87,53 @@
       start_period: 30s
     restart: unless-stopped
     networks:
       - zrb
 
   kebab-zrb-app-name-webserver:
     <<: *airflow-common
-    container_name: "kebab-zrb-app-name-webserver"
+    container_name: "${CONTAINER_PREFIX:-my}-kebab-zrb-app-name-webserver"
     command: webserver
     ports:
       - "${AIRFLOW_WEBSERVER_PORT:-8080}:8080"
     healthcheck:
       test: ["CMD", "curl", "--fail", "http://localhost:8080/health"]
       interval: 30s
       timeout: 10s
       retries: 5
       start_period: 30s
     restart: unless-stopped
     depends_on:
       <<: *airflow-common-depends-on
-      airflow-init:
+      kebab-zrb-app-name-init:
         condition: service_completed_successfully
     networks:
       - zrb
 
   kebab-zrb-app-name-scheduler:
     <<: *airflow-common
-    container_name: "kebab-zrb-app-name-scheduler"
+    container_name: "${CONTAINER_PREFIX:-my}-kebab-zrb-app-name-scheduler"
     command: scheduler
     healthcheck:
       test: ["CMD", "curl", "--fail", "http://localhost:8974/health"]
       interval: 30s
       timeout: 10s
       retries: 5
       start_period: 30s
     restart: unless-stopped
     depends_on:
       <<: *airflow-common-depends-on
-      airflow-init:
+      kebab-zrb-app-name-init:
         condition: service_completed_successfully
     networks:
       - zrb
 
   kebab-zrb-app-name-worker:
     <<: *airflow-common
-    container_name: "kebab-zrb-app-name-worker"
+    container_name: "${CONTAINER_PREFIX:-my}-kebab-zrb-app-name-worker"
     command: celery worker
     healthcheck:
       # yamllint disable rule:line-length
       test:
         - "CMD-SHELL"
         - 'celery --app airflow.providers.celery.executors.celery_executor.app inspect ping -d "celery@$${HOSTNAME}" || celery --app airflow.executors.celery_executor.app inspect ping -d "celery@$${HOSTNAME}"'
       interval: 30s
@@ -144,46 +144,46 @@
       <<: *airflow-common-env
       # Required to handle warm shutdown of the celery workers properly
       # See https://airflow.apache.org/docs/docker-stack/entrypoint.html#signal-propagation
       DUMB_INIT_SETSID: "0"
     restart: unless-stopped
     depends_on:
       <<: *airflow-common-depends-on
-      airflow-init:
+      kebab-zrb-app-name-init:
         condition: service_completed_successfully
     networks:
       - zrb
 
   kebab-zrb-app-name-triggerer:
     <<: *airflow-common
-    container_name: "kebab-zrb-app-name-triggerer"
+    container_name: "${CONTAINER_PREFIX:-my}-kebab-zrb-app-name-triggerer"
     command: triggerer
     healthcheck:
       test: ["CMD-SHELL", 'airflow jobs check --job-type TriggererJob --hostname "$${HOSTNAME}"']
       interval: 30s
       timeout: 10s
       retries: 5
       start_period: 30s
     restart: unless-stopped
     depends_on:
       <<: *airflow-common-depends-on
-      airflow-init:
+      kebab-zrb-app-name-init:
         condition: service_completed_successfully
     networks:
       - zrb
 
   kebab-zrb-app-name-init:
     <<: *airflow-common
-    container_name: "kebab-zrb-app-name-init"
+    container_name: "${CONTAINER_PREFIX:-my}-kebab-zrb-app-name-init"
     entrypoint: /bin/bash
     # yamllint disable rule:line-length
     command:
       - -c
       - |
-        if [[ -z "${AIRFLOW_UID}" ]]; then
+        if [[ -z "${AIRFLOW_UID:-50000}" ]]; then
           echo
           echo -e "\033[1;33mWARNING!!!: AIRFLOW_UID not set!\e[0m"
           echo "If you are on Linux, you SHOULD follow the instructions below to set "
           echo "AIRFLOW_UID environment variable, otherwise files will be owned by root."
           echo "For other operating systems you can get rid of the warning with manually created .env file:"
           echo "    See: https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html#setting-the-right-airflow-user"
           echo
@@ -218,15 +218,15 @@
           echo
           echo -e "\033[1;33mWARNING!!!: You have not enough resources to run Airflow (see above)!\e[0m"
           echo "Please follow the instructions to increase amount of resources available:"
           echo "   https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html#before-you-begin"
           echo
         fi
         mkdir -p /sources/logs /sources/dags /sources/plugins
-        chown -R "${AIRFLOW_UID}:0" /sources/{logs,dags,plugins}
+        chown -R "${AIRFLOW_UID:-50000}:0" /sources/{logs,dags,plugins}
         exec /entrypoint airflow version
     # yamllint enable rule:line-length
     environment:
       <<: *airflow-common-env
       _AIRFLOW_DB_MIGRATE: 'true'
       _AIRFLOW_WWW_USER_CREATE: 'true'
       _AIRFLOW_WWW_USER_USERNAME: ${_AIRFLOW_WWW_USER_USERNAME:-airflow}
@@ -236,15 +236,15 @@
     volumes:
       - ${AIRFLOW_PROJ_DIR:-.}:/sources
     networks:
       - zrb
 
   kebab-zrb-app-name-cli:
     <<: *airflow-common
-    container_name: "kebab-zrb-app-name-cli"
+    container_name: "${CONTAINER_PREFIX:-my}-kebab-zrb-app-name-cli"
     profiles:
       - debug
     environment:
       <<: *airflow-common-env
       CONNECTION_CHECK_MAX_COUNT: "0"
     # Workaround for entrypoint issue. See: https://github.com/apache/airflow/issues/16252
     command:
@@ -253,29 +253,29 @@
       - airflow
     networks:
       - zrb
 
   # You can enable flower by adding "--profile flower" option e.g. docker-compose --profile flower up
   # or by explicitly targeted on the command line e.g. docker-compose up flower.
   # See: https://docs.docker.com/compose/profiles/
-  flower:
+  kebab-zrb-app-name-flower:
     <<: *airflow-common
     command: celery flower
-    container_name: "flower"
+    container_name: "${CONTAINER_PREFIX:-my}-kebab-zrb-app-name-flower"
     profiles:
       - flower
     ports:
       - "5555:5555"
     healthcheck:
       test: ["CMD", "curl", "--fail", "http://localhost:5555/"]
       interval: 30s
       timeout: 10s
       retries: 5
       start_period: 30s
     restart: unless-stopped
     depends_on:
       <<: *airflow-common-depends-on
-      airflow-init:
+      kebab-zrb-app-name-init:
         condition: service_completed_successfully
     networks:
       - zrb
```

### Comparing `zrb_extras-0.0.2/PKG-INFO` & `zrb_extras-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrb-extras
-Version: 0.0.2
+Version: 0.0.3
 Summary: Collection of Zrb additional utilities
 Home-page: https://github.com/goFrendiAsgard/zrb-extras
 License: AGPL-3.0-or-later
 Author: Go Frendi Gunawan
 Author-email: gofrendiasgard@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

