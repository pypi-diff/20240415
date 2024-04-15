# Comparing `tmp/dmk_packages-0.6.1.tar.gz` & `tmp/dmk_packages-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.6.1.tar", last modified: Tue Apr  9 02:18:09 2024, max compression
+gzip compressed data, was "dmk_packages-0.6.2.tar", last modified: Mon Apr 15 05:51:13 2024, max compression
```

## Comparing `dmk_packages-0.6.1.tar` & `dmk_packages-0.6.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-09 02:18:09.235592 dmk_packages-0.6.1/
--rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/LICENSE
--rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-09 02:18:09.235349 dmk_packages-0.6.1/PKG-INFO
--rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/README.md
--rw-r--r--   0 tommie     (501) staff       (20)      584 2024-04-09 01:40:27.000000 dmk_packages-0.6.1/pyproject.toml
--rw-r--r--   0 tommie     (501) staff       (20)       38 2024-04-09 02:18:09.235655 dmk_packages-0.6.1/setup.cfg
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-09 02:18:09.229451 dmk_packages-0.6.1/src/
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-09 02:18:09.230862 dmk_packages-0.6.1/src/dmk_packages/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/src/dmk_packages/__init__.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-09 02:18:09.234167 dmk_packages-0.6.1/src/dmk_packages/crawler/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 tommie     (501) staff       (20)     6703 2024-04-09 01:39:29.000000 dmk_packages-0.6.1/src/dmk_packages/crawler/bigkinds.py
--rw-r--r--   0 tommie     (501) staff       (20)     7812 2024-04-09 02:17:24.000000 dmk_packages-0.6.1/src/dmk_packages/crawler/clien.py
--rw-r--r--   0 tommie     (501) staff       (20)     6418 2024-04-09 01:26:16.000000 dmk_packages-0.6.1/src/dmk_packages/crawler/fnguide.py
--rw-r--r--   0 tommie     (501) staff       (20)     2743 2024-04-09 01:39:49.000000 dmk_packages-0.6.1/src/dmk_packages/crawler/fnguide_pdf_update.py
--rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 tommie     (501) staff       (20)    15349 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 tommie     (501) staff       (20)    12855 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/src/dmk_packages/crawler/youtube.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-09 02:18:09.234710 dmk_packages-0.6.1/src/dmk_packages/database/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/src/dmk_packages/database/__init__.py
--rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/src/dmk_packages/database/database.py
--rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.6.1/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-09 02:18:09.235057 dmk_packages-0.6.1/src/dmk_packages.egg-info/
--rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-09 02:18:09.000000 dmk_packages-0.6.1/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 tommie     (501) staff       (20)      684 2024-04-09 02:18:09.000000 dmk_packages-0.6.1/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 tommie     (501) staff       (20)        1 2024-04-09 02:18:09.000000 dmk_packages-0.6.1/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 tommie     (501) staff       (20)       41 2024-04-09 02:18:09.000000 dmk_packages-0.6.1/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 tommie     (501) staff       (20)       13 2024-04-09 02:18:09.000000 dmk_packages-0.6.1/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.695471 dmk_packages-0.6.2/
+-rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/LICENSE
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-15 05:51:13.695086 dmk_packages-0.6.2/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/README.md
+-rw-r--r--   0 layla      (501) staff       (20)      584 2024-04-15 05:48:43.000000 dmk_packages-0.6.2/pyproject.toml
+-rw-r--r--   0 layla      (501) staff       (20)       38 2024-04-15 05:51:13.695564 dmk_packages-0.6.2/setup.cfg
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.682505 dmk_packages-0.6.2/src/
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.685380 dmk_packages-0.6.2/src/dmk_packages/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/src/dmk_packages/__init__.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.692862 dmk_packages-0.6.2/src/dmk_packages/crawler/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     6713 2024-04-15 02:00:53.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 layla      (501) staff       (20)     7812 2024-04-15 02:00:53.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 layla      (501) staff       (20)     6418 2024-04-15 02:00:53.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 layla      (501) staff       (20)     2743 2024-04-15 02:00:53.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/fnguide_pdf_update.py
+-rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 layla      (501) staff       (20)    15349 2024-04-15 02:00:30.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 layla      (501) staff       (20)    13392 2024-04-15 05:34:36.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.693928 dmk_packages-0.6.2/src/dmk_packages/database/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-15 03:09:28.000000 dmk_packages-0.6.2/src/dmk_packages/database/database.py
+-rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.694646 dmk_packages-0.6.2/src/dmk_packages.egg-info/
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)      684 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 layla      (501) staff       (20)        1 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 layla      (501) staff       (20)       41 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 layla      (501) staff       (20)       13 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.6.1/LICENSE` & `dmk_packages-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.1/PKG-INFO` & `dmk_packages-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.1
+Version: 0.6.2
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.1/README.md` & `dmk_packages-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.1/pyproject.toml` & `dmk_packages-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.6.1"
+version = "0.6.2"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.6.1/src/dmk_packages/crawler/bigkinds.py` & `dmk_packages-0.6.2/src/dmk_packages/crawler/bigkinds.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                         "url": df["URL"][i],
                         "except": df["분석제외 여부"][i],
                         "created_at": self.crawl_date,
                     }
                     data_list.append(data)
             return data_list
         except Exception as e:
-            logger.error(f"데이터 적재 실패 | error_comment : {e}")
+            logger.error(f"데이터 저장 or 변환 실패 | error_comment : {e}")
 
     async def bigkinds_crawl(self, cat):
         """
         playwright 크롤러 전반적인 운영
         """
         # playwright 실행 및 크롤링
         logger.info(f"[{cat}] 크롤링 시작")
```

### Comparing `dmk_packages-0.6.1/src/dmk_packages/crawler/clien.py` & `dmk_packages-0.6.2/src/dmk_packages/crawler/clien.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.1/src/dmk_packages/crawler/fnguide.py` & `dmk_packages-0.6.2/src/dmk_packages/crawler/fnguide.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.1/src/dmk_packages/crawler/fnguide_pdf_update.py` & `dmk_packages-0.6.2/src/dmk_packages/crawler/fnguide_pdf_update.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.1/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.6.2/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.1/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.6.2/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.1/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.6.2/src/dmk_packages/crawler/youtube.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 import time
 from typing import List
+from datetime import datetime
 
 import pendulum
 from loguru import logger
-from sqlalchemy import text
+from sqlalchemy.sql import func
+from sqlalchemy import text, Column, Integer, String, Date, DateTime, UniqueConstraint
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 
 from dmk_packages.database import database as db
 
 
 class YoutubeDBHandler:
     # ==============================================================================
     # NOTE : 한투(postgres)로 데이터베이스 설정
-    def __init__(self, target="KOREAINVESTMENT_DMK"):
-        self._krinv_engine = db.get_engine(target)
-        self._meta_table = "t_metadata_youtube"
-        if not self._krinv_engine:
+    def __init__(self, target="KOREAINVESTMENT_DMK", meta_table_name="t_metadata_youtube"):
+        self._db_engine = db.get_engine(target)
+        self._meta_table = meta_table_name
+        db.create_to_postgres(
+            self._db_engine,
+            self._meta_table,
+            Column("id", Integer, primary_key=True, autoincrement=True),
+            Column("keyword", String),
+            Column("next_page_token", String),
+            Column("target_date", Date),
+            Column("created_at", DateTime, nullable=False, server_default=func.now()),
+            UniqueConstraint("id", name="t_metadata_youtube_pk")
+        )
+        if not self._db_engine:
             raise ValueError("데이터베이스 엔진 설정에 실패했습니다.")
     # ==============================================================================
 
     # ==============================================================================
     # NOTE : json 응답에 있는 "next_page_token" 키에 해당하는 값을 metadata 테이블에 저장
     def _save_page_token(self, keyword, target_date, next_page_token):
         query = f"""
         INSERT INTO {self._meta_table} (keyword, next_page_token, target_date)
         VALUES ('{keyword}', '{next_page_token}', '{target_date}');
         """
 
         try:
-            with self._krinv_engine.begin() as connection:
+            with self._db_engine.begin() as connection:
                 connection.execute(text(query))
             logger.info(
                 f"[{keyword}][{target_date}]: Metadata insertion completed."
             )
         except Exception as err:
             logger.error(err)
     # ==============================================================================
@@ -45,15 +57,15 @@
         SELECT next_page_token
         FROM {self._meta_table}
         WHERE keyword = '{keyword}'
             AND target_date = '{target_date}';
         """
 
         try:
-            with self._krinv_engine.begin() as connection:
+            with self._db_engine.begin() as connection:
                 result = connection.execute(text(query)).fetchone()
                 return result[0] if result else False
         except Exception as err:
             logger.error(err)
     # ==============================================================================
 
     # ==============================================================================
@@ -63,15 +75,15 @@
         UPDATE {self._meta_table}
         SET next_page_token = '{next_page_token}'
         WHERE keyword = '{keyword}'
             AND target_date = '{target_date}'
         """
 
         try:
-            with self._krinv_engine.begin() as connection:
+            with self._db_engine.begin() as connection:
                 connection.execute(text(query))
             logger.info(f"[{keyword}][{target_date}]: Metadata update completed.")
         except Exception as err:
             logger.error(err)
     # ==============================================================================
 
 
@@ -276,16 +288,15 @@
 
         except Exception as err:
             logger.error(err)
     # ==============================================================================
 
     # ==============================================================================
     # NOTE : _results 값 반환
-    def get_videos_info(self, keywords_target_dates):
-        keyword, target_date = keywords_target_dates
+    def get_videos_info(self, keyword, target_date):
         next_page_token = self._get_page_token(keyword, target_date)
 
         if next_page_token == 'None':
             logger.info(f"[{keyword}][{target_date}]: 이미 수집 완료")
         elif not next_page_token:
             # logger.info(f"[{keyword}][{target_date}]: 수집 필요")
             self._stack_videos_info(keyword, target_date)
```

### Comparing `dmk_packages-0.6.1/src/dmk_packages/database/database.py` & `dmk_packages-0.6.2/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.1/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.6.2/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.1/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.6.2/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.1
+Version: 0.6.2
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.1/src/dmk_packages.egg-info/SOURCES.txt` & `dmk_packages-0.6.2/src/dmk_packages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

