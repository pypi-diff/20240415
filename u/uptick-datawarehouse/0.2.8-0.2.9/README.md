# Comparing `tmp/uptick_datawarehouse-0.2.8.tar.gz` & `tmp/uptick_datawarehouse-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptick_datawarehouse-0.2.8.tar", max compression
+gzip compressed data, was "uptick_datawarehouse-0.2.9.tar", max compression
```

## Comparing `uptick_datawarehouse-0.2.8.tar` & `uptick_datawarehouse-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0       24 2023-01-13 01:44:11.272938 uptick_datawarehouse-0.2.8/public_readme.md
--rw-r--r--   0        0        0      526 2023-07-04 23:19:52.151183 uptick_datawarehouse-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      200 2023-01-13 01:48:03.658500 uptick_datawarehouse-0.2.8/uptick_datawarehouse/model_settings.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.929168 uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/__init__.py
--rw-r--r--   0        0        0      191 2023-01-13 01:47:26.046172 uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/apps.py
--rw-r--r--   0        0        0      271 2023-01-12 03:28:28.929570 uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/migrations/0001_schema.py
--rw-r--r--   0        0        0    14332 2023-01-21 02:47:03.096787 uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/migrations/0002_changesummary_chargesummary_paymentmethodsummary_recurringcreditsummary_revenueforecastsummary_subsc.py
--rw-r--r--   0        0        0      699 2023-01-23 04:43:50.589352 uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/migrations/0003_auto_20230123_0443.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.930097 uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/migrations/__init__.py
--rw-r--r--   0        0        0    12040 2023-01-23 04:43:41.277818 uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/models.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.930464 uptick_datawarehouse-0.2.8/uptick_datawarehouse/superblocks/__init__.py
--rw-r--r--   0        0        0      175 2023-01-13 01:47:39.075510 uptick_datawarehouse-0.2.8/uptick_datawarehouse/superblocks/apps.py
--rw-r--r--   0        0        0      263 2023-01-12 03:28:28.930815 uptick_datawarehouse-0.2.8/uptick_datawarehouse/superblocks/migrations/0001_schema.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.930876 uptick_datawarehouse-0.2.8/uptick_datawarehouse/superblocks/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.932203 uptick_datawarehouse-0.2.8/uptick_datawarehouse/vitally/__init__.py
--rw-r--r--   0        0        0      167 2023-01-13 01:47:43.709643 uptick_datawarehouse-0.2.8/uptick_datawarehouse/vitally/apps.py
--rw-r--r--   0        0        0      259 2023-01-12 03:28:28.932792 uptick_datawarehouse-0.2.8/uptick_datawarehouse/vitally/migrations/0001_schema.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.932871 uptick_datawarehouse-0.2.8/uptick_datawarehouse/vitally/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.933549 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/__init__.py
--rw-r--r--   0        0        0      171 2023-01-13 01:47:49.225586 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/apps.py
--rw-r--r--   0        0        0      289 2023-01-12 03:28:28.934044 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0001_schema.py
--rw-r--r--   0        0        0    10093 2023-01-21 03:00:22.637434 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0002_initial.py
--rw-r--r--   0        0        0      396 2023-02-05 23:37:37.374239 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0003_serverusage_contractor_addons_used.py
--rw-r--r--   0        0        0      945 2023-04-12 07:38:38.179175 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0004_customreportsummary.py
--rw-r--r--   0        0        0      915 2023-07-04 23:19:50.124823 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0005_auto_20230606_0658.py
--rw-r--r--   0        0        0      391 2023-07-04 23:19:52.151323 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0006_usagemetrics_for_date.py
--rw-r--r--   0        0        0      935 2023-07-04 23:19:52.151461 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0007_auto_20230704_2306.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.934250 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/__init__.py
--rw-r--r--   0        0        0     8142 2023-07-04 23:19:52.151672 uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/models.py
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 uptick_datawarehouse-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/public_readme.md
+-rw-r--r--   0        0        0      526 2023-10-09 11:58:35.192324 uptick_datawarehouse-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/model_settings.py
+-rw-r--r--   0        0        0        0 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/__init__.py
+-rw-r--r--   0        0        0      191 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/apps.py
+-rw-r--r--   0        0        0      271 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/migrations/0001_schema.py
+-rw-r--r--   0        0        0    14332 2023-06-05 09:09:52.897259 uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/migrations/0002_changesummary_chargesummary_paymentmethodsummary_recurringcreditsummary_revenueforecastsummary_subsc.py
+-rw-r--r--   0        0        0      699 2023-06-05 09:09:52.897348 uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/migrations/0003_auto_20230123_0443.py
+-rw-r--r--   0        0        0        0 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/migrations/__init__.py
+-rw-r--r--   0        0        0    12040 2023-06-05 09:09:52.897502 uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/models.py
+-rw-r--r--   0        0        0        0 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/superblocks/__init__.py
+-rw-r--r--   0        0        0      175 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/superblocks/apps.py
+-rw-r--r--   0        0        0      263 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/superblocks/migrations/0001_schema.py
+-rw-r--r--   0        0        0        0 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/superblocks/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/vitally/__init__.py
+-rw-r--r--   0        0        0      167 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/vitally/apps.py
+-rw-r--r--   0        0        0      259 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/vitally/migrations/0001_schema.py
+-rw-r--r--   0        0        0        0 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/vitally/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/__init__.py
+-rw-r--r--   0        0        0      171 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/apps.py
+-rw-r--r--   0        0        0      289 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0001_schema.py
+-rw-r--r--   0        0        0    10093 2023-06-05 09:09:52.897658 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0002_initial.py
+-rw-r--r--   0        0        0      396 2023-06-05 09:09:52.897744 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0003_serverusage_contractor_addons_used.py
+-rw-r--r--   0        0        0      945 2023-06-05 09:09:52.897842 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0004_customreportsummary.py
+-rw-r--r--   0        0        0      915 2023-06-06 19:23:17.243077 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0005_auto_20230606_0658.py
+-rw-r--r--   0        0        0      391 2023-10-05 10:23:41.215036 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0006_usagemetrics_for_date.py
+-rw-r--r--   0        0        0      935 2023-10-05 10:23:41.215421 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0007_auto_20230704_2306.py
+-rw-r--r--   0        0        0      348 2023-10-09 11:58:29.704858 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0008_remove_constancesetting_last_reported.py
+-rw-r--r--   0        0        0        0 2023-01-15 22:08:06.000000 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/__init__.py
+-rw-r--r--   0        0        0     8084 2023-10-09 11:58:29.705320 uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/models.py
+-rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 uptick_datawarehouse-0.2.9/PKG-INFO
```

### Comparing `uptick_datawarehouse-0.2.8/pyproject.toml` & `uptick_datawarehouse-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uptick-datawarehouse"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["william chu <william.chu@uptickhq.com>"]
 readme = "public_readme.md"
 
 packages = [{ include = "app" }, { include = "uptick_datawarehouse" }]
 exclude = ["app"]
```

### Comparing `uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/migrations/0002_changesummary_chargesummary_paymentmethodsummary_recurringcreditsummary_revenueforecastsummary_subsc.py` & `uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/migrations/0002_changesummary_chargesummary_paymentmethodsummary_recurringcreditsummary_revenueforecastsummary_subsc.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/migrations/0003_auto_20230123_0443.py` & `uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/migrations/0003_auto_20230123_0443.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.8/uptick_datawarehouse/subscriptionmanager/models.py` & `uptick_datawarehouse-0.2.9/uptick_datawarehouse/subscriptionmanager/models.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0002_initial.py` & `uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0004_customreportsummary.py` & `uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0004_customreportsummary.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0005_auto_20230606_0658.py` & `uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0005_auto_20230606_0658.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/migrations/0007_auto_20230704_2306.py` & `uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/migrations/0007_auto_20230704_2306.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.8/uptick_datawarehouse/workforce/models.py` & `uptick_datawarehouse-0.2.9/uptick_datawarehouse/workforce/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,15 @@
         db_table = 'workforce"."address_summary'
 
 
 class ConstanceSetting(models.Model):
     slug = models.CharField(max_length=100)
     setting_name = models.TextField()
     setting_value = models.TextField(null=True)
-    last_reported = models.DateTimeField()
-    last_synced = models.DateTimeField(null=True)  # soft rename
+    last_synced = models.DateTimeField(null=True)
 
     class Meta:
         managed = model_settings.DATAWAREHOUSE_MANAGED_MODELS
         app_label = 'workforce'
         default_permissions = ()
         db_table = 'workforce"."constance_summary'
```

