# Comparing `tmp/news-signals-0.5.0.tar.gz` & `tmp/news_signals-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-signals-0.5.0.tar", last modified: Fri Mar 29 08:01:58 2024, max compression
+gzip compressed data, was "news_signals-0.6.0.tar", last modified: Mon Apr 15 11:10:40 2024, max compression
```

## Comparing `news-signals-0.5.0.tar` & `news_signals-0.6.0.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:01:58.315519 news-signals-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 08:01:52.000000 news-signals-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-29 08:01:52.000000 news-signals-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-03-29 08:01:58.315519 news-signals-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-03-29 08:01:52.000000 news-signals-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 08:01:52.000000 news-signals-0.5.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:01:58.303519 news-signals-0.5.0/news_signals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/newsapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/representative_story.py
--rw-r--r--   0 runner    (1001) docker     (127)    49404 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    19313 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/summarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_newsapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_representative_story.py
--rw-r--r--   0 runner    (1001) docker     (127)    30372 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13998 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/wikidata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-29 08:01:52.000000 news-signals-0.5.0/news_signals/yfinance_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:01:58.315519 news-signals-0.5.0/news_signals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-03-29 08:01:58.000000 news-signals-0.5.0/news_signals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-03-29 08:01:58.000000 news-signals-0.5.0/news_signals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 08:01:58.000000 news-signals-0.5.0/news_signals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-29 08:01:58.000000 news-signals-0.5.0/news_signals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 08:01:58.000000 news-signals-0.5.0/news_signals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:01:58.299519 news-signals-0.5.0/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:01:58.307519 news-signals-0.5.0/resources/test/
--rw-r--r--   0 runner    (1001) docker     (127)    28512 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/elon_musk_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100.small.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:01:58.315519 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)   110293 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)   113236 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)    90390 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)   131955 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)   123388 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)   109117 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)    91683 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)    94002 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)   100871 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (127)   135305 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28298 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/politics_china_australia_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (127)   235658 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/sample_stories.json
--rw-r--r--   0 runner    (1001) docker     (127)   218541 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/tesla_stories.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:01:58.315519 news-signals-0.5.0/resources/test/wiki-current-events-portal/
--rw-r--r--   0 runner    (1001) docker     (127)   439022 2024-03-29 08:01:52.000000 news-signals-0.5.0/resources/test/wiki-current-events-portal/example_monthly_page_jan_2023.html
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 08:01:58.315519 news-signals-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-29 08:01:52.000000 news-signals-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:10:40.593434 news_signals-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 11:10:36.000000 news_signals-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 11:10:36.000000 news_signals-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-15 11:10:40.593434 news_signals-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-15 11:10:36.000000 news_signals-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 11:10:36.000000 news_signals-0.6.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:10:40.581434 news_signals-0.6.0/news_signals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49404 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19313 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30372 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13998 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/wikidata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-15 11:10:36.000000 news_signals-0.6.0/news_signals/yfinance_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:10:40.593434 news_signals-0.6.0/news_signals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-15 11:10:40.000000 news_signals-0.6.0/news_signals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-15 11:10:40.000000 news_signals-0.6.0/news_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:10:40.000000 news_signals-0.6.0/news_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 11:10:40.000000 news_signals-0.6.0/news_signals.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 11:10:40.000000 news_signals-0.6.0/news_signals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 11:10:40.000000 news_signals-0.6.0/news_signals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:10:40.577434 news_signals-0.6.0/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:10:40.585435 news_signals-0.6.0/resources/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    28512 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/elon_musk_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100.small.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:10:40.593434 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)   110293 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)   113236 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90390 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)   131955 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)   123388 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)   109117 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)    91683 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)    94002 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)   100871 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (127)   135305 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28298 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/politics_china_australia_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (127)   235658 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/sample_stories.json
+-rw-r--r--   0 runner    (1001) docker     (127)   218541 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/tesla_stories.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:10:40.593434 news_signals-0.6.0/resources/test/wiki-current-events-portal/
+-rw-r--r--   0 runner    (1001) docker     (127)   439022 2024-04-15 11:10:36.000000 news_signals-0.6.0/resources/test/wiki-current-events-portal/example_monthly_page_jan_2023.html
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:10:40.593434 news_signals-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-15 11:10:36.000000 news_signals-0.6.0/setup.py
```

### Comparing `news-signals-0.5.0/LICENSE` & `news_signals-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/PKG-INFO` & `news_signals-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-signals
-Version: 0.5.0
+Version: 0.6.0
 Summary: A library for working with text and timeseries data.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: arrow>=1.1.1
 Requires-Dist: gdown>=4.6.4
 Requires-Dist: google-cloud-storage>=2.10.0
@@ -22,23 +22,23 @@
 Requires-Dist: Wikidata>=0.7.0
 
 # News Signals
 
 ### Example Colab Notebooks
 
 These notebooks let you try out `news-signals` without installing anything!
+The Colab notebooks below are also available as jupyter notebooks in [research/news-signals-example-notebooks](research/news-signals-example-notebooks)
 
 - [Create a Signals Dataset from a CSV of Entity Names](https://drive.google.com/file/d/1Czm6JxIVapE6tnu9mGzRK9j2NmC0blPR/view?usp=share_link)         
 - [Find Emerging Categories in a Newsfeed](https://drive.google.com/file/d/1NVBdCfKL3qdSIGITcLsewGETTqn-V9j6/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=oJa-xWusaCQ)       
 - [Searching the Aylien NewsAPI Using An Entity Name](https://drive.google.com/file/d/1zKCSjWqxRJCPWBaGKXt5oQwkOzT8aDSg/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=HdoOiMXOrQ8)      
 - [An Overview of News Signals Datasets](https://drive.google.com/file/d/1zM4J3jFA9v2LDTFKOpaa3EUUGhOdQieo/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=wOMDSMxVUHY)
 
-The Colab notebooks above are also available as jupyter notebooks in [research/news-signals-example-notebooks](research/news-signals-example-notebooks)
 
-**2023-11-30: NEW**: [Create_Wikimedia_Signals.ipynb](research/news-signals-example-notebooks/Create_Wikimedia_Signals.ipynb) shows how to build and explore a `WikimediaSignal` which does not a NewsAPI account and works out-of-the-box for anyone.
+**2023-11-30: NEW**: [Create_Wikimedia_Signals.ipynb](research/news-signals-example-notebooks/Create_Wikimedia_Signals.ipynb) shows how to build and explore a `WikimediaSignal` which does require not a NewsAPI account and works out-of-the-box for anyone.
 
 ## Quickstart
 
 
 #### Install news-signals in a new environment
 ```
 conda create -n test-signals-pypi python=3.8
```

### Comparing `news-signals-0.5.0/README.md` & `news_signals-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # News Signals
 
 ### Example Colab Notebooks
 
 These notebooks let you try out `news-signals` without installing anything!
+The Colab notebooks below are also available as jupyter notebooks in [research/news-signals-example-notebooks](research/news-signals-example-notebooks)
 
 - [Create a Signals Dataset from a CSV of Entity Names](https://drive.google.com/file/d/1Czm6JxIVapE6tnu9mGzRK9j2NmC0blPR/view?usp=share_link)         
 - [Find Emerging Categories in a Newsfeed](https://drive.google.com/file/d/1NVBdCfKL3qdSIGITcLsewGETTqn-V9j6/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=oJa-xWusaCQ)       
 - [Searching the Aylien NewsAPI Using An Entity Name](https://drive.google.com/file/d/1zKCSjWqxRJCPWBaGKXt5oQwkOzT8aDSg/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=HdoOiMXOrQ8)      
 - [An Overview of News Signals Datasets](https://drive.google.com/file/d/1zM4J3jFA9v2LDTFKOpaa3EUUGhOdQieo/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=wOMDSMxVUHY)
 
-The Colab notebooks above are also available as jupyter notebooks in [research/news-signals-example-notebooks](research/news-signals-example-notebooks)
 
-**2023-11-30: NEW**: [Create_Wikimedia_Signals.ipynb](research/news-signals-example-notebooks/Create_Wikimedia_Signals.ipynb) shows how to build and explore a `WikimediaSignal` which does not a NewsAPI account and works out-of-the-box for anyone.
+**2023-11-30: NEW**: [Create_Wikimedia_Signals.ipynb](research/news-signals-example-notebooks/Create_Wikimedia_Signals.ipynb) shows how to build and explore a `WikimediaSignal` which does require not a NewsAPI account and works out-of-the-box for anyone.
 
 ## Quickstart
 
 
 #### Install news-signals in a new environment
 ```
 conda create -n test-signals-pypi python=3.8
```

### Comparing `news-signals-0.5.0/news_signals/anomaly_detection.py` & `news_signals-0.6.0/news_signals/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/aql_builder.py` & `news_signals-0.6.0/news_signals/aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/data.py` & `news_signals-0.6.0/news_signals/data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/dataset_transformations.py` & `news_signals-0.6.0/news_signals/dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/exogenous_signals.py` & `news_signals-0.6.0/news_signals/exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/newsapi.py` & `news_signals-0.6.0/news_signals/newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/plotting.py` & `news_signals-0.6.0/news_signals/plotting.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/representative_story.py` & `news_signals-0.6.0/news_signals/representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/signals.py` & `news_signals-0.6.0/news_signals/signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/signals_dataset.py` & `news_signals-0.6.0/news_signals/signals_dataset.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/summarization.py` & `news_signals-0.6.0/news_signals/summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_anomaly_detection.py` & `news_signals-0.6.0/news_signals/test_anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_aql_builder.py` & `news_signals-0.6.0/news_signals/test_aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_data.py` & `news_signals-0.6.0/news_signals/test_data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_dataset_transformations.py` & `news_signals-0.6.0/news_signals/test_dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_exogenous_signals.py` & `news_signals-0.6.0/news_signals/test_exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_newsapi.py` & `news_signals-0.6.0/news_signals/test_newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_representative_story.py` & `news_signals-0.6.0/news_signals/test_representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_signals.py` & `news_signals-0.6.0/news_signals/test_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_signals_dataset.py` & `news_signals-0.6.0/news_signals/test_signals_dataset.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/test_summarization.py` & `news_signals-0.6.0/news_signals/test_summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/users.py` & `news_signals-0.6.0/news_signals/users.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/wikidata_utils.py` & `news_signals-0.6.0/news_signals/wikidata_utils.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals/yfinance_timeseries.py` & `news_signals-0.6.0/news_signals/yfinance_timeseries.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/news_signals.egg-info/PKG-INFO` & `news_signals-0.6.0/news_signals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-signals
-Version: 0.5.0
+Version: 0.6.0
 Summary: A library for working with text and timeseries data.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: arrow>=1.1.1
 Requires-Dist: gdown>=4.6.4
 Requires-Dist: google-cloud-storage>=2.10.0
@@ -22,23 +22,23 @@
 Requires-Dist: Wikidata>=0.7.0
 
 # News Signals
 
 ### Example Colab Notebooks
 
 These notebooks let you try out `news-signals` without installing anything!
+The Colab notebooks below are also available as jupyter notebooks in [research/news-signals-example-notebooks](research/news-signals-example-notebooks)
 
 - [Create a Signals Dataset from a CSV of Entity Names](https://drive.google.com/file/d/1Czm6JxIVapE6tnu9mGzRK9j2NmC0blPR/view?usp=share_link)         
 - [Find Emerging Categories in a Newsfeed](https://drive.google.com/file/d/1NVBdCfKL3qdSIGITcLsewGETTqn-V9j6/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=oJa-xWusaCQ)       
 - [Searching the Aylien NewsAPI Using An Entity Name](https://drive.google.com/file/d/1zKCSjWqxRJCPWBaGKXt5oQwkOzT8aDSg/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=HdoOiMXOrQ8)      
 - [An Overview of News Signals Datasets](https://drive.google.com/file/d/1zM4J3jFA9v2LDTFKOpaa3EUUGhOdQieo/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=wOMDSMxVUHY)
 
-The Colab notebooks above are also available as jupyter notebooks in [research/news-signals-example-notebooks](research/news-signals-example-notebooks)
 
-**2023-11-30: NEW**: [Create_Wikimedia_Signals.ipynb](research/news-signals-example-notebooks/Create_Wikimedia_Signals.ipynb) shows how to build and explore a `WikimediaSignal` which does not a NewsAPI account and works out-of-the-box for anyone.
+**2023-11-30: NEW**: [Create_Wikimedia_Signals.ipynb](research/news-signals-example-notebooks/Create_Wikimedia_Signals.ipynb) shows how to build and explore a `WikimediaSignal` which does require not a NewsAPI account and works out-of-the-box for anyone.
 
 ## Quickstart
 
 
 #### Install news-signals in a new environment
 ```
 conda create -n test-signals-pypi python=3.8
```

### Comparing `news-signals-0.5.0/news_signals.egg-info/SOURCES.txt` & `news_signals-0.6.0/news_signals.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 VERSION
 setup.py
 news_signals/__init__.py
 news_signals/anomaly_detection.py
 news_signals/aql_builder.py
+news_signals/cli.py
 news_signals/data.py
 news_signals/dataset_transformations.py
 news_signals/exogenous_signals.py
 news_signals/log.py
 news_signals/newsapi.py
 news_signals/plotting.py
 news_signals/representative_story.py
@@ -28,14 +29,15 @@
 news_signals/test_summarization.py
 news_signals/users.py
 news_signals/wikidata_utils.py
 news_signals/yfinance_timeseries.py
 news_signals.egg-info/PKG-INFO
 news_signals.egg-info/SOURCES.txt
 news_signals.egg-info/dependency_links.txt
+news_signals.egg-info/entry_points.txt
 news_signals.egg-info/requires.txt
 news_signals.egg-info/top_level.txt
 resources/test/elon_musk_timeseries.json
 resources/test/nasdaq100.small.csv
 resources/test/politics_china_australia_timeseries.json
 resources/test/sample_stories.json
 resources/test/tesla_stories.json
```

### Comparing `news-signals-0.5.0/resources/test/elon_musk_timeseries.json` & `news_signals-0.6.0/resources/test/elon_musk_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news_signals-0.6.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/politics_china_australia_timeseries.json` & `news_signals-0.6.0/resources/test/politics_china_australia_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/sample_stories.json` & `news_signals-0.6.0/resources/test/sample_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/tesla_stories.json` & `news_signals-0.6.0/resources/test/tesla_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/resources/test/wiki-current-events-portal/example_monthly_page_jan_2023.html` & `news_signals-0.6.0/resources/test/wiki-current-events-portal/example_monthly_page_jan_2023.html`

 * *Files identical despite different names*

### Comparing `news-signals-0.5.0/setup.py` & `news_signals-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,12 +31,16 @@
 setup(
     name="news-signals",
     version=version,
     description="A library for working with text and timeseries data.",
     install_requires=INSTALL_REQUIRES,
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    readme="README.md",
     packages=["news_signals"],
     data_files=["LICENSE", "VERSION", "README.md"],
+    entry_points={
+        'console_scripts': [
+            'generate-dataset=news_signals.cli:generate_dataset'
+        ]
+    },
     include_package_data=True
 )
```

