# Comparing `tmp/bfgcardplay-1.1.0.tar.gz` & `tmp/bfgcardplay-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgcardplay-1.1.0.tar", last modified: Sun Jan  7 12:14:51 2024, max compression
+gzip compressed data, was "bfgcardplay-1.1.1.tar", last modified: Mon Apr 15 14:30:36 2024, max compression
```

## Comparing `bfgcardplay-1.1.0.tar` & `bfgcardplay-1.1.1.tar`

### file list

```diff
@@ -1,59 +1,70 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2024-01-07 12:14:51.181384 bfgcardplay-1.1.0/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4615 2024-01-07 12:14:51.181384 bfgcardplay-1.1.0/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.1.0/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2024-01-07 12:14:51.171384 bfgcardplay-1.1.0/bfgcardplay/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      216 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2024-01-07 12:12:25.000000 bfgcardplay-1.1.0/bfgcardplay/_version.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.1.0/bfgcardplay/logger.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2024-01-07 12:14:51.178051 bfgcardplay-1.1.0/bfgcardplay/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3446 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/card_player_components.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2222 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/cards.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    20361 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/dashboard.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4541 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/data_classes.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    12345 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/declarer_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4009 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/defender_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9751 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/first_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16101 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/first_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    18736 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/first_seat_declarer_nt.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    21812 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/first_seat_declarer_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16423 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/first_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2103 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/fourth_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6308 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/fourth_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5329 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/fourth_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/global_variables.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3935 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/manager.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      665 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/opening_lead.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6982 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    43373 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/opening_lead_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    42960 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3113 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/second_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    10502 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/second_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6579 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/second_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3714 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/suggested_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2095 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/third_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17144 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/third_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    15193 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/third_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7517 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/src/utilities.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2024-01-07 12:14:51.181384 bfgcardplay-1.1.0/bfgcardplay/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2986 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/blitz.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      557 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_first_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      574 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_first_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      520 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_fourth_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      252 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_fourth_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    11743 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    15311 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_opening_lead_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1941 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      568 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_second_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      462 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_third_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      743 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_third_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6565 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/test_utilities.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      619 2024-01-07 12:11:58.000000 bfgcardplay-1.1.0/bfgcardplay/tests/utilities.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2024-01-07 12:14:51.171384 bfgcardplay-1.1.0/bfgcardplay.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4615 2024-01-07 12:14:51.000000 bfgcardplay-1.1.0/bfgcardplay.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1802 2024-01-07 12:14:51.000000 bfgcardplay-1.1.0/bfgcardplay.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2024-01-07 12:14:51.000000 bfgcardplay-1.1.0/bfgcardplay.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2024-01-07 12:14:51.000000 bfgcardplay-1.1.0/bfgcardplay.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2024-01-07 12:14:51.181384 bfgcardplay-1.1.0/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1431 2023-06-30 08:31:25.000000 bfgcardplay-1.1.0/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-15 14:30:36.514781 bfgcardplay-1.1.1/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     4679 2024-04-15 14:30:36.514781 bfgcardplay-1.1.1/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        2 2021-07-03 11:00:42.000000 bfgcardplay-1.1.1/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-15 14:30:36.511448 bfgcardplay-1.1.1/bfgcardplay/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      216 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)       22 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/_version.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      912 2021-11-08 15:49:34.000000 bfgcardplay-1.1.1/bfgcardplay/logger.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-15 14:30:36.514781 bfgcardplay-1.1.1/bfgcardplay/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        0 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     3446 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/card_player_components.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2222 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/cards.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    20361 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/dashboard.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     4541 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/data_classes.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    12345 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/declarer_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     4009 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/defender_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     9751 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/first_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    16101 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/first_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    18736 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/first_seat_declarer_nt.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    21812 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/first_seat_declarer_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    17428 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2103 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/fourth_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     6308 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     5329 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/fourth_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      134 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/global_variables.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     3935 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/manager.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      665 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/opening_lead.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     6982 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    43373 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    42960 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     3113 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/second_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    10502 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/second_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     6737 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/second_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     3714 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/suggested_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2095 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/third_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    17962 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/third_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    15322 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     7517 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/src/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-15 14:30:36.514781 bfgcardplay-1.1.1/bfgcardplay/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        0 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2986 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/blitz.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-15 14:30:36.514781 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      931 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/first_seat_declarer.pbn
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1129 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/first_seat_defender.pbn
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      572 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/fourth_seat_declarer.pbn
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      292 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/fourth_seat_defender.pbn
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1383 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/player.pbn
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      802 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/second_seat_declarer.pbn
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      339 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/second_seat_defender.pbn
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1013 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/third_seat_declarer.pbn
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1465 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_data/third_seat_defender.pbn
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      557 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_first_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      674 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      520 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      252 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_fourth_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    11743 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    15311 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1941 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      568 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_second_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      266 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_second_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      462 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_third_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      867 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     6565 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/test_utilities.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      619 2024-04-15 14:25:14.000000 bfgcardplay-1.1.1/bfgcardplay/tests/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-15 14:30:36.511448 bfgcardplay-1.1.1/bfgcardplay.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     4679 2024-04-15 14:30:36.000000 bfgcardplay-1.1.1/bfgcardplay.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2308 2024-04-15 14:30:36.000000 bfgcardplay-1.1.1/bfgcardplay.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        1 2024-04-15 14:30:36.000000 bfgcardplay-1.1.1/bfgcardplay.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)       12 2024-04-15 14:30:36.000000 bfgcardplay-1.1.1/bfgcardplay.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)       38 2024-04-15 14:30:36.514781 bfgcardplay-1.1.1/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1431 2023-06-30 08:31:24.000000 bfgcardplay-1.1.1/setup.py
```

### Comparing `bfgcardplay-1.1.0/PKG-INFO` & `bfgcardplay-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.1.0
-Summary:              A collection of modules that facilitate cardplay in the BfG environment.         
+Version: 1.1.1
+Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
+Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
-Download-URL: https://pypi.org/project/bfgcardplay/
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.1.1 15 April 2024
+
+1. Modifications to first_player defender and third_player_defender
+
+------
+
 Version 1.1.0 7 Jan 2024
 
 1. Major refactor
 
 ------
 
 Version 1.0.15 18 Sep 2023
@@ -332,9 +337,7 @@
 ------
 
 Version 0.0.0 - 3 July 2021
 
 Created
 
 ------
-
-
```

### Comparing `bfgcardplay-1.1.0/bfgcardplay/logger.py` & `bfgcardplay-1.1.1/bfgcardplay/logger.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/card_player_components.py` & `bfgcardplay-1.1.1/bfgcardplay/src/card_player_components.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/cards.py` & `bfgcardplay-1.1.1/bfgcardplay/src/cards.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/dashboard.py` & `bfgcardplay-1.1.1/bfgcardplay/src/dashboard.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/data_classes.py` & `bfgcardplay-1.1.1/bfgcardplay/src/data_classes.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/declarer_play.py` & `bfgcardplay-1.1.1/bfgcardplay/src/declarer_play.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/defender_play.py` & `bfgcardplay-1.1.1/bfgcardplay/src/defender_play.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/first_seat.py` & `bfgcardplay-1.1.1/bfgcardplay/src/first_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/first_seat_declarer.py` & `bfgcardplay-1.1.1/bfgcardplay/src/first_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/first_seat_declarer_nt.py` & `bfgcardplay-1.1.1/bfgcardplay/src/first_seat_declarer_nt.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/first_seat_declarer_suit.py` & `bfgcardplay-1.1.1/bfgcardplay/src/first_seat_declarer_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/first_seat_defender.py` & `bfgcardplay-1.1.1/bfgcardplay/src/first_seat_defender.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,17 +226,22 @@
         # if deduce_partner_void_in_trumps(player):
         #     manager.voids[player.partner_seat][player.trump_suit.name] = True
 
         partners_seat = player.partner_seat
         partners_voids = player.voids[partners_seat]
         if not partners_voids[player.trump_suit.name]:
             for suit in SUITS:
-                if player.voids[partners_seat][suit] and player.unplayed_cards[suit]:
+                if (player.voids[partners_seat][suit] and
+                        player.unplayed_cards[suit]):
                     manager.set_suit_to_develop(player.seat, Suit(suit))
-                    manager.set_suit_strategy(player.seat, suit, 'ruff_in_void')
+                    manager.set_suit_strategy(
+                        player.seat,
+                        suit,
+                        'ruff_in_void'
+                    )
                     return log(inspect.stack(), Suit(suit))
         return None
 
     def _select_suit_for_nt_contract(self) -> Suit:
         """Return the trick lead suit for the defending a suit contract."""
         player = self.player
 
@@ -273,15 +278,16 @@
         best_suit = self._best_suit(score_reasons)
         return log(inspect.stack(), best_suit)
 
     def _suit_after_partner_signal(self) -> Suit:
         player = self.player
         if len(player.board.tricks) == 2 and player.dummy_on_right:
             partners_lead = player.board.tricks[0].cards[0]
-            if partners_lead.value >= CARD_VALUES['T'] or partners_lead.value < CARD_VALUES['6']:
+            if (partners_lead.value >= CARD_VALUES['T'] or
+                    partners_lead.value < CARD_VALUES['6']):
                 if player.unplayed_cards[partners_lead.suit.name]:
                     return log(inspect.stack(), partners_lead.suit)
         return None
 
     def _suit_to_develop(self) -> Suit:
         player = self.player
         manager = global_vars.manager
@@ -313,23 +319,26 @@
 
     def _is_winner_defender(self) -> Suit:
         player = self.player
         if len(player.board.tricks) > 6:
             for suit in SUITS:
                 cards = player.unplayed_cards[suit]
                 if cards:
-                    if player.is_winner_defender(player.unplayed_cards[suit][0]):
+                    if player.is_winner_defender(
+                            player.unplayed_cards[suit][0]
+                        ):
                         return log(inspect.stack(), Suit(suit))
         return None
 
     def _liked_suit(self) -> Suit:
         player = self.player
         manager = global_vars.manager
         for suit in SUITS:
-            if manager.like_dislike(player.partner_seat, suit) and player.unplayed_cards[suit]:
+            if (manager.like_dislike(player.partner_seat, suit) and
+                    player.unplayed_cards[suit]):
                 return log(inspect.stack(), Suit(suit))
         return None
 
     def _select_card_from_suit(self, suit: Suit) -> Card:
         """Return the card to lead from the given suit."""
         player = self.player
         manager = global_vars.manager
@@ -346,25 +355,30 @@
                         return log(inspect.stack(), suit_cards[-1])
 
         # Winning card
         if player.trump_suit:
             if player.is_winner_defender(player.unplayed_cards[suit][0]):
                 return log(inspect.stack(), cards[0])
 
+        if self._all_winners(suit):
+            return log(inspect.stack(), player.unplayed_cards[suit][0])
+
         # Top of touching honours
         for index, card in enumerate(cards[:-1]):
             if card.is_honour and card.value == cards[index+1].value + 1:
                 return log(inspect.stack(), card)
 
         # Top of doubleton
         if len(cards) == 2:
             return log(inspect.stack(), cards[0])
 
         # Return winners
+        # TODO sort out invalid for defender
         winners = player.winners[suit.name]
+        ic(winners)
         if winners and winners[-1] in cards:
             return log(inspect.stack(), winners[-1])
 
         # Return bottom card
         return log(inspect.stack(), cards[-1])
 
     def _sequences(self) -> Suit:
@@ -401,21 +415,36 @@
         player = self.player
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         for suit in SUITS:
             if not self.player.suit_cards[suit]:
                 suit_scores[suit] -= self.VOID_SCORE
             if player.trump_suit:
                 dummy_short_trumps = dummy_is_short_trump_hand(player)
-                if ((dummy_short_trumps and not player.dummys_suit_cards[suit])):
+                if (dummy_short_trumps and not player.dummys_suit_cards[suit]):
                     suit_scores[suit] -= self.RUFF_AND_DISCARD_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
 
     def _trumps(self) -> list[tuple[str, int]]:
         """Assign score to suits based on void."""
         suit_scores = {suit_name: 0 for suit_name in SUITS}
         player = self.player
         if player.trump_suit:
             my_cards = player.unplayed_cards[player.trump_suit.name]
             dummys_cards = player.dummys_suit_cards[player.trump_suit.name]
             if len(my_cards) > len(dummys_cards):
                 suit_scores[player.trump_suit.name] += self.TRUMP_SCORE
         return [(suit_name, score) for suit_name, score in suit_scores.items()]
+
+    def _all_winners(self, suit: Suit) -> bool:
+        """Return True if all of the cards held are winners."""
+        player = self.player
+        all_winners = True
+        unplayed_cards = len(player.total_unplayed_cards[suit])
+        missing_cards = unplayed_cards - len(player.suit_cards[suit])
+        if len(player.unplayed_cards[suit]) < missing_cards:
+            return False
+        for index in range(missing_cards):
+            if not player.is_winner_defender(
+                    player.unplayed_cards[suit][index]
+                ):
+                all_winners = False
+        return all_winners
```

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/fourth_seat.py` & `bfgcardplay-1.1.1/bfgcardplay/src/fourth_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/fourth_seat_declarer.py` & `bfgcardplay-1.1.1/bfgcardplay/src/fourth_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/fourth_seat_defender.py` & `bfgcardplay-1.1.1/bfgcardplay/src/fourth_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/manager.py` & `bfgcardplay-1.1.1/bfgcardplay/src/manager.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/opening_lead.py` & `bfgcardplay-1.1.1/bfgcardplay/src/opening_lead.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/opening_lead_card.py` & `bfgcardplay-1.1.1/bfgcardplay/src/opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/opening_lead_suit.py` & `bfgcardplay-1.1.1/bfgcardplay/src/opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/player.py` & `bfgcardplay-1.1.1/bfgcardplay/src/player.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/second_seat.py` & `bfgcardplay-1.1.1/bfgcardplay/src/second_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/second_seat_declarer.py` & `bfgcardplay-1.1.1/bfgcardplay/src/second_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/second_seat_defender.py` & `bfgcardplay-1.1.1/bfgcardplay/src/second_seat_defender.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,22 +87,27 @@
         #                 return card
         return None
 
     def _play_winner(self) -> Card:
         player = self.player
         cards = self.cards
         suit = self.trick.suit.name
+        if self.trick.cards[0].value > player.unplayed_cards[suit][0].value:
+            return None
+
         if player.trick_number >= 9:
             if not player.dummys_unplayed_cards[suit]:
                 dummys_top_value = 0
             else:
                 dummys_top_value = player.dummys_unplayed_cards[suit][0].value
 
-            dummy_safe = (player.dummy_on_right and cards[0].value < dummys_top_value or
-                          player.dummy_on_left and cards[0].value > dummys_top_value)
+            dummy_safe = ((player.dummy_on_right and
+                          cards[0].value < dummys_top_value) or
+                          (player.dummy_on_left and
+                          cards[0].value > dummys_top_value))
             if dummy_safe:
                 return log(inspect.stack(), cards[0])
         return None
 
     def _play_doubleton_king(self) -> Card:
         player = self.player
         suit = self.trick.suit.name
```

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/suggested_card.py` & `bfgcardplay-1.1.1/bfgcardplay/src/suggested_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/third_seat.py` & `bfgcardplay-1.1.1/bfgcardplay/src/third_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/third_seat_declarer.py` & `bfgcardplay-1.1.1/bfgcardplay/src/third_seat_declarer.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,16 @@
 
         # Win trick if possible
         winning_card = self._get_winning_card()
         if winning_card:
             return winning_card
 
         # Cover honour with honour
-        if trick.cards[1].is_honour and trick.cards[1].value > trick.cards[0].value:
+        if (trick.cards[1].is_honour and
+                trick.cards[1].value > trick.cards[0].value):
             for card in cards[::-1]:
                 if card.value > trick.cards[1].value:
                     return log(inspect.stack(), card)
 
         return log(inspect.stack(), cards[-1])
 
     def _select_card_in_suit_to_develop(self, suit: Suit) -> Card:
@@ -106,57 +107,65 @@
 
         # Play bottom of tenace if missing King
         missing_king = manager.missing_king[player.seat][suit.name]
         if player.is_tenace(cards[0], cards[1]) and missing_king:
             return log(inspect.stack(), cards[1])
 
         # Force out honour
-        if len(cards) > 1 and len(player.opponents_unplayed_cards[suit]) > 1:
-            if (cards[1].value > player.opponents_unplayed_cards[suit][1].value and
+        opps_unplayed_cards = player.opponents_unplayed_cards[suit.name]
+        if len(cards) > 1 and len(opps_unplayed_cards) > 1:
+            if (cards[1].value > opps_unplayed_cards[1].value and
                     cards[1].value > trick.cards[1].value):
                 return log(inspect.stack(), cards[1])
 
         # Play winner if needed to make contract
         tricks_needed = player.tricks_needed - player.declarers_tricks
         if tricks_needed <= player.sure_tricks.count:
             card = play_lowest_winning_card(player, cards, trick)
-            return log(inspect.stack(), card)
+            if card:
+                return log(inspect.stack(), card)
 
-        if len(player.opponents_unplayed_cards[suit]) == 1:
+        if len(opps_unplayed_cards) == 1:
             card = play_lowest_winning_card(player, cards, trick)
-            return log(inspect.stack(), card)
+            if card:
+                return log(inspect.stack(), card)
 
-        if len(player.partners_unplayed_cards[suit.name]) < len(player.unplayed_cards[suit.name]):
+        unplayed_cards = player.unplayed_cards[suit.name]
+        partners_unplayed_cards = player.partners_unplayed_cards[suit.name]
+        if len(partners_unplayed_cards) < len(unplayed_cards):
             return log(inspect.stack(), cards[-1])
 
         if not player.is_winner_declarer(trick.cards[0], trick):
             for index, card in enumerate(cards[:-1]):
-                if card.value > trick.cards[1].value and card. value > cards[index+1].value + 1:
+                if (card.value > trick.cards[1].value and
+                        card. value > cards[index+1].value + 1):
                     return log(inspect.stack(), card)
 
         return log(inspect.stack(), cards[-1])
 
     def _manager_win_trick(self, suit) -> Card:
         player = self.player
         cards = self.cards
         manager = global_vars.manager
         if manager.win_trick[player.seat]:
+            opps_unplayed_cards = player.opponents_unplayed_cards[suit.name]
             manager.win_trick[player.seat] = False
             for card in cards[::-1]:
-                if card.value > player.opponents_unplayed_cards[suit.name][0].value:
+                if card.value > opps_unplayed_cards[0].value:
                     return log(inspect.stack(), card)
         return None
 
     def _missing_ace(self, suit) -> Card:
         player = self.player
         manager = global_vars.manager
         if manager.suit_strategy(player.seat)[suit.name] == 'missing_ace':
             if not self.trick.cards[0].is_honour:
                 for card in self.cards:
-                    if card.is_honour and card.value > self.trick.cards[1].value:
+                    if (card.is_honour and
+                            card.value > self.trick.cards[1].value):
                         return log(inspect.stack(), card)
         return None
 
     def _missing_king(self, suit) -> Card:
         player = self.player
         trick = self.trick
         cards = self.cards
@@ -172,15 +181,16 @@
         return None
 
     def _missing_queen(self, suit) -> Card:
         player = self.player
         manager = global_vars.manager
         (ace, king, queen, jack) = SuitCards(suit.name).cards('A', 'J')
         missing_queen = queen in player.opponents_unplayed_cards[suit.name]
-        if manager.suit_strategy(player.seat)[suit.name] == 'missing_queen' and missing_queen:
+        manage_strategy = manager.suit_strategy(player.seat)[suit.name]
+        if (manage_strategy == 'missing_queen' and missing_queen):
             card = self._get_winning_card()
             if card:
                 return card
         return None
 
     def _play_suit_out(self) -> Card:
         player = self.player
@@ -237,15 +247,17 @@
 
         # Cover honour with honour
         card = self._cover_honour_with_honour()
         if card:
             return card
 
         # Push out honour
-        if cards[0].is_honour and not player.is_winner_declarer(cards[0]) and len(cards) > 1:
+        if (cards[0].is_honour and
+                not player.is_winner_declarer(cards[0]) and
+                len(cards) > 1):
             return log(inspect.stack(), cards[1])
 
         # Overtake partner if appropriate
         card = self._overtake_partner()
         if card:
             return card
 
@@ -267,16 +279,18 @@
 
     def _deblock_suit(self) -> Card:
         player = self.player
         trick = self.trick
         cards = self.cards
         if trick.cards[0].value < cards[0].value:
             values = trick_card_values(trick, player.trump_suit)
-            is_winner = player.is_winner_declarer(trick.cards[0], trick) and values[0] > values[1]
-            if is_winner and len(player.partners_unplayed_cards[trick.suit.name]) > 1:
+            is_winner = (player.is_winner_declarer(trick.cards[0], trick) and
+                         values[0] > values[1])
+            if (len(player.partners_unplayed_cards[trick.suit.name]) > 1 and
+                    is_winner):
                 return log(inspect.stack(), cards[-1])
 
             our_cards = player.our_unplayed_cards[trick.suit.name]
             partners_length = len(player.partners_unplayed_cards[trick.suit.name])
             my_length = len(player.unplayed_cards[trick.suit.name])
             if (player.is_winner_declarer(our_cards[0], trick) and
                     player.is_winner_declarer(our_cards[1], trick) and
@@ -301,65 +315,71 @@
                         card.value != cards[index+1].value + 1):
                     if not self._ace_is_deprecated(trick, card):
                         return log(inspect.stack(), card)
         return None
 
     def _cover_honour_with_honour(self) -> Card:
         trick = self.trick
-        if trick.cards[1].is_honour and trick.cards[1].value > trick.cards[0].value:
+        if (trick.cards[1].is_honour and
+                trick.cards[1].value > trick.cards[0].value):
             for card in self.cards[::-1]:
-                if card.value > trick.cards[0].value and card.value > trick.cards[1].value:
+                if (card.value > trick.cards[0].value and
+                        card.value > trick.cards[1].value):
                     return log(inspect.stack(), card)
 
     def _get_card_over_top_of_tenace(self) -> Card:
         player = self.player
         trick = self.trick
-        top_in_tenace = player.get_suit_tenaces(player.our_unplayed_cards[trick.suit.name])
+        our_unplayed_cards = player.our_unplayed_cards[trick.suit.name]
+        top_in_tenace = player.get_suit_tenaces(our_unplayed_cards)
         if top_in_tenace:
             for card in self.cards:
                 if card.value < top_in_tenace.value + 1:
                     return log(inspect.stack(), card)
         return None
 
     def _card_from_all_winners(self) -> Card:
         player = self.player
         trick = self.trick
         cards = self.cards
+        opps_unplayed_cards = player.opponents_unplayed_cards[trick.suit]
         if (player.holds_all_winners_in_suit(trick.suit, trick) or
                 player.sure_tricks.count >= 13 - player.trick_number):
-            if player.opponents_unplayed_cards[trick.suit]:
-                if (trick.cards[0].value > player.opponents_unplayed_cards[trick.suit][0].value and
+            if opps_unplayed_cards:
+                if (trick.cards[0].value > opps_unplayed_cards[0].value and
                         trick.cards[0].value > trick.cards[1].value):
                     return log(inspect.stack(), cards[-1])
                 else:
                     card = play_lowest_winning_card(player, cards, trick)
                     return log(inspect.stack(), card)
         return None
 
     def _card_from_probable_winners(self) -> Card:
         player = self.player
         trick = self.trick
         cards = self.cards
+        opps_unplayed_cards = player.opponents_unplayed_cards[trick.suit]
         if player.holds_all_winners_in_suit(trick.suit, trick):
-            if player.opponents_unplayed_cards[trick.suit]:
-                if (trick.cards[0].value > player.opponents_unplayed_cards[trick.suit][0].value and
+            if opps_unplayed_cards:
+                if (trick.cards[0].value > opps_unplayed_cards[0].value and
                         trick.cards[0].value > trick.cards[1].value):
                     return log(inspect.stack(), cards[-1])
                 else:
                     return log(inspect.stack(), cards[0])
         return None
 
     def _card_from_suit_to_develop(self, card_value) -> Card:
         player = self.player
         trick = self.trick
         cards = self.cards
         manager = global_vars.manager
         opponents_cards = []
+        manage_strategy = manager.suit_strategy(player.seat)[trick.suit.name]
         if (manager.suit_to_develop(player.seat) == trick.suit or
-                manager.suit_strategy(player.seat)[trick.suit.name] == 'missing_queen'):
+                manage_strategy == 'missing_queen'):
             opponents_cards = player.opponents_unplayed_cards[trick.suit.name]
 
             card = self._card_from_tenace_in_my_hand(cards)
             if card:
                 return card
 
             if opponents_cards:
@@ -387,16 +407,17 @@
     def _select_card_if_void(self) -> Card:
         """Return card if cannot follow suit."""
         player = self.player
         trick = self.trick
 
         # Trump if appropriate
         if player.trump_suit:
+            trumps = player.trump_suit
             if not player.is_winner_declarer(trick.cards[0], trick):
-                opponents_trumps = player.opponents_unplayed_cards[player.trump_suit.name]
+                opponents_trumps = player.opponents_unplayed_cards[trumps]
                 if player.trump_cards and not opponents_trumps:
                     return log(inspect.stack(), player.trump_cards[-1])
                 if player.trump_cards and opponents_trumps:
                     if self._trump_partners_card():
                         card_value = trick.cards[1].value
                         if trick.cards[1].suit == player.trump_suit:
                             card_value += 13
@@ -405,38 +426,43 @@
                             if card.value + 13 > card_value:
                                 return log(inspect.stack(), card)
 
         opponents_cards = player.opponents_unplayed_cards[trick.suit.name]
 
         # Find card to discard
         if player.trump_suit:
-            suits = {suit_name: suit for suit_name, suit in SUITS.items() if suit_name != player.trump_suit.name}
+            suits = {suit_name: suit for suit_name, suit in SUITS.items()
+                     if suit_name != player.trump_suit.name}
         else:
             suits = {suit_name: suit for suit_name, suit in SUITS.items()}
 
         # Find a loser
         suit_length: dict[str, int] = {}
         for suit_name in suits.keys():
             if player.suit_cards[suit_name]:
                 suit_length[suit_name] = len(player.suit_cards[suit_name])
                 our_cards = player.our_unplayed_cards[suit_name]
                 opponents_cards = player.opponents_unplayed_cards[suit_name]
                 if opponents_cards:
+                    unplayed_cards = player.unplayed_cards[suit_name]
                     if (our_cards[0].value < opponents_cards[0].value and
-                            len(player.unplayed_cards[suit_name]) > len(opponents_cards) / 2):
-                        return log(inspect.stack(), player.suit_cards[suit_name][-1])
+                            len(unplayed_cards) > len(opponents_cards) / 2):
+                        return log(inspect.stack(),
+                                   player.suit_cards[suit_name][-1])
                 elif (player.board.contract.denomination.is_suit and
                       not self.player.is_declarer):
-                    return log(inspect.stack(), player.suit_cards[suit_name][-1])
+                    return log(inspect.stack(),
+                               player.suit_cards[suit_name][-1])
 
         # Only trumps left
         if not suit_length:
             return log(inspect.stack(), player.trump_cards[-1])
 
         # Return smallest in longest suit
         # TODO we might not want to do this
         sorted_suit_length = {
             key: value for key, value in sorted(suit_length.items(),
-                                                key=lambda item: item[1], reverse=True)
+                                                key=lambda item: item[1],
+                                                reverse=True)
             }
         long_suit = list(sorted_suit_length)[0]
         return log(inspect.stack(), player.suit_cards[long_suit][-1])
```

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/third_seat_defender.py` & `bfgcardplay-1.1.1/bfgcardplay/src/third_seat_defender.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,17 @@
         # Play winner if all winners
         card = self._all_winners_in_long_suit()
         if card:
             return card
 
         if len(cards) >= 5:
             for card in cards[::-1]:
+                if player.is_winner_defender(trick.cards[0], trick):
+                    return log(inspect.stack(), cards[-1])
+
                 if player.is_winner_defender(card, trick):
                     return log(inspect.stack(), card)
         return None
 
     def _all_winners_in_long_suit(self) -> Card | None:
         # Play winner if all winners
         player = self.player
```

### Comparing `bfgcardplay-1.1.0/bfgcardplay/src/utilities.py` & `bfgcardplay-1.1.1/bfgcardplay/src/utilities.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/blitz.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/blitz.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/test_first_seat_declarer.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/test_first_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/test_first_seat_defender.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/test_first_seat_defender.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,19 @@
     board = boards['0']
     assert next_card(board).name == '8H'
 
 
 def test_play_winners():
     """Play winners in _select_card_from_suit."""
     board = boards['1']
-    assert next_card(board).name == '9H'
+    assert next_card(board).name == 'JH'
 
 
 def test_play_winners_not_in_hand():
     """Play winners in _select_card_from_suit."""
     board = boards['2']
     assert next_card(board).name == '4D'
+
+
+def test_play_winners_in_hand():
+    board = boards['3']
+    assert next_card(board).name == 'AS'
```

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/test_fourth_seat_declarer.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/test_fourth_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/test_opening_lead_card.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/test_opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/test_opening_lead_suit.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/test_opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/test_player.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/test_player.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/test_second_seat_declarer.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/test_second_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/test_third_seat_defender.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/test_third_seat_defender.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,11 +19,16 @@
 
 def test_dont_play_high_card_if_partner_played_higher():
     """Do Not return highest card in _play_high_card."""
     board = boards['2']
     assert next_card(board).name != 'KS'
 
 
+def test_dont_play_high_card_if_partner_played_winner():
+    board = boards['4']
+    assert next_card(board).name != 'AC'
+
+
 def test_all_winners_in_long_suit():
     # Play winner if all winners
     board = boards['3']
     assert next_card(board).name == 'KH'
```

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/test_utilities.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay/tests/utilities.py` & `bfgcardplay-1.1.1/bfgcardplay/tests/utilities.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.1.0/bfgcardplay.egg-info/PKG-INFO` & `bfgcardplay-1.1.1/bfgcardplay.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.1.0
-Summary:              A collection of modules that facilitate cardplay in the BfG environment.         
+Version: 1.1.1
+Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
+Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
-Download-URL: https://pypi.org/project/bfgcardplay/
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.1.1 15 April 2024
+
+1. Modifications to first_player defender and third_player_defender
+
+------
+
 Version 1.1.0 7 Jan 2024
 
 1. Major refactor
 
 ------
 
 Version 1.0.15 18 Sep 2023
@@ -332,9 +337,7 @@
 ------
 
 Version 0.0.0 - 3 July 2021
 
 Created
 
 ------
-
-
```

### Comparing `bfgcardplay-1.1.0/bfgcardplay.egg-info/SOURCES.txt` & `bfgcardplay-1.1.1/bfgcardplay.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -42,11 +42,21 @@
 bfgcardplay/tests/test_first_seat_defender.py
 bfgcardplay/tests/test_fourth_seat_declarer.py
 bfgcardplay/tests/test_fourth_seat_defender.py
 bfgcardplay/tests/test_opening_lead_card.py
 bfgcardplay/tests/test_opening_lead_suit.py
 bfgcardplay/tests/test_player.py
 bfgcardplay/tests/test_second_seat_declarer.py
+bfgcardplay/tests/test_second_seat_defender.py
 bfgcardplay/tests/test_third_seat_declarer.py
 bfgcardplay/tests/test_third_seat_defender.py
 bfgcardplay/tests/test_utilities.py
-bfgcardplay/tests/utilities.py
+bfgcardplay/tests/utilities.py
+bfgcardplay/tests/test_data/first_seat_declarer.pbn
+bfgcardplay/tests/test_data/first_seat_defender.pbn
+bfgcardplay/tests/test_data/fourth_seat_declarer.pbn
+bfgcardplay/tests/test_data/fourth_seat_defender.pbn
+bfgcardplay/tests/test_data/player.pbn
+bfgcardplay/tests/test_data/second_seat_declarer.pbn
+bfgcardplay/tests/test_data/second_seat_defender.pbn
+bfgcardplay/tests/test_data/third_seat_declarer.pbn
+bfgcardplay/tests/test_data/third_seat_defender.pbn
```

### Comparing `bfgcardplay-1.1.0/setup.py` & `bfgcardplay-1.1.1/setup.py`

 * *Files identical despite different names*

