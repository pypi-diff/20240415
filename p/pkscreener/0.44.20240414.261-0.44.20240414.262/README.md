# Comparing `tmp/pkscreener-0.44.20240414.261.tar.gz` & `tmp/pkscreener-0.44.20240414.262.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240414.261.tar", last modified: Sun Apr 14 11:07:17 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240414.262.tar", last modified: Sun Apr 14 14:33:23 2024, max compression
```

## Comparing `pkscreener-0.44.20240414.261.tar` & `pkscreener-0.44.20240414.262.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/
--rw-rw-rw-   0        0        0     1086 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 11:07:17.158985 pkscreener-0.44.20240414.261/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2995 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27580 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20761 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113669 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46036 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    74366 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-14 11:07:09.000000 pkscreener-0.44.20240414.261/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   113082 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    18453 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-14 11:07:17.000000 pkscreener-0.44.20240414.261/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-14 11:07:17.174610 pkscreener-0.44.20240414.261/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-14 11:04:29.000000 pkscreener-0.44.20240414.261/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:33:23.858971 pkscreener-0.44.20240414.262/
+-rw-rw-rw-   0        0        0     1086 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-14 14:33:23.858971 pkscreener-0.44.20240414.262/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 14:33:23.843320 pkscreener-0.44.20240414.262/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:33:23.858971 pkscreener-0.44.20240414.262/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2995 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27587 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113858 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46266 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    74375 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-14 14:33:17.000000 pkscreener-0.44.20240414.262/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   113141 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    18453 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:33:23.843320 pkscreener-0.44.20240414.262/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-14 14:33:23.858971 pkscreener-0.44.20240414.262/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-14 14:30:36.000000 pkscreener-0.44.20240414.262/setup.py
```

### Comparing `pkscreener-0.44.20240414.261/LICENSE` & `pkscreener-0.44.20240414.262/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/LICENSE-Others` & `pkscreener-0.44.20240414.262/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/PKG-INFO` & `pkscreener-0.44.20240414.262/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240414.261
+Version: 0.44.20240414.262
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.261.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.262.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240414.261/README.md` & `pkscreener-0.44.20240414.262/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240414.261/pkscreener/__init__.py` & `pkscreener-0.44.20240414.262/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
                         asList=asList,
                         renderStyle=renderStyle,
                         parent=selectedMenu,
                     )
             elif selectedMenu.level == 3:
                 self.level = 4
                 # next levelsub-menu of the selected sub-menu
-                if selectedMenu.parent.menuKey == "6" and selectedMenu.menuKey == "7":
+                if selectedMenu.parent.menuKey == "6" and selectedMenu.menuKey in ["7","10"]:
                     return self.renderLevel4_X_Lorenzian_Menus(
                         skip=skip,
                         asList=asList,
                         renderStyle=renderStyle,
                         parent=selectedMenu,
                     )
                 if selectedMenu.parent.menuKey == "7" and selectedMenu.menuKey == "3":
```

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files 3% similar despite different names*

```diff
@@ -298,26 +298,22 @@
                 eodDiffs.append(round(endOfDayLTP - morningLTP,2))
                 sqrOffDiffs.append(round(row["High"][-1] - morningLTP,2))
                 index += 1
             except:
                 eodLTPs.append("0")
                 eodDiffs.append("0")
                 continue
-        save_df["AlertTime"] = morningTimestamps
-        screen_df["AlertTime"] = morningTimestamps
-        save_df["SqrOffLTP"] = sellLTPs
-        screen_df["SqrOffLTP"] = sellLTPs
-        save_df["SqrOff"] = sellTimestamps
-        screen_df["SqrOff"] = sellTimestamps
-        screen_df["SqrOffDiff"] = sqrOffDiffs
-        save_df["SqrOffDiff"] = sqrOffDiffs
-        save_df["EoDLTP"] = eodLTPs
-        screen_df["EoDLTP"] = eodLTPs
-        save_df["EoDDiff"] = eodDiffs
-        screen_df["EoDDiff"] = eodDiffs
+        diffColumns = ["AlertTime", "SqrOff", "SqrOffLTP", "SqrOffDiff", "EoDLTP", "EoDDiff"]
+        diffValues = [morningTimestamps, sellTimestamps, sellLTPs, sqrOffDiffs,eodLTPs, eodDiffs]
+        for col in diffColumns:
+            save_df[col] = diffValues[diffColumns.index(col)]
+            screen_df.loc[:, col] = save_df.loc[:, col].apply(
+                lambda x: x if col in ["AlertTime", "SqrOff", "SqrOffLTP", "EoDLTP"] else ((colorText.GREEN if x >= 0 else colorText.FAIL) + str(x) + colorText.END)
+            )
+
         columns = save_df.columns
         lastIndex = len(save_df)
         for col in columns:
             if col in ["Stock", "Pattern", "LTP", "SqrOffLTP","SqrOffDiff","AlertTime", "EoDLTP", "EoDDiff", "%Chng"]:
                 if col == "Stock":
                     save_df.loc[lastIndex,col] = "PORTFOLIO"
                 elif col == "Pattern":
@@ -327,18 +323,20 @@
                 elif col == "%Chng":
                     ltpSum = sum(save_df["LTP"].dropna(inplace=False).astype(float))
                     change_pct = sum(save_df["EoDDiff"].dropna(inplace=False).astype(float))*100/ltpSum
                     save_df.loc[lastIndex,col] = f"{round(2*change_pct,2)}%" # when summing above for LTP, the total of LTP gets summed up too. Hence *2 here.
             else:
                 save_df.loc[lastIndex,col] = ""
             screen_df.loc[lastIndex,col] = save_df.loc[lastIndex,col]
-        save_df.loc[lastIndex,"EoDDiff"] = str(save_df.loc[lastIndex,"EoDDiff"]) + f'({round(100*2*save_df.loc[lastIndex,"EoDDiff"]/ltpSum,2)}%)'
-        save_df.loc[lastIndex,"SqrOffDiff"] = str(save_df.loc[lastIndex,"SqrOffDiff"]) + f'({round(100*2*save_df.loc[lastIndex,"SqrOffDiff"]/ltpSum,2)}%)'
-        screen_df.loc[lastIndex,"EoDDiff"] = save_df.loc[lastIndex,"EoDDiff"]
-        screen_df.loc[lastIndex,"SqrOffDiff"] = save_df.loc[lastIndex,"SqrOffDiff"]
+        eodDiff = save_df.loc[lastIndex,"EoDDiff"]
+        sqrOffDiff = save_df.loc[lastIndex,"SqrOffDiff"]
+        save_df.loc[lastIndex,"EoDDiff"] = str(eodDiff) + f'({round(100*2*eodDiff/ltpSum,2)}%)'
+        save_df.loc[lastIndex,"SqrOffDiff"] = str(sqrOffDiff) + f'({round(100*2*sqrOffDiff/ltpSum,2)}%)'
+        screen_df.loc[lastIndex,"EoDDiff"] = (colorText.GREEN if eodDiff >= 0 else colorText.FAIL) + save_df.loc[lastIndex,"EoDDiff"] + colorText.END
+        screen_df.loc[lastIndex,"SqrOffDiff"] = (colorText.GREEN if sqrOffDiff >= 0 else colorText.FAIL) + save_df.loc[lastIndex,"SqrOffDiff"] + colorText.END
         save_df.set_index("Stock", inplace=True)
         screen_df.set_index("Stock", inplace=True)
         PKMarketOpenCloseAnalyser.allIntradayCandles = None
         if 'index' in save_df.columns:
             save_df.drop('index', axis=1, inplace=True, errors="ignore")
         if 'index' in screen_df.columns:
             screen_df.drop('index', axis=1, inplace=True, errors="ignore")
```

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/ScreeningStatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -682,38 +682,41 @@
         try:
             # Let's only consider those candles that are after the alert issue-time in the mornings
             diff_df = diff_df[diff_df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber}:00+05:30').to_datetime64()]
         except:
             diff_df = diff_df[diff_df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber}:00+05:30', utc=True)]
             pass
         index = len(diff_df)
-        if diff_df["diff"][-1] < 0:
-            while(diff_df["diff"][index-1] < 0 and index >=0):
-                index -= 1
-        else:
-            while(diff_df["diff"][index-1] >= 0 and index >=0):
-                index -= 1
+        crossOver = 0
+        while (crossOver < nthCrossover and index >=0):
+            if diff_df["diff"][index-1] < 0:
+                while(diff_df["diff"][index-1] < 0 and index >=0):
+                    index -= 1
+            else:
+                while(diff_df["diff"][index-1] >= 0 and index >=0):
+                    index -= 1
+            crossOver += 1
         ts = diff_df.tail(len(diff_df)-index +1).head(1).index[-1]
         return ts, df[df.index == ts] #df.head(len(df) -index +1).tail(1)
     
     # Find stock showing RSI crossing with RSI 9 SMA
-    def findRSICrossingMA(self, df, screenDict, saveDict, maLength=9):
+    def findRSICrossingMA(self, df, screenDict, saveDict,lookFor=1, maLength=9):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data[::-1]
         maRsi = pktalib.MA(data['RSI'], timeperiod=maLength)
         data = data[::-1].head(3)
         maRsi = maRsi[::-1].head(3)
         saved = self.findCurrentSavedValue(screenDict,saveDict,"Trend")
-        if maRsi.iloc[0] <= data['RSI'].iloc[0] and maRsi.iloc[1] > data['RSI'].iloc[1]:
+        if lookFor in [1,3] and maRsi.iloc[0] <= data['RSI'].iloc[0] and maRsi.iloc[1] > data['RSI'].iloc[1]:
             screenDict['MA-Signal'] = saved[0] + colorText.BOLD + colorText.GREEN + f'RSI-MA-Buy' + colorText.END
             saveDict['MA-Signal'] = saved[1] + f'RSI-MA-Buy'
             return True
-        elif maRsi.iloc[0] >= data['RSI'].iloc[0] and maRsi.iloc[1] < data['RSI'].iloc[1]:
+        elif lookFor in [2,3] and maRsi.iloc[0] >= data['RSI'].iloc[0] and maRsi.iloc[1] < data['RSI'].iloc[1]:
             screenDict['MA-Signal'] = saved[0] + colorText.BOLD + colorText.FAIL + f'RSI-MA-Sell' + colorText.END
             saveDict['MA-Signal'] = saved[1] + f'RSI-MA-Sell'
             return True
         return False
     
     # Find stocks with rising RSI from lower levels
     def findRisingRSI(self, df):
```

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/StockScreener.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,16 +217,18 @@
                     isValidRsi = screener.validateRSI(
                         processedData, screeningDictionary, saveDictionary, minRSI, maxRSI
                     )
                     if not isValidRsi:
                         return returnLegibleData()
                 elif executeOption == 6:
                     if reversalOption == 10:
-                        hasRSIMAReversal = screener.findRSICrossingMA(processedData,screeningDictionary,
-                            saveDictionary)
+                        hasRSIMAReversal = screener.findRSICrossingMA(processedData,
+                                                                      screeningDictionary,
+                                                                      saveDictionary,
+                                                                      lookFor=maLength) # 1 =Buy, 2 =Sell, 3 = Any
                         if not hasRSIMAReversal:
                             return returnLegibleData()
                     elif reversalOption == 9:
                         hasRisingRSIReversal = screener.findRisingRSI(processedData)
                         if not hasRisingRSIReversal:
                             return returnLegibleData()
                     elif reversalOption == 8:
```

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1182,15 +1182,15 @@
                 input(
                     colorText.BOLD
                     + colorText.WARN
                     + """[+] Select Option:"""
                     + colorText.END
                 )
             )
-            if resp >= 0 and resp <= 9:
+            if resp >= 0 and resp <= 10:
                 return resp
             raise ValueError
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             input(
                 colorText.BOLD
                 + colorText.FAIL
@@ -1248,19 +1248,19 @@
                         print(
                             colorText.BOLD
                             + colorText.FAIL
                             + "\n[!] Invalid Input! NR timeframe should be single integer value!\n"
                             + colorText.END
                         )
                         raise ValueError
-                elif resp == 7:
+                elif resp in [7,10]:
                     m3 = menus()
                     m3.renderForMenu(menu,asList=True)
                     lMenu =  m3.find(str(resp))
-                    return 7, tools.promptSubMenuOptions(lMenu)
+                    return resp, tools.promptSubMenuOptions(lMenu)
                 return resp, None
             raise ValueError
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             input(
                 colorText.BOLD
                 + colorText.FAIL
```

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/classes/keys.py` & `pkscreener-0.44.20240414.262/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/courbd.ttf` & `pkscreener-0.44.20240414.262/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/globals.py` & `pkscreener-0.44.20240414.262/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,20 +797,20 @@
             )
             input("PRess <Enter> to continue...")
             return
     if executeOption == 6:
         selectedMenu = m2.find(str(executeOption))
         if len(options) >= 4:
             reversalOption = int(options[3])
-            if reversalOption in [4, 6, 7]:
+            if reversalOption in [4, 6, 7, 10]:
                 if len(options) >= 5:
                     if str(options[4]).isnumeric():
                         maLength = int(options[4])
                     elif str(options[4]).upper() == "D":
-                        maLength = 50 if reversalOption == 4 else (3 if reversalOption == 7 else 7)
+                        maLength = 50 if reversalOption == 4 else (3 if reversalOption in [7] else (2 if reversalOption in [10] else 7))
                 elif defaultAnswer == "Y" and user is not None:
                     # bot mode
                     maLength = 50 if reversalOption == 4 else (3 if reversalOption == 7 else 7)
                 else:
                     reversalOption, maLength = Utility.tools.promptReversalScreening(
                         selectedMenu
                     )
@@ -818,15 +818,15 @@
             reversalOption, maLength = Utility.tools.promptReversalScreening(
                 selectedMenu
             )
         if reversalOption is None or reversalOption == 0 or maLength == 0:
             return
         else:
             selectedChoice["3"] = str(reversalOption)
-            if str(reversalOption) == "7":
+            if str(reversalOption) in ["7", "10"]:
                 selectedChoice["4"] = str(maLength)
     if executeOption == 7:
         selectedMenu = m2.find(str(executeOption))
         maLength = 0
         if len(options) >= 4:
             respChartPattern = int(options[3])
             selectedChoice["3"] = options[3]
@@ -1586,15 +1586,15 @@
     global selectedChoice, menuChoiceHierarchy
     menuChoiceHierarchy = f'{level0MenuDict[selectedChoice["0"]].strip()}>{level1_X_MenuDict[selectedChoice["1"]].strip()}>{level2_X_MenuDict[selectedChoice["2"]].strip()}'
     if selectedChoice["2"] == "6":
         menuChoiceHierarchy = (
             menuChoiceHierarchy
             + f'>{level3_X_Reversal_MenuDict[selectedChoice["3"]].strip()}'
         )
-        if len(selectedChoice) >= 5 and selectedChoice["3"] == "7":
+        if len(selectedChoice) >= 5 and selectedChoice["3"] in ["7","10"]:
             menuChoiceHierarchy = (
             menuChoiceHierarchy
             + f'>{level4_X_Lorenzian_MenuDict[selectedChoice["4"]].strip()}'
         )
     elif selectedChoice["2"] == "7":
         menuChoiceHierarchy = (
             menuChoiceHierarchy
@@ -1727,16 +1727,16 @@
                     caption_df.rename(columns={"%Chng": "Ch%","Volume":"Vol"}, inplace=True)
                     for col in caption_df.columns:
                         caption_df[col] = caption_df[col].astype(str)
                     caption_results = colorText.miniTabulator().tabulate(
                         caption_df,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
-                        maxcolwidths=[None,None,3,3]
-                    ).encode("utf-8").decode(STD_ENCODING).replace("-+-----+-----+-----+","-+-----+---+---+").replace("%  ","%").replace("=+=====+=====+=====+","=+=====+===+===+").replace("Vol  |","Vol|").replace("x  ","x")
+                        maxcolwidths=[None,None,4,3]
+                    ).encode("utf-8").decode(STD_ENCODING).replace("-+-----+-----+-----+","-+-----+----+---+").replace("%  ","% ").replace("=+=====+=====+=====+","=+=====+====+===+").replace("Vol  |","Vol|").replace("x  ","x")
                     caption = f"{caption}.Open attached image for more. 5 samples:<pre>{caption_results}</pre><i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
                 if not testing and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
                         menuChoiceHierarchy,
                         user,
                         tabulated_results,
                         markdown_results,
```

### Comparing `pkscreener-0.44.20240414.261/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240414.262/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240414.262/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240414.262/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240414.262/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240414.261
+Version: 0.44.20240414.262
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.261.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.262.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.260/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240414.261/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240414.262/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.261/setup.py` & `pkscreener-0.44.20240414.262/setup.py`

 * *Files identical despite different names*

