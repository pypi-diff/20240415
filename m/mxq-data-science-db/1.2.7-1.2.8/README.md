# Comparing `tmp/mxq_data_science_db-1.2.7.tar.gz` & `tmp/mxq_data_science_db-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxq_data_science_db-1.2.7.tar", max compression
+gzip compressed data, was "mxq_data_science_db-1.2.8.tar", max compression
```

## Comparing `mxq_data_science_db-1.2.7.tar` & `mxq_data_science_db-1.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1404 2024-01-10 12:04:51.418729 mxq_data_science_db-1.2.7/README.md
--rw-r--r--   0        0        0        0 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/db/__init__.py
--rw-r--r--   0        0        0     2150 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/db/db.py
--rw-r--r--   0        0        0     1963 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/db/models/base.py
--rw-r--r--   0        0        0     4741 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/db/models/db_comex.py
--rw-r--r--   0        0        0     1960 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/db/models/db_commodity.py
--rw-r--r--   0        0        0     1554 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/db/models/db_economia.py
--rw-r--r--   0        0        0        0 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/settings/__init__.py
--rw-r--r--   0        0        0      714 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/settings/logger.py
--rw-r--r--   0        0        0     4223 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/settings/settings.py
--rw-r--r--   0        0        0        0 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/utils/__init__.py
--rw-r--r--   0        0        0     4271 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/utils/data_lake.py
--rw-r--r--   0        0        0     5390 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/utils/dropbox.py
--rw-r--r--   0        0        0     1461 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/utils/teams_alert.py
--rw-r--r--   0        0        0      504 2024-01-10 12:04:51.422729 mxq_data_science_db-1.2.7/mxq_data_science_db/utils/utils.py
--rw-r--r--   0        0        0      439 2024-01-10 12:05:18.722810 mxq_data_science_db-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     2009 1970-01-01 00:00:00.000000 mxq_data_science_db-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1404 2024-04-15 10:32:14.210790 mxq_data_science_db-1.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 10:32:14.210790 mxq_data_science_db-1.2.8/mxq_data_science_db/db/__init__.py
+-rw-r--r--   0        0        0     2150 2024-04-15 10:32:14.210790 mxq_data_science_db-1.2.8/mxq_data_science_db/db/db.py
+-rw-r--r--   0        0        0     1963 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/db/models/base.py
+-rw-r--r--   0        0        0     4741 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/db/models/db_comex.py
+-rw-r--r--   0        0        0     1960 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/db/models/db_commodity.py
+-rw-r--r--   0        0        0     1554 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/db/models/db_economia.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/settings/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/settings/logger.py
+-rw-r--r--   0        0        0     4141 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/settings/settings.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/utils/__init__.py
+-rw-r--r--   0        0        0     4271 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/utils/data_lake.py
+-rw-r--r--   0        0        0     5390 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/utils/dropbox.py
+-rw-r--r--   0        0        0     1461 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/utils/teams_alert.py
+-rw-r--r--   0        0        0      504 2024-04-15 10:32:14.214789 mxq_data_science_db-1.2.8/mxq_data_science_db/utils/utils.py
+-rw-r--r--   0        0        0      439 2024-04-15 10:32:32.362850 mxq_data_science_db-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2009 1970-01-01 00:00:00.000000 mxq_data_science_db-1.2.8/PKG-INFO
```

### Comparing `mxq_data_science_db-1.2.7/README.md` & `mxq_data_science_db-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/db/db.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/db/db.py`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/db/models/base.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/db/models/base.py`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/db/models/db_comex.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/db/models/db_comex.py`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/db/models/db_commodity.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/db/models/db_commodity.py`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/db/models/db_economia.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/db/models/db_economia.py`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/settings/logger.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/settings/logger.py`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/settings/settings.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/settings/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,18 +109,18 @@
 
         get_secret_value_response = client.get_secret_value(SecretId=aws_secretmanager)
 
         return json.loads(get_secret_value_response["SecretString"])
 
     def _set_DB_from_secret(self):
         """Set secrets for HMG e PROD"""
-        self.DB_GCP_HOST = self.sql_secret_json["DB_GCP_HOST"]
         self.DB_GCP_PORT = self.sql_secret_json["DB_GCP_PORT"]
         self.db_secret = self.sql_secret_json.get(self.DATABASE.upper())
         assert self.db_secret, "Database secret not found in AWS secret"
+        self.DB_GCP_HOST = self.db_secret.get(self.ENV.upper()).get("HOST")
         self.DB_GCP_USER = self.db_secret.get(self.ENV.upper()).get("USER")
         self.DB_GCP_PASSWORD = self.db_secret.get(self.ENV.upper()).get("PASSWORD")
 
     def _dev_secrets(self):
         """Set secrets for development"""
         self.DB_GCP_HOST = os.environ.get("DB_GCP_HOST", "127.0.01") 
         self.DB_GCP_PORT = 3306
@@ -129,13 +129,10 @@
 
     def build_db_url(self):
         """Build MySQL url
 
         Returns:
             mysql url
         """
-        if self.ENV == Settings.HMG:
-            db = self.DATABASE + "_hmg"
-        else:
-            db = self.DATABASE
+        db = self.DATABASE
 
         return f"mysql://{self.DB_GCP_USER}:{self.DB_GCP_PASSWORD}@{self.DB_GCP_HOST}:{self.DB_GCP_PORT}/{db}"
```

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/utils/data_lake.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/utils/data_lake.py`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/utils/dropbox.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/utils/dropbox.py`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/mxq_data_science_db/utils/teams_alert.py` & `mxq_data_science_db-1.2.8/mxq_data_science_db/utils/teams_alert.py`

 * *Files identical despite different names*

### Comparing `mxq_data_science_db-1.2.7/PKG-INFO` & `mxq_data_science_db-1.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxq-data-science-db
-Version: 1.2.7
+Version: 1.2.8
 Summary: Package to manage DBs and Models
 Author: Miguel Hentoux
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

