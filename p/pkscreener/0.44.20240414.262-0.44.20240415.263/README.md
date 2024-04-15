# Comparing `tmp/pkscreener-0.44.20240414.262.tar.gz` & `tmp/pkscreener-0.44.20240415.263.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240414.262.tar", last modified: Sun Apr 14 14:33:23 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240415.263.tar", last modified: Mon Apr 15 10:23:21 2024, max compression
```

## Comparing `pkscreener-0.44.20240414.262.tar` & `pkscreener-0.44.20240415.263.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 14:33:23.858971 pkscreener-0.44.20240414.262/
--rw-rw-rw-   0        0        0     1086 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-14 14:33:23.858971 pkscreener-0.44.20240414.262/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 14:33:23.843320 pkscreener-0.44.20240414.262/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 14:33:23.858971 pkscreener-0.44.20240414.262/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2995 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27587 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113858 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46266 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    74375 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-14 14:33:17.000000 pkscreener-0.44.20240414.262/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   113141 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    18453 2024-04-14 14:30:35.000000 pkscreener-0.44.20240414.262/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-14 14:33:23.843320 pkscreener-0.44.20240414.262/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-14 14:33:23.000000 pkscreener-0.44.20240414.262/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-14 14:33:23.858971 pkscreener-0.44.20240414.262/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-14 14:30:36.000000 pkscreener-0.44.20240414.262/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:23:21.238567 pkscreener-0.44.20240415.263/
+-rw-rw-rw-   0        0        0     1086 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-15 10:23:21.238567 pkscreener-0.44.20240415.263/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 10:23:21.222944 pkscreener-0.44.20240415.263/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:23:21.238567 pkscreener-0.44.20240415.263/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2995 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27587 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113858 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46266 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    74375 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-15 10:23:12.000000 pkscreener-0.44.20240415.263/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   113144 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    18453 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:23:21.222944 pkscreener-0.44.20240415.263/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-15 10:23:21.238567 pkscreener-0.44.20240415.263/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-15 10:20:08.000000 pkscreener-0.44.20240415.263/setup.py
```

### Comparing `pkscreener-0.44.20240414.262/LICENSE` & `pkscreener-0.44.20240415.263/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/LICENSE-Others` & `pkscreener-0.44.20240415.263/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/PKG-INFO` & `pkscreener-0.44.20240415.263/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240414.262
+Version: 0.44.20240415.263
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.262.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240415.263.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240414.262/README.md` & `pkscreener-0.44.20240415.263/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240414.262/pkscreener/__init__.py` & `pkscreener-0.44.20240415.263/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/classes/keys.py` & `pkscreener-0.44.20240415.263/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/courbd.ttf` & `pkscreener-0.44.20240415.263/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/globals.py` & `pkscreener-0.44.20240415.263/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1729,15 +1729,15 @@
                         caption_df[col] = caption_df[col].astype(str)
                     caption_results = colorText.miniTabulator().tabulate(
                         caption_df,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=[None,None,4,3]
                     ).encode("utf-8").decode(STD_ENCODING).replace("-+-----+-----+-----+","-+-----+----+---+").replace("%  ","% ").replace("=+=====+=====+=====+","=+=====+====+===+").replace("Vol  |","Vol|").replace("x  ","x")
-                    caption = f"{caption}.Open attached image for more. 5 samples:<pre>{caption_results}</pre><i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
+                    caption = f"{caption}.Open attached image for more. 5 samples:<pre>{caption_results}</pre>" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
                 if not testing and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
                         menuChoiceHierarchy,
                         user,
                         tabulated_results,
                         markdown_results,
                         caption,
```

### Comparing `pkscreener-0.44.20240414.262/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240415.263/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240415.263/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240415.263/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240415.263/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240414.262
+Version: 0.44.20240415.263
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240414.262.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240415.263.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.261/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240414.262/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240415.263/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240414.262/setup.py` & `pkscreener-0.44.20240415.263/setup.py`

 * *Files identical despite different names*

