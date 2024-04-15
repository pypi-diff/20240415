# Comparing `tmp/slurpit_nautobot-0.8.66.tar.gz` & `tmp/slurpit_nautobot-0.8.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpit_nautobot-0.8.66.tar", max compression
+gzip compressed data, was "slurpit_nautobot-0.8.67.tar", max compression
```

## Comparing `slurpit_nautobot-0.8.66.tar` & `slurpit_nautobot-0.8.67.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.66/LICENSE
--rw-r--r--   0        0        0       19 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.66/README.md
--rw-r--r--   0        0        0      559 2024-04-09 07:52:32.891145 slurpit_nautobot-0.8.66/pyproject.toml
--rw-r--r--   0        0        0     1262 2024-04-09 07:52:32.891145 slurpit_nautobot-0.8.66/src/slurpit_nautobot/__init__.py
--rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/api/__init__.py
--rw-r--r--   0        0        0     1993 2024-04-08 23:59:23.573558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/api/serializers.py
--rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.66/src/slurpit_nautobot/api/urls.py
--rw-r--r--   0        0        0     9406 2024-04-08 23:59:23.573558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/api/views.py
--rw-r--r--   0        0        0     2547 2024-04-08 23:59:23.573558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/decorators.py
--rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/filtersets.py
--rw-r--r--   0        0        0     7715 2024-04-08 23:59:23.573558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/forms.py
--rw-r--r--   0        0        0    10458 2024-04-08 23:59:23.573558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/importer.py
--rw-r--r--   0        0        0        0 2024-04-09 07:52:32.963145 slurpit_nautobot-0.8.66/src/slurpit_nautobot/management/__init__.py
--rw-r--r--   0        0        0     1159 2024-04-08 23:59:23.573558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/management/choices.py
--rw-r--r--   0        0        0     9130 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/migrations/0001_initial.py
--rw-r--r--   0        0        0     1053 2024-03-17 14:29:31.470119 slurpit_nautobot-0.8.66/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py
--rw-r--r--   0        0        0      749 2024-04-08 23:59:23.577558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/migrations/0003_manufacturer.py
--rw-r--r--   0        0        0      763 2024-04-08 23:59:23.577558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py
--rw-r--r--   0        0        0        0 2024-04-09 07:52:32.967145 slurpit_nautobot-0.8.66/src/slurpit_nautobot/migrations/__init__.py
--rw-r--r--   0        0        0     4984 2024-04-08 23:59:23.577558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/__init__.py
--rw-r--r--   0        0        0     3069 2024-04-08 23:59:23.577558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/device.py
--rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/logs.py
--rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/mapping.py
--rw-r--r--   0        0        0      844 2024-04-08 23:59:23.577558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/planning.py
--rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/setting.py
--rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/navigation.py
--rw-r--r--   0        0        0      101 2024-04-08 23:59:23.577558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/references/__init__.py
--rw-r--r--   0        0        0     1888 2024-04-08 23:59:23.581558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/references/generic.py
--rw-r--r--   0        0        0      648 2024-04-08 23:59:23.581558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/references/imports.py
--rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/search.py
--rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/slurpitch.py
--rw-r--r--   0        0        0     4757 2024-04-08 23:59:23.581558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/tables.py
--rw-r--r--   0        0        0     1181 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/template_content.py
--rw-r--r--   0        0        0     3832 2024-04-08 23:59:23.581558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
--rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
--rw-r--r--   0        0        0     3425 2024-04-08 23:59:23.581558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
--rw-r--r--   0        0        0    22100 2024-04-08 23:59:23.585558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
--rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
--rw-r--r--   0        0        0    17724 2024-04-08 23:59:23.585558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
--rw-r--r--   0        0        0     3547 2024-04-08 23:59:23.585558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
--rw-r--r--   0        0        0     3533 2024-04-08 23:59:23.585558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
--rw-r--r--   0        0        0     6485 2024-04-08 23:59:23.585558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
--rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
--rw-r--r--   0        0        0     3549 2024-04-08 23:59:23.585558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
--rw-r--r--   0        0        0     4275 2024-04-08 23:59:23.589558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
--rw-r--r--   0        0        0     3177 2024-04-08 23:59:23.589558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
--rw-r--r--   0        0        0     9226 2024-04-08 23:59:23.589558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
--rw-r--r--   0        0        0     2368 2024-04-08 23:59:23.589558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
--rw-r--r--   0        0        0     2841 2024-04-08 23:59:23.589558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
--rw-r--r--   0        0        0     2915 2024-04-08 23:59:23.589558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
--rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
--rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/urls.py
--rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/utilities.py
--rw-r--r--   0        0        0     1490 2024-04-08 23:59:23.593558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/validator.py
--rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/__init__.py
--rw-r--r--   0        0        0    10130 2024-04-08 23:59:23.593558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/datamapping.py
--rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/logging.py
--rw-r--r--   0        0        0    13967 2024-04-08 23:59:23.593558 slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/onboarding.py
--rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/reconcile.py
--rw-r--r--   0        0        0    18388 2024-04-09 07:52:32.891145 slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/setting.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.66/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.67/LICENSE
+-rw-r--r--   0        0        0       19 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.67/README.md
+-rw-r--r--   0        0        0      559 2024-04-15 01:41:52.123553 slurpit_nautobot-0.8.67/pyproject.toml
+-rw-r--r--   0        0        0     1262 2024-04-15 01:41:52.123553 slurpit_nautobot-0.8.67/src/slurpit_nautobot/__init__.py
+-rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/api/__init__.py
+-rw-r--r--   0        0        0     1993 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/api/serializers.py
+-rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.67/src/slurpit_nautobot/api/urls.py
+-rw-r--r--   0        0        0     9406 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/api/views.py
+-rw-r--r--   0        0        0     2547 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/decorators.py
+-rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/filtersets.py
+-rw-r--r--   0        0        0     7715 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/forms.py
+-rw-r--r--   0        0        0    10767 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/importer.py
+-rw-r--r--   0        0        0        0 2024-04-15 01:41:52.171553 slurpit_nautobot-0.8.67/src/slurpit_nautobot/management/__init__.py
+-rw-r--r--   0        0        0     1159 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/management/choices.py
+-rw-r--r--   0        0        0     9130 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1053 2024-03-17 14:29:31.470119 slurpit_nautobot-0.8.67/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py
+-rw-r--r--   0        0        0      749 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/migrations/0003_manufacturer.py
+-rw-r--r--   0        0        0      763 2024-04-15 01:40:54.571188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py
+-rw-r--r--   0        0        0        0 2024-04-15 01:41:52.175553 slurpit_nautobot-0.8.67/src/slurpit_nautobot/migrations/__init__.py
+-rw-r--r--   0        0        0     4984 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/__init__.py
+-rw-r--r--   0        0        0     3069 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/device.py
+-rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/logs.py
+-rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/mapping.py
+-rw-r--r--   0        0        0      844 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/planning.py
+-rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/setting.py
+-rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/navigation.py
+-rw-r--r--   0        0        0      101 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/references/__init__.py
+-rw-r--r--   0        0        0     1888 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/references/generic.py
+-rw-r--r--   0        0        0      648 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/references/imports.py
+-rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/search.py
+-rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/slurpitch.py
+-rw-r--r--   0        0        0     7586 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/tables.py
+-rw-r--r--   0        0        0     1506 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/template_content.py
+-rw-r--r--   0        0        0     3832 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
+-rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
+-rw-r--r--   0        0        0     3425 2024-04-15 01:40:54.575188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
+-rw-r--r--   0        0        0    22100 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
+-rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
+-rw-r--r--   0        0        0    17754 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
+-rw-r--r--   0        0        0     3637 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
+-rw-r--r--   0        0        0     3623 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
+-rw-r--r--   0        0        0     6591 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
+-rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
+-rw-r--r--   0        0        0     3628 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
+-rw-r--r--   0        0        0     4275 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
+-rw-r--r--   0        0        0     3177 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
+-rw-r--r--   0        0        0     9226 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
+-rw-r--r--   0        0        0     2368 2024-04-15 01:40:54.579187 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
+-rw-r--r--   0        0        0     2841 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
+-rw-r--r--   0        0        0     2915 2024-04-15 01:40:54.583188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
+-rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
+-rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/urls.py
+-rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/utilities.py
+-rw-r--r--   0        0        0     1490 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/validator.py
+-rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/__init__.py
+-rw-r--r--   0        0        0    10366 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/datamapping.py
+-rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/logging.py
+-rw-r--r--   0        0        0    14365 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/onboarding.py
+-rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/reconcile.py
+-rw-r--r--   0        0        0    18895 2024-04-15 01:40:54.587188 slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/setting.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.67/PKG-INFO
```

### Comparing `slurpit_nautobot-0.8.66/LICENSE` & `slurpit_nautobot-0.8.67/LICENSE`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/pyproject.toml` & `slurpit_nautobot-0.8.67/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slurpit_nautobot"
-version = "0.8.66"
+version = "0.8.67"
 description = ""
 authors = ["Pieter <pieter@slurpit.io>"]
 readme = "README.md"
 packages = [{include = "slurpit_nautobot", from = "src"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/__init__.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nautobot.apps import NautobotAppConfig
 from nautobot.apps import config as app_config
 
 class SlurpitConfig(NautobotAppConfig):
     name = "slurpit_nautobot"
     verbose_name = "Slurp'it Plugin"
     description = "Sync Slurp'it into Nautobot"
-    version = '0.8.66'
+    version = '0.8.67'
     base_url = "slurpit"   
     default_settings = {
         'DeviceType': {'model': "Slurp'it"},
         'Role': {'name': "Slurp'it"},
         'Location': {'name': 'Slurp\'it'},
         'LocationType': {'name': 'Slurp\'it'},
         'Region': {'name': 'Slurp\'it'},
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/api/serializers.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/api/serializers.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/api/views.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/api/views.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/decorators.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/decorators.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/filtersets.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/filtersets.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/forms.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/forms.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/importer.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from django.utils import timezone
 from django.db.models.expressions import RawSQL
 
 from . import get_config
 from .models import SlurpitImportedDevice, SlurpitStagedDevice, ensure_slurpit_tags, SlurpitLog, SlurpitSetting, SlurpitPlanning, SlurpitSnapshot
 from .management.choices import *
 from .references import base_name, plugin_type, custom_field_data_name
-from .references.generic import get_default_objects, status_inventory, status_offline, get_create_dcim_objects
+from .references.generic import get_default_objects, status_inventory, status_offline, get_create_dcim_objects, set_device_custom_fields
 from .references.imports import *
 
 BATCH_SIZE = 256
 columns = ('slurpit_id', 'disabled', 'hostname', 'fqdn', 'ipv4', 'device_os', 'device_type', 'brand', 'createddate', 'changeddate')
 
 
 def get_devices(offset):
@@ -27,24 +27,28 @@
         headers = {
                         'authorization': setting.api_key,
                         'useragent': f"{plugin_type}/requests",
                         'accept': 'application/json'
                     }
         uri_devices = f"{uri_base}/api/devices?offset={offset}&limit={BATCH_SIZE}"
         r = requests.get(uri_devices, headers=headers, timeout=15, verify=False)
-        r.raise_for_status()
+        # r.raise_for_status()
         data = r.json()
         log_message = f"Syncing the devices from Slurp'it in {plugin_type.capitalize()}."
         SlurpitLog.info(category=LogCategoryChoices.ONBOARD, message=log_message)
-        return data
+        return data, ""
     except ObjectDoesNotExist:
         setting = None
         log_message = "Need to set the setting parameter"
         SlurpitLog.failure(category=LogCategoryChoices.ONBOARD, message=log_message)
-        return None
+        return None, log_message
+    except Exception as e:
+        log_message = "Please confirm the Slurp'it server is running and reachable."
+        return None, log_message
+
 
 def start_device_import():
     with connection.cursor() as cursor:
         cursor.execute(f"truncate {SlurpitStagedDevice._meta.db_table} cascade")
 
 def import_devices(devices):
     to_insert = []
@@ -150,14 +154,15 @@
                     result.mapped_device.status=status_inventory()
                     
                 set_device_custom_fields(result.mapped_device, {
                     'slurpit_hostname': device.hostname,
                     'slurpit_fqdn': device.fqdn,
                     'slurpit_ipv4': device.ipv4,
                 })   
+                result.mapped_device.name = device.hostname
                 result.mapped_device.save()
         offset += BATCH_SIZE
 
     SlurpitLog.info(category=LogCategoryChoices.ONBOARD, message=f"Sync updated {count} devices")
 
 def import_from_queryset(qs: QuerySet, **extra):
     count = len(qs)
@@ -221,15 +226,17 @@
                         'authorization': setting.api_key,
                         'useragent': f"{plugin_type}/requests",
                         'accept': 'application/json'
                     }
         uri_devices = f"{uri_base}/api/devices/snapshot/single/{hostname}/{planning_id}"
 
         r = requests.get(uri_devices, headers=headers, timeout=15, verify=False)
-        r.raise_for_status()
+        #r.raise_for_status()
+        if r.status_code != 200:
+            return None
         data = r.json()
         log_message = f"Get the latest data from Slurp'it in {plugin_type.capitalize()} on planning ID."
         SlurpitLog.info(category=LogCategoryChoices.ONBOARD, message=log_message)
         return data
     except ObjectDoesNotExist:
         setting = None
         log_message = "Need to set the setting parameter"
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/management/choices.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/management/choices.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/migrations/0001_initial.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/migrations/0003_manufacturer.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/migrations/0003_manufacturer.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/__init__.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/device.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/device.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/logs.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/logs.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/planning.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/planning.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/models/setting.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/models/setting.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/navigation.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/navigation.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/references/generic.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/references/generic.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/references/imports.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/references/imports.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/slurpitch.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/slurpitch.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/template_content.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/template_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # template_content.py
 from django.urls import reverse
 from nautobot.apps.ui import TemplateExtension
+from django.shortcuts import get_object_or_404
+from nautobot.dcim.models import Device
 
 class DeviceExtraTabs(TemplateExtension):
     """Template extension to add extra tabs to the object detail tabs."""
 
     model = 'dcim.device'
 
     def detail_tabs(self):
@@ -17,14 +19,22 @@
         - The <url> key's value is used to render the HTML link for the tab
 
         These tabs will be visible (in this instance) on the Device model's detail page as
         set by the DeviceContent.model attribute "dcim.device"
 
         This example demonstrates defining two tabs. The tabs will be ordered by their position in list.
         """
+        device = get_object_or_404(Device, pk=self.context["object"].pk)
+
+        if device:
+            slurpit_hostname = device.custom_field_data['slurpit_hostname']
+            if slurpit_hostname is None:
+                return []
+
+
         return [
             {
                 "title": "Slurpit",
                 "url": reverse("plugins:slurpit_nautobot:slurpit_planning", kwargs={"pk": self.context["object"].pk}),
                 "weight": 50000
             }
         ]
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html`

 * *Files 0% similar despite different names*

```diff
@@ -221,22 +221,22 @@
                         fill="none" stroke="#ddd" stroke-width="20"/>
                 <circle class="circle-bar"
                         cx="80" cy="80" r="70"
                         fill="none" stroke="#4CAF50" stroke-width="20"
                         stroke-dasharray="439.8" stroke-dashoffset="439.8"/>
               </svg>
               <div class="progress-text" id="progressText">
-                Sending devices <br> from Nautobot to Slurpit<br><span class="sync-percent" id="percent">0%</span><br>
+                Sending devices <br> from Netbox to Slurp'it<br><span class="sync-percent" id="percent">0%</span><br>
                 <span> Total Devices: <span id="total-cnt">100</span></span><br>
                 <span> Done Devices: <span id="done-cnt">30</span></span><br>
                 <span> Failed Devices: <span id="failed-cnt">10</span></span>
               </div>
             </div>
             <textarea  name="logs" cols="40" rows="10" class=" form-control mb-2" placeholder="Logs" id="logs" style="height: 80px;"></textarea>
-            <p><b>Don't refresh website or close modal before 100%</b></p>
+            <p>Don't <b>refresh</b> or close the modal before 100%</p>
           </div>
           <div class="modal-footer">
             <button type="button" class="btn btn-danger" data-dismiss="modal">Close</button>
           </div>
           
       </form>
       <!-- Modal Body -->
@@ -492,20 +492,21 @@
       headers: {
         'Content-Type': 'application/x-www-form-urlencoded'
       },
       body: data
     }).then(function(response) {
       return response.json();
     }).then(function(res){
-      current_cnt++;
-      if(res["status"] == undefined) done_count++;  
+      
+      if(res["status"] == undefine && res['error'] == undefine) done_count++;  
       else {
         failed_count++;
-        logsElement.append("Failed to import "+res["item_name"]+"\n")
+        logsElement.append("Failed to import "+res["item_name"]+"\n");
       }
+      current_cnt++;
       update_status();  
       send_device();
     }).catch(function(error) {
       failed_count++;
       current_cnt++;
       update_status();
       send_device();
```

#### html2text {}

```diff
@@ -37,14 +37,14 @@
 render_form device_form %} {% elif request.GET.subtab == 'ipam' %} {%
 render_form iprange_form %} {% endif %}
 {% if appliance_type != 'push' %} {% trans "Push" %} {% endif %}
 {% endif %}
 Close
 {% csrf_token %}
 Sending devices
-from Nautobot to Slurpit
+from Netbox to Slurp'it
 0%
 Total Devices: 100
 Done Devices: 30
 Failed Devices: 10
-DDoonn''tt rreeffrreesshh wweebbssiittee oorr cclloossee mmooddaall bbeeffoorree 110000%%
+Don't rreeffrreesshh or close the modal before 100%
 Close
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,17 @@
                         <button type="submit" name="_rename" formaction="{% url 'plugins:slurpit_nautobot:onboard' %}?conflicted=update&return_url={% url 'plugins:slurpit_nautobot:importeddevice_list' %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn">
                           <i class="mdi mdi-pencil" aria-hidden="true"></i> {% trans "Update existing device" %}
                         </button>
                     </li>
                   </ul>
                   {% endblock %}
                 </div>
+                <span>In green is the incoming change from Slurp'it</span>
               </div>
+              
             </div>
             
             {% block table %}
               {% include "slurpit_nautobot/table.html" %}
             {% endblock %}
           </div>
         </div>
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,17 @@
                         <button type="submit" name="_rename" formaction="{% url 'plugins:slurpit_nautobot:onboard' %}?migrate=update&return_url={% url 'plugins:slurpit_nautobot:importeddevice_list' %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn">
                           <i class="mdi mdi-pencil" aria-hidden="true"></i> {% trans "Update existing device" %}
                         </button>
                     </li>
                   </ul>
                   {% endblock %}
                 </div>
+                <span>In green is the incoming change from Slurp'it</span>
               </div>
+              
             </div>
             {% block table %}
               {% include "slurpit_nautobot/table.html" %}
             {% endblock %}
           </div>
         </div>
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,18 @@
           throw new Error(`HTTP error! Status: ${response.status}`);
         }
         return response.json();
       })
       .then(data => {
         action = data["action"];
 
-        if(action == "import") {
+        if(action == 'error') {
+          location.reload();
+        }
+        else if(action == "import") {
           newOffset = data["offset"];
           
           if(newOffset != offset) {
             offset = newOffset;
             statusCaptionText = "Imported "+newOffset+" devices from slurpit to nautobot"
             statusCaptionElement.innerHTML = statusCaptionText;
             import_device();
@@ -162,11 +165,12 @@
           }
         }else if(action == "process") {
           location.reload();
         }
         
       })
       .catch(error => {
-        console.error('Fetch error:', error);
+        // console.error('Fetch error:', error);
+        location.reload();
       });
     }
   </script>
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,20 @@
       {% block subtitle %}{% endblock %}
     </div>
 
     {# Controls #}
     {% block controls %}{% endblock controls %}
 
   </div>
+  <style>
+    .greenLink a {
+      color: #007dff !important
+    }
+  </style>
+
 {% endblock header %}
 
 {% block content %}
   <ul class="nav nav-tabs px-3">
         
     <li class="nav-item {% if request.GET.tab == 'new' or request.GET.tab is None %}active{% endif %}" role="presentation">
       <a class="nav-tab nav-link " href="?tab=new">
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/templates/slurpit_nautobot/table.html` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/templates/slurpit_nautobot/table.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/urls.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/urls.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/validator.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/validator.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/datamapping.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/datamapping.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 # from nautobot.ipam.models import IPRange
 
 BATCH_SIZE = 128
 
 def get_device_dict(instance):
     device_dict = model_to_dict(instance)
     # Assuming 'device_type' is a ForeignKey, for example.
-    device_dict['device_type'] = str(instance.device_type)
-    device_dict['platform'] = str(instance.platform)
-    device_dict['primary_ip4'] = str(instance.primary_ip4)
-    device_dict['primary_ip6'] = str(instance.primary_ip6)
+    device_dict['device_type'] = str(instance.device_type) if instance.device_type is not None else None
+    device_dict['platform'] = str(instance.platform) if instance.platform is not None else None
+    device_dict['primary_ip4'] = str(instance.primary_ip4) if instance.primary_ip4 is not None else None
+    device_dict['primary_ip6'] = str(instance.primary_ip6) if instance.primary_ip6 is not None else None
+
 
     for custom_field in device_dict['_custom_field_data']:
         device_dict[f'cf_{custom_field}'] = device_dict['_custom_field_data'][custom_field]
 
     return device_dict
 
 def post_slurpit_device(row, item_name):
@@ -142,15 +143,15 @@
                     mapping_values = model_to_dict(device)
                 
                 row = {}
                 objs = SlurpitMapping.objects.filter(mapping_type=subtab)
                 if objs:
                     for obj in objs:
                         target_field = obj.target_field.split('|')[1]
-                        row[obj.source_field] = str(mapping_values[target_field])
+                        row[obj.source_field] = str(mapping_values[target_field]) if mapping_values[target_field] is not None else None
 
                 if test is not None:
                     if subtab == "device":
                         res = post_slurpit_device(row, device.name)
                     else:
                         res = None
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/logging.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/logging.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/onboarding.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/onboarding.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from ..management.choices import *
 from ..importer import get_dcim_device, import_from_queryset, run_import, get_devices, BATCH_SIZE, import_devices, process_import, start_device_import
 from ..decorators import slurpit_plugin_registered
 from ..references import base_name, custom_field_data_name
 from ..references.generic import create_form, get_form_device_data, SlurpitViewMixim, get_default_objects, set_device_custom_fields, status_inventory
 from ..references.imports import * 
 
+from django.http import HttpResponse, HttpResponseRedirect, JsonResponse
+
 @method_decorator(slurpit_plugin_registered, name='dispatch')
 class SlurpitImportedDeviceListView(SlurpitViewMixim, generic.ObjectListView):
     conflicted_queryset = models.SlurpitImportedDevice.objects.filter(mapped_device_id__isnull=True, hostname__in=Device.objects.values('name'))
     to_onboard_queryset = models.SlurpitImportedDevice.objects.filter(mapped_device_id__isnull=True).exclude(pk__in=conflicted_queryset.values('pk'))
     onboarded_queryset = models.SlurpitImportedDevice.objects.filter(mapped_device_id__isnull=False)
     migrate_queryset = models.SlurpitImportedDevice.objects.filter(
                 mapped_device_id__isnull=False
@@ -56,15 +58,15 @@
         self.queryset = self.to_onboard_queryset
 
         if request.GET.get('tab') == "migrate":
             self.queryset = self.migrate_queryset
             self.table = tables.MigratedDeviceTable
         elif request.GET.get('tab') == "conflicted":
             self.queryset = self.conflicted_queryset
-            self.table = tables.SlurpitImportedDeviceTable
+            self.table = tables.ConflictDeviceTable
         elif request.GET.get('tab') == "onboarded":
             self.queryset = self.onboarded_queryset
 
         return super().get(request, *args, **kwargs)
     
     def post(self, request):
         pks = map(int, request.POST.getlist('pk'))
@@ -277,18 +279,24 @@
     def get(self, request, *args, **kwargs):
         offset = request.GET.get("offset", None)
         try:
             if offset is not None:
                 offset = int(offset)
                 if offset == 0:
                     start_device_import()
-                devices = get_devices(offset)
+                devices, log_message = get_devices(offset)
                 if devices is not None and len(devices) > 0:
                     import_devices(devices)
                     offset += len(devices)
+
+                if devices is None:
+                    messages.error(request, "Please confirm the Slurp'it server is running and reachable.")
+                    # return HttpResponseRedirect(reverse("plugins:slurpit_netbox:onboard"))
+                    return JsonResponse({"action": "error", "error": "ERROR"})
+
                 return JsonResponse({"action": "import", "offset": offset})
             
             process_import()
             messages.info(request, "Synced the devices from Slurp'it.")
             return JsonResponse({"action": "process"})
         except requests.exceptions.RequestException as e:
             messages.error(request, "An error occured during querying Slurp'it!")
```

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/reconcile.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/reconcile.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.66/src/slurpit_nautobot/views/setting.py` & `slurpit_nautobot-0.8.67/src/slurpit_nautobot/views/setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,29 @@
 from ..tables import SlurpitPlanningTable
 from ..management.choices import *
 from ..decorators import slurpit_plugin_registered
 from ..importer import get_latest_data_on_planning, import_plannings
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 from ..filtersets import SlurpitPlanningFilterSet
 
+from json import JSONEncoder
+import json
+
+class OrderedEncoder(JSONEncoder):
+    def encode(self, o):
+        if isinstance(o, dict):
+            return "{" + ", ".join(f'{self.encode(k)}: {self.encode(v)}' for k, v in o.items()) + "}"
+        return super().encode(o)
+
+
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
 BATCH_SIZE = 128
 
+
 @method_decorator(slurpit_plugin_registered, name='dispatch')
 class SettingsView(View):
     
     app_label = "dcim"
     model_name = "device"
     
     def get(self, request):
@@ -341,15 +352,15 @@
             self.form.id = planning.planning_id
             result_type = request.GET.get('result_type')
             
             if result_type is None:
                 result_type = "planning"
 
             cache_key = (
-                f"slurpit_plan_{planning.planning_id}_{device.serial}_{result_type}"
+                f"slurpit_plan_{planning.planning_id}_{device.name}_{result_type}"
             )
 
             url_no_refresh = get_refresh_url(request, pk)
 
             if sync == "sync":
                 if appliance_type != "cloud":
                     sync_snapshot(cache_key, device.name, planning)
@@ -377,15 +388,19 @@
                     # Empty case
                     if temp.count() == 0:
                         if appliance_type != "cloud":
                             sync_snapshot(cache_key, device.name, planning)
                         temp = SlurpitSnapshot.objects.filter(hostname=device.name, planning_id=planning.planning_id, result_type=result_key)
 
                     for r in temp:
-                        r = r.content
+                        try:
+                            r = json.loads(r.content)
+                        except:
+                            r = r.content
+
                         # raw = r[result_key]
                         data.append({**r})
                     result_status = "Live"
                     cache.set(cache_key, (datetime.now(), data), 60 * 60 * 8)
                     
                 except Exception as e:
                     messages.error(request, e)
@@ -439,19 +454,22 @@
         temp = data[plan.name]["planning_results"]
 
         if temp is not None:
             count = SlurpitSnapshot.objects.filter(hostname=device_name, planning_id=plan.planning_id).delete()[0]
             SlurpitLog.info(category=LogCategoryChoices.PLANNING, message=f"Sync deleted {count} snapshots for planning {plan.name}")
             
         for item in temp:
-            new_items.append(SlurpitSnapshot(hostname=device_name, planning_id=plan.planning_id, content=item, result_type="planning_result"))
-        
+            content = json.dumps(item, cls=OrderedEncoder)
+            new_items.append(SlurpitSnapshot(hostname=device_name, planning_id=plan.planning_id, content=content, result_type="planning_result"))
+
         temp = data[plan.name]["template_results"]
         for item in temp:
-            new_items.append(SlurpitSnapshot(hostname=device_name, planning_id=plan.planning_id, content=item, result_type="template_result"))
+            content = json.dumps(item, cls=OrderedEncoder)
+            new_items.append(SlurpitSnapshot(hostname=device_name, planning_id=plan.planning_id, content=content, result_type="template_result"))
+
         
         SlurpitSnapshot.objects.bulk_create(new_items, batch_size=BATCH_SIZE, ignore_conflicts=True)
         SlurpitLog.info(category=LogCategoryChoices.PLANNING, message=f"Sync imported {len(new_items)} snapshots for planning {plan.name}")
 
 class SlurpitPlanningListView(generic.ObjectListView):
     queryset = SlurpitPlanning.objects.all()
     filterset = SlurpitPlanningFilterSet
```

