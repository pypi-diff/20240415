# Comparing `tmp/mns-scheduler-1.0.2.3.tar.gz` & `tmp/mns-scheduler-1.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.2.3.tar", last modified: Sat Apr 13 10:20:23 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.2.4.tar", last modified: Mon Apr 15 03:00:32 2024, max compression
```

## Comparing `mns-scheduler-1.0.2.3.tar` & `mns-scheduler-1.0.2.4.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.067426 mns-scheduler-1.0.2.3/
--rw-rw-rw-   0        0        0       62 2024-04-13 10:20:23.066897 mns-scheduler-1.0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.038054 mns-scheduler-1.0.2.3/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.041046 mns-scheduler-1.0.2.3/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.2.3/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.042043 mns-scheduler-1.0.2.3/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20330 2024-04-11 14:07:31.000000 mns-scheduler-1.0.2.3/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.042043 mns-scheduler-1.0.2.3/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.043041 mns-scheduler-1.0.2.3/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.045035 mns-scheduler-1.0.2.3/mns_scheduler/concept/em/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/em/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.045035 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.046032 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/app/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.048027 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     1660 2024-04-13 10:19:34.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.049026 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/symbol/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8578 2024-04-13 07:36:39.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.050022 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/web/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/web/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.051020 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/wen_cai/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.052017 mns-scheduler-1.0.2.3/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.2.3/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.053014 mns-scheduler-1.0.2.3/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.054011 mns-scheduler-1.0.2.3/mns_scheduler/ipo/
--rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.2.3/mns_scheduler/ipo/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.2.3/mns_scheduler/ipo/auto_ipo_buy_api.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.054011 mns-scheduler-1.0.2.3/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.056006 mns-scheduler-1.0.2.3/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.2.3/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7028 2024-01-09 10:50:05.000000 mns-scheduler-1.0.2.3/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.057003 mns-scheduler-1.0.2.3/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.2.3/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.057003 mns-scheduler-1.0.2.3/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.057003 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.058000 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.058998 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.059995 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0     7527 2024-04-02 14:49:34.000000 mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.061274 mns-scheduler-1.0.2.3/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.2.3/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.062300 mns-scheduler-1.0.2.3/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.2.3/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.064850 mns-scheduler-1.0.2.3/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.2.3/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.2.3/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.2.3/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.3/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-12 05:21:45.000000 mns-scheduler-1.0.2.3/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.066385 mns-scheduler-1.0.2.3/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.3/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    13768 2024-04-02 14:52:18.000000 mns-scheduler-1.0.2.3/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.2.3/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:20:23.066897 mns-scheduler-1.0.2.3/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-04-13 10:20:22.000000 mns-scheduler-1.0.2.3/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3014 2024-04-13 10:20:22.000000 mns-scheduler-1.0.2.3/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 10:20:22.000000 mns-scheduler-1.0.2.3/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-13 10:20:22.000000 mns-scheduler-1.0.2.3/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 10:20:23.067426 mns-scheduler-1.0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-04-13 10:20:21.000000 mns-scheduler-1.0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.983014 mns-scheduler-1.0.2.4/
+-rw-rw-rw-   0        0        0       62 2024-04-15 03:00:32.982017 mns-scheduler-1.0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.949103 mns-scheduler-1.0.2.4/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.951098 mns-scheduler-1.0.2.4/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.2.4/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.953092 mns-scheduler-1.0.2.4/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20330 2024-04-11 14:07:31.000000 mns-scheduler-1.0.2.4/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.954089 mns-scheduler-1.0.2.4/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.954089 mns-scheduler-1.0.2.4/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.957082 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.957082 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.958079 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/app/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.959077 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     1662 2024-04-15 02:52:26.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.961071 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8757 2024-04-15 03:00:19.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.962069 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.963066 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/wen_cai/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.965060 mns-scheduler-1.0.2.4/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.2.4/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.965060 mns-scheduler-1.0.2.4/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.966058 mns-scheduler-1.0.2.4/mns_scheduler/ipo/
+-rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.2.4/mns_scheduler/ipo/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.2.4/mns_scheduler/ipo/auto_ipo_buy_api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.967056 mns-scheduler-1.0.2.4/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.968052 mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7028 2024-01-09 10:50:05.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.969049 mns-scheduler-1.0.2.4/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.970048 mns-scheduler-1.0.2.4/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.970048 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.971044 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.972042 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.973039 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0     7527 2024-04-02 14:49:34.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.975034 mns-scheduler-1.0.2.4/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.2.4/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.976031 mns-scheduler-1.0.2.4/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.2.4/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.979024 mns-scheduler-1.0.2.4/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-12 05:21:45.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.981019 mns-scheduler-1.0.2.4/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    13768 2024-04-02 14:52:18.000000 mns-scheduler-1.0.2.4/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.2.4/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.982017 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-04-15 03:00:32.000000 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3014 2024-04-15 03:00:32.000000 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 03:00:32.000000 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 03:00:32.000000 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 03:00:32.983014 mns-scheduler-1.0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-15 03:00:19.000000 mns-scheduler-1.0.2.4/setup.py
```

### Comparing `mns-scheduler-1.0.2.3/README.md` & `mns-scheduler-1.0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.2.4/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.2.4/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 sys.path.append(project_path)
 
 import mns_common.component.concept.ths_concept_common_service_api as ths_concept_common_service_api
 from mns_common.db.MongodbUtil import MongodbUtil
 from loguru import logger
 import mns_common.utils.data_frame_util as data_frame_util
 import mns_common.constant.db_name_constant as db_name_constant
+
 mongodb_util = MongodbUtil('27017')
 
 
 def update_ths_concept_detail(ths_symbol_all_concepts, symbol):
     all_ths_concept = ths_concept_common_service_api.get_all_ths_concept()
     for concept_one in ths_symbol_all_concepts.itertuples():
         try:
```

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from loguru import logger
 import mns_common.utils.data_frame_util as data_frame_util
 from datetime import datetime
 from mns_common.utils.async_fun import async_fun
 import mns_scheduler.concept.ths.common.ths_concept_sync_common_api as ths_concept_sync_common_api
 import threading
 import mns_scheduler.concept.ths.common.ths_concept_update_common_api as ths_concept_update_common_api
+import mns_common.utils.date_handle_util as date_handle_util
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 17
 project_path = file_path[0:end]
 sys.path.append(project_path)
 mongodb_util = MongodbUtil('27017')
 # 分页大小
@@ -87,17 +88,19 @@
         try:
             ths_concept_json = ths_stock_api.get_symbol_add_new_concept(stock_one.symbol)
             logger.info("同步symbol概念信息:{}", stock_one.symbol)
             symbol_ths_concept_all_df = pd.DataFrame(ths_concept_json)
             if data_frame_util.is_empty(symbol_ths_concept_all_df):
                 continue
 
-            ths_concept_update_common_api.update_ths_concept_detail(symbol_ths_concept_all_df, stock_one.symbol)
-
             now_date = datetime.now()
+            # 开盘交易前不同步 资源开销过大
+            if date_handle_util.is_close_time(now_date):
+                ths_concept_update_common_api.update_ths_concept_detail(symbol_ths_concept_all_df, stock_one.symbol)
+
             str_day = now_date.strftime('%Y-%m-%d')
             str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
             symbol_ths_concept_all_df.loc[:, 'str_day'] = str_day
             symbol_ths_concept_all_df.loc[:, 'str_now_date'] = str_now_date
             symbol_ths_concept_all_df.loc[:, 'symbol'] = stock_one.symbol
             symbol_ths_concept_all_df.loc[:, 'name'] = stock_one.name
             symbol_ths_concept_all_df.loc[:, 'index'] = 1
@@ -171,8 +174,8 @@
 
     # 等待所有线程完成
     for thread in threads:
         thread.join()
 
 
 if __name__ == '__main__':
-    sync_symbol_all_concept('002130')
+    sync_symbol_all_concept(None)
```

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.2.4/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.2.4/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.2.4/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.2.4/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.2.4/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.2.4/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.2.4/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.2.4/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.2.4/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.2.4/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.2.4/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.2.4/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.3/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.2.4/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

