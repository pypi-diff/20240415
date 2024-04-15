# Comparing `tmp/airbyte_source_harvest-0.2.0.tar.gz` & `tmp/airbyte_source_harvest-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_harvest-0.2.0.tar", max compression
+gzip compressed data, was "airbyte_source_harvest-1.0.0.tar", max compression
```

## Comparing `airbyte_source_harvest-0.2.0.tar` & `airbyte_source_harvest-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,40 @@
--rw-r--r--   0        0        0     4519 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/README.md
--rw-r--r--   0        0        0      746 2024-04-08 12:45:56.865265 airbyte_source_harvest-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/__init__.py
--rw-r--r--   0        0        0     1224 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/auth.py
--rw-r--r--   0        0        0     1101 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/availability_strategy.py
--rw-r--r--   0        0        0      233 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/run.py
--rw-r--r--   0        0        0      604 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/billable_rates.json
--rw-r--r--   0        0        0      624 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/clients.json
--rw-r--r--   0        0        0     1174 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/company.json
--rw-r--r--   0        0        0      955 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/contacts.json
--rw-r--r--   0        0        0      604 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/cost_rates.json
--rw-r--r--   0        0        0      386 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/estimate_item_categories.json
--rw-r--r--   0        0        0     1151 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/estimate_messages.json
--rw-r--r--   0        0        0     1930 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/estimates.json
--rw-r--r--   0        0        0      565 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/expense_categories.json
--rw-r--r--   0        0        0     3377 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses.json
--rw-r--r--   0        0        0      533 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses_categories.json
--rw-r--r--   0        0        0      513 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses_clients.json
--rw-r--r--   0        0        0      636 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses_projects.json
--rw-r--r--   0        0        0      573 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses_team.json
--rw-r--r--   0        0        0      516 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/invoice_item_categories.json
--rw-r--r--   0        0        0     1458 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/invoice_messages.json
--rw-r--r--   0        0        0     1080 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/invoice_payments.json
--rw-r--r--   0        0        0     3573 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/invoices.json
--rw-r--r--   0        0        0     2233 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/project_assignments.json
--rw-r--r--   0        0        0      822 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/project_budget.json
--rw-r--r--   0        0        0     1932 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/projects.json
--rw-r--r--   0        0        0      495 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/roles.json
--rw-r--r--   0        0        0     1067 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/task_assignments.json
--rw-r--r--   0        0        0      646 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/tasks.json
--rw-r--r--   0        0        0      576 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/time_clients.json
--rw-r--r--   0        0        0     3977 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/time_entries.json
--rw-r--r--   0        0        0      699 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/time_projects.json
--rw-r--r--   0        0        0      572 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/time_tasks.json
--rw-r--r--   0        0        0      636 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/time_team.json
--rw-r--r--   0        0        0      772 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/uninvoiced.json
--rw-r--r--   0        0        0     1145 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/user_assignments.json
--rw-r--r--   0        0        0     1678 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/schemas/users.json
--rw-r--r--   0        0        0     6014 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/source.py
--rw-r--r--   0        0        0     4771 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/spec.json
--rw-r--r--   0        0        0    14079 2024-04-08 09:25:38.000000 airbyte_source_harvest-0.2.0/source_harvest/streams.py
--rw-r--r--   0        0        0     5224 1970-01-01 00:00:00.000000 airbyte_source_harvest-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/README.md
+-rw-r--r--   0        0        0      767 2024-04-15 16:09:38.876249 airbyte_source_harvest-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/__init__.py
+-rw-r--r--   0        0        0     4047 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/config_migrations.py
+-rw-r--r--   0        0        0    75102 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/manifest.yaml
+-rw-r--r--   0        0        0      331 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/run.py
+-rw-r--r--   0        0        0      604 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/billable_rates.json
+-rw-r--r--   0        0        0      624 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/clients.json
+-rw-r--r--   0        0        0     1174 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/company.json
+-rw-r--r--   0        0        0      955 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/contacts.json
+-rw-r--r--   0        0        0      604 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/cost_rates.json
+-rw-r--r--   0        0        0      386 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/estimate_item_categories.json
+-rw-r--r--   0        0        0     1151 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/estimate_messages.json
+-rw-r--r--   0        0        0     1930 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/estimates.json
+-rw-r--r--   0        0        0      565 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expense_categories.json
+-rw-r--r--   0        0        0     3377 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses.json
+-rw-r--r--   0        0        0      533 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_categories.json
+-rw-r--r--   0        0        0      513 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_clients.json
+-rw-r--r--   0        0        0      636 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_projects.json
+-rw-r--r--   0        0        0      573 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_team.json
+-rw-r--r--   0        0        0      516 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_item_categories.json
+-rw-r--r--   0        0        0     1458 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_messages.json
+-rw-r--r--   0        0        0     1080 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_payments.json
+-rw-r--r--   0        0        0     3573 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/invoices.json
+-rw-r--r--   0        0        0     2233 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/project_assignments.json
+-rw-r--r--   0        0        0      822 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/project_budget.json
+-rw-r--r--   0        0        0     1932 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/projects.json
+-rw-r--r--   0        0        0      495 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/roles.json
+-rw-r--r--   0        0        0     1067 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/task_assignments.json
+-rw-r--r--   0        0        0      646 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/tasks.json
+-rw-r--r--   0        0        0      576 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_clients.json
+-rw-r--r--   0        0        0     3977 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_entries.json
+-rw-r--r--   0        0        0      699 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_projects.json
+-rw-r--r--   0        0        0      572 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_tasks.json
+-rw-r--r--   0        0        0      636 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/time_team.json
+-rw-r--r--   0        0        0      772 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/uninvoiced.json
+-rw-r--r--   0        0        0     1145 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/user_assignments.json
+-rw-r--r--   0        0        0     1678 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/schemas/users.json
+-rw-r--r--   0        0        0      476 2024-04-15 15:43:42.000000 airbyte_source_harvest-1.0.0/source_harvest/source.py
+-rw-r--r--   0        0        0     5224 1970-01-01 00:00:00.000000 airbyte_source_harvest-1.0.0/PKG-INFO
```

### Comparing `airbyte_source_harvest-0.2.0/README.md` & `airbyte_source_harvest-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/pyproject.toml` & `airbyte_source_harvest-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.0"
+version = "1.0.0"
 name = "airbyte-source-harvest"
 description = "Source implementation for Harvest."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -27,7 +27,8 @@
 [tool.poetry.scripts]
 source-harvest = "source_harvest.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.11.0"
 pytest-mock = "^3.6.1"
 pytest = "^6.1"
+freezegun = "^1.4.0"
```

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/__init__.py` & `airbyte_source_harvest-1.0.0/source_harvest/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/billable_rates.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/billable_rates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/clients.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/clients.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/company.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/company.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/contacts.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/cost_rates.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/cost_rates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/estimate_messages.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/estimate_messages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/estimates.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/estimates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/expense_categories.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/expense_categories.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses_categories.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_categories.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses_clients.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_clients.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses_projects.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_projects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/expenses_team.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/expenses_team.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/invoice_item_categories.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_item_categories.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/invoice_messages.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_messages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/invoice_payments.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/invoice_payments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/invoices.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/project_assignments.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/project_assignments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/project_budget.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/project_budget.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/projects.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/task_assignments.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/task_assignments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/tasks.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/tasks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/time_clients.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/time_clients.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/time_entries.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/time_entries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/time_projects.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/time_projects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/time_tasks.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/time_tasks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/time_team.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/time_team.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/uninvoiced.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/uninvoiced.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/user_assignments.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/user_assignments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/source_harvest/schemas/users.json` & `airbyte_source_harvest-1.0.0/source_harvest/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_harvest-0.2.0/PKG-INFO` & `airbyte_source_harvest-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-harvest
-Version: 0.2.0
+Version: 1.0.0
 Summary: Source implementation for Harvest.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

