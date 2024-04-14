# Comparing `tmp/webscraperr-0.1.7.tar.gz` & `tmp/webscraperr-0.1.8.tar.gz`

## Comparing `webscraperr-0.1.7.tar` & `webscraperr-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 webscraperr-0.1.7/src/webscraperr/__init__.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 webscraperr-0.1.7/src/webscraperr/config.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 webscraperr-0.1.7/src/webscraperr/db.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 webscraperr-0.1.7/src/webscraperr/driver.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 webscraperr-0.1.7/src/webscraperr/exceptions.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 webscraperr-0.1.7/src/webscraperr/utils.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 webscraperr-0.1.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 webscraperr-0.1.7/LICENSE
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 webscraperr-0.1.7/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 webscraperr-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 webscraperr-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 webscraperr-0.1.8/src/webscraperr/__init__.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 webscraperr-0.1.8/src/webscraperr/config.py
+-rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 webscraperr-0.1.8/src/webscraperr/db.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 webscraperr-0.1.8/src/webscraperr/driver.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 webscraperr-0.1.8/src/webscraperr/exceptions.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 webscraperr-0.1.8/src/webscraperr/utils.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 webscraperr-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 webscraperr-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 webscraperr-0.1.8/README.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 webscraperr-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 webscraperr-0.1.8/PKG-INFO
```

### Comparing `webscraperr-0.1.7/src/webscraperr/__init__.py` & `webscraperr-0.1.8/src/webscraperr/__init__.py`

 * *Files identical despite different names*

### Comparing `webscraperr-0.1.7/src/webscraperr/config.py` & `webscraperr-0.1.8/src/webscraperr/config.py`

 * *Files identical despite different names*

### Comparing `webscraperr-0.1.7/src/webscraperr/db.py` & `webscraperr-0.1.8/src/webscraperr/db.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,26 +44,28 @@
     with connect(**database_config['AUTH']) as conn:
         cursor = conn.cursor()
         cursor.execute(f"""
             CREATE TABLE IF NOT EXISTS`{database_config['DATABASE']}`.`{database_config['TABLE']}` (
             `ID` INT NOT NULL AUTO_INCREMENT,
             `URL` VARCHAR(255) NOT NULL,
             `INFO` JSON NULL,
+            `CATEGORY` VARCHAR(255) NULL,
             PRIMARY KEY (`ID`),
             UNIQUE INDEX `URL_UNIQUE` (`URL` ASC) VISIBLE);
         """)
 
 def init_sqlite(database_config: dict):
     with sqlite3.connect(database_config['DATABASE']) as conn:
         conn.execute(f"""
             CREATE TABLE IF NOT EXISTS {database_config['TABLE']} (
         ID   INTEGER NOT NULL
                     PRIMARY KEY AUTOINCREMENT,
         URL  TEXT    NOT NULL
                     UNIQUE,
+        CATEGORY TEXT NULL,
         INFO TEXT
         );
     """)
 
 class WebScraperDBSqlite:
     def __init__(self, config):
         self.config = config
@@ -77,45 +79,50 @@
         return self
     
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.conn:
             self.conn.commit()
             self.conn.close()
 
-    def get_all(self):
-        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']}")
+    def get_all(self, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE CATEGORY=?", [category])
         return self.cursor.fetchall()
 
-    def get_all_without_info(self):
-        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE INFO IS NULL")
+    def get_all_without_info(self, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE INFO IS NULL AND CATEGORY=?", [category])
         return self.cursor.fetchall()
     
-    def get_all_with_info(self):
-        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE INFO IS NOT NULL")
+    def get_all_with_info(self, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE INFO IS NOT NULL AND CATEGORY=?", [category])
         return self.cursor.fetchall()
     
     def get_by_id(self, id: int):
         self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE ID=?", [id])
         return self.cursor.fetchone()
 
     def get_by_url(self, url: int):
         self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE URL=?", [url])
         return self.cursor.fetchone()
 
-    def save_url(self, url: str):
-        self.cursor.execute(f"INSERT OR IGNORE INTO {self.config['TABLE']}(URL) VALUES(?)", [url])
+    def save_url(self, url: str, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"INSERT OR IGNORE INTO {self.config['TABLE']}(URL, CATEGORY) VALUES(?, ?)", [url, category])
 
     def save_urls(self, urls: list):
-        self.cursor.executemany(f"INSERT OR IGNORE INTO {self.config['TABLE']}(URL) VALUES(?)", urls)
+        self.cursor.executemany(f"INSERT OR IGNORE INTO {self.config['TABLE']}(URL, CATEGORY) VALUES(?, ?)", urls)
 
-    def save_url_and_info(self, url: str, info: str):
-        self.cursor.execute(f"INSERT OR IGNORE INTO {self.config['TABLE']}(URL, INFO) VALUES(?, ?)", [url, info])
+    def save_url_and_info(self, url: str, info: str, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"INSERT OR IGNORE INTO {self.config['TABLE']}(URL, INFO) VALUES(?, ?, ?)", [url, info, category])
 
     def save_url_and_info_many(self, datas: list):
-        self.cursor.executemany(f"INSERT OR IGNORE INTO {self.config['TABLE']}(URL, INFO) VALUES(?, ?)", datas)
+        self.cursor.executemany(f"INSERT OR IGNORE INTO {self.config['TABLE']}(URL, INFO, CATEGORY) VALUES(?, ?, ?)", datas)
 
     def set_info_by_id(self, id: int, info: str):
         self.cursor.execute(f"UPDATE {self.config['TABLE']} SET INFO=? WHERE ID=?", [info, id])
     
     def set_info_by_url(self, url: str, info: str):
         self.cursor.execute(f"UPDATE {self.config['TABLE']} SET INFO=? WHERE URL=?", [info, url])
 
@@ -134,45 +141,50 @@
         return self
     
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.conn:
             self.conn.commit()
             self.conn.close()
     
-    def get_all(self):
-        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']}")
+    def get_all(self, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE CATEGORY=%s", (category, ))
         return self.cursor.fetchall()
     
-    def get_all_without_info(self):
-        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE INFO IS NULL")
+    def get_all_without_info(self, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE INFO IS NULL AND CATEGORY=%s", (category, ))
         return self.cursor.fetchall()
     
-    def get_all_with_info(self):
-        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE INFO IS NOT NULL")
+    def get_all_with_info(self, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE INFO IS NOT NULL AND CATEGORY=%s", (category, ))
         return self.cursor.fetchall()
     
     def get_by_url(self, url: str):
         self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE URL=%s", (url, ))
         return self.cursor.fetchone()
 
     def get_by_id(self, id: int):
         self.cursor.execute(f"SELECT * FROM {self.config['TABLE']} WHERE ID=%s", (id, ))
         return self.cursor.fetchone()
 
-    def save_url(self, url: str):
-        self.cursor.execute(f"INSERT IGNORE INTO {self.config['TABLE']}(URL) VALUES(%s)", (url,))
+    def save_url(self, url: str, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"INSERT IGNORE INTO {self.config['TABLE']}(URL, CATEGORY) VALUES(%s, %s)", (url, category))
     
     def save_urls(self, urls: str):
-        self.cursor.executemany(f"INSERT IGNORE INTO {self.config['TABLE']}(URL) VALUES(%s)", urls)
+        self.cursor.executemany(f"INSERT IGNORE INTO {self.config['TABLE']}(URL, CATEGORY) VALUES(%s, %s)", urls)
     
-    def save_url_and_info(self, url: str, info: str):
-        self.cursor.execute(f"INSERT IGNORE INTO {self.config['TABLE']}(URL, INFO) VALUES(%s, %s)", (url, info))
+    def save_url_and_info(self, url: str, info: str, category=None):
+        category = 'NULL' if category is None else category
+        self.cursor.execute(f"INSERT IGNORE INTO {self.config['TABLE']}(URL, INFO, CATEGORY) VALUES(%s, %s, %s)", (url, info, category))
 
     def save_url_and_info_many(self, datas: list):
-        self.cursor.executemany(f"INSERT IGNORE INTO {self.config['TABLE']}(URL, INFO) VALUES(%s, %s)", datas)
+        self.cursor.executemany(f"INSERT IGNORE INTO {self.config['TABLE']}(URL, INFO, CATEGORY) VALUES(%s, %s, %s)", datas)
 
     def set_info_by_id(self, id: int, info: str):
         self.cursor.execute(f"UPDATE {self.config['TABLE']} SET INFO=%s WHERE ID=%s", (info, id))
 
     def set_info_by_url(self, url: str, info: str):
         self.cursor.execute(f"UPDATE {self.config['TABLE']} SET INFO=%s WHERE URL=%s", (info, url))
```

### Comparing `webscraperr-0.1.7/src/webscraperr/exceptions.py` & `webscraperr-0.1.8/src/webscraperr/exceptions.py`

 * *Files identical despite different names*

### Comparing `webscraperr-0.1.7/.gitignore` & `webscraperr-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `webscraperr-0.1.7/LICENSE` & `webscraperr-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `webscraperr-0.1.7/README.md` & `webscraperr-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `webscraperr-0.1.7/pyproject.toml` & `webscraperr-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dependencies = [
   'requests',
   'parsel',
   'mysql-connector-python',
   'selenium-wire',
   'undetected-chromedriver'
 ]
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Ziegfred Zorrilla", email="ziegfredzorrilla23@gmail.com" },
 ]
 description = "A package for web scraping"
 readme = "README.md"
 requires-python = ">=3.11.2"
 classifiers = [
```

### Comparing `webscraperr-0.1.7/PKG-INFO` & `webscraperr-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: webscraperr
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for web scraping
 Project-URL: Homepage, https://github.com/zvz23/webscraperr
 Author-email: Ziegfred Zorrilla <ziegfredzorrilla23@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

