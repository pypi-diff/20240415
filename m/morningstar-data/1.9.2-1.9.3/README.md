# Comparing `tmp/morningstar_data-1.9.2.tar.gz` & `tmp/morningstar_data-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morningstar_data-1.9.2.tar", max compression
+gzip compressed data, was "morningstar_data-1.9.3.tar", max compression
```

## Comparing `morningstar_data-1.9.2.tar` & `morningstar_data-1.9.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      558 2024-04-02 15:51:51.237457 morningstar_data-1.9.2/LICENSE
--rw-r--r--   0        0        0    11417 2024-04-02 15:51:51.237457 morningstar_data-1.9.2/README.md
--rw-r--r--   0        0        0      168 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/__init__.py
--rw-r--r--   0        0        0      598 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/_base.py
--rw-r--r--   0        0        0     4233 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/_utils.py
--rw-r--r--   0        0        0       82 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/_version.py
--rw-r--r--   0        0        0       61 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/datalake/__init__.py
--rw-r--r--   0        0        0       62 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/datalake/_data_objects/__init__.py
--rw-r--r--   0        0        0      557 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/datalake/_data_objects/_file.py
--rw-r--r--   0        0        0      763 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/datalake/_data_objects/_table.py
--rw-r--r--   0        0        0      996 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/datalake/_data_objects/csvfile.py
--rw-r--r--   0        0        0     2202 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/datalake/_data_objects/temptable.py
--rw-r--r--   0        0        0      544 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/datalake/_error_messages.py
--rw-r--r--   0        0        0      937 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/datalake/_exceptions.py
--rw-r--r--   0        0        0     5604 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/datalake/base.py
--rw-r--r--   0        0        0     1171 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/__init__.py
--rw-r--r--   0        0        0     2432 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_api.py
--rw-r--r--   0        0        0      179 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_backend_apis/__init__.py
--rw-r--r--   0        0        0     2075 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_backend_apis/_delivery_backend.py
--rw-r--r--   0        0        0     4790 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_backend_apis/_holdings_backend.py
--rw-r--r--   0        0        0     3372 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_backend_apis/_signed_url_backend.py
--rw-r--r--   0        0        0     3795 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_base_api.py
--rw-r--r--   0        0        0     5076 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_config.py
--rw-r--r--   0        0        0     1999 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_config_key.py
--rw-r--r--   0        0        0     7854 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_core_api.py
--rw-r--r--   0        0        0      197 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_data_objects/__init__.py
--rw-r--r--   0        0        0     2296 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_data_objects/_custom_data_points_types.py
--rw-r--r--   0        0        0    26798 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_data_objects/_data_points_object.py
--rw-r--r--   0        0        0     7574 2024-04-02 15:51:51.245457 morningstar_data-1.9.2/morningstar_data/direct/_data_objects/_investments_object.py
--rw-r--r--   0        0        0     2887 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_data_point.py
--rw-r--r--   0        0        0     1453 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_data_type.py
--rw-r--r--   0        0        0     1614 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_decorator.py
--rw-r--r--   0        0        0    13819 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_error_messages.py
--rw-r--r--   0        0        0     3464 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_investment/__init__.py
--rw-r--r--   0        0        0     4620 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_investment/_asset_flow_data.py
--rw-r--r--   0        0        0     1560 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_investment/_common.py
--rw-r--r--   0        0        0     9136 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_investment/_data.py
--rw-r--r--   0        0        0     8526 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_investment/_normal_data.py
--rw-r--r--   0        0        0     5127 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_investment/_peer_group_data.py
--rw-r--r--   0        0        0      162 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_portfolio/__init__.py
--rw-r--r--   0        0        0     1273 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_portfolio/_common.py
--rw-r--r--   0        0        0     8263 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
--rw-r--r--   0        0        0     8023 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_portfolio/_portfolio_settings.py
--rw-r--r--   0        0        0      719 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_portfolio/_portfolio_type.py
--rw-r--r--   0        0        0    11071 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_portfolio_data_set.py
--rw-r--r--   0        0        0     3356 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/_utils.py
--rw-r--r--   0        0        0    13081 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/asset_flow.py
--rw-r--r--   0        0        0    16435 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/custom_database.py
--rw-r--r--   0        0        0     1513 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/data_type.py
--rw-r--r--   0        0        0    45132 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/holdings.py
--rw-r--r--   0        0        0    18226 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/investment.py
--rw-r--r--   0        0        0    32429 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/lookup.py
--rw-r--r--   0        0        0     6154 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/peer_group.py
--rw-r--r--   0        0        0    19460 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/performance_report.py
--rw-r--r--   0        0        0    37410 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/portfolio.py
--rw-r--r--   0        0        0    11511 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/returns.py
--rw-r--r--   0        0        0      455 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/user_items/__init__.py
--rw-r--r--   0        0        0      582 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/user_items/_utils.py
--rw-r--r--   0        0        0     7910 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/user_items/data_set.py
--rw-r--r--   0        0        0    13091 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/user_items/investment_lists.py
--rw-r--r--   0        0        0    11276 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/user_items/portfolio.py
--rw-r--r--   0        0        0    10433 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/direct/user_items/search_criteria.py
--rw-r--r--   0        0        0     4768 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/lookup.py
--rw-r--r--   0        0        0       90 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/mdapi/__init__.py
--rw-r--r--   0        0        0     2359 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/mdapi/_exceptions.py
--rw-r--r--   0        0        0     6116 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/mdapi/_mdapi.py
--rw-r--r--   0        0        0     1303 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/mdapi/_types.py
--rw-r--r--   0        0        0      128 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/utils/__init__.py
--rw-r--r--   0        0        0    10975 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/utils/_delivery_config.py
--rw-r--r--   0        0        0     5814 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/utils/_helpers.py
--rw-r--r--   0        0        0    18093 2024-04-02 15:51:51.249457 morningstar_data-1.9.2/morningstar_data/utils/delivery.py
--rw-r--r--   0        0        0     2316 2024-04-02 15:54:56.677678 morningstar_data-1.9.2/pyproject.toml
--rw-r--r--   0        0        0    12424 1970-01-01 00:00:00.000000 morningstar_data-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0      558 2024-04-15 19:48:03.045795 morningstar_data-1.9.3/LICENSE
+-rw-r--r--   0        0        0    11417 2024-04-15 19:48:03.045795 morningstar_data-1.9.3/README.md
+-rw-r--r--   0        0        0      168 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/__init__.py
+-rw-r--r--   0        0        0      598 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/_base.py
+-rw-r--r--   0        0        0     4233 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/_utils.py
+-rw-r--r--   0        0        0       82 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/_version.py
+-rw-r--r--   0        0        0       61 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/__init__.py
+-rw-r--r--   0        0        0      557 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/_file.py
+-rw-r--r--   0        0        0      763 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/_table.py
+-rw-r--r--   0        0        0      996 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/csvfile.py
+-rw-r--r--   0        0        0     2202 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/temptable.py
+-rw-r--r--   0        0        0      544 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_error_messages.py
+-rw-r--r--   0        0        0      937 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/_exceptions.py
+-rw-r--r--   0        0        0     5604 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/datalake/base.py
+-rw-r--r--   0        0        0     1171 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/__init__.py
+-rw-r--r--   0        0        0     2432 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_api.py
+-rw-r--r--   0        0        0      179 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/__init__.py
+-rw-r--r--   0        0        0     2075 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_delivery_backend.py
+-rw-r--r--   0        0        0     4790 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_holdings_backend.py
+-rw-r--r--   0        0        0     3372 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_signed_url_backend.py
+-rw-r--r--   0        0        0     3795 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_base_api.py
+-rw-r--r--   0        0        0     5076 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_config.py
+-rw-r--r--   0        0        0     1999 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_config_key.py
+-rw-r--r--   0        0        0     7854 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_core_api.py
+-rw-r--r--   0        0        0      197 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_objects/__init__.py
+-rw-r--r--   0        0        0     2296 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_custom_data_points_types.py
+-rw-r--r--   0        0        0    26798 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_data_points_object.py
+-rw-r--r--   0        0        0     7574 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_investments_object.py
+-rw-r--r--   0        0        0     2887 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_point.py
+-rw-r--r--   0        0        0     1453 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_data_type.py
+-rw-r--r--   0        0        0     1614 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_decorator.py
+-rw-r--r--   0        0        0    14042 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_error_messages.py
+-rw-r--r--   0        0        0     3711 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/__init__.py
+-rw-r--r--   0        0        0     4620 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_asset_flow_data.py
+-rw-r--r--   0        0        0     1560 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_common.py
+-rw-r--r--   0        0        0     9136 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_data.py
+-rw-r--r--   0        0        0     8526 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_normal_data.py
+-rw-r--r--   0        0        0     5127 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_investment/_peer_group_data.py
+-rw-r--r--   0        0        0      162 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/__init__.py
+-rw-r--r--   0        0        0     1273 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_common.py
+-rw-r--r--   0        0        0     8263 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
+-rw-r--r--   0        0        0     8023 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_settings.py
+-rw-r--r--   0        0        0      719 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_type.py
+-rw-r--r--   0        0        0    11071 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_portfolio_data_set.py
+-rw-r--r--   0        0        0     3356 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/_utils.py
+-rw-r--r--   0        0        0    13081 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/asset_flow.py
+-rw-r--r--   0        0        0    16435 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/custom_database.py
+-rw-r--r--   0        0        0     1513 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/data_type.py
+-rw-r--r--   0        0        0    45132 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/holdings.py
+-rw-r--r--   0        0        0    18226 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/investment.py
+-rw-r--r--   0        0        0    32429 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/lookup.py
+-rw-r--r--   0        0        0     6154 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/peer_group.py
+-rw-r--r--   0        0        0    19460 2024-04-15 19:48:03.057795 morningstar_data-1.9.3/morningstar_data/direct/performance_report.py
+-rw-r--r--   0        0        0    37410 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/portfolio.py
+-rw-r--r--   0        0        0    11511 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/returns.py
+-rw-r--r--   0        0        0      455 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/__init__.py
+-rw-r--r--   0        0        0      582 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/_utils.py
+-rw-r--r--   0        0        0     7910 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/data_set.py
+-rw-r--r--   0        0        0    13091 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/investment_lists.py
+-rw-r--r--   0        0        0    11276 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/portfolio.py
+-rw-r--r--   0        0        0    10433 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/direct/user_items/search_criteria.py
+-rw-r--r--   0        0        0     4768 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/lookup.py
+-rw-r--r--   0        0        0       90 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/mdapi/__init__.py
+-rw-r--r--   0        0        0     2359 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/mdapi/_exceptions.py
+-rw-r--r--   0        0        0     6116 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/mdapi/_mdapi.py
+-rw-r--r--   0        0        0     1303 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/mdapi/_types.py
+-rw-r--r--   0        0        0      128 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/utils/__init__.py
+-rw-r--r--   0        0        0    10975 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/utils/_delivery_config.py
+-rw-r--r--   0        0        0     5814 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/utils/_helpers.py
+-rw-r--r--   0        0        0    18353 2024-04-15 19:48:03.061795 morningstar_data-1.9.3/morningstar_data/utils/delivery.py
+-rw-r--r--   0        0        0     2316 2024-04-15 19:50:17.752446 morningstar_data-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0    12424 1970-01-01 00:00:00.000000 morningstar_data-1.9.3/PKG-INFO
```

### Comparing `morningstar_data-1.9.2/LICENSE` & `morningstar_data-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/README.md` & `morningstar_data-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/_base.py` & `morningstar_data-1.9.3/morningstar_data/_base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/_utils.py` & `morningstar_data-1.9.3/morningstar_data/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/datalake/_data_objects/_file.py` & `morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/_file.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/datalake/_data_objects/_table.py` & `morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/_table.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/datalake/_data_objects/csvfile.py` & `morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/csvfile.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/datalake/_data_objects/temptable.py` & `morningstar_data-1.9.3/morningstar_data/datalake/_data_objects/temptable.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/datalake/_error_messages.py` & `morningstar_data-1.9.3/morningstar_data/datalake/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/datalake/_exceptions.py` & `morningstar_data-1.9.3/morningstar_data/datalake/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/datalake/base.py` & `morningstar_data-1.9.3/morningstar_data/datalake/base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/__init__.py` & `morningstar_data-1.9.3/morningstar_data/direct/__init__.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_api.py` & `morningstar_data-1.9.3/morningstar_data/direct/_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_backend_apis/_delivery_backend.py` & `morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_delivery_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_backend_apis/_holdings_backend.py` & `morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_holdings_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_backend_apis/_signed_url_backend.py` & `morningstar_data-1.9.3/morningstar_data/direct/_backend_apis/_signed_url_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_base_api.py` & `morningstar_data-1.9.3/morningstar_data/direct/_base_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_config.py` & `morningstar_data-1.9.3/morningstar_data/direct/_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_config_key.py` & `morningstar_data-1.9.3/morningstar_data/direct/_config_key.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_core_api.py` & `morningstar_data-1.9.3/morningstar_data/direct/_core_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_data_objects/_custom_data_points_types.py` & `morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_custom_data_points_types.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_data_objects/_data_points_object.py` & `morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_data_points_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_data_objects/_investments_object.py` & `morningstar_data-1.9.3/morningstar_data/direct/_data_objects/_investments_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_data_point.py` & `morningstar_data-1.9.3/morningstar_data/direct/_data_point.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_data_type.py` & `morningstar_data-1.9.3/morningstar_data/direct/_data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_decorator.py` & `morningstar_data-1.9.3/morningstar_data/direct/_decorator.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_error_messages.py` & `morningstar_data-1.9.3/morningstar_data/direct/_error_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,7 +122,10 @@
 
 # Add custom error messages here for data lookup
 RESOURCE_NOT_FOUND_ERROR_DATA_SET_LOOKUP = "Requested resource does not exist for the given `universe`."
 RESOURCE_NOT_FOUND_ERROR_DATA_POINT_LOOKUP = "Requested resource does not exist for the given `data_point_ids`."
 
 # Add custom errors for environment
 MALFORMED_JWT_ERROR = "Invalid JWT format. JWT should look like 'header.payload.signature' where header and payload are base64 encoded strings and signature is a hex string."
+
+# Add custom errors for delivery
+FAILED_DELIVERY_ERROR = "The delivery has failed. Please check your delivery configuration for job_id: {}. Please contact Analytics Lab support team at Morningstar for additional support."
```

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_exceptions.py` & `morningstar_data-1.9.3/morningstar_data/direct/_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,7 +115,15 @@
         else:
             super().__init__(message)
 
 
 class UnauthorizedDeliveryException(Exception):
     def __init__(self, message: str = _error_messages.DELIVERY_ACCESS_ERROR) -> None:
         super().__init__(message)
+
+
+class FailedDeliveryError(Exception):
+    def __init__(self, message: Optional[str] = None) -> None:
+        if not message:
+            super().__init__(_error_messages.FAILED_DELIVERY_ERROR)
+        else:
+            super().__init__(message)
```

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_investment/_asset_flow_data.py` & `morningstar_data-1.9.3/morningstar_data/direct/_investment/_asset_flow_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_investment/_common.py` & `morningstar_data-1.9.3/morningstar_data/direct/_investment/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_investment/_data.py` & `morningstar_data-1.9.3/morningstar_data/direct/_investment/_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_investment/_normal_data.py` & `morningstar_data-1.9.3/morningstar_data/direct/_investment/_normal_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_investment/_peer_group_data.py` & `morningstar_data-1.9.3/morningstar_data/direct/_investment/_peer_group_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_portfolio/_common.py` & `morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py` & `morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_portfolio/_portfolio_settings.py` & `morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_settings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_portfolio/_portfolio_type.py` & `morningstar_data-1.9.3/morningstar_data/direct/_portfolio/_portfolio_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_portfolio_data_set.py` & `morningstar_data-1.9.3/morningstar_data/direct/_portfolio_data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/_utils.py` & `morningstar_data-1.9.3/morningstar_data/direct/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/asset_flow.py` & `morningstar_data-1.9.3/morningstar_data/direct/asset_flow.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/custom_database.py` & `morningstar_data-1.9.3/morningstar_data/direct/custom_database.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/data_type.py` & `morningstar_data-1.9.3/morningstar_data/direct/data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/holdings.py` & `morningstar_data-1.9.3/morningstar_data/direct/holdings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/investment.py` & `morningstar_data-1.9.3/morningstar_data/direct/investment.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/lookup.py` & `morningstar_data-1.9.3/morningstar_data/direct/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/peer_group.py` & `morningstar_data-1.9.3/morningstar_data/direct/peer_group.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/performance_report.py` & `morningstar_data-1.9.3/morningstar_data/direct/performance_report.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/portfolio.py` & `morningstar_data-1.9.3/morningstar_data/direct/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/returns.py` & `morningstar_data-1.9.3/morningstar_data/direct/returns.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/user_items/_utils.py` & `morningstar_data-1.9.3/morningstar_data/direct/user_items/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/user_items/data_set.py` & `morningstar_data-1.9.3/morningstar_data/direct/user_items/data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/user_items/investment_lists.py` & `morningstar_data-1.9.3/morningstar_data/direct/user_items/investment_lists.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/user_items/portfolio.py` & `morningstar_data-1.9.3/morningstar_data/direct/user_items/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/direct/user_items/search_criteria.py` & `morningstar_data-1.9.3/morningstar_data/direct/user_items/search_criteria.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/lookup.py` & `morningstar_data-1.9.3/morningstar_data/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/mdapi/_exceptions.py` & `morningstar_data-1.9.3/morningstar_data/mdapi/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/mdapi/_mdapi.py` & `morningstar_data-1.9.3/morningstar_data/mdapi/_mdapi.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/mdapi/_types.py` & `morningstar_data-1.9.3/morningstar_data/mdapi/_types.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/utils/_delivery_config.py` & `morningstar_data-1.9.3/morningstar_data/utils/_delivery_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/utils/_helpers.py` & `morningstar_data-1.9.3/morningstar_data/utils/_helpers.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.2/morningstar_data/utils/delivery.py` & `morningstar_data-1.9.3/morningstar_data/utils/delivery.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import polling2
 import simplejson as json
 from boto3.s3.transfer import TransferConfig
 from botocore.exceptions import ClientError
 
 from ..direct import _decorator
 from ..direct._backend_apis import DeliveryAPIBackend
+from ..direct._error_messages import FAILED_DELIVERY_ERROR
+from ..direct._exceptions import FailedDeliveryError
 from ._delivery_config import DeliveryConfig, DeliveryType
 from ._helpers import (
     _create_feed_body,
     _create_output_file_name,
     _encrypt_ftp_password,
     _get_bucket_name,
     _get_job_name,
@@ -229,14 +231,15 @@
                 check_success=lambda response: _delivery_finished(response),
             )
         except polling2.TimeoutException as te:
             _logger.info(f"Timeout for the request. Exception as {te}.")
 
     response_json = _api_backend.do_get_request(url)
     _logger.info(f"Delivery status: {response_json}")
+
     return str(response_json["jobStatus"])  # "DONE" or "FAILED" or "RUNNING"
 
 
 @_decorator.typechecked
 def deliver(
     config: Union[DeliveryConfig, List[DeliveryConfig]],
     wait_for_delivery: bool = False,
@@ -421,8 +424,10 @@
 
     _logger.info(f"Final config for creating post body: {config}")
     job_id: str = _mds_deliver_file(config, feed_id)
     res = {"job_id": job_id, "message": "Delivery has been submitted."}
 
     # if flag is set True, poll the api, return the delivery status
     res["delivery_status"] = delivery_status(job_id, poll=wait_for_delivery)
+    if str(res["delivery_status"]).lower() == "failed":
+        raise FailedDeliveryError((FAILED_DELIVERY_ERROR).format(res["job_id"])) from None
     return res
```

### Comparing `morningstar_data-1.9.2/pyproject.toml` & `morningstar_data-1.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morningstar_data"
-version = "1.9.2"
+version = "1.9.3"
 description = "Morningstar Data"
 authors = ["Morningstar, Inc."]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.morningstar.com/products/md-python-package"
 documentation = "https://docs-analyticslab.morningstar.com/latest/index.html"
```

### Comparing `morningstar_data-1.9.2/PKG-INFO` & `morningstar_data-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morningstar-data
-Version: 1.9.2
+Version: 1.9.3
 Summary: Morningstar Data
 Home-page: https://www.morningstar.com/products/md-python-package
 License: Apache-2.0
 Author: Morningstar, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

