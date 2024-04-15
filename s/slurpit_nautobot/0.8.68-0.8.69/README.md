# Comparing `tmp/slurpit_nautobot-0.8.68.tar.gz` & `tmp/slurpit_nautobot-0.8.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpit_nautobot-0.8.68.tar", max compression
+gzip compressed data, was "slurpit_nautobot-0.8.69.tar", max compression
```

## Comparing `slurpit_nautobot-0.8.68.tar` & `slurpit_nautobot-0.8.69.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.68/LICENSE
--rw-r--r--   0        0        0       19 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.68/README.md
--rw-r--r--   0        0        0      559 2024-04-15 15:48:35.568364 slurpit_nautobot-0.8.68/pyproject.toml
--rw-r--r--   0        0        0     1262 2024-04-15 15:48:35.572364 slurpit_nautobot-0.8.68/src/slurpit_nautobot/__init__.py
--rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/api/__init__.py
--rw-r--r--   0        0        0     1993 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/api/serializers.py
--rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.68/src/slurpit_nautobot/api/urls.py
--rw-r--r--   0        0        0     9406 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/api/views.py
--rw-r--r--   0        0        0     2547 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/decorators.py
--rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/filtersets.py
--rw-r--r--   0        0        0     7715 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/forms.py
--rw-r--r--   0        0        0    10767 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/importer.py
--rw-r--r--   0        0        0        0 2024-04-15 15:48:35.628364 slurpit_nautobot-0.8.68/src/slurpit_nautobot/management/__init__.py
--rw-r--r--   0        0        0     1159 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/management/choices.py
--rw-r--r--   0        0        0     9130 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/migrations/0001_initial.py
--rw-r--r--   0        0        0     1053 2024-03-17 14:29:31.470119 slurpit_nautobot-0.8.68/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py
--rw-r--r--   0        0        0      749 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/migrations/0003_manufacturer.py
--rw-r--r--   0        0        0      763 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py
--rw-r--r--   0        0        0        0 2024-04-15 15:48:35.636364 slurpit_nautobot-0.8.68/src/slurpit_nautobot/migrations/__init__.py
--rw-r--r--   0        0        0     4984 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/__init__.py
--rw-r--r--   0        0        0     3069 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/device.py
--rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/logs.py
--rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/mapping.py
--rw-r--r--   0        0        0      844 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/planning.py
--rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/setting.py
--rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/navigation.py
--rw-r--r--   0        0        0      101 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/references/__init__.py
--rw-r--r--   0        0        0     1888 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/references/generic.py
--rw-r--r--   0        0        0      648 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/references/imports.py
--rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/search.py
--rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/slurpitch.py
--rw-r--r--   0        0        0     7586 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/tables.py
--rw-r--r--   0        0        0     1506 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/template_content.py
--rw-r--r--   0        0        0     3832 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
--rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
--rw-r--r--   0        0        0     3425 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
--rw-r--r--   0        0        0    22100 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
--rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
--rw-r--r--   0        0        0    17583 2024-04-15 15:48:35.572364 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
--rw-r--r--   0        0        0     3637 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
--rw-r--r--   0        0        0     3623 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
--rw-r--r--   0        0        0     6638 2024-04-15 15:48:35.572364 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
--rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
--rw-r--r--   0        0        0     3628 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
--rw-r--r--   0        0        0     4044 2024-04-15 15:48:35.572364 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
--rw-r--r--   0        0        0     3177 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
--rw-r--r--   0        0        0     9226 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
--rw-r--r--   0        0        0     2368 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
--rw-r--r--   0        0        0     2841 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
--rw-r--r--   0        0        0     2915 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
--rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
--rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/urls.py
--rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/utilities.py
--rw-r--r--   0        0        0     1490 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/validator.py
--rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/__init__.py
--rw-r--r--   0        0        0    10511 2024-04-15 15:48:35.572364 slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/datamapping.py
--rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/logging.py
--rw-r--r--   0        0        0    14365 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/onboarding.py
--rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/reconcile.py
--rw-r--r--   0        0        0    18895 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/setting.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.68/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.69/LICENSE
+-rw-r--r--   0        0        0       19 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.69/README.md
+-rw-r--r--   0        0        0      559 2024-04-15 16:02:55.626182 slurpit_nautobot-0.8.69/pyproject.toml
+-rw-r--r--   0        0        0     1262 2024-04-15 16:02:55.626182 slurpit_nautobot-0.8.69/src/slurpit_nautobot/__init__.py
+-rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/api/__init__.py
+-rw-r--r--   0        0        0     1993 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/api/serializers.py
+-rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.69/src/slurpit_nautobot/api/urls.py
+-rw-r--r--   0        0        0     9406 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/api/views.py
+-rw-r--r--   0        0        0     2547 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/decorators.py
+-rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/filtersets.py
+-rw-r--r--   0        0        0     7715 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/forms.py
+-rw-r--r--   0        0        0    10767 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/importer.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:02:55.706183 slurpit_nautobot-0.8.69/src/slurpit_nautobot/management/__init__.py
+-rw-r--r--   0        0        0     1159 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/management/choices.py
+-rw-r--r--   0        0        0     9130 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1053 2024-03-17 14:29:31.470119 slurpit_nautobot-0.8.69/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py
+-rw-r--r--   0        0        0      749 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/migrations/0003_manufacturer.py
+-rw-r--r--   0        0        0      763 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:02:55.710183 slurpit_nautobot-0.8.69/src/slurpit_nautobot/migrations/__init__.py
+-rw-r--r--   0        0        0     4984 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/__init__.py
+-rw-r--r--   0        0        0     3069 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/device.py
+-rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/logs.py
+-rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/mapping.py
+-rw-r--r--   0        0        0      844 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/planning.py
+-rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/setting.py
+-rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/navigation.py
+-rw-r--r--   0        0        0      101 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/references/__init__.py
+-rw-r--r--   0        0        0     1888 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/references/generic.py
+-rw-r--r--   0        0        0      648 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/references/imports.py
+-rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/search.py
+-rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/slurpitch.py
+-rw-r--r--   0        0        0     7586 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/tables.py
+-rw-r--r--   0        0        0     1506 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/template_content.py
+-rw-r--r--   0        0        0     3832 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
+-rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
+-rw-r--r--   0        0        0     3425 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
+-rw-r--r--   0        0        0    22100 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
+-rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
+-rw-r--r--   0        0        0    17583 2024-04-15 15:48:35.572364 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
+-rw-r--r--   0        0        0     3637 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
+-rw-r--r--   0        0        0     3623 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
+-rw-r--r--   0        0        0     6638 2024-04-15 15:48:35.572364 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
+-rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
+-rw-r--r--   0        0        0     3628 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
+-rw-r--r--   0        0        0     4044 2024-04-15 15:48:35.572364 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
+-rw-r--r--   0        0        0     3177 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
+-rw-r--r--   0        0        0     9331 2024-04-15 16:02:55.626182 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
+-rw-r--r--   0        0        0     2368 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
+-rw-r--r--   0        0        0     2841 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
+-rw-r--r--   0        0        0     2915 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
+-rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
+-rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/urls.py
+-rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/utilities.py
+-rw-r--r--   0        0        0     1490 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/validator.py
+-rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/__init__.py
+-rw-r--r--   0        0        0    10511 2024-04-15 15:48:35.572364 slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/datamapping.py
+-rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/logging.py
+-rw-r--r--   0        0        0    14365 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/onboarding.py
+-rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/reconcile.py
+-rw-r--r--   0        0        0    18895 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/setting.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.69/PKG-INFO
```

### Comparing `slurpit_nautobot-0.8.68/LICENSE` & `slurpit_nautobot-0.8.69/LICENSE`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/pyproject.toml` & `slurpit_nautobot-0.8.69/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slurpit_nautobot"
-version = "0.8.68"
+version = "0.8.69"
 description = ""
 authors = ["Pieter <pieter@slurpit.io>"]
 readme = "README.md"
 packages = [{include = "slurpit_nautobot", from = "src"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/__init__.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nautobot.apps import NautobotAppConfig
 from nautobot.apps import config as app_config
 
 class SlurpitConfig(NautobotAppConfig):
     name = "slurpit_nautobot"
     verbose_name = "Slurp'it Plugin"
     description = "Sync Slurp'it into Nautobot"
-    version = '0.8.68'
+    version = '0.8.69'
     base_url = "slurpit"   
     default_settings = {
         'DeviceType': {'model': "Slurp'it"},
         'Role': {'name': "Slurp'it"},
         'Location': {'name': 'Slurp\'it'},
         'LocationType': {'name': 'Slurp\'it'},
         'Region': {'name': 'Slurp\'it'},
```

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/api/serializers.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/api/serializers.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/api/views.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/api/views.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/decorators.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/decorators.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/filtersets.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/filtersets.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/forms.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/forms.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/importer.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/importer.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/management/choices.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/management/choices.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/migrations/0001_initial.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/migrations/0003_manufacturer.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/migrations/0003_manufacturer.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/__init__.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/device.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/device.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/logs.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/logs.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/planning.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/planning.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/models/setting.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/models/setting.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/navigation.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/navigation.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/references/generic.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/references/generic.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/references/imports.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/references/imports.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/slurpitch.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/slurpitch.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/tables.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/tables.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/template_content.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/template_content.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
                 </div>
 
                 <div class="row">
                   <div class="col-md-8 pt-3">
                     <p>
                       <b><a href="https://learning.slurpit.io/courses/offers/783fcc2c-f0f8-4a41-bc7c-64f1d03e43e8" target="_BLANK">Click here</a></b> to learn on how to use and configure the plugin.
                     </p>
+                    <p><b>Plugin version:</b> {{ settings.PLUGINS_CONFIG.slurpit_nautobot.version }}</p>
                   </div>
                 </div>
                
               </div>
             </div>
           </form>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% load buttons %} {% load i18n %} {% load form_helpers %}
 NNaauuttoobboott SSeerrvveerr {% trans "Save" %}
 {% render_form form %}
 Push: Data will be pushed from Slurp'it to Nautobot
 Pull: Data can be pulled from Slurp'it
 Both: Pull & Push functionality are available
 _CC_ll_ii_cc_kk_ _hh_ee_rr_ee to learn on how to use and configure the plugin.
+PPlluuggiinn vveerrssiioonn:: {{ settings.PLUGINS_CONFIG.slurpit_nautobot.version }}
 {% if appliance_type == 'both' or appliance_type == 'push' %}
 PPlluuggiinn AAPPII _{_%_ _i_f_ _p_u_s_h___a_p_i___k_e_y_ _=_=_ _'_'_ _%_}_ _{_%_ _t_r_a_n_s_ _"_G_e_n_e_r_a_t_e_"_ _%_}_ _{_%_ _e_l_s_e_ _%_}_ _{_%
 _t_r_a_n_s_ _"_S_h_o_w_"_ _%_}_ _{_%_ _e_n_d_i_f_ _%_}
 API Key {% if push_api_key == '' %} NO API KEY {% else %}
         ******************************************* {% endif %}
 {% if debug == True %}
 ** AAPPII ccaallllss:: **
```

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/templates/slurpit_nautobot/table.html` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/templates/slurpit_nautobot/table.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/urls.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/urls.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/validator.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/validator.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/datamapping.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/datamapping.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/logging.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/logging.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/onboarding.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/onboarding.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/reconcile.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/reconcile.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.68/src/slurpit_nautobot/views/setting.py` & `slurpit_nautobot-0.8.69/src/slurpit_nautobot/views/setting.py`

 * *Files identical despite different names*
