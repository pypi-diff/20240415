# Comparing `tmp/tushare-1.4.5.tar.gz` & `tmp/tushare-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tushare-1.4.5.tar", last modified: Thu Mar 14 06:39:11 2024, max compression
+gzip compressed data, was "tushare-1.4.6.tar", last modified: Mon Apr 15 07:17:13 2024, max compression
```

## Comparing `tushare-1.4.5.tar` & `tushare-1.4.6.tar`

### file list

```diff
@@ -1,102 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.990508 tushare-1.4.5/
--rw-rw-rw-   0        0        0     1503 2023-12-22 01:48:49.000000 tushare-1.4.5/LICENSE
--rw-rw-rw-   0        0        0     3098 2024-03-14 06:39:11.990508 tushare-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    13252 2023-12-22 01:48:49.000000 tushare-1.4.5/README.md
--rw-rw-rw-   0        0        0       42 2024-03-14 06:39:11.990508 tushare-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     3401 2024-03-14 06:34:56.000000 tushare-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.865790 tushare-1.4.5/tushare/
--rw-rw-rw-   0        0        0     4764 2024-03-14 06:34:56.000000 tushare-1.4.5/tushare/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.897116 tushare-1.4.5/tushare/bond/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/bond/__init__.py
--rw-rw-rw-   0        0        0      232 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/bond/bonds.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.897116 tushare-1.4.5/tushare/coins/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/coins/__init__.py
--rw-rw-rw-   0        0        0     8266 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/coins/market.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.897116 tushare-1.4.5/tushare/data/
--rw-rw-rw-   0        0        0       21 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.912692 tushare-1.4.5/tushare/fund/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/fund/__init__.py
--rw-rw-rw-   0        0        0     5854 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/fund/cons.py
--rw-rw-rw-   0        0        0    14851 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/fund/nav.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.912692 tushare-1.4.5/tushare/futures/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/futures/__init__.py
--rw-rw-rw-   0        0        0      799 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/futures/cons.py
--rw-rw-rw-   0        0        0    17968 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/futures/domestic.py
--rw-rw-rw-   0        0        0     5425 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/futures/domestic_cons.py
--rw-rw-rw-   0        0        0     1431 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/futures/intlfutures.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.912692 tushare-1.4.5/tushare/internet/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/internet/__init__.py
--rw-rw-rw-   0        0        0     7415 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/internet/boxoffice.py
--rw-rw-rw-   0        0        0     4178 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/internet/caixinnews.py
--rw-rw-rw-   0        0        0     3595 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/internet/indexes.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.928046 tushare-1.4.5/tushare/pro/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/pro/__init__.py
--rw-rw-rw-   0        0        0     1312 2023-12-22 06:39:33.000000 tushare-1.4.5/tushare/pro/client.py
--rw-rw-rw-   0        0        0    10332 2024-02-29 01:16:49.000000 tushare-1.4.5/tushare/pro/data_pro.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.943729 tushare-1.4.5/tushare/stock/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/stock/__init__.py
--rw-rw-rw-   0        0        0    12833 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/stock/billboard.py
--rw-rw-rw-   0        0        0    10539 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/stock/classifying.py
--rw-rw-rw-   0        0        0    31812 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/stock/cons.py
--rw-rw-rw-   0        0        0    20304 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/stock/fundamental.py
--rw-rw-rw-   0        0        0     2118 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/stock/globals.py
--rw-rw-rw-   0        0        0     6611 2023-12-26 08:48:19.000000 tushare-1.4.5/tushare/stock/histroy_divide.py
--rw-rw-rw-   0        0        0    25443 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/stock/indictor.py
--rw-rw-rw-   0        0        0    14211 2023-12-22 01:48:49.000000 tushare-1.4.5/tushare/stock/macro.py
--rw-rw-rw-   0        0        0     1453 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/stock/macro_vars.py
--rw-rw-rw-   0        0        0     2454 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/stock/minsdata.py
--rw-rw-rw-   0        0        0      454 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/stock/news_vars.py
--rw-rw-rw-   0        0        0     6944 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/stock/newsevent.py
--rw-rw-rw-   0        0        0     4449 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/stock/ref_vars.py
--rw-rw-rw-   0        0        0    38227 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/stock/reference.py
--rw-rw-rw-   0        0        0    23115 2024-02-29 04:12:19.000000 tushare-1.4.5/tushare/stock/rtq.py
--rw-rw-rw-   0        0        0     4200 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/stock/rtq_vars.py
--rw-rw-rw-   0        0        0     6422 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/stock/shibor.py
--rw-rw-rw-   0        0        0    55619 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/stock/trading.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.943729 tushare-1.4.5/tushare/subs/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/subs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.959259 tushare-1.4.5/tushare/subs/ht_subs/
--rw-rw-rw-   0        0        0      132 2024-02-29 01:16:49.000000 tushare-1.4.5/tushare/subs/ht_subs/__init__.py
--rw-rw-rw-   0        0        0     7368 2024-02-29 01:08:08.000000 tushare-1.4.5/tushare/subs/ht_subs/covert.py
--rw-rw-rw-   0        0        0     8340 2024-02-29 01:16:49.000000 tushare-1.4.5/tushare/subs/ht_subs/subscribe.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.959259 tushare-1.4.5/tushare/subs/model/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/subs/model/__init__.py
--rw-rw-rw-   0        0        0      375 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/subs/model/min.py
--rw-rw-rw-   0        0        0     4211 2024-03-14 06:34:04.000000 tushare-1.4.5/tushare/subs/model/tick.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.959259 tushare-1.4.5/tushare/subs/tgw_subs/
--rw-rw-rw-   0        0        0       69 2024-02-28 12:47:02.000000 tushare-1.4.5/tushare/subs/tgw_subs/__init__.py
--rw-rw-rw-   0        0        0     5474 2024-03-14 06:38:37.000000 tushare-1.4.5/tushare/subs/tgw_subs/convert.py
--rw-rw-rw-   0        0        0      903 2024-02-29 04:23:47.000000 tushare-1.4.5/tushare/subs/tgw_subs/login.py
--rw-rw-rw-   0        0        0     3336 2024-02-29 04:22:43.000000 tushare-1.4.5/tushare/subs/tgw_subs/subscribe.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.959259 tushare-1.4.5/tushare/subs/ts_subs/
--rw-rw-rw-   0        0        0      107 2024-02-29 01:16:26.000000 tushare-1.4.5/tushare/subs/ts_subs/__init__.py
--rw-rw-rw-   0        0        0     6086 2024-02-29 01:16:26.000000 tushare-1.4.5/tushare/subs/ts_subs/subscribe.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.974905 tushare-1.4.5/tushare/trader/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/trader/__init__.py
--rw-rw-rw-   0        0        0    11360 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/trader/trader.py
--rw-rw-rw-   0        0        0      752 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/trader/utils.py
--rw-rw-rw-   0        0        0     1787 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/trader/vars.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.990508 tushare-1.4.5/tushare/util/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/__init__.py
--rw-rw-rw-   0        0        0     2581 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/common.py
--rw-rw-rw-   0        0        0     1456 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/conns.py
--rw-rw-rw-   0        0        0     2931 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/dateu.py
--rw-rw-rw-   0        0        0     1119 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/form_date.py
--rw-rw-rw-   0        0        0     3452 2024-02-29 04:12:19.000000 tushare-1.4.5/tushare/util/format_stock_code.py
--rw-rw-rw-   0        0        0     6863 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/formula.py
--rw-rw-rw-   0        0        0     8980 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/mailmerge.py
--rw-rw-rw-   0        0        0      942 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/netbase.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.990508 tushare-1.4.5/tushare/util/protobuf/
--rw-rw-rw-   0        0        0        0 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/protobuf/__init__.py
--rw-rw-rw-   0        0        0      779 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/protobuf/funcs.py
--rw-rw-rw-   0        0        0    11347 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/protobuf/response_pb2.py
--rw-rw-rw-   0        0        0     1167 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/store.py
--rw-rw-rw-   0        0        0     1515 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/upass.py
--rw-rw-rw-   0        0        0    69946 2023-12-22 01:48:50.000000 tushare-1.4.5/tushare/util/vars.py
--rw-rw-rw-   0        0        0     2471 2024-01-15 12:05:06.000000 tushare-1.4.5/tushare/util/verify_token.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:39:11.897116 tushare-1.4.5/tushare.egg-info/
--rw-rw-rw-   0        0        0     3098 2024-03-14 06:39:11.000000 tushare-1.4.5/tushare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2024-03-14 06:39:11.000000 tushare-1.4.5/tushare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 06:39:11.000000 tushare-1.4.5/tushare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2024-03-14 06:39:11.000000 tushare-1.4.5/tushare.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-14 06:39:11.000000 tushare-1.4.5/tushare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.734267 tushare-1.4.6/
+-rw-rw-rw-   0        0        0     1503 2023-12-05 12:24:54.000000 tushare-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0     2682 2024-04-15 07:17:13.733273 tushare-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0    13252 2023-12-05 12:24:54.000000 tushare-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.504311 tushare-1.4.6/baks/
+-rw-rw-rw-   0        0        0        0 2023-12-06 03:13:15.000000 tushare-1.4.6/baks/__init__.py
+-rw-rw-rw-   0        0        0     5940 2024-01-08 11:04:14.000000 tushare-1.4.6/baks/demo.py
+-rw-rw-rw-   0        0        0    21085 2024-01-03 02:14:34.000000 tushare-1.4.6/baks/rtqc.py
+-rw-rw-rw-   0        0        0      250 2024-01-03 02:18:59.000000 tushare-1.4.6/baks/setup.py
+-rw-rw-rw-   0        0        0     2647 2024-01-11 10:42:42.000000 tushare-1.4.6/baks/sss.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 07:17:13.735284 tushare-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     3441 2024-04-15 07:16:56.000000 tushare-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.506312 tushare-1.4.6/tushare/
+-rw-rw-rw-   0        0        0     4764 2024-04-15 07:15:35.000000 tushare-1.4.6/tushare/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.546287 tushare-1.4.6/tushare/bond/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/bond/__init__.py
+-rw-rw-rw-   0        0        0      232 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/bond/bonds.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.550299 tushare-1.4.6/tushare/coins/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/coins/__init__.py
+-rw-rw-rw-   0        0        0     8266 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/coins/market.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.552313 tushare-1.4.6/tushare/data/
+-rw-rw-rw-   0        0        0       21 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.559608 tushare-1.4.6/tushare/fund/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/fund/__init__.py
+-rw-rw-rw-   0        0        0     5854 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/fund/cons.py
+-rw-rw-rw-   0        0        0    14851 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/fund/nav.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.577414 tushare-1.4.6/tushare/futures/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/futures/__init__.py
+-rw-rw-rw-   0        0        0      799 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/futures/cons.py
+-rw-rw-rw-   0        0        0    17968 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/futures/domestic.py
+-rw-rw-rw-   0        0        0     5425 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/futures/domestic_cons.py
+-rw-rw-rw-   0        0        0     1431 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/futures/intlfutures.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.589279 tushare-1.4.6/tushare/internet/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/internet/__init__.py
+-rw-rw-rw-   0        0        0     7415 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/internet/boxoffice.py
+-rw-rw-rw-   0        0        0     4178 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/internet/caixinnews.py
+-rw-rw-rw-   0        0        0     3595 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/internet/indexes.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.595301 tushare-1.4.6/tushare/pro/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/pro/__init__.py
+-rw-rw-rw-   0        0        0     1312 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/pro/client.py
+-rw-rw-rw-   0        0        0    10332 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/pro/data_pro.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.650293 tushare-1.4.6/tushare/stock/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/__init__.py
+-rw-rw-rw-   0        0        0    12833 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/billboard.py
+-rw-rw-rw-   0        0        0    10539 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/classifying.py
+-rw-rw-rw-   0        0        0    31812 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/cons.py
+-rw-rw-rw-   0        0        0    20304 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/fundamental.py
+-rw-rw-rw-   0        0        0     2118 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/globals.py
+-rw-rw-rw-   0        0        0     6611 2023-12-26 02:04:14.000000 tushare-1.4.6/tushare/stock/histroy_divide.py
+-rw-rw-rw-   0        0        0    25443 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/indictor.py
+-rw-rw-rw-   0        0        0    14211 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/macro.py
+-rw-rw-rw-   0        0        0     1453 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/macro_vars.py
+-rw-rw-rw-   0        0        0     2454 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/minsdata.py
+-rw-rw-rw-   0        0        0      454 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/news_vars.py
+-rw-rw-rw-   0        0        0     6944 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/newsevent.py
+-rw-rw-rw-   0        0        0     4449 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/ref_vars.py
+-rw-rw-rw-   0        0        0    38227 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/reference.py
+-rw-rw-rw-   0        0        0    23123 2024-04-15 07:05:15.000000 tushare-1.4.6/tushare/stock/rtq.py
+-rw-rw-rw-   0        0        0     4200 2023-12-21 10:04:11.000000 tushare-1.4.6/tushare/stock/rtq_vars.py
+-rw-rw-rw-   0        0        0   158208 2024-01-03 02:19:25.000000 tushare-1.4.6/tushare/stock/rtqc.pyd
+-rw-rw-rw-   0        0        0     6422 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/stock/shibor.py
+-rw-rw-rw-   0        0        0    55619 2023-12-06 08:37:29.000000 tushare-1.4.6/tushare/stock/trading.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.653289 tushare-1.4.6/tushare/subs/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/subs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.659309 tushare-1.4.6/tushare/subs/ht_subs/
+-rw-rw-rw-   0        0        0      132 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/ht_subs/__init__.py
+-rw-rw-rw-   0        0        0     7368 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/ht_subs/covert.py
+-rw-rw-rw-   0        0        0     8340 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/ht_subs/subscribe.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.671274 tushare-1.4.6/tushare/subs/model/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/subs/model/__init__.py
+-rw-rw-rw-   0        0        0      375 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/subs/model/min.py
+-rw-rw-rw-   0        0        0     4297 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/model/tick.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.679285 tushare-1.4.6/tushare/subs/tgw_subs/
+-rw-rw-rw-   0        0        0       69 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/tgw_subs/__init__.py
+-rw-rw-rw-   0        0        0     5331 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/tgw_subs/convert.py
+-rw-rw-rw-   0        0        0      903 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/tgw_subs/login.py
+-rw-rw-rw-   0        0        0     3336 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/tgw_subs/subscribe.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.683267 tushare-1.4.6/tushare/subs/ts_subs/
+-rw-rw-rw-   0        0        0      107 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/ts_subs/__init__.py
+-rw-rw-rw-   0        0        0     6086 2024-02-29 04:32:13.000000 tushare-1.4.6/tushare/subs/ts_subs/subscribe.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.692354 tushare-1.4.6/tushare/trader/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/trader/__init__.py
+-rw-rw-rw-   0        0        0    11360 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/trader/trader.py
+-rw-rw-rw-   0        0        0      752 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/trader/utils.py
+-rw-rw-rw-   0        0        0     1787 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/trader/vars.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.724303 tushare-1.4.6/tushare/util/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/__init__.py
+-rw-rw-rw-   0        0        0     2581 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/common.py
+-rw-rw-rw-   0        0        0     1456 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/conns.py
+-rw-rw-rw-   0        0        0     2931 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/dateu.py
+-rw-rw-rw-   0        0        0     1119 2023-12-07 07:55:43.000000 tushare-1.4.6/tushare/util/form_date.py
+-rw-rw-rw-   0        0        0     3452 2024-02-19 08:00:44.000000 tushare-1.4.6/tushare/util/format_stock_code.py
+-rw-rw-rw-   0        0        0     6863 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/formula.py
+-rw-rw-rw-   0        0        0     8980 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/mailmerge.py
+-rw-rw-rw-   0        0        0      942 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/netbase.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.731323 tushare-1.4.6/tushare/util/protobuf/
+-rw-rw-rw-   0        0        0        0 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/protobuf/__init__.py
+-rw-rw-rw-   0        0        0      779 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/protobuf/funcs.py
+-rw-rw-rw-   0        0        0    11347 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/protobuf/response_pb2.py
+-rw-rw-rw-   0        0        0     1167 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/store.py
+-rw-rw-rw-   0        0        0     1515 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/upass.py
+-rw-rw-rw-   0        0        0    69946 2023-12-05 12:24:54.000000 tushare-1.4.6/tushare/util/vars.py
+-rw-rw-rw-   0        0        0     2471 2024-01-12 02:52:02.000000 tushare-1.4.6/tushare/util/verify_token.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:17:13.541306 tushare-1.4.6/tushare.egg-info/
+-rw-rw-rw-   0        0        0     2682 2024-04-15 07:17:13.000000 tushare-1.4.6/tushare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2237 2024-04-15 07:17:13.000000 tushare-1.4.6/tushare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 07:17:13.000000 tushare-1.4.6/tushare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-15 07:17:13.000000 tushare-1.4.6/tushare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 07:17:13.000000 tushare-1.4.6/tushare.egg-info/top_level.txt
```

### Comparing `tushare-1.4.5/LICENSE` & `tushare-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/PKG-INFO` & `tushare-1.4.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,94 @@
 Metadata-Version: 2.1
 Name: tushare
-Version: 1.4.5
+Version: 1.4.6
 Summary: A utility for crawling historical and Real-time Quotes data of China stocks
 Home-page: https://tushare.pro
 Author: Jimmy Liu
 Author-email: waditu@163.com
 License: BSD
-Description: 
-        TuShare
-        ===============
-        
-        .. image:: https://api.travis-ci.org/waditu/tushare.png?branch=master
-            :target: https://travis-ci.org/waditu/tushare
-        
-        .. image:: https://badge.fury.io/py/tushare.png
-            :target: http://badge.fury.io/py/tushare
-        
-        * easy to use as most of the data returned are pandas DataFrame objects
-        * can be easily saved as csv, excel or json files
-        * can be inserted into MySQL or Mongodb
-        
-        Target Users
-        --------------
-        
-        * financial market analyst of China
-        * learners of financial data analysis with pandas/NumPy
-        * people who are interested in China financial data
-        
-        Installation
-        --------------
-        
-            pip install tushare
-            
-        Upgrade
-        ---------------
-        
-            pip install tushare --upgrade
-            
-        Quick Start
-        --------------
-        
-        ::
-        
-            import tushare as ts
-            
-            ts.get_hist_data('600848')
-            
-        return::
-        
-                        open    high   close     low     volume    p_change  ma5     
-            date
-            2012-01-11   6.880   7.380   7.060   6.880   14129.96     2.62   7.060
-            2012-01-12   7.050   7.100   6.980   6.900    7895.19    -1.13   7.020
-            2012-01-13   6.950   7.000   6.700   6.690    6611.87    -4.01   6.913
-            2012-01-16   6.680   6.750   6.510   6.480    2941.63    -2.84   6.813
-            2012-01-17   6.660   6.880   6.860   6.460    8642.57     5.38   6.822
-            2012-01-18   7.000   7.300   6.890   6.880   13075.40     0.44   6.788
-            2012-01-19   6.690   6.950   6.890   6.680    6117.32     0.00   6.770
-            2012-01-20   6.870   7.080   7.010   6.870    6813.09     1.74   6.832
-            
-            
-        Log
-        --------------
-        1.4.0
-        -------
-        - 增加 银河证券实时行情数据入口
-        1.3.9
-        -------
-        - realtime_quote 实时盘口TICK快照(爬虫版)
-        - 修复dc 指数和股票数据抓取问题
-        - 将数字类型统一转换成 float类型
-        1.2.73
-        -------
-        - 支持华泰实时数据15SECOND
-            
-        
 Keywords: Global Financial Data
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/plain
+License-File: LICENSE
+
+
+TuShare
+===============
+
+.. image:: https://api.travis-ci.org/waditu/tushare.png?branch=master
+    :target: https://travis-ci.org/waditu/tushare
+
+.. image:: https://badge.fury.io/py/tushare.png
+    :target: http://badge.fury.io/py/tushare
+
+* easy to use as most of the data returned are pandas DataFrame objects
+* can be easily saved as csv, excel or json files
+* can be inserted into MySQL or Mongodb
+
+Target Users
+--------------
+
+* financial market analyst of China
+* learners of financial data analysis with pandas/NumPy
+* people who are interested in China financial data
+
+Installation
+--------------
+
+    pip install tushare
+    
+Upgrade
+---------------
+
+    pip install tushare --upgrade
+    
+Quick Start
+--------------
+
+::
+
+    import tushare as ts
+    
+    ts.get_hist_data('600848')
+    
+return::
+
+                open    high   close     low     volume    p_change  ma5     
+    date
+    2012-01-11   6.880   7.380   7.060   6.880   14129.96     2.62   7.060
+    2012-01-12   7.050   7.100   6.980   6.900    7895.19    -1.13   7.020
+    2012-01-13   6.950   7.000   6.700   6.690    6611.87    -4.01   6.913
+    2012-01-16   6.680   6.750   6.510   6.480    2941.63    -2.84   6.813
+    2012-01-17   6.660   6.880   6.860   6.460    8642.57     5.38   6.822
+    2012-01-18   7.000   7.300   6.890   6.880   13075.40     0.44   6.788
+    2012-01-19   6.690   6.950   6.890   6.680    6117.32     0.00   6.770
+    2012-01-20   6.870   7.080   7.010   6.870    6813.09     1.74   6.832
+    
+    
+Log
+--------------
+1.4.6
+-------
+- 修复 realtime_quote 实时盘口TICK快照(爬虫版)
+- 修复dc OPEN和LOW 值相反问题
+1.4.0
+-------
+- 增加 银河证券实时行情数据入口
+1.3.9
+-------
+- realtime_quote 实时盘口TICK快照(爬虫版)
+- 修复dc 指数和股票数据抓取问题
+- 将数字类型统一转换成 float类型
+1.2.73
+-------
+- 支持华泰实时数据15SECOND
+    
+
+
```

### Comparing `tushare-1.4.5/README.md` & `tushare-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/setup.py` & `tushare-1.4.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,18 @@
     2012-01-18   7.000   7.300   6.890   6.880   13075.40     0.44   6.788
     2012-01-19   6.690   6.950   6.890   6.680    6117.32     0.00   6.770
     2012-01-20   6.870   7.080   7.010   6.870    6813.09     1.74   6.832
     
     
 Log
 --------------
+1.4.6
+-------
+- 修复 realtime_quote 实时盘口TICK快照(爬虫版)
+- 修复dc OPEN和LOW 值相反问题
 1.4.0
 -------
 - 增加 银河证券实时行情数据入口
 1.3.9
 -------
 - realtime_quote 实时盘口TICK快照(爬虫版)
 - 修复dc 指数和股票数据抓取问题
@@ -75,27 +79,29 @@
 1.2.73
 -------
 - 支持华泰实时数据15SECOND
     
 """
 
 def read_install_requires():
-    requires = []
-    with open('requirements.txt') as f:
-        for line in f.readlines():
-            line = line.strip()
-            if not line or line.startswith('#'):
-                continue
-            requires.append(line)
-    return requires
+    reqs = [
+        'pandas',
+        'requests',
+        'lxml',
+        'simplejson',
+        'bs4',
+        'websocket-client==0.57.0',
+        'tqdm'
+    ]
+    return reqs
 
 
 setup(
     name='tushare',
-    version='1.4.5',
+    version='1.4.6',
     description='A utility for crawling historical and Real-time Quotes data of China stocks',
     # long_description=read("README.rst"),
     long_description=long_desc,
     long_description_content_type='text/plain',
     author='Jimmy Liu',
     author_email='waditu@163.com',
     license='BSD',
```

### Comparing `tushare-1.4.5/tushare/__init__.py` & `tushare-1.4.6/tushare/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding:utf-8 -*- 
 import codecs
 import os
 
-__version__ = '1.4.5'
+__version__ = '1.4.6'
 __author__ = 'Jimmy Liu'
 
 """
 for trading data
 """
 from tushare.stock.trading import (get_hist_data, get_tick_data,
                                    get_today_all, get_realtime_quotes,
```

### Comparing `tushare-1.4.5/tushare/coins/market.py` & `tushare-1.4.6/tushare/coins/market.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/fund/cons.py` & `tushare-1.4.6/tushare/fund/cons.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/fund/nav.py` & `tushare-1.4.6/tushare/fund/nav.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/futures/cons.py` & `tushare-1.4.6/tushare/futures/cons.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/futures/domestic.py` & `tushare-1.4.6/tushare/futures/domestic.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/futures/domestic_cons.py` & `tushare-1.4.6/tushare/futures/domestic_cons.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/futures/intlfutures.py` & `tushare-1.4.6/tushare/futures/intlfutures.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/internet/boxoffice.py` & `tushare-1.4.6/tushare/internet/boxoffice.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/internet/caixinnews.py` & `tushare-1.4.6/tushare/internet/caixinnews.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/internet/indexes.py` & `tushare-1.4.6/tushare/internet/indexes.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/pro/client.py` & `tushare-1.4.6/tushare/pro/client.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/pro/data_pro.py` & `tushare-1.4.6/tushare/pro/data_pro.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/billboard.py` & `tushare-1.4.6/tushare/stock/billboard.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/classifying.py` & `tushare-1.4.6/tushare/stock/classifying.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/cons.py` & `tushare-1.4.6/tushare/stock/cons.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/fundamental.py` & `tushare-1.4.6/tushare/stock/fundamental.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/globals.py` & `tushare-1.4.6/tushare/stock/globals.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/histroy_divide.py` & `tushare-1.4.6/tushare/stock/histroy_divide.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/indictor.py` & `tushare-1.4.6/tushare/stock/indictor.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/macro.py` & `tushare-1.4.6/tushare/stock/macro.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/macro_vars.py` & `tushare-1.4.6/tushare/stock/macro_vars.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/minsdata.py` & `tushare-1.4.6/tushare/stock/minsdata.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/newsevent.py` & `tushare-1.4.6/tushare/stock/newsevent.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/ref_vars.py` & `tushare-1.4.6/tushare/stock/ref_vars.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/reference.py` & `tushare-1.4.6/tushare/stock/reference.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/rtq.py` & `tushare-1.4.6/tushare/stock/rtq.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,18 +559,18 @@
         params["secid"] = f"1.{symbol}"
     # print(params["secid"])
     response = requests.get(url, headers=rtqv.dc_cookies, cookies=rtqv.dc_headers, params=params)
     data_info = response.json()["data"]
     if not data_info:
         return pd.DataFrame()
     name = data_info["f58"]
-    open = data_info["f45"]  # / 100
+    open = data_info["f46"]  # / 100
     high = data_info["f44"]  # / 100
     pre_close = data_info["f60"]  # / 100
-    low = data_info["f46"]  # / 100
+    low =  data_info["f45"] # / 100
     price = data_info["f43"]  # / 100 if data_info["f43"] != "-" else ""
     b5_v = format_str_to_float(data_info["f12"])
     b5_p = data_info["f11"]  # / 100 if data_info["f11"] != "-" else ""
     b4_v = format_str_to_float(data_info["f14"])
     b4_p = data_info["f13"]  # / 100 if data_info["f13"] != "-" else ""
     b3_v = format_str_to_float(data_info["f16"])
     b3_p = data_info["f15"]  # / 100 if data_info["f15"] != "-" else ""
@@ -632,18 +632,20 @@
         return float(x) if x != "" else 0
     except:
         return 0
 
 
 if __name__ == '__main__':
     # df = realtime_quote(ts_code="000688.SH,000010.SH,000012.SH,399005.SZ", src="sina")
-    df = realtime_list(src="sina", page_count=1)
-    print(df)
+    # df = realtime_list(src="sina", page_count=1)
+    # print(df)
     ts_code = '399005.SZ'
     ts_code = '000001.SZ'
     # ts_code = '836149.BJ'
     # ts_code = '600000.SH'
     # ts_code = '000001.SH'
     # ts_code = '000010.SH'
     ts_code = '688111.SH'
     df = realtime_quote(src="dc", ts_code=ts_code)
     print(df)
+
+
```

### Comparing `tushare-1.4.5/tushare/stock/rtq_vars.py` & `tushare-1.4.6/tushare/stock/rtq_vars.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/shibor.py` & `tushare-1.4.6/tushare/stock/shibor.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/stock/trading.py` & `tushare-1.4.6/tushare/stock/trading.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/subs/ht_subs/covert.py` & `tushare-1.4.6/tushare/subs/ht_subs/covert.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/subs/ht_subs/subscribe.py` & `tushare-1.4.6/tushare/subs/ht_subs/subscribe.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/subs/model/tick.py` & `tushare-1.4.6/tushare/subs/model/tick.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from datetime import datetime
-from typing import Optional
-
-from pydantic import BaseModel
-
-
-class TsTick(BaseModel):
-    ts_code: str
-    name: Optional[str]
-    trade_time: Optional[datetime]
-    pre_close_price: Optional[float]
-    last_price: Optional[float]
-    open_price: Optional[float]
-    high_price: Optional[float]
-    low_price: Optional[float]
-    close_price: Optional[float]
-    volume: Optional[int]           # 成交量
-    amount: Optional[int]           # 成交金额
-    count: Optional[int]            # 交易数量
-    ask_price1: Optional[float]     # 申卖价, 委托档位卖1档价格
-    ask_volume1: Optional[int]      # 申卖量
-    bid_price1: Optional[float]     # 申买价, 委托档位买1档价格
-    bid_volume1: Optional[int]      # 申买量
-    ask_price2: Optional[float]
-    ask_volume2: Optional[int]
-    bid_price2: Optional[float]
-    bid_volume2: Optional[int]
-    ask_price3: Optional[float]
-    ask_volume3: Optional[int]
-    bid_price3: Optional[float]
-    bid_volume3: Optional[int]
-    ask_price4: Optional[float]
-    ask_volume4: Optional[int]
-    bid_price4: Optional[float]
-    bid_volume4: Optional[int]
-    ask_price5: Optional[float]
-    ask_volume5: Optional[int]
-    bid_price5: Optional[float]
-    bid_volume5: Optional[int]
-    ask_price6: Optional[float]
-    ask_volume6: Optional[int]
-    bid_price6: Optional[float]
-    bid_volume6: Optional[int]
-    ask_price7: Optional[float]
-    ask_volume7: Optional[int]
-    bid_price7: Optional[float]
-    bid_volume7: Optional[int]
-    ask_price8: Optional[float]
-    ask_volume8: Optional[int]
-    bid_price8: Optional[float]
-    bid_volume8: Optional[int]
-    ask_price9: Optional[float]
-    ask_volume9: Optional[int]
-    bid_price9: Optional[float]
-    bid_volume9: Optional[int]
-    ask_price10: Optional[float]
-    ask_volume10: Optional[int]
-    bid_price10: Optional[float]
-    bid_volume10: Optional[int]
-
-
-class TsTickIdx(BaseModel):
-    ts_code: str
-    name: Optional[str]
-    trade_time: Optional[datetime]
-    last_price: Optional[float]                 # last_price    单位元
-    pre_close_price: Optional[float]            # pre_close_price
-    high_price: Optional[float]                 # high_price
-    open_price: Optional[float]                 # open_price
-    low_price: Optional[float]                  # low_price
-    close_price: Optional[float]                # close_price
-    volume: Optional[int]                       # volume, 成交总量
-    amount: Optional[float]                     # amount, 成交总金额
-
-
-class TsTickOpt(BaseModel):
-    ts_code: str
-    instrument_id: str
-    trade_time: Optional[datetime]
-    pre_price: Optional[float]                  # 单位元
-    price: Optional[float]
-    open: Optional[float]
-    high: Optional[float]
-    low: Optional[float]
-    close: Optional[float]
-    open_int: Optional[int]
-    vol: Optional[float]
-    amount: Optional[float]
-    num: Optional[int]
-    ask_price1: Optional[float]
-    ask_volume1: Optional[int]
-    bid_price1: Optional[float]
-    bid_volume1: Optional[int]
-    pre_delta: Optional[float]              # 昨虚实度，暂未提供
-    dif_price1: Optional[float]
-    dif_price2: Optional[float]
-    high_limit_price: Optional[float]
-    low_limit_price: Optional[float]
-    refer_price: Optional[float]            # 参考价，港股使用
-
-
-class TsTickFuture(BaseModel):
-    ts_code: str
-    instrument_id: Optional[str]
-    trade_time: Optional[datetime]
-    pre_price: Optional[float]
-    price: Optional[float]
-    open: Optional[float]
-    high: Optional[float]
-    low: Optional[float]
-    close: Optional[float]
-    open_int: Optional[int]
-    vol: Optional[int]
-    amount: Optional[int]                  # 单数量
-    num: Optional[int]
-    ask_price1: Optional[float]
-    ask_volume1: Optional[int]
-    bid_price1: Optional[float]
-    bid_volume1: Optional[int]
-    pre_delta: Optional[float]
-    curr_delta: Optional[float]
-    dif_price1: Optional[float]
-    dif_price2: Optional[float]
-    high_limit_price: Optional[float]
-    low_limit_price: Optional[float]
-    refer_price: Optional[float]
-    pre_settle_price: Optional[float]
-    settle_price: Optional[float]
+from datetime import datetime
+from typing import Optional
+
+from pydantic import BaseModel
+
+
+class TsTick(BaseModel):
+    ts_code: str
+    name: Optional[str]
+    trade_time: Optional[datetime]
+    pre_close_price: Optional[float]
+    last_price: Optional[float]
+    open_price: Optional[float]
+    high_price: Optional[float]
+    low_price: Optional[float]
+    close_price: Optional[float]
+    volume: Optional[int]           # 成交量
+    amount: Optional[int]           # 成交金额
+    count: Optional[int]            # 交易数量
+    ask_price1: Optional[float]     # 申卖价, 委托档位卖1档价格
+    ask_volume1: Optional[int]      # 申卖量
+    bid_price1: Optional[float]     # 申买价, 委托档位买1档价格
+    bid_volume1: Optional[int]      # 申买量
+    ask_price2: Optional[float]
+    ask_volume2: Optional[int]
+    bid_price2: Optional[float]
+    bid_volume2: Optional[int]
+    ask_price3: Optional[float]
+    ask_volume3: Optional[int]
+    bid_price3: Optional[float]
+    bid_volume3: Optional[int]
+    ask_price4: Optional[float]
+    ask_volume4: Optional[int]
+    bid_price4: Optional[float]
+    bid_volume4: Optional[int]
+    ask_price5: Optional[float]
+    ask_volume5: Optional[int]
+    bid_price5: Optional[float]
+    bid_volume5: Optional[int]
+    ask_price6: Optional[float]
+    ask_volume6: Optional[int]
+    bid_price6: Optional[float]
+    bid_volume6: Optional[int]
+    ask_price7: Optional[float]
+    ask_volume7: Optional[int]
+    bid_price7: Optional[float]
+    bid_volume7: Optional[int]
+    ask_price8: Optional[float]
+    ask_volume8: Optional[int]
+    bid_price8: Optional[float]
+    bid_volume8: Optional[int]
+    ask_price9: Optional[float]
+    ask_volume9: Optional[int]
+    bid_price9: Optional[float]
+    bid_volume9: Optional[int]
+    ask_price10: Optional[float]
+    ask_volume10: Optional[int]
+    bid_price10: Optional[float]
+    bid_volume10: Optional[int]
+
+
+class TsTickIdx(BaseModel):
+    ts_code: str
+    name: Optional[str]
+    trade_time: Optional[datetime]
+    last_price: Optional[float]                 # last_price
+    pre_close_price: Optional[float]            # pre_close_price
+    high_price: Optional[float]                 # high_price
+    open_price: Optional[float]                 # open_price
+    low_price: Optional[float]                  # low_price
+    close_price: Optional[float]                # close_price
+    volume: Optional[int]                       # volume, 成交总量
+    amount: Optional[float]                     # amount, 成交总金额
+
+
+class TsTickOpt(BaseModel):
+    ts_code: str
+    instrument_id: str
+    trade_time: Optional[datetime]
+    pre_price: Optional[float]
+    price: Optional[float]
+    open: Optional[float]
+    high: Optional[float]
+    low: Optional[float]
+    close: Optional[float]
+    open_int: Optional[int]
+    vol: Optional[float]
+    amount: Optional[float]
+    num: Optional[int]
+    ask_price1: Optional[float]
+    ask_volume1: Optional[int]
+    bid_price1: Optional[float]
+    bid_volume1: Optional[int]
+    pre_delta: Optional[float]              # 昨虚实度，暂未提供
+    dif_price1: Optional[float]
+    dif_price2: Optional[float]
+    high_limit_price: Optional[float]
+    low_limit_price: Optional[float]
+    refer_price: Optional[float]            # 参考价，港股使用
+
+
+class TsTickFuture(BaseModel):
+    ts_code: str
+    instrument_id: Optional[str]
+    trade_time: Optional[datetime]
+    pre_price: Optional[float]
+    price: Optional[float]
+    open: Optional[float]
+    high: Optional[float]
+    low: Optional[float]
+    close: Optional[float]
+    open_int: Optional[int]
+    vol: Optional[int]
+    amount: Optional[int]                  # 单数量
+    num: Optional[int]
+    ask_price1: Optional[float]
+    ask_volume1: Optional[int]
+    bid_price1: Optional[float]
+    bid_volume1: Optional[int]
+    pre_delta: Optional[float]
+    curr_delta: Optional[float]
+    dif_price1: Optional[float]
+    dif_price2: Optional[float]
+    high_limit_price: Optional[float]
+    low_limit_price: Optional[float]
+    refer_price: Optional[float]
+    pre_settle_price: Optional[float]
+    settle_price: Optional[float]
```

### Comparing `tushare-1.4.5/tushare/subs/tgw_subs/convert.py` & `tushare-1.4.6/tushare/subs/tgw_subs/convert.py`

 * *Files 18% similar despite different names*

```diff
@@ -58,22 +58,22 @@
         'variety_category': 5
     }
     """
     item = TsTickIdx(
         ts_code=get_ts_code(tgw_data.get("market_type"), tgw_data.get("security_code")),
         name=None,
         trade_time=datetime.strptime(str(tgw_data.get('orig_time'))[:-3], '%Y%m%d%H%M%S'),
-        last_price=tgw_data.get('last_index')/1000000,
-        pre_close_price=tgw_data.get('pre_close_index')/1000000,
-        open_price=tgw_data.get('open_index')/1000000,
-        high_price=tgw_data.get('high_index')/1000000,
-        low_price=tgw_data.get('low_index')/1000000,
-        close_price=tgw_data.get('close_index')/1000000,
-        volume=tgw_data.get('total_volume_trade')/100,
-        amount=tgw_data.get('total_value_trade')/100000,
+        last_price=tgw_data.get('last_index'),
+        pre_close_price=tgw_data.get('pre_close_index'),
+        open_price=tgw_data.get('open_index'),
+        high_price=tgw_data.get('high_index'),
+        low_price=tgw_data.get('low_index'),
+        close_price=tgw_data.get('close_index'),
+        volume=tgw_data.get('total_volume_trade'),
+        amount=tgw_data.get('total_value_trade'),
     )
     return item
 
 
 def convert_tick_stock(tgw_data: dict) -> TsTick:
     """
     tick_demo = {
@@ -134,27 +134,27 @@
         'IOPV': 0,
         'high_limited': 7810000,
         'low_limited': 6390000
     }
     """
     extra = {}
     for i in range(1, 11):
-        extra[f'ask_price{i}'] = tgw_data.get(f'offer_price{i}')/1000000
-        extra[f'ask_volume{i}'] = tgw_data.get(f'offer_volume{i}')/100
-        extra[f'bid_price{i}'] = tgw_data.get(f'bid_price{i}')/1000000
-        extra[f'bid_volume{i}'] = tgw_data.get(f'bid_volume{i}')/100
+        extra[f'ask_price{i}'] = tgw_data.get(f'offer_price{i}')
+        extra[f'ask_volume{i}'] = tgw_data.get(f'offer_volume{i}')
+        extra[f'bid_price{i}'] = tgw_data.get(f'bid_price{i}')
+        extra[f'bid_volume{i}'] = tgw_data.get(f'bid_volume{i}')
     item = TsTick(
         ts_code=get_ts_code(tgw_data.get("market_type"), tgw_data.get("security_code")),
         name=None,
         trade_time=datetime.strptime(str(tgw_data.get('orig_time'))[:-3], '%Y%m%d%H%M%S'),
-        pre_close_price=tgw_data.get("pre_close_price")/1000000,
-        last_price=tgw_data.get("last_price")/1000000,
-        open_price=tgw_data.get("open_price")/1000000,
-        high_price=tgw_data.get("high_price")/1000000,
-        low_price=tgw_data.get("low_price")/1000000,
-        close_price=tgw_data.get("close_price")/1000000,
-        volume=tgw_data.get("total_volume_trade")/100,
-        amount=tgw_data.get("total_value_trade")/1000000,
+        pre_close_price=tgw_data.get("pre_close_price"),
+        last_price=tgw_data.get("last_price"),
+        open_price=tgw_data.get("open_price"),
+        high_price=tgw_data.get("high_price"),
+        low_price=tgw_data.get("low_price"),
+        close_price=tgw_data.get("close_price"),
+        volume=tgw_data.get("total_volume_trade"),
+        amount=tgw_data.get("total_value_trade"),
         count=tgw_data.get("num_trades"),
         **extra
     )
     return item
```

### Comparing `tushare-1.4.5/tushare/subs/tgw_subs/login.py` & `tushare-1.4.6/tushare/subs/tgw_subs/login.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/subs/tgw_subs/subscribe.py` & `tushare-1.4.6/tushare/subs/tgw_subs/subscribe.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/subs/ts_subs/subscribe.py` & `tushare-1.4.6/tushare/subs/ts_subs/subscribe.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/trader/trader.py` & `tushare-1.4.6/tushare/trader/trader.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/trader/utils.py` & `tushare-1.4.6/tushare/trader/utils.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/trader/vars.py` & `tushare-1.4.6/tushare/trader/vars.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/common.py` & `tushare-1.4.6/tushare/util/common.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/conns.py` & `tushare-1.4.6/tushare/util/conns.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/dateu.py` & `tushare-1.4.6/tushare/util/dateu.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/form_date.py` & `tushare-1.4.6/tushare/util/form_date.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/format_stock_code.py` & `tushare-1.4.6/tushare/util/format_stock_code.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/formula.py` & `tushare-1.4.6/tushare/util/formula.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/mailmerge.py` & `tushare-1.4.6/tushare/util/mailmerge.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/netbase.py` & `tushare-1.4.6/tushare/util/netbase.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/protobuf/funcs.py` & `tushare-1.4.6/tushare/util/protobuf/funcs.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/protobuf/response_pb2.py` & `tushare-1.4.6/tushare/util/protobuf/response_pb2.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/store.py` & `tushare-1.4.6/tushare/util/store.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/upass.py` & `tushare-1.4.6/tushare/util/upass.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/vars.py` & `tushare-1.4.6/tushare/util/vars.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare/util/verify_token.py` & `tushare-1.4.6/tushare/util/verify_token.py`

 * *Files identical despite different names*

### Comparing `tushare-1.4.5/tushare.egg-info/PKG-INFO` & `tushare-1.4.6/tushare.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,94 @@
 Metadata-Version: 2.1
 Name: tushare
-Version: 1.4.5
+Version: 1.4.6
 Summary: A utility for crawling historical and Real-time Quotes data of China stocks
 Home-page: https://tushare.pro
 Author: Jimmy Liu
 Author-email: waditu@163.com
 License: BSD
-Description: 
-        TuShare
-        ===============
-        
-        .. image:: https://api.travis-ci.org/waditu/tushare.png?branch=master
-            :target: https://travis-ci.org/waditu/tushare
-        
-        .. image:: https://badge.fury.io/py/tushare.png
-            :target: http://badge.fury.io/py/tushare
-        
-        * easy to use as most of the data returned are pandas DataFrame objects
-        * can be easily saved as csv, excel or json files
-        * can be inserted into MySQL or Mongodb
-        
-        Target Users
-        --------------
-        
-        * financial market analyst of China
-        * learners of financial data analysis with pandas/NumPy
-        * people who are interested in China financial data
-        
-        Installation
-        --------------
-        
-            pip install tushare
-            
-        Upgrade
-        ---------------
-        
-            pip install tushare --upgrade
-            
-        Quick Start
-        --------------
-        
-        ::
-        
-            import tushare as ts
-            
-            ts.get_hist_data('600848')
-            
-        return::
-        
-                        open    high   close     low     volume    p_change  ma5     
-            date
-            2012-01-11   6.880   7.380   7.060   6.880   14129.96     2.62   7.060
-            2012-01-12   7.050   7.100   6.980   6.900    7895.19    -1.13   7.020
-            2012-01-13   6.950   7.000   6.700   6.690    6611.87    -4.01   6.913
-            2012-01-16   6.680   6.750   6.510   6.480    2941.63    -2.84   6.813
-            2012-01-17   6.660   6.880   6.860   6.460    8642.57     5.38   6.822
-            2012-01-18   7.000   7.300   6.890   6.880   13075.40     0.44   6.788
-            2012-01-19   6.690   6.950   6.890   6.680    6117.32     0.00   6.770
-            2012-01-20   6.870   7.080   7.010   6.870    6813.09     1.74   6.832
-            
-            
-        Log
-        --------------
-        1.4.0
-        -------
-        - 增加 银河证券实时行情数据入口
-        1.3.9
-        -------
-        - realtime_quote 实时盘口TICK快照(爬虫版)
-        - 修复dc 指数和股票数据抓取问题
-        - 将数字类型统一转换成 float类型
-        1.2.73
-        -------
-        - 支持华泰实时数据15SECOND
-            
-        
 Keywords: Global Financial Data
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/plain
+License-File: LICENSE
+
+
+TuShare
+===============
+
+.. image:: https://api.travis-ci.org/waditu/tushare.png?branch=master
+    :target: https://travis-ci.org/waditu/tushare
+
+.. image:: https://badge.fury.io/py/tushare.png
+    :target: http://badge.fury.io/py/tushare
+
+* easy to use as most of the data returned are pandas DataFrame objects
+* can be easily saved as csv, excel or json files
+* can be inserted into MySQL or Mongodb
+
+Target Users
+--------------
+
+* financial market analyst of China
+* learners of financial data analysis with pandas/NumPy
+* people who are interested in China financial data
+
+Installation
+--------------
+
+    pip install tushare
+    
+Upgrade
+---------------
+
+    pip install tushare --upgrade
+    
+Quick Start
+--------------
+
+::
+
+    import tushare as ts
+    
+    ts.get_hist_data('600848')
+    
+return::
+
+                open    high   close     low     volume    p_change  ma5     
+    date
+    2012-01-11   6.880   7.380   7.060   6.880   14129.96     2.62   7.060
+    2012-01-12   7.050   7.100   6.980   6.900    7895.19    -1.13   7.020
+    2012-01-13   6.950   7.000   6.700   6.690    6611.87    -4.01   6.913
+    2012-01-16   6.680   6.750   6.510   6.480    2941.63    -2.84   6.813
+    2012-01-17   6.660   6.880   6.860   6.460    8642.57     5.38   6.822
+    2012-01-18   7.000   7.300   6.890   6.880   13075.40     0.44   6.788
+    2012-01-19   6.690   6.950   6.890   6.680    6117.32     0.00   6.770
+    2012-01-20   6.870   7.080   7.010   6.870    6813.09     1.74   6.832
+    
+    
+Log
+--------------
+1.4.6
+-------
+- 修复 realtime_quote 实时盘口TICK快照(爬虫版)
+- 修复dc OPEN和LOW 值相反问题
+1.4.0
+-------
+- 增加 银河证券实时行情数据入口
+1.3.9
+-------
+- realtime_quote 实时盘口TICK快照(爬虫版)
+- 修复dc 指数和股票数据抓取问题
+- 将数字类型统一转换成 float类型
+1.2.73
+-------
+- 支持华泰实时数据15SECOND
+    
+
+
```

### Comparing `tushare-1.4.5/tushare.egg-info/SOURCES.txt` & `tushare-1.4.6/tushare.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 LICENSE
 README.md
 setup.py
+baks/__init__.py
+baks/demo.py
+baks/rtqc.py
+baks/setup.py
+baks/sss.py
 tushare/__init__.py
 tushare.egg-info/PKG-INFO
 tushare.egg-info/SOURCES.txt
 tushare.egg-info/dependency_links.txt
 tushare.egg-info/requires.txt
 tushare.egg-info/top_level.txt
 tushare/bond/__init__.py
@@ -40,14 +45,15 @@
 tushare/stock/minsdata.py
 tushare/stock/news_vars.py
 tushare/stock/newsevent.py
 tushare/stock/ref_vars.py
 tushare/stock/reference.py
 tushare/stock/rtq.py
 tushare/stock/rtq_vars.py
+tushare/stock/rtqc.pyd
 tushare/stock/shibor.py
 tushare/stock/trading.py
 tushare/subs/__init__.py
 tushare/subs/ht_subs/__init__.py
 tushare/subs/ht_subs/covert.py
 tushare/subs/ht_subs/subscribe.py
 tushare/subs/model/__init__.py
```

